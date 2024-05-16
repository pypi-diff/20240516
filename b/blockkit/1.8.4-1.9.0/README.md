# Comparing `tmp/blockkit-1.8.4.tar.gz` & `tmp/blockkit-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockkit-1.8.4.tar", last modified: Tue May  7 11:00:18 2024, max compression
+gzip compressed data, was "blockkit-1.9.0.tar", last modified: Thu May 16 10:34:28 2024, max compression
```

## Comparing `blockkit-1.8.4.tar` & `blockkit-1.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:18.614948 blockkit-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 11:00:14.000000 blockkit-1.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 11:00:14.000000 blockkit-1.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-07 11:00:18.614948 blockkit-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-07 11:00:14.000000 blockkit-1.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:18.610948 blockkit-1.8.4/blockkit/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/components.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/display.py
--rw-r--r--   0 runner    (1001) docker     (127)    22902 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/surfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-07 11:00:14.000000 blockkit-1.8.4/blockkit/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:18.614948 blockkit-1.8.4/blockkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-07 11:00:18.000000 blockkit-1.8.4/blockkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-07 11:00:18.000000 blockkit-1.8.4/blockkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 11:00:18.000000 blockkit-1.8.4/blockkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 11:00:18.000000 blockkit-1.8.4/blockkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 11:00:18.000000 blockkit-1.8.4/blockkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 11:00:18.614948 blockkit-1.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-07 11:00:14.000000 blockkit-1.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 11:00:18.614948 blockkit-1.8.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-05-07 11:00:14.000000 blockkit-1.8.4/tests/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-07 11:00:14.000000 blockkit-1.8.4/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (127)    52104 2024-05-07 11:00:14.000000 blockkit-1.8.4/tests/test_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)    51891 2024-05-07 11:00:14.000000 blockkit-1.8.4/tests/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-05-07 11:00:14.000000 blockkit-1.8.4/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-05-07 11:00:14.000000 blockkit-1.8.4/tests/test_surfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:34:28.538929 blockkit-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-16 10:34:24.000000 blockkit-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 10:34:24.000000 blockkit-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-16 10:34:28.538929 blockkit-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4555 2024-05-16 10:34:24.000000 blockkit-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:34:28.538929 blockkit-1.9.0/blockkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-16 10:34:24.000000 blockkit-1.9.0/blockkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-16 10:34:24.000000 blockkit-1.9.0/blockkit/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-16 10:34:24.000000 blockkit-1.9.0/blockkit/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-16 10:34:24.000000 blockkit-1.9.0/blockkit/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24763 2024-05-16 10:34:24.000000 blockkit-1.9.0/blockkit/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-16 10:34:24.000000 blockkit-1.9.0/blockkit/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-05-16 10:34:24.000000 blockkit-1.9.0/blockkit/generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-16 10:34:24.000000 blockkit-1.9.0/blockkit/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4134 2024-05-16 10:34:24.000000 blockkit-1.9.0/blockkit/surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-16 10:34:24.000000 blockkit-1.9.0/blockkit/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:34:28.538929 blockkit-1.9.0/blockkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-05-16 10:34:28.000000 blockkit-1.9.0/blockkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-16 10:34:28.000000 blockkit-1.9.0/blockkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 10:34:28.000000 blockkit-1.9.0/blockkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 10:34:28.000000 blockkit-1.9.0/blockkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 10:34:28.000000 blockkit-1.9.0/blockkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 10:34:28.538929 blockkit-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-16 10:34:24.000000 blockkit-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 10:34:28.538929 blockkit-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-05-16 10:34:24.000000 blockkit-1.9.0/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-16 10:34:24.000000 blockkit-1.9.0/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54137 2024-05-16 10:34:24.000000 blockkit-1.9.0/tests/test_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51891 2024-05-16 10:34:24.000000 blockkit-1.9.0/tests/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-05-16 10:34:24.000000 blockkit-1.9.0/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-05-16 10:34:24.000000 blockkit-1.9.0/tests/test_surfaces.py
```

### Comparing `blockkit-1.8.4/LICENSE` & `blockkit-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.4/PKG-INFO` & `blockkit-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: blockkit
-Version: 1.8.4
+Version: 1.9.0
 Summary: A fast way to build Block Kit interfaces in Python.
 Home-page: https://github.com/imryche/blockkit
 Author: Dmitry Chernyshov
 Author-email: imryche13@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pydantic<3,>=2
