# Comparing `tmp/direct7-0.0.6.tar.gz` & `tmp/direct7-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon May 13 06:17:17 2024, from Unix
+gzip compressed data, last modified: Thu May 16 05:23:36 2024, from Unix
```

## Comparing `direct7-0.0.6.tar` & `direct7-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 direct7-0.0.6/main.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 direct7-0.0.6/src/direct7/__init__.py
--rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 direct7-0.0.6/src/direct7/client.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 direct7-0.0.6/src/direct7/errors.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 direct7-0.0.6/src/direct7/number_lookup.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 direct7-0.0.6/src/direct7/slack.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 direct7-0.0.6/src/direct7/sms.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 direct7-0.0.6/src/direct7/verify.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 direct7-0.0.6/src/direct7/viber.py
--rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 direct7-0.0.6/src/direct7/whatsapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 direct7-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     6078 2020-02-02 00:00:00.000000 direct7-0.0.6/tests/test_sdk.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 direct7-0.0.6/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 direct7-0.0.6/LICENSE
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 direct7-0.0.6/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 direct7-0.0.6/pyproject.toml
--rw-r--r--   0 sisira    (1000) sisira    (1000)     7305 2024-05-13 06:17:16.000000 direct7-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 direct7-0.0.7/main.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/__init__.py
+-rw-r--r--   0        0        0     5778 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/client.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/errors.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/number_lookup.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/slack.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/sms.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/verify.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/viber.py
+-rw-r--r--   0        0        0    10572 2020-02-02 00:00:00.000000 direct7-0.0.7/src/direct7/whatsapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 direct7-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0    14774 2020-02-02 00:00:00.000000 direct7-0.0.7/tests/test_sdk.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 direct7-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 direct7-0.0.7/LICENSE
+-rw-r--r--   0        0        0     6720 2020-02-02 00:00:00.000000 direct7-0.0.7/README.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 direct7-0.0.7/pyproject.toml
+-rw-r--r--   0 sisira    (1000) sisira    (1000)     7264 2024-05-16 05:23:35.000000 direct7-0.0.7/PKG-INFO
```

### Comparing `direct7-0.0.6/src/direct7/client.py` & `direct7-0.0.7/src/direct7/client.py`

 * *Files identical despite different names*

### Comparing `direct7-0.0.6/src/direct7/number_lookup.py` & `direct7-0.0.7/src/direct7/number_lookup.py`

 * *Files identical despite different names*

### Comparing `direct7-0.0.6/src/direct7/slack.py` & `direct7-0.0.7/src/direct7/slack.py`

 * *Files identical despite different names*

### Comparing `direct7-0.0.6/src/direct7/sms.py` & `direct7-0.0.7/src/direct7/sms.py`

 * *Files identical despite different names*

### Comparing `direct7-0.0.6/src/direct7/verify.py` & `direct7-0.0.7/src/direct7/verify.py`

 * *Files identical despite different names*

### Comparing `direct7-0.0.6/src/direct7/viber.py` & `direct7-0.0.7/src/direct7/viber.py`

 * *Files identical despite different names*

### Comparing `direct7-0.0.6/src/direct7/whatsapp.py` & `direct7-0.0.7/src/direct7/whatsapp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 import logging
+import uuid
 
 log = logging.getLogger(__name__)
 
 
 class WHATSAPP:
 
     def __init__(self, client):
         self._client = client
 
     def send_whatsapp_freeform_message(self, originator: str, recipient: str, message_type: str, first_name: str = None,
-                                       last_name: str = None, formatted_name: str = None, birthday: str = None,
+                                       last_name: str = None, formatted_name: str = None, middle_name: str = None,
+                                       suffix: str = None, prefix: str = None, birthday: str = None,
                                        phones: list = None,
                                        emails: list = None, urls: list = None, latitude: str = None,
                                        longitude: str = None,
                                        name: str = None, address: str = None,
-                                       type: str = None, url: str = None, caption: str = None, body: str = None):
+                                       type: str = None, url: str = None, caption: str = None, body: str = None,
+                                       message_id: uuid.UUID = None, emoji: str = None,
+                                       contact_addresses: list = None, ):
         """
         Send a WhatsApp message to a single/multiple recipients.
+        :param prefix: Prefix for the contact's name, such as Mr., Ms., Dr., etc.
+        :param suffix: Suffix for the contact's name, if applicable.
+        :param middle_name: Contact's middle name.
+        :param contact_addresses:
+        :param emoji:
+        :param message_id:
+        :param birthday: Contact's birthday in YYYY-MM-DD format.
         :param originator: str - The message originator.
         :param recipient: str - The message recipient.
         :param message_type: str - The type of message ("CONTACTS", "LOCATION", "ATTACHMENT", "TEXT").
         :param first_name: str - First name for "CONTACTS" message type.
         :param last_name: str - Last name for "CONTACTS" message type.
         :param formatted_name: str - Display name for "CONTACTS" message type.
         :param phones: list - Phone number for "CONTACTS" message type.
@@ -45,19 +56,23 @@
 
         if message_type == "CONTACTS":
             message["content"]["contacts"] = [{
                 "name": {
                     "first_name": first_name,
                     "last_name": last_name,
                     "formatted_name": formatted_name,
+                    "middle_name": middle_name,
+                    "suffix": suffix,
+                    "prefix": prefix,
                 },
+                "addresses": contact_addresses,
                 "birthday": birthday,
-                "phones": [{"phone": phone} for phone in phones] if phones else None,
-                "emails": [{"email": email} for email in emails] if emails else None,
-                "urls": [{"url": url} for url in urls if urls] if urls else None
+                "phones": phones,
+                "emails": emails,
+                "urls": urls
             }]
         elif message_type == "LOCATION":
             message["content"]["location"] = {
                 "latitude": latitude,
                 "longitude": longitude,
                 "name": name,
                 "address": address
@@ -69,25 +84,32 @@
                 "caption": caption
             }
         elif message_type == "TEXT":
             message["content"]["text"] = {
                 "body": body
             }
 
+        elif message_type == "REACTION":
+            message["content"]["reaction"] = {
+                "message_id": message_id,
+                "emoji": emoji
+            }
+
         response = self._client.post(
             self._client.host(), "/whatsapp/v2/send", params={"messages": [message]})
         log.info("Message sent successfully.")
         return response
 
     def send_whatsapp_templated_message(self, originator: str, recipient: str, template_id: str,
                                         body_parameter_values: dict = {}, media_type: str = None,
                                         media_url: str = None,
                                         latitude: str = None, longitude: str = None, location_name: str = None,
                                         location_address: str = None, lto_expiration_time_ms: str = None,
-                                        coupon_code: str = None, quick_replies: dict = None, actions: dict = None, carousel_cards: list = []):
+                                        coupon_code: str = None, quick_replies: dict = None, actions: dict = None,
+                                        carousel_cards: list = []):
         """
         Send a WhatsApp message to a single/multiple recipients.
         :param originator: str - The message originator.
         :param recipient: str - The message recipient.
         :param template_id: str - The template ID for text messages.
         :param body_parameter_values: dict - The body parameter values for text templates.
         :param media_type: str - The type of media (e.g., "image", "video").
