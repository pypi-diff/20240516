# Comparing `tmp/prefect_slack-0.2.4.tar.gz` & `tmp/prefect_slack-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_slack-0.2.4.tar", last modified: Fri Apr 26 15:04:08 2024, max compression
+gzip compressed data, was "prefect_slack-0.2.5.tar", last modified: Fri May  3 16:56:48 2024, max compression
```

## Comparing `prefect_slack-0.2.4.tar` & `prefect_slack-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.386895 prefect_slack-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-26 15:04:08.386895 prefect_slack-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.382895 prefect_slack-0.2.4/prefect_slack/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/prefect_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:04:08.000000 prefect_slack-0.2.4/prefect_slack/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/prefect_slack/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/prefect_slack/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.386895 prefect_slack-0.2.4/prefect_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-04-26 15:04:08.000000 prefect_slack-0.2.4/prefect_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-26 15:04:08.000000 prefect_slack-0.2.4/prefect_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:04:08.000000 prefect_slack-0.2.4/prefect_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 15:04:08.000000 prefect_slack-0.2.4/prefect_slack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-26 15:04:08.000000 prefect_slack-0.2.4/prefect_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-26 15:04:08.000000 prefect_slack-0.2.4/prefect_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:04:08.386895 prefect_slack-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:08.386895 prefect_slack-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/tests/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-26 15:03:49.000000 prefect_slack-0.2.4/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:48.648417 prefect_slack-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-03 16:56:48.648417 prefect_slack-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:48.644417 prefect_slack-0.2.5/prefect_slack/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/prefect_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-03 16:56:48.000000 prefect_slack-0.2.5/prefect_slack/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/prefect_slack/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/prefect_slack/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:48.644417 prefect_slack-0.2.5/prefect_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-03 16:56:48.000000 prefect_slack-0.2.5/prefect_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-03 16:56:48.000000 prefect_slack-0.2.5/prefect_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 16:56:48.000000 prefect_slack-0.2.5/prefect_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-03 16:56:48.000000 prefect_slack-0.2.5/prefect_slack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-03 16:56:48.000000 prefect_slack-0.2.5/prefect_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-03 16:56:48.000000 prefect_slack-0.2.5/prefect_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 16:56:48.648417 prefect_slack-0.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 16:56:48.644417 prefect_slack-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/tests/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/tests/test_notification_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-03 16:56:34.000000 prefect_slack-0.2.5/tests/test_version.py
```

### Comparing `prefect_slack-0.2.4/LICENSE` & `prefect_slack-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.4/PKG-INFO` & `prefect_slack-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-slack
-Version: 0.2.4
+Version: 0.2.5
 Summary: Prefect integrations with Slack
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-slack
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `prefect_slack-0.2.4/README.md` & `prefect_slack-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.4/prefect_slack/messages.py` & `prefect_slack-0.2.5/prefect_slack/messages.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Tasks for sending Slack messages"""
+"""Tasks for sending Slack messages."""
 
 from typing import TYPE_CHECKING, Dict, Optional, Sequence, Union
 
 from prefect import get_run_logger, task
 from prefect_slack.credentials import SlackCredentials, SlackWebhook
 
 if TYPE_CHECKING:  # pragma: no cover
@@ -19,38 +19,38 @@
         Sequence[Union[Dict, "slack_sdk.models.attachments.Attachment"]]
     ] = None,
     slack_blocks: Optional[
         Sequence[Union[Dict, "slack_sdk.models.blocks.Block"]]
     ] = None,
 ) -> Dict:
     """
-    Sends a message to a Slack channel
+    Sends a message to a Slack channel.
 
     Args:
         channel: The name of the channel in which to post the chat message
-            (e.g. #general)
+            (e.g. #general).
         slack_credentials: Instance of `SlackCredentials` initialized with a Slack
-            bot token
+            bot token.
         text: Contents of the message. It's a best practice to always provide a `text`
             argument when posting a message. The `text` argument is used in places where
             content cannot be rendered such as: system push notifications, assistive
             technology such as screen readers, etc.
         attachments: List of objects defining secondary context in the posted Slack
             message. The [Slack API docs](https://api.slack.com/messaging/composing/layouts#building-attachments)
             provide guidance on building attachments.
         slack_blocks: List of objects defining the layout and formatting of the posted
             message. The [Slack API docs](https://api.slack.com/block-kit/building)
             provide guidance on building messages with blocks.
 
     Returns:
         Dict: Response from the Slack API. Example response structures can be found in
-            the [Slack API docs](https://api.slack.com/methods/chat.postMessage#examples)
+            the [Slack API docs](https://api.slack.com/methods/chat.postMessage#examples).
 
-    Examples:
-        Post a message at the end of a flow run
+    Example:
+        Post a message at the end of a flow run.
 
         ```python
         from prefect import flow
         from prefect.context import get_run_context
         from prefect_slack import SlackCredentials
         from prefect_slack.messages import send_chat_message
 
@@ -89,15 +89,15 @@
         Sequence[Union[Dict, "slack_sdk.models.attachments.Attachment"]]
     ] = None,
     slack_blocks: Optional[
         Sequence[Union[Dict, "slack_sdk.models.blocks.Block"]]
     ] = None,
 ) -> None:
     """
-    Sends a message via an incoming webhook
+    Sends a message via an incoming webhook.
 
     Args:
         slack_webhook: Instance of `SlackWebhook` initialized with a Slack
             webhook URL.
         text: Contents of the message. It's a best practice to always provide a `text`
             argument when posting a message. The `text` argument is used in places where
             content cannot be rendered such as: system push notifications, assistive
@@ -105,16 +105,16 @@
         attachments: List of objects defining secondary context in the posted Slack
             message. The [Slack API docs](https://api.slack.com/messaging/composing/layouts#building-attachments)
             provide guidance on building attachments.
         slack_blocks: List of objects defining the layout and formatting of the posted
             message. The [Slack API docs](https://api.slack.com/block-kit/building)
             provide guidance on building messages with blocks.
 
-    Examples:
-        Post a message at the end of a flow run
+    Example:
+        Post a message at the end of a flow run.
 
         ```python
         from prefect import flow
         from prefect_slack import SlackWebhook
         from prefect_slack.messages import send_incoming_webhook_message
```

### Comparing `prefect_slack-0.2.4/prefect_slack.egg-info/PKG-INFO` & `prefect_slack-0.2.5/prefect_slack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-slack
-Version: 0.2.4
+Version: 0.2.5
 Summary: Prefect integrations with Slack
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-slack
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
```

### Comparing `prefect_slack-0.2.4/pyproject.toml` & `prefect_slack-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.4/tests/conftest.py` & `prefect_slack-0.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_slack-0.2.4/tests/test_messages.py` & `prefect_slack-0.2.5/tests/test_messages.py`

 * *Files identical despite different names*

