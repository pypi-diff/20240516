# Comparing `tmp/confluence-junction-0.1.1.tar.gz` & `tmp/confluence_junction-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confluence-junction-0.1.1.tar", max compression
+gzip compressed data, was "confluence_junction-0.1.2.tar", max compression
```

## Comparing `confluence-junction-0.1.1.tar` & `confluence_junction-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1077 2021-03-05 23:49:51.276954 confluence-junction-0.1.1/LICENSE
--rw-r--r--   0        0        0     8425 2021-03-05 23:49:51.276954 confluence-junction-0.1.1/README.md
--rw-r--r--   0        0        0     1753 2021-03-05 23:49:51.280954 confluence-junction-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       85 2021-03-05 23:49:51.280954 confluence-junction-0.1.1/src/junction/__init__.py
--rw-r--r--   0        0        0     6835 2021-03-05 23:49:51.280954 confluence-junction-0.1.1/src/junction/cli.py
--rw-r--r--   0        0        0     1035 2021-03-05 23:49:51.280954 confluence-junction-0.1.1/src/junction/confluence/__init__.py
--rw-r--r--   0        0        0     4687 2021-03-05 23:49:51.280954 confluence-junction-0.1.1/src/junction/confluence/api/__init__.py
--rw-r--r--   0        0        0     4867 2021-03-05 23:49:51.280954 confluence-junction-0.1.1/src/junction/confluence/api/content_api.py
--rw-r--r--   0        0        0    14258 2021-03-05 23:49:51.280954 confluence-junction-0.1.1/src/junction/confluence/models/__init__.py
--rw-r--r--   0        0        0     4484 2021-03-05 23:49:51.284953 confluence-junction-0.1.1/src/junction/confluence/models/json.py
--rw-r--r--   0        0        0     2604 2021-03-05 23:49:51.284953 confluence-junction-0.1.1/src/junction/confluence/models/subclassing.py
--rw-r--r--   0        0        0    24082 2021-03-05 23:49:51.284953 confluence-junction-0.1.1/src/junction/delta.py
--rw-r--r--   0        0        0     8226 2021-03-05 23:49:51.284953 confluence-junction-0.1.1/src/junction/git/__init__.py
--rw-r--r--   0        0        0     1592 2021-03-05 23:49:51.284953 confluence-junction-0.1.1/src/junction/markdown/__init__.py
--rw-r--r--   0        0        0     1299 2021-03-05 23:49:51.284953 confluence-junction-0.1.1/src/junction/markdown/children.py
--rw-r--r--   0        0        0     1940 2021-03-05 23:49:51.284953 confluence-junction-0.1.1/src/junction/markdown/codeblocks.py
--rw-r--r--   0        0        0     2898 2021-03-05 23:49:51.284953 confluence-junction-0.1.1/src/junction/markdown/info_panels.py
--rw-r--r--   0        0        0     2011 2021-03-05 23:49:51.284953 confluence-junction-0.1.1/src/junction/markdown/status.py
--rw-r--r--   0        0        0     1370 2021-03-05 23:49:51.284953 confluence-junction-0.1.1/src/junction/markdown/toc.py
--rw-r--r--   0        0        0     1610 2021-03-05 23:49:51.284953 confluence-junction-0.1.1/src/junction/markdown/wiki_links.py
--rw-r--r--   0        0        0     1540 2021-03-05 23:49:51.284953 confluence-junction-0.1.1/src/junction/util.py
--rw-r--r--   0        0        0     9882 2021-03-05 23:51:27.946883 confluence-junction-0.1.1/setup.py
--rw-r--r--   0        0        0    10082 2021-03-05 23:51:27.947862 confluence-junction-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-16 05:51:02.922478 confluence_junction-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8425 2024-05-16 05:51:02.922478 confluence_junction-0.1.2/README.md
+-rw-r--r--   0        0        0     1737 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       85 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/__init__.py
+-rw-r--r--   0        0        0     7015 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/cli.py
+-rw-r--r--   0        0        0     1035 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/confluence/__init__.py
+-rw-r--r--   0        0        0     4783 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/confluence/api/__init__.py
+-rw-r--r--   0        0        0     4867 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/confluence/api/content_api.py
+-rw-r--r--   0        0        0    14260 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/confluence/models/__init__.py
+-rw-r--r--   0        0        0     4532 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/confluence/models/json.py
+-rw-r--r--   0        0        0     2604 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/confluence/models/subclassing.py
+-rw-r--r--   0        0        0    24247 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/delta.py
+-rw-r--r--   0        0        0     8495 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/git/__init__.py
+-rw-r--r--   0        0        0     1903 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/markdown/__init__.py
+-rw-r--r--   0        0        0     2432 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/markdown/checklists.py
+-rw-r--r--   0        0        0     1299 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/markdown/children.py
+-rw-r--r--   0        0        0      566 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/markdown/codeblocks.py
+-rw-r--r--   0        0        0      816 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/markdown/emdash.py
+-rw-r--r--   0        0        0     2898 2024-05-16 05:51:02.926478 confluence_junction-0.1.2/src/junction/markdown/info_panels.py
+-rw-r--r--   0        0        0     2017 2024-05-16 05:51:02.930478 confluence_junction-0.1.2/src/junction/markdown/status.py
+-rw-r--r--   0        0        0     1370 2024-05-16 05:51:02.930478 confluence_junction-0.1.2/src/junction/markdown/toc.py
+-rw-r--r--   0        0        0     1621 2024-05-16 05:51:02.930478 confluence_junction-0.1.2/src/junction/markdown/wiki_links.py
+-rw-r--r--   0        0        0     1583 2024-05-16 05:51:02.930478 confluence_junction-0.1.2/src/junction/util.py
+-rw-r--r--   0        0        0    10086 1970-01-01 00:00:00.000000 confluence_junction-0.1.2/PKG-INFO
```

### Comparing `confluence-junction-0.1.1/LICENSE` & `confluence_junction-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `confluence-junction-0.1.1/README.md` & `confluence_junction-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `confluence-junction-0.1.1/pyproject.toml` & `confluence_junction-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "confluence-junction"
-version = "0.1.1"
+version = "0.1.2"
 description = "Publish to and manage Confluence spaces with markdown files tracked in Git."
 authors = ["HUU <readabook123@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/HUU/Junction"
 keywords = ["confluence", "markdown", "git", "sync", "convert"]
 classifiers = [
@@ -24,33 +24,32 @@
 packages = [
     { include = "junction", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.22.0"
-markdown = "^3.0.1"
-markdownsuperscript = "^2.1.1"
-markdownsubscript = "^2.1.1"
-markdown-urlize = "^0.2.0"
-markdown-emdash = "^0.1.0"
+markdown = "^3.6"
 gitpython = "^3.0.5"
-click = "^7.0"
+click = "^8.0"
 click-log = "^0.3.2"
 colorama = "^0.4.3"
+pymdown-extensions = "^10.8.1"
 
 [tool.poetry.dev-dependencies]
 ipykernel = "^5.1.4"
 notebook = "^6.0.3"
-black = "==19.10b0"
+black = "^24.4.2"
 flake8 = "^3.7.9"
 pre-commit = "^2.0.1"
 rope = "^0.16.0"
+types-markdown = "^3.6.0.20240316"
+types-requests = "^2.31.0.20240406"
 pycodestyle = "^2.6.0"
-mypy = "^0.770"
+mypy = "^0.982"
 pyflakes = "^2.2.0"
 
 [tool.poetry.scripts]
 junction = "junction.cli:main"
 
 [tool.tox]
 legacy_tox_ini = """
```

### Comparing `confluence-junction-0.1.1/src/junction/cli.py` & `confluence_junction-0.1.2/src/junction/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,19 @@
     Looks for files under [content-path] affected by all commits from [SINCE] to the head of [BRANCH]
     and then performs Confluence API calls to realize those changes onto the wiki.
 
     [SINCE] must be a valid commitish within the targeted git repository and should be part of the history
     of [BRANCH] i.e. you can get from SINCE to the HEAD of [BRANCH].
     """
 
+    if my_ctx.repo is None:
+        raise click.BadParameter(
+            "junction must be run from within a git repository, or git-dir must point to a git repository"
+        )
+
     filter_path = Path(content_path) if content_path else git_dir
     commits = find_commits_on_branch_after(branch, since, my_ctx.repo)
     deltas = {
         c: Delta.from_modifications(
             filter_modifications_to_folder(get_modifications(c), filter_path)
         )
         for c in commits
```

### Comparing `confluence-junction-0.1.1/src/junction/confluence/__init__.py` & `confluence_junction-0.1.2/src/junction/confluence/__init__.py`

 * *Files identical despite different names*

### Comparing `confluence-junction-0.1.1/src/junction/confluence/api/__init__.py` & `confluence_junction-0.1.2/src/junction/confluence/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,21 +120,27 @@
 
         if method == "GET":
             response = requests.get(url, auth=self.basic_auth, headers=headers)
         elif method == "POST":
             data = self.__json_encoder.encode(body)
             logger.debug(data)
             response = requests.post(
-                url, data=data, auth=self.basic_auth, headers=headers,
+                url,
+                data=data,
+                auth=self.basic_auth,
+                headers=headers,
             )
         elif method == "PUT":
             data = self.__json_encoder.encode(body)
             logger.debug(data)
             response = requests.put(
-                url, data=data, auth=self.basic_auth, headers=headers,
+                url,
+                data=data,
+                auth=self.basic_auth,
+                headers=headers,
             )
         elif method == "DELETE":
             response = requests.delete(url, auth=self.basic_auth, headers=headers)
         else:
             raise NotImplementedError(
                 "API client does not support {} method".format(method)
             )
```

### Comparing `confluence-junction-0.1.1/src/junction/confluence/api/content_api.py` & `confluence_junction-0.1.2/src/junction/confluence/api/content_api.py`

 * *Files identical despite different names*

### Comparing `confluence-junction-0.1.1/src/junction/confluence/models/__init__.py` & `confluence_junction-0.1.2/src/junction/confluence/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,17 +338,17 @@
 
     id: Optional[str] = None
     type: Optional[str] = None
     status: Optional[str] = None
     space: Optional[Space] = None
     history: Optional["ContentHistory"] = None
     version: Optional["Version"] = None
-    ancestors: Optional[
-        List["ContentPage"]
-    ] = None  # this really isn't the right type, but in 99% cases it is and it makes the type checker quiet down
+    ancestors: Optional[List["ContentPage"]] = (
+        None  # this really isn't the right type, but in 99% cases it is and it makes the type checker quiet down
+    )
     operations: Optional[List[OperationCheckResult]] = None
     children: Optional["ContentChildren"] = None
     childTypes: Optional["ContentChildType"] = None
     descendants: Optional["ContentChildren"] = None
     containers: Optional[Union[Space, "Content"]] = None
     body: Optional[Body] = None
     restrictions: Optional["ContentRestrictions"] = None
```

### Comparing `confluence-junction-0.1.1/src/junction/confluence/models/json.py` & `confluence_junction-0.1.2/src/junction/confluence/models/json.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,26 +83,28 @@
         hints = get_type_hints(target_klass)
         for key, value in dict.items():
             if hasattr(new_obj, key):
                 if key not in hints:
                     setattr(
                         new_obj,
                         key,
-                        value
-                        if not issubclass(value.__class__, Mapping)
-                        else DotDict(value),
+                        (
+                            value
+                            if not issubclass(value.__class__, Mapping)
+                            else DotDict(value)
+                        ),
                     )
                 else:
                     setattr(
                         new_obj, key, self.__marshal_hinted_class(value, hints[key])
                     )
         return new_obj
 
     def __marshal_hinted_class(self, value: Any, hint: Any) -> Any:
-        if get_origin(hint) is Union and (hint_args := get_args(hint))[1] is NoneType:  # type: ignore
+        if get_origin(hint) is Union and (hint_args := get_args(hint))[1] is NoneType:
             # this is an Optional[T]..unwrap the real type:
             hint = hint_args[0]
         elif hasattr(hint, "__bound__"):
             # this is a TypeVar (probably from a generic), fetch the type binding information
             hint = hint.__bound__
 
         if get_origin(hint) is list and issubclass(value.__class__, Iterable):
```

### Comparing `confluence-junction-0.1.1/src/junction/confluence/models/subclassing.py` & `confluence_junction-0.1.2/src/junction/confluence/models/subclassing.py`

 * *Files identical despite different names*

### Comparing `confluence-junction-0.1.1/src/junction/delta.py` & `confluence_junction-0.1.2/src/junction/delta.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,16 @@
 class PageAction(ABC):
     """Base class for all actions against individual pages.  A page action should target an individual page in Confluence,
     though it may also trigger additional actions affecting other pages as needed to successfully complete the requested action,
     for example generating index pages for new folders.
 
     Page actions should attempt to be somewhat replayable.  This ensures if Junction fails while executing a Delta that it can simply
     be re-run.  This isn't quite full idempotency as some actions are inherently un-idempotent.  This could be changed to full idempotency
-    if index pages were made explicit (via the git/Modification API) rather than implicit as needed by a particular page action."""
+    if index pages were made explicit (via the git/Modification API) rather than implicit as needed by a particular page action.
+    """
 
     def __init__(self, title: str):
         self.title = title
 
     @abstractmethod
     def execute(self, api_client: Confluence) -> Any:
         pass
@@ -143,17 +144,19 @@
                 else None
             )
 
             update_request = UpdateContent(
                 title=self.new_title,
                 type="page",
                 version=Version(
-                    number=old_page.version.number + 1
-                    if old_page.version and old_page.version.number
-                    else 2
+                    number=(
+                        old_page.version.number + 1
+                        if old_page.version and old_page.version.number
+                        else 2
+                    )
                 ),
                 ancestors=[Content(id=parent.id)] if parent else None,
             )
 
             if old_page.id:
                 logger.info(
                     "Moving %s to %s.",
@@ -333,21 +336,25 @@
                 self.ancestor_titles, current_ancestors
             )
 
             update_request = UpdateContent(
                 title=self.title,
                 type="page",
                 version=Version(
-                    number=existing.version.number + 1
-                    if existing.version and existing.version.number
-                    else 2
+                    number=(
+                        existing.version.number + 1
+                        if existing.version and existing.version.number
+                        else 2
+                    )
+                ),
+                ancestors=(
+                    [Content(id=existing.ancestors[-1].id)]
+                    if existing.ancestors
+                    else []
                 ),
-                ancestors=[Content(id=existing.ancestors[-1].id)]
-                if existing.ancestors
-                else [],
                 body=Body(
                     storage=ContentBody(value=self.new_body, representation="storage")
                 ),
             )
 
             if existing.id:
                 logger.info(
```

### Comparing `confluence-junction-0.1.1/src/junction/git/__init__.py` & `confluence_junction-0.1.2/src/junction/git/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,16 +69,16 @@
     RENAME = 2
     DELETE = 3
     MODIFY = 4
     UNKNOWN = 5
 
 
 class Modification:
-    """ Represents a modification to the filesystem.  This is used to abstract the details of git from other subsystems that consume information
-    about changes such as the Delta API. """
+    """Represents a modification to the filesystem.  This is used to abstract the details of git from other subsystems that consume information
+    about changes such as the Delta API."""
 
     def __init__(
         self,
         old_path: Optional[Union[str, Path]],
         new_path: Optional[Union[str, Path]],
         change_type: ModificationType,
         source_code: Optional[str] = None,
@@ -139,16 +139,23 @@
             Modification -- A modification representing the provided diff.
         """
         old_path = diff.a_path
         new_path = diff.b_path
         change_type = Modification._determine_modification_type(diff)
 
         tree_path = new_path if new_path else old_path
+
         source_code = (
-            tree[tree_path].data_stream.read()
+            tree[
+                (
+                    tree_path
+                    if tree_path
+                    else "this should not be possible make mypy happy"
+                )
+            ].data_stream.read()
             if change_type != ModificationType.DELETE
             else None
         )
 
         mod = Modification(old_path, new_path, change_type, source_code)
         logger.debug(
             "%s, with %s bytes of source code.",
@@ -207,16 +214,20 @@
                 modification_type = ModificationType.ADD
             elif not new_path_in_folder and old_path_in_folder and mod.previous_path:
                 modification_type = ModificationType.DELETE
             else:
                 modification_type = mod.change_type
 
             yield Modification(
-                mod.previous_path.relative_to(folder)
-                if mod.previous_path and old_path_in_folder
-                else None,
-                mod.path.relative_to(folder)
-                if mod.path and new_path_in_folder
-                else None,
+                (
+                    mod.previous_path.relative_to(folder)
+                    if mod.previous_path and old_path_in_folder
+                    else None
+                ),
+                (
+                    mod.path.relative_to(folder)
+                    if mod.path and new_path_in_folder
+                    else None
+                ),
                 modification_type,
                 mod.source_code,
             )
```

### Comparing `confluence-junction-0.1.1/src/junction/markdown/__init__.py` & `confluence_junction-0.1.2/src/junction/markdown/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 import logging
 
 from typing import Union, Optional
 
 from markdown import Markdown
 from markdown.extensions.sane_lists import SaneListExtension
 from markdown.extensions.tables import TableExtension
-from mdx_superscript import SuperscriptExtension
-from mdx_subscript import SubscriptExtension
-from mdx_emdash import EmDashExtension
-from mdx_urlize import UrlizeExtension
-
-from junction.markdown.codeblocks import CodeBlockExtension
+from pymdownx.caret import InsertSupExtension
+from pymdownx.magiclink import MagiclinkExtension
+from pymdownx.superfences import SuperFencesCodeExtension
+from pymdownx.tilde import DeleteSubExtension
+
+from junction.markdown.checklists import ChecklistExtension
+from junction.markdown.codeblocks import confluence_code_format
+from junction.markdown.emdash import EmDashExtension
 from junction.markdown.status import StatusExtension
 from junction.markdown.toc import TableOfContentsExtension
 from junction.markdown.children import ChildrenExtension
 from junction.markdown.info_panels import InfoPanelExtension
 from junction.markdown.wiki_links import WikiLinkExtension
 
 
 logger = logging.getLogger(__name__)
 
 
 junctionMarkdown = Markdown(
     extensions=[
         SaneListExtension(),
-        SuperscriptExtension(),
-        SubscriptExtension(),
+        InsertSupExtension(),
+        DeleteSubExtension(),
         EmDashExtension(),
-        UrlizeExtension(),
-        CodeBlockExtension(),
+        MagiclinkExtension(),
+        ChecklistExtension(),
+        SuperFencesCodeExtension(
+            custom_fences=[
+                {"name": "*", "class": "*", "format": confluence_code_format}
+            ]
+        ),
         StatusExtension(),
         TableOfContentsExtension(),
         ChildrenExtension(),
         InfoPanelExtension(),
         WikiLinkExtension(),
         TableExtension(),
     ]
```

### Comparing `confluence-junction-0.1.1/src/junction/markdown/children.py` & `confluence_junction-0.1.2/src/junction/markdown/children.py`

 * *Files identical despite different names*

### Comparing `confluence-junction-0.1.1/src/junction/markdown/info_panels.py` & `confluence_junction-0.1.2/src/junction/markdown/info_panels.py`

 * *Files identical despite different names*

### Comparing `confluence-junction-0.1.1/src/junction/markdown/status.py` & `confluence_junction-0.1.2/src/junction/markdown/status.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,52 +3,54 @@
 from markdown.extensions import Extension
 from markdown.inlinepatterns import InlineProcessor
 import xml.etree.ElementTree as etree
 import re
 
 
 class StatusExtension(Extension):
-    """ Markdown extension that generates Confluence status macros (the little colored pills).
+    """Markdown extension that generates Confluence status macros (the little colored pills).
     Supports red, yellow, green, grey, blue, and purple.  Some examples:
     ```
     Milestone 1 &status-green:Complete;
     Milestone 2 &status-yellow:In Progress;
     Milestone 3 &status-grey:Planning;
     ```
     """
 
     def extendMarkdown(self, md: Markdown) -> None:
-        md.inlinePatterns.add("status-red", StatusPattern("red"), "<reference")
-        md.inlinePatterns.add("status-yellow", StatusPattern("yellow"), "<reference")
-        md.inlinePatterns.add("status-green", StatusPattern("green"), "<reference")
-        md.inlinePatterns.add("status-grey", StatusPattern("grey"), "<reference")
-        md.inlinePatterns.add("status-purple", StatusPattern("purple"), "<reference")
-        md.inlinePatterns.add("status-blue", StatusPattern("blue"), "<reference")
+        md.inlinePatterns.register(StatusPattern("red"), "status-red", 25)
+        md.inlinePatterns.register(StatusPattern("yellow"), "status-yellow", 25)
+        md.inlinePatterns.register(StatusPattern("green"), "status-green", 25)
+        md.inlinePatterns.register(StatusPattern("grey"), "status-grey", 25)
+        md.inlinePatterns.register(StatusPattern("purple"), "status-purple", 25)
+        md.inlinePatterns.register(StatusPattern("blue"), "status-blue", 25)
 
 
 class StatusPattern(InlineProcessor):
     def __init__(self, color: str):
         self._color = color
         super().__init__(r"&status-{}:(?P<title>[^;]+);".format(self._color))
 
-    def handleMatch(self, match: re.Match, data: str) -> Tuple[etree.Element, int, int]:
+    def handleMatch(  # type: ignore
+        self, match: re.Match[str], data: str
+    ) -> Tuple[etree.Element, int, int]:
         el = etree.Element(
             "ac:structured-macro",
             {
                 "ac:name": "status",
                 "ac:schema-version": "1",
                 "ac:macro-id": "d4fcf299-d2f0-4eec-807a-1e4a3c8fe0dc",
             },
         )
 
         etree.SubElement(el, "ac:parameter", {"ac:name": "title"}).text = match.group(
             "title"
         )
-        etree.SubElement(
-            el, "ac:parameter", {"ac:name": "colour"}
-        ).text = self._color.capitalize()
+        etree.SubElement(el, "ac:parameter", {"ac:name": "colour"}).text = (
+            self._color.capitalize()
+        )
 
         return el, match.start(0), match.end(0)
 
 
 def makeExtension(**kwargs: Any) -> StatusExtension:
     return StatusExtension(**kwargs)
```

### Comparing `confluence-junction-0.1.1/src/junction/markdown/toc.py` & `confluence_junction-0.1.2/src/junction/markdown/toc.py`

 * *Files identical despite different names*

### Comparing `confluence-junction-0.1.1/src/junction/markdown/wiki_links.py` & `confluence_junction-0.1.2/src/junction/markdown/wiki_links.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 
 class WikiLinkExtension(Extension):
     """Markdown extension for rendering links prefixed with '&' as links to other pages
     in Confluence.  Links in Confluence are based on page titles e.g. `&[Display Text](Target Page Name)`
     """
 
     def extendMarkdown(self, md: Markdown) -> None:
-        md.inlinePatterns.add("wiki-link", WikiLinkPattern(md), "<reference")
+        md.inlinePatterns.register(WikiLinkPattern(md), "wiki-link", 25)
 
 
 class WikiLinkPattern(LinkInlineProcessor):
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(r"\&\[", *args, **kwargs)
 
-    def handleMatch(
+    def handleMatch(  # type: ignore
         self, m: re.Match, data: str
     ) -> Tuple[Optional[etree.Element], Optional[int], Optional[int]]:
         text, index, handled = self.getText(data, m.end(0))
 
         if not handled:
             return None, None, None
```

### Comparing `confluence-junction-0.1.1/src/junction/util.py` & `confluence_junction-0.1.2/src/junction/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,8 +46,9 @@
 
     def __getattr__(self, k: Any) -> Any:
         try:
             return self[k]
         except KeyError as ex:
             raise AttributeError(f"No attribute called: {k}") from ex
 
-    __setattr__ = OrderedDict.__setitem__
+    def __setattr__(self, name: str, value: Any) -> None:
+        self[name] = value
```

### Comparing `confluence-junction-0.1.1/setup.py` & `confluence_junction-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,52 +1,232 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: confluence-junction
+Version: 0.1.2
+Summary: Publish to and manage Confluence spaces with markdown files tracked in Git.
+Home-page: https://github.com/HUU/Junction
+License: MIT
+Keywords: confluence,markdown,git,sync,convert
+Author: HUU
+Author-email: readabook123@protonmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Documentation
+Classifier: Topic :: Office/Business
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: Version Control :: Git
+Classifier: Topic :: Text Editors :: Text Processing
+Classifier: Topic :: Text Processing :: Markup :: HTML
+Requires-Dist: click (>=8.0,<9.0)
+Requires-Dist: click-log (>=0.3.2,<0.4.0)
+Requires-Dist: colorama (>=0.4.3,<0.5.0)
+Requires-Dist: gitpython (>=3.0.5,<4.0.0)
+Requires-Dist: markdown (>=3.6,<4.0)
+Requires-Dist: pymdown-extensions (>=10.8.1,<11.0.0)
+Requires-Dist: requests (>=2.22.0,<3.0.0)
+Project-URL: Repository, https://github.com/HUU/Junction
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+![Junction, publish and manage Confluence with git workflows](https://github.com/HUU/Junction/raw/master/docs/logo.png?raw=true)
 
-packages = \
-['junction',
- 'junction.confluence',
- 'junction.confluence.api',
- 'junction.confluence.models',
- 'junction.git',
- 'junction.markdown']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click-log>=0.3.2,<0.4.0',
- 'click>=7.0,<8.0',
- 'colorama>=0.4.3,<0.5.0',
- 'gitpython>=3.0.5,<4.0.0',
- 'markdown-emdash>=0.1.0,<0.2.0',
- 'markdown-urlize>=0.2.0,<0.3.0',
- 'markdown>=3.0.1,<4.0.0',
- 'markdownsubscript>=2.1.1,<3.0.0',
- 'markdownsuperscript>=2.1.1,<3.0.0',
- 'requests>=2.22.0,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['junction = junction.cli:main']}
-
-setup_kwargs = {
-    'name': 'confluence-junction',
-    'version': '0.1.1',
-    'description': 'Publish to and manage Confluence spaces with markdown files tracked in Git.',
-    'long_description': '![Junction, publish and manage Confluence with git workflows](https://github.com/HUU/Junction/raw/master/docs/logo.png?raw=true)\n\nWith Junction you can write and manage your documentation directly in your codebase, using Markdown and your existing Git workflows (pull requests, code review, release branches, etc) and then automatically publish your changes to Confluence.  This gives you the best of both worlds: in-repo documentation that fits natively into your development workflows, with the discoverability and centrality of Confluence.\n\n![MIT License](https://img.shields.io/badge/license-MIT-green) [![Python 3.8](https://img.shields.io/badge/python-3.8-blue)](https://pypi.org/project/confluence-junction) ![Build and Test](https://github.com/HUU/Junction/workflows/Build%20and%20Test/badge.svg)\n\n# Install\n\nEnsure you are using Python 3.8 (or newer); Junction does not work with older versions of Python.  Install using `pip`:\n```sh\npip install confluence-junction\n```\nThis will install the library and CLI.\nIn your Python code:\n```python\nimport junction\n```\nIn your shell:\n```sh\njunction --help\n```\n\n# Overview\n\nJunction works by inspecting the changes made on a commit-by-commit basis to your Git repository, and determining what needs to be changed in Confluence to reflect those changes.  Junction (currently) expects to manage the entire [space in Confluence](https://confluence.atlassian.com/doc/spaces-139459.html).  Thus when using Junction you must tell it which Space to target and update.  You must not manually change, create, or modify pages in the target space, or else Junction may be unable to synchronize the state in Git with the state in Confluence.\n\nTo allow mixing code (and other items) with markdown files for Junction in a single repository, you can tell Junction a subpath within your repository that functions as the root e.g. all markdown files will be kept in `docs/`.  All files should end with the `.md` extension.\n\nThe page will gets its title from the file name, and its contents will be translated into Confluence markup.  See [this example for what output looks like in Confluence](#output-example).\n\n# Usage\n\nCollect a set of credentials that Junction will use to login to Confluence.  You will need to create an [API token](https://confluence.atlassian.com/cloud/api-tokens-938839638.html) to use instead of a password.  **I recommend you make a dedicated user account with access permissions limited to the space(s) you want to manage with Junction**.\n\nIn your git repository, create a folder structure and markdown files you would like to publish.  Commit those changes.\n```\n.\n├── (your code and other files)\n└── docs/\n    ├── Welcome.md\n    ├── Installation.md\n    └── Advanced Usage\n    |   ├── Airflow.md\n    |   ├── Visual Studio Online.md\n    |   ├── Atlassian Bamboo.md\n    |   └── GitHub Actions.md\n    └── Credits.md\n```\n\nJunction is designed as a library, and also provides "helpers" that make using it in different contexts easy (in particularly, as part of automated workflows e.g. in post-push builds).\n\nThe simplest way to use Junction is the included CLI `junction`:\n```sh\njunction -s "SPACE_KEY" -c "https://jihugh.atlassian.net/wiki/rest/api" -u "account@email.com" -p "YOUR_API_ACCESS_TOKEN" delta --content-path docs/ HEAD~5 master\n```\n> You can put the API, user, and key into environment variables to avoid specifying them for every invocation of Junction.  The variables are `CONFLUENCE_API`, `CONFLUENCE_API_USER`, and `CONFLUENCE_API_KEY` respectively.\n\nThe CLI is fully documented, so make use of the `--help` option to navigate all of the configuration options.\n\n### Dry Run\n\nYou can check what the `junction` CLI will do to your space without actually uploading the changes to Confluence by using the `--dry-run` flag.\n\n![Dry run example output](https://github.com/HUU/Junction/raw/master/docs/dry_run_example.gif?raw=true)\n\n### Python Library\n\nUsing the Python library will let you create your own wrappers and tools, for example an AirFlow DAG.  Here is an equivalent of the above CLI usage in Python:\n\n```python\nfrom pathlib import Path\nfrom git import Repo\nfrom junction.git import find_commits_on_branch_after, filter_modifications_to_folder, get_modifications\nfrom junction.delta import Delta\nfrom junction.confluence import Confluence\n\ncf = Confluence("https://jihugh.atlassian.net/wiki/rest/api", "account@email.com", "YOUR_API_ACCESS_TOKEN", "SPACE_KEY")\nrepo = Repo("."). # current working directory must be the root of the Git repository for this to work\n\ncommits = find_commits_on_branch_after("master", "HEAD~5", repo)\ndeltas = [Delta.from_modifications(filter_modifications_to_folder(get_modification(commit), Path("docs/"))) for commit in commits]\n\nfor delta in deltas:\n    delta.execute(cf)\n```\n\n# Output Example\n\nThe following markdown sample, stored in `Sample.md`, produces a page in Confluence that looks like [this](https://github.com/HUU/Junction/blob/master/docs/example_output.png?raw=true).  This shows all of the major supported features and markup.  It is intentionally very similar to GitHub-style markdown, with some extensions and differences to account for Confluence-specific features.\n\n    # Text\n\n    It\'s very easy to make some words **bold** and other words *italic* with Markdown. You can even [link to Google!](http://google.com).\n    Even some fancy formats like Subscripts~with tilde~ and Superscripts^with caret^.\n\n    # Lists\n\n    Sometimes you want numbered lists:\n\n    1. One\n    2. Two\n    3. Three\n\n    Sometimes you want bullet points:\n\n    * Start a line with a star\n    * Profit!\n\n    Alternatively,\n\n    - Dashes work just as well\n    - And if you have sub points, put four spaces before the dash or star:\n        - Like this\n        - And this\n\n    # Headers\n\n    Sometimes it\'s useful to have different levels of headings to structure your documents. Start lines with a `#` to create headings. Multiple `##` in a row denote smaller heading sizes.\n\n    ### This is a third-tier heading\n\n    You can use one `#` all the way up to `######` six for different heading sizes.\n\n    # Blockquotes\n\n    If you\'d like to quote someone, use the > character before the line:\n\n    > Coffee. The finest organic suspension ever devised... I beat the Borg with it.\n    > - Captain Janeway\n\n    # Code\n\n    You can embed `inline code fragments` by surrounding it in backticks.  For longer blocks of\n    code, use "code fencing":\n\n    ```\n    if (isAwesome){\n      return true\n    }\n    ```\n\n    And if you\'d like to use syntax highlighting, include the language:\n\n    ```php\n    <?php\n        echo "Hello World"\n    ?>\n    ```\n\n    # Tables\n\n    You can create tables by assembling a list of words and dividing them with hyphens `-` (for the first row), and then separating each column with a pipe `|`:\n\n    First Header | Second Header\n    ------------ | -------------\n    Content from cell 1 | Content from cell 2\n    Content in the first column | Content in the second column\n\n    # Confluence-specific Elements\n\n    You can link to other wiki pages by referencing their page titles.  Use normal link syntax, but prepend a `&` like &[this](Page Title).\n\n    ## Supported Macros\n\n    You can embed the Confluence child pages macro by placing it on its own line:\n\n    :include-children:\n\n    ...or the table of contents macro:\n\n    :include-toc:\n\n    ## Status Blocks\n\n    You can create Confluence status macros (colored pills), including in the middle of the line &status-green:like this;\n\n    &status-green:Complete; &status-yellow:In Progress; &status-grey:Planning; &status-red:Failed; &status-blue:Unknown; &status-purple:Cancelled;\n\n    ## Info Panels\n\n    Info: You can create info panels by prepending a paragraph with one of `Info:`, `Warning:`, `Error:`, or `Success:`.\n\n    Warning: The prefix will be removed from the contents.\n\n    Error: You cannot put multiple paragraphs inside an info panel, just a single block of text\n    like this.\n\n    Success: like other block elements, each info panel must be located on its own line (fenced between two new lines).\n\n# Contributing\n\nThis is a hobby project of mine, and I may not be able to work on it immediately upon request.   If you are interested in contributing, feel free to open a PR by following [the contribution guidelines](https://github.com/HUU/Junction/blob/master/CONTRIBUTING.md).\n',
-    'author': 'HUU',
-    'author_email': 'readabook123@protonmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/HUU/Junction',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+With Junction you can write and manage your documentation directly in your codebase, using Markdown and your existing Git workflows (pull requests, code review, release branches, etc) and then automatically publish your changes to Confluence.  This gives you the best of both worlds: in-repo documentation that fits natively into your development workflows, with the discoverability and centrality of Confluence.
 
+![MIT License](https://img.shields.io/badge/license-MIT-green) [![Python 3.8](https://img.shields.io/badge/python-3.8-blue)](https://pypi.org/project/confluence-junction) ![Build and Test](https://github.com/HUU/Junction/workflows/Build%20and%20Test/badge.svg)
+
+# Install
+
+Ensure you are using Python 3.8 (or newer); Junction does not work with older versions of Python.  Install using `pip`:
+```sh
+pip install confluence-junction
+```
+This will install the library and CLI.
+In your Python code:
+```python
+import junction
+```
+In your shell:
+```sh
+junction --help
+```
+
+# Overview
+
+Junction works by inspecting the changes made on a commit-by-commit basis to your Git repository, and determining what needs to be changed in Confluence to reflect those changes.  Junction (currently) expects to manage the entire [space in Confluence](https://confluence.atlassian.com/doc/spaces-139459.html).  Thus when using Junction you must tell it which Space to target and update.  You must not manually change, create, or modify pages in the target space, or else Junction may be unable to synchronize the state in Git with the state in Confluence.
+
+To allow mixing code (and other items) with markdown files for Junction in a single repository, you can tell Junction a subpath within your repository that functions as the root e.g. all markdown files will be kept in `docs/`.  All files should end with the `.md` extension.
+
+The page will gets its title from the file name, and its contents will be translated into Confluence markup.  See [this example for what output looks like in Confluence](#output-example).
+
+# Usage
+
+Collect a set of credentials that Junction will use to login to Confluence.  You will need to create an [API token](https://confluence.atlassian.com/cloud/api-tokens-938839638.html) to use instead of a password.  **I recommend you make a dedicated user account with access permissions limited to the space(s) you want to manage with Junction**.
+
+In your git repository, create a folder structure and markdown files you would like to publish.  Commit those changes.
+```
+.
+├── (your code and other files)
+└── docs/
+    ├── Welcome.md
+    ├── Installation.md
+    └── Advanced Usage
+    |   ├── Airflow.md
+    |   ├── Visual Studio Online.md
+    |   ├── Atlassian Bamboo.md
+    |   └── GitHub Actions.md
+    └── Credits.md
+```
+
+Junction is designed as a library, and also provides "helpers" that make using it in different contexts easy (in particularly, as part of automated workflows e.g. in post-push builds).
+
+The simplest way to use Junction is the included CLI `junction`:
+```sh
+junction -s "SPACE_KEY" -c "https://jihugh.atlassian.net/wiki/rest/api" -u "account@email.com" -p "YOUR_API_ACCESS_TOKEN" delta --content-path docs/ HEAD~5 master
+```
+> You can put the API, user, and key into environment variables to avoid specifying them for every invocation of Junction.  The variables are `CONFLUENCE_API`, `CONFLUENCE_API_USER`, and `CONFLUENCE_API_KEY` respectively.
+
+The CLI is fully documented, so make use of the `--help` option to navigate all of the configuration options.
+
+### Dry Run
+
+You can check what the `junction` CLI will do to your space without actually uploading the changes to Confluence by using the `--dry-run` flag.
+
+![Dry run example output](https://github.com/HUU/Junction/raw/master/docs/dry_run_example.gif?raw=true)
+
+### Python Library
+
+Using the Python library will let you create your own wrappers and tools, for example an AirFlow DAG.  Here is an equivalent of the above CLI usage in Python:
+
+```python
+from pathlib import Path
+from git import Repo
+from junction.git import find_commits_on_branch_after, filter_modifications_to_folder, get_modifications
+from junction.delta import Delta
+from junction.confluence import Confluence
+
+cf = Confluence("https://jihugh.atlassian.net/wiki/rest/api", "account@email.com", "YOUR_API_ACCESS_TOKEN", "SPACE_KEY")
+repo = Repo("."). # current working directory must be the root of the Git repository for this to work
+
+commits = find_commits_on_branch_after("master", "HEAD~5", repo)
+deltas = [Delta.from_modifications(filter_modifications_to_folder(get_modification(commit), Path("docs/"))) for commit in commits]
+
+for delta in deltas:
+    delta.execute(cf)
+```
+
+# Output Example
+
+The following markdown sample, stored in `Sample.md`, produces a page in Confluence that looks like [this](https://github.com/HUU/Junction/blob/master/docs/example_output.png?raw=true).  This shows all of the major supported features and markup.  It is intentionally very similar to GitHub-style markdown, with some extensions and differences to account for Confluence-specific features.
+
+    # Text
+
+    It's very easy to make some words **bold** and other words *italic* with Markdown. You can even [link to Google!](http://google.com).
+    Even some fancy formats like Subscripts~with tilde~ and Superscripts^with caret^.
+
+    # Lists
+
+    Sometimes you want numbered lists:
+
+    1. One
+    2. Two
+    3. Three
+
+    Sometimes you want bullet points:
+
+    * Start a line with a star
+    * Profit!
+
+    Alternatively,
+
+    - Dashes work just as well
+    - And if you have sub points, put four spaces before the dash or star:
+        - Like this
+        - And this
+
+    # Headers
+
+    Sometimes it's useful to have different levels of headings to structure your documents. Start lines with a `#` to create headings. Multiple `##` in a row denote smaller heading sizes.
+
+    ### This is a third-tier heading
+
+    You can use one `#` all the way up to `######` six for different heading sizes.
+
+    # Blockquotes
+
+    If you'd like to quote someone, use the > character before the line:
+
+    > Coffee. The finest organic suspension ever devised... I beat the Borg with it.
+    > - Captain Janeway
+
+    # Code
+
+    You can embed `inline code fragments` by surrounding it in backticks.  For longer blocks of
+    code, use "code fencing":
+
+    ```
+    if (isAwesome){
+      return true
+    }
+    ```
+
+    And if you'd like to use syntax highlighting, include the language:
+
+    ```php
+    <?php
+        echo "Hello World"
+    ?>
+    ```
+
+    # Tables
+
+    You can create tables by assembling a list of words and dividing them with hyphens `-` (for the first row), and then separating each column with a pipe `|`:
+
+    First Header | Second Header
+    ------------ | -------------
+    Content from cell 1 | Content from cell 2
+    Content in the first column | Content in the second column
+
+    # Confluence-specific Elements
+
+    You can link to other wiki pages by referencing their page titles.  Use normal link syntax, but prepend a `&` like &[this](Page Title).
+
+    ## Supported Macros
+
+    You can embed the Confluence child pages macro by placing it on its own line:
+
+    :include-children:
+
+    ...or the table of contents macro:
+
+    :include-toc:
+
+    ## Status Blocks
+
+    You can create Confluence status macros (colored pills), including in the middle of the line &status-green:like this;
+
+    &status-green:Complete; &status-yellow:In Progress; &status-grey:Planning; &status-red:Failed; &status-blue:Unknown; &status-purple:Cancelled;
+
+    ## Info Panels
+
+    Info: You can create info panels by prepending a paragraph with one of `Info:`, `Warning:`, `Error:`, or `Success:`.
+
+    Warning: The prefix will be removed from the contents.
+
+    Error: You cannot put multiple paragraphs inside an info panel, just a single block of text
+    like this.
+
+    Success: like other block elements, each info panel must be located on its own line (fenced between two new lines).
+
+# Contributing
+
+This is a hobby project of mine, and I may not be able to work on it immediately upon request.   If you are interested in contributing, feel free to open a PR by following [the contribution guidelines](https://github.com/HUU/Junction/blob/master/CONTRIBUTING.md).
 
-setup(**setup_kwargs)
```