+Requires-Dist: pydantic[email]<3,>=2
 Provides-Extra: gen
 Requires-Dist: black; extra == "gen"
 
 
 ![Screenshot](https://github.com/imryche/blockkit/raw/master/images/logo.png)
 
 ![Build status](https://github.com/imryche/blockkit/actions/workflows/python-app.yml/badge.svg)
```

### Comparing `blockkit-1.8.4/README.md` & `blockkit-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.4/blockkit/blocks.py` & `blockkit-1.9.0/blockkit/blocks.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.4/blockkit/components.py` & `blockkit-1.9.0/blockkit/components.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.4/blockkit/display.py` & `blockkit-1.9.0/blockkit/display.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.4/blockkit/elements.py` & `blockkit-1.9.0/blockkit/elements.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import itertools
 from datetime import date, datetime, time
 from typing import List, Optional, Union
 
-from pydantic import AnyUrl, Field, model_validator
+from pydantic import AnyUrl, EmailStr, Field, model_validator
 from pydantic.networks import HttpUrl
 
 from blockkit.components import Component
 from blockkit.enums import ListStyle, Style
 from blockkit.objects import (
     Confirm,
     DispatchActionConfig,
@@ -48,14 +48,16 @@
     "UsersSelect",
     "NumberInput",
     "RichTextPreformatted",
     "RichTextQuote",
     "RichTextSection",
     "RichTextList",
     "FileInput",
+    "EmailTextInput",
+    "URLTextInput",
 ]
 
 
 class ActionableComponent(Component):
     action_id: Optional[str] = Field(None, min_length=1, max_length=255)
 
 
@@ -734,7 +736,62 @@
     ):
         super().__init__(
             action_id=action_id,
             filetypes=filetypes,
             max_files=max_files,
         )
 
+
+class EmailTextInput(FocusableElement):
+    type: str = "email_text_input"
+    placeholder: Union[PlainText, str, None] = None
+    initial_value: Optional[EmailStr] = None
+    dispatch_action_config: Optional[DispatchActionConfig] = None
+
+    _validate_placeholder = validator(
+        "placeholder", validate_text_length, max_length=150
+    )
+
+    def __init__(
+        self,
+        *,
+        action_id: Optional[str] = None,
+        placeholder: Union[PlainText, str, None] = None,
+        initial_value: Optional[EmailStr] = None,
+        dispatch_action_config: Optional[DispatchActionConfig] = None,
+        focus_on_load: Optional[bool] = None,
+    ):
+        super().__init__(
+            action_id=action_id,
+            placeholder=placeholder,
+            initial_value=initial_value,
+            dispatch_action_config=dispatch_action_config,
+            focus_on_load=focus_on_load,
+        )
+
+
+class URLTextInput(FocusableElement):
+    type: str = "url_text_input"
+    placeholder: Union[PlainText, str, None] = None
+    initial_value: Optional[AnyUrl] = None
+    dispatch_action_config: Optional[DispatchActionConfig] = None
+
+    _validate_placeholder = validator(
+        "placeholder", validate_text_length, max_length=150
+    )
+
+    def __init__(
+        self,
+        *,
+        action_id: Optional[str] = None,
+        placeholder: Union[PlainText, str, None] = None,
+        initial_value: Optional[AnyUrl] = None,
+        dispatch_action_config: Optional[DispatchActionConfig] = None,
+        focus_on_load: Optional[bool] = None,
+    ):
+        super().__init__(
+            action_id=action_id,
+            placeholder=placeholder,
+            initial_value=initial_value,
+            dispatch_action_config=dispatch_action_config,
+            focus_on_load=focus_on_load,
+        )
```

### Comparing `blockkit-1.8.4/blockkit/generators.py` & `blockkit-1.9.0/blockkit/generators.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.4/blockkit/objects.py` & `blockkit-1.9.0/blockkit/objects.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.4/blockkit/surfaces.py` & `blockkit-1.9.0/blockkit/surfaces.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.4/blockkit/validators.py` & `blockkit-1.9.0/blockkit/validators.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,8 +48,9 @@
 def validate_datetime(v: Union[int, datetime]) -> Optional[int]:
     if v is not None:
         if type(v) == datetime:
             return int(v.timestamp())
         else:
             _ = datetime.fromtimestamp(v)
             return v
-    return v
+    return v
+
```

### Comparing `blockkit-1.8.4/blockkit.egg-info/PKG-INFO` & `blockkit-1.9.0/blockkit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: blockkit
-Version: 1.8.4
+Version: 1.9.0
 Summary: A fast way to build Block Kit interfaces in Python.
 Home-page: https://github.com/imryche/blockkit
 Author: Dmitry Chernyshov
 Author-email: imryche13@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pydantic<3,>=2
+Requires-Dist: pydantic[email]<3,>=2
 Provides-Extra: gen
 Requires-Dist: black; extra == "gen"
 
 
 ![Screenshot](https://github.com/imryche/blockkit/raw/master/images/logo.png)
 
 ![Build status](https://github.com/imryche/blockkit/actions/workflows/python-app.yml/badge.svg)
```

### Comparing `blockkit-1.8.4/blockkit.egg-info/SOURCES.txt` & `blockkit-1.9.0/blockkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.4/setup.py` & `blockkit-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 # Package meta-data.
 NAME = "blockkit"
 DESCRIPTION = "A fast way to build Block Kit interfaces in Python."
 URL = "https://github.com/imryche/blockkit"
 EMAIL = "imryche13@gmail.com"
 AUTHOR = "Dmitry Chernyshov"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "1.8.4"
+VERSION = "1.9.0"
 
-REQUIRED = ["pydantic>=2,<3"]
+REQUIRED = ["pydantic[email]>=2,<3"]
 EXTRAS = {"gen": ["black"]}
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Import the README and use it as the long-description.
 try:
     with open(os.path.join(here, "README.md"), encoding="utf-8") as f:
```

### Comparing `blockkit-1.8.4/tests/test_blocks.py` & `blockkit-1.9.0/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.4/tests/test_components.py` & `blockkit-1.9.0/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.4/tests/test_elements.py` & `blockkit-1.9.0/tests/test_elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from blockkit.elements import (
     Button,
     ChannelsSelect,
     Checkboxes,
     ConversationsSelect,
     DatePicker,
     DatetimePicker,
+    EmailTextInput,
     ExternalSelect,
     FileInput,
     Image,
     MultiChannelsSelect,
     MultiConversationsSelect,
     MultiExternalSelect,
     MultiStaticSelect,
@@ -24,14 +25,15 @@
     RadioButtons,
     RichTextList,
     RichTextPreformatted,
     RichTextQuote,
     RichTextSection,
     StaticSelect,
     TimePicker,
+    URLTextInput,
     UsersSelect,
 )
 from blockkit.objects import (
     Confirm,
     DispatchActionConfig,
     Emoji,
     Filter,
@@ -1576,7 +1578,64 @@
     }
 
 
 def test_fileinput_excessive_max_files_raises_exception():
     with pytest.raises(ValidationError):
         FileInput(max_files=11)
 
+
+def test_builds_email_text_input():
+    assert EmailTextInput(
+        action_id="action_id",
+        initial_value="dima@botsignals.co",
+        dispatch_action_config=DispatchActionConfig(
+            trigger_actions_on=["on_character_entered"]
+        ),
+        focus_on_load=True,
+        placeholder=PlainText(text="placeholder"),
+    ).build() == {
+        "type": "email_text_input",
+        "action_id": "action_id",
+        "initial_value": "dima@botsignals.co",
+        "dispatch_action_config": {"trigger_actions_on": ["on_character_entered"]},
+        "focus_on_load": True,
+        "placeholder": {"type": "plain_text", "text": "placeholder"},
+    }
+
+
+def test_email_text_input_excessive_placeholder_raises_exception():
+    with pytest.raises(ValidationError):
+        EmailTextInput(placeholder=PlainText(text="p" * 151))
+
+
+def test_email_text_input_invalid_initial_value_raises_exception():
+    with pytest.raises(ValidationError):
+        EmailTextInput(initial_value="dimabotsignals.co")
+
+
+def test_builds_url_text_input():
+    assert URLTextInput(
+        action_id="action_id",
+        initial_value="https://example.com/",
+        dispatch_action_config=DispatchActionConfig(
+            trigger_actions_on=["on_character_entered"]
+        ),
+        focus_on_load=True,
+        placeholder=PlainText(text="placeholder"),
+    ).build() == {
+        "type": "url_text_input",
+        "action_id": "action_id",
+        "initial_value": "https://example.com/",
+        "dispatch_action_config": {"trigger_actions_on": ["on_character_entered"]},
+        "focus_on_load": True,
+        "placeholder": {"type": "plain_text", "text": "placeholder"},
+    }
+
+
+def test_url_text_input_excessive_placeholder_raises_exception():
+    with pytest.raises(ValidationError):
+        URLTextInput(placeholder=PlainText(text="p" * 151))
+
+
+def test_url_text_input_invalid_initial_value_raises_exception():
+    with pytest.raises(ValidationError):
+        URLTextInput(initial_value="foo bar")
```

### Comparing `blockkit-1.8.4/tests/test_generators.py` & `blockkit-1.9.0/tests/test_generators.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.4/tests/test_objects.py` & `blockkit-1.9.0/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `blockkit-1.8.4/tests/test_surfaces.py` & `blockkit-1.9.0/tests/test_surfaces.py`

 * *Files identical despite different names*