@@ -146,14 +168,73 @@
             }
 
         response = self._client.post(
             self._client.host(), "/whatsapp/v2/send", params={"messages": [message]})
         log.info("Message sent successfully.")
         return response
 
+    def send_whatsapp_interactive_message(self, originator: str, recipient: str, interactive_type: str,
+                                          header_type: str = None, header_text: str = None,
+                                          header_link: str = None, header_file_name: str = None, body_text: str = None,
+                                          footer_text: str = None, parameters: dict = None, sections: list = None,
+                                          buttons: list = None, list_button_text: str = None, ):
+        """
+        Send a WhatsApp interactive message to a single/multiple recipients.
+        :param originator: str - The message originator.
+        :param recipient: str - The message recipient.
+        :param interactive_type:
+
+        """
+        message = {
+            "originator": originator,
+            "recipients": [{"recipient": recipient}],
+            "content": {
+                "message_type": "INTERACTIVE",
+                "interactive": {
+                    "type": interactive_type,
+                    "header": {
+                        "type": header_type,
+                    },
+                    "body": {
+                        "text": body_text,
+                    },
+                    "footer": {
+                        "text": footer_text,
+                    }
+                }
+            }
+        }
+        if header_type == "text":
+            message["content"]["interactive"]["header"]["text"] = header_text
+
+        elif header_type == "image" or header_type == "video" or header_type == "document":
+            message["content"]["interactive"]["header"][header_type] = {
+                "filename": header_file_name if header_type == "document" else None,
+                "link": header_link
+            }
+
+        if interactive_type == "cta_url":
+            message["content"]["interactive"]["action"] = {
+                "parameters": parameters,
+            }
+        elif interactive_type == "button":
+            message["content"]["interactive"]["action"] = {
+                "buttons": buttons,
+            }
+        elif interactive_type == "list":
+            message["content"]["interactive"]["action"] = {
+                "sections": sections,
+                "button": list_button_text
+            }
+
+        response = self._client.post(
+            self._client.host(), "/whatsapp/v2/send", params={"messages": [message]})
+        log.info("Message sent successfully.")
+        return response
+
     def get_status(self, request_id: str):
         """
         Get the status for a whatsapp message request.
         :param params:
         request_id : str - The request ID of the whatsapp message request.
         :return:
         """
```

### Comparing `direct7-0.0.6/.gitignore` & `direct7-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `direct7-0.0.6/LICENSE` & `direct7-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `direct7-0.0.6/README.md` & `direct7-0.0.7/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
 ```python
 from direct7 import Client
 
 client = Client(api_token="Your API token")
 
 client.sms.send_messages(
-        {"recipients": ["+9199XXXXXXXXXX"],"content": "مرحبا بالعالم!", "unicode": True},
+        {"recipients": ["+9199XXXXXXXX"],"content": "مرحبا بالعالم!", "unicode": True},
         originator="Sender",
         report_url="https://the_url_to_receive_delivery_report.com",
         )
 ```
 
 ### Check SMS Request Status
 
@@ -117,37 +117,36 @@
 # otp_id is the id returned in the response of send_otp
 client.verify.get_status(otp_id="0012c7f5-2ba5-49db-8901-4ee9be6dc8d1")
 ```
 
 
 ### Whatsapp
 
-### Send Whatsapp Free-form Message (Contact Details)
+### Send Whatsapp Free-form Message (Location Details)
 
 ```python
 from direct7 import Client
 
 client = Client(api_token="Your API token")
 
-client.whatsapp.send_whatsapp_freeform_message( originator="9181XXXXXXXX",
-                                                recipient="9190XXXXXXXX",
-                                                message_type="CONTACTS", first_name="Amal",
-                                                last_name="Anu", formatted_name="Amal Anu",
-                                                phones=["9181XXXXXXXX", "9181XXXXXXXX"],
-                                                emails=["amal@gmail.com", "amal2@gmail1.com"])
+client.whatsapp.send_whatsapp_freeform_message(originator="91906152XXXX",
+                                               recipient="91906112XXXX",
+                                                message_type="LOCATION", latitude="12.93803129081362",
+                                                longitude="77.61088653615994",
+                                                name="Mobile Pvt Ltd", address="30, Hosur Rd, 7th Block, Koramangala, Bengaluru, Karnataka 560095")
 ```
 
 ### Send Whatsapp Templated Message.
 
 ```python
 from direct7 import Client
 
 client = Client(api_token="Your API token")
 
-client.whatsapp.send_whatsapp_templated_message(originator="91906152XXXX", recipient="91906152XXXX", template_id="monthly_promotion", body_parameter_values={"0": "promotion"})
+client.whatsapp.send_whatsapp_templated_message(originator="91906152XXXX", recipient="91906112XXXX", template_id="monthly_promotion", body_parameter_values={"0": "promotion"})
 ```
 
 ### Check Whatsapp Request Status
 
 ```python
 from direct7 import Client
```

### Comparing `direct7-0.0.6/pyproject.toml` & `direct7-0.0.7/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "direct7"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Direct7 Networks", email="support@d7networks.com" },
 ]
 description = "Python SDK for Direct7  Platform REST API"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `direct7-0.0.6/PKG-INFO` & `direct7-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.2
 Name: direct7
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python SDK for Direct7  Platform REST API
 Project-URL: Homepage, https://github.com/d7networks/direct7-python-sdk
 Project-URL: Bug Tracker, https://github.com/d7networks/direct7-python-sdk/issues
 Author-email: Direct7 Networks <support@d7networks.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -68,15 +68,15 @@
 
 ```python
 from direct7 import Client
 
 client = Client(api_token="Your API token")
 
 client.sms.send_messages(
-        {"recipients": ["+9199XXXXXXXXXX"],"content": "مرحبا بالعالم!", "unicode": True},
+        {"recipients": ["+9199XXXXXXXX"],"content": "مرحبا بالعالم!", "unicode": True},
         originator="Sender",
         report_url="https://the_url_to_receive_delivery_report.com",
         )
 ```
 
 ### Check SMS Request Status
 
@@ -131,37 +131,36 @@
 # otp_id is the id returned in the response of send_otp
 client.verify.get_status(otp_id="0012c7f5-2ba5-49db-8901-4ee9be6dc8d1")
 ```
 
 
 ### Whatsapp
 
-### Send Whatsapp Free-form Message (Contact Details)
+### Send Whatsapp Free-form Message (Location Details)
 
 ```python
 from direct7 import Client
 
 client = Client(api_token="Your API token")
 
-client.whatsapp.send_whatsapp_freeform_message( originator="9181XXXXXXXX",
-                                                recipient="9190XXXXXXXX",
-                                                message_type="CONTACTS", first_name="Amal",
-                                                last_name="Anu", formatted_name="Amal Anu",
-                                                phones=["9181XXXXXXXX", "9181XXXXXXXX"],
-                                                emails=["amal@gmail.com", "amal2@gmail1.com"])
+client.whatsapp.send_whatsapp_freeform_message(originator="91906152XXXX",
+                                               recipient="91906112XXXX",
+                                                message_type="LOCATION", latitude="12.93803129081362",
+                                                longitude="77.61088653615994",
+                                                name="Mobile Pvt Ltd", address="30, Hosur Rd, 7th Block, Koramangala, Bengaluru, Karnataka 560095")
 ```
 
 ### Send Whatsapp Templated Message.
 
 ```python
 from direct7 import Client
 
 client = Client(api_token="Your API token")
 
-client.whatsapp.send_whatsapp_templated_message(originator="91906152XXXX", recipient="91906152XXXX", template_id="monthly_promotion", body_parameter_values={"0": "promotion"})
+client.whatsapp.send_whatsapp_templated_message(originator="91906152XXXX", recipient="91906112XXXX", template_id="monthly_promotion", body_parameter_values={"0": "promotion"})
 ```
 
 ### Check Whatsapp Request Status
 
 ```python
 from direct7 import Client
```

