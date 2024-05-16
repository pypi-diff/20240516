# Comparing `tmp/sms_message_aws_sns_local-0.0.8.tar.gz` & `tmp/sms_message_aws_sns_local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sms_message_aws_sns_local-0.0.8.tar", last modified: Fri Dec  8 10:12:11 2023, max compression
+gzip compressed data, was "sms_message_aws_sns_local-0.0.9.tar", last modified: Sun Dec 10 20:26:20 2023, max compression
```

## Comparing `sms_message_aws_sns_local-0.0.8.tar` & `sms_message_aws_sns_local-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:12:11.605341 sms_message_aws_sns_local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-08 10:12:11.605341 sms_message_aws_sns_local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2023-12-08 10:11:41.000000 sms_message_aws_sns_local-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      806 2023-12-08 10:11:41.000000 sms_message_aws_sns_local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-08 10:12:11.605341 sms_message_aws_sns_local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2023-12-08 10:11:41.000000 sms_message_aws_sns_local-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:12:11.605341 sms_message_aws_sns_local-0.0.8/sms_message_aws_sns_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:12:11.605341 sms_message_aws_sns_local-0.0.8/sms_message_aws_sns_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)    10942 2023-12-08 10:11:41.000000 sms_message_aws_sns_local-0.0.8/sms_message_aws_sns_local/src/SendAwsSms.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-08 10:11:41.000000 sms_message_aws_sns_local-0.0.8/sms_message_aws_sns_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-08 10:12:11.605341 sms_message_aws_sns_local-0.0.8/sms_message_aws_sns_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-08 10:12:11.000000 sms_message_aws_sns_local-0.0.8/sms_message_aws_sns_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2023-12-08 10:12:11.000000 sms_message_aws_sns_local-0.0.8/sms_message_aws_sns_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-08 10:12:11.000000 sms_message_aws_sns_local-0.0.8/sms_message_aws_sns_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-08 10:12:11.000000 sms_message_aws_sns_local-0.0.8/sms_message_aws_sns_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-08 10:12:11.000000 sms_message_aws_sns_local-0.0.8/sms_message_aws_sns_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 20:26:20.703035 sms_message_aws_sns_local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-10 20:26:20.703035 sms_message_aws_sns_local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2023-12-10 20:25:54.000000 sms_message_aws_sns_local-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2023-12-10 20:25:54.000000 sms_message_aws_sns_local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-10 20:26:20.703035 sms_message_aws_sns_local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-12-10 20:25:54.000000 sms_message_aws_sns_local-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 20:26:20.703035 sms_message_aws_sns_local-0.0.9/sms_message_aws_sns_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 20:26:20.703035 sms_message_aws_sns_local-0.0.9/sms_message_aws_sns_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    11145 2023-12-10 20:25:54.000000 sms_message_aws_sns_local-0.0.9/sms_message_aws_sns_local/src/SendAwsSms.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 20:25:54.000000 sms_message_aws_sns_local-0.0.9/sms_message_aws_sns_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 20:26:20.703035 sms_message_aws_sns_local-0.0.9/sms_message_aws_sns_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-10 20:26:20.000000 sms_message_aws_sns_local-0.0.9/sms_message_aws_sns_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2023-12-10 20:26:20.000000 sms_message_aws_sns_local-0.0.9/sms_message_aws_sns_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-10 20:26:20.000000 sms_message_aws_sns_local-0.0.9/sms_message_aws_sns_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-10 20:26:20.000000 sms_message_aws_sns_local-0.0.9/sms_message_aws_sns_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2023-12-10 20:26:20.000000 sms_message_aws_sns_local-0.0.9/sms_message_aws_sns_local.egg-info/top_level.txt
```

### Comparing `sms_message_aws_sns_local-0.0.8/README.md` & `sms_message_aws_sns_local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sms_message_aws_sns_local-0.0.8/pyproject.toml` & `sms_message_aws_sns_local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sms_message_aws_sns_local-0.0.8/setup.py` & `sms_message_aws_sns_local-0.0.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,19 @@
 package_dir = PACKAGE_NAME  # .replace("-", "_")
 
 with open('README.md') as f:
     readme = f.read()
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',
+    version='0.0.9',
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles AWS SMS",
     long_description="PyPI Package for Circles AWS SMS",
-    #long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/circ-zone/sms-message-aws-local-python-package.git",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     install_requires=["message-local"],
     classifiers=[
```

### Comparing `sms_message_aws_sns_local-0.0.8/sms_message_aws_sns_local/src/SendAwsSms.py` & `sms_message_aws_sns_local-0.0.9/sms_message_aws_sns_local/src/SendAwsSms.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 import boto3
-import botocore
-from enum import Enum
 from dotenv import load_dotenv
-import requests
 import http
 import json
 import time
-import logging
 from botocore.exceptions import ClientError
 import os
 from logger_local.Logger import Logger
-from logger_local.LoggerComponentEnum import LoggerComponentEnum
 
 from url_local.url_circlez import OurUrl
 from api_management_local.api_management_local import APIManagementsLocal
-#from api_management_local import indirect
-from message_local.Message import Message
+# from api_management_local import indirect
+from message_local.MessageLocal import MessageLocal
+from message_local.MessageImportance import MessageImportance
 
 # TODO Please fix all the lint error - Please use VS Code extention for that
 
 # TODO Please import message-local
 
 load_dotenv()
-BETWEEN_SOFT_AND_HARD=0
-MORE_THAN_HARD_LIMIT=1
+BETWEEN_SOFT_AND_HARD = 0
+MORE_THAN_HARD_LIMIT = 1
 SMS_MESSAGE_AWS_SNS_LOCAL_PYTHON_PACKAGE_COMPONENT_ID = 208
 SMS_MESSAGE_AWS_SNS_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME = "sms_message_aws_sns_local_python_package"
 DEVELOPER_EMAIL = "emad.a@circ.zone"
-logger = logging.getLogger(__name__)
+logger = Logger.create_logger(object={
+    "component_id": SMS_MESSAGE_AWS_SNS_LOCAL_PYTHON_PACKAGE_COMPONENT_ID,
+    "component_name": SMS_MESSAGE_AWS_SNS_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME,
+    "component_category": "Code",
+    "developer_email": DEVELOPER_EMAIL
+})
 
-# TODO const SMS_MESSAGE_AWS_SNS_API_TYPE_ID=6 # For API-Management
+SMS_MESSAGE_AWS_SNS_API_TYPE_ID = 6  # For API-Management
 
-#TODO Please add SMSMessage Class (SmsMessage.py) in messag_local in message-local-python-package
 
+# TODO Please add SMSMessage Class (SmsMessage.py) in messag_local in message-local-python-package
 
-class SmsMessageAwsSns(Message):
+
+class SmsMessageAwsSns(MessageLocal):
     def __init__(self, sns_resource):
         self.sns_resource = sns_resource
+        super().__init__(original_body="body", importance=MessageImportance.HIGH, original_subject="subject",
+                         api_type_id=SMS_MESSAGE_AWS_SNS_API_TYPE_ID, is_http_api=True, endpoint="endpoint")
 
     def create_topic(self, name):
         """
         Creates a notification topic.
 
         :param name: The name of the topic to create.
         :return: The newly created topic.
@@ -100,29 +104,46 @@
         except ClientError:
             logger.exception(
                 "Couldn't publish message to topic %s.", topic.arn)
             raise
         else:
             return message_id
 
+    def send(self, phone_number, message):
+        self.publish_text_message(phone_number, message)
+
+    def was_read(self):
+        """read"""
+        return True
+
+    def display(self):
+        """display"""
+        return "Message displayed"
+
+    def _can_send(self, sender_profile_id: int = None, api_data: dict = None, outgoing_body: dict = None) -> bool:
+        """can send"""
+        return True
+
+    def _after_send_attempt(self) -> None:
+        """after send"""
+        pass
+
+    def get_id(self):
+        return 0
 
 
 def usage_demo():
     print("-" * 88)
     print("Welcome to the Amazon Simple Notification Service (Amazon SNS) demo!")
     print("-" * 88)
 
-    logging.basicConfig(level=logging.INFO,
-                        format="%(levelname)s: %(message)s")
-
     sns_client = boto3.client("sns")
     sns_resource = boto3.resource("sns")
 
-    
-    topic_name = os.getenv("AWS_SNS_TOPIC_NAME")  
+    topic_name = os.getenv("AWS_SNS_TOPIC_NAME")
     print(f"Creating topic {topic_name}.")
 
     phone_number = input(
         "Enter a phone number (in E.164 format) that can receive SMS messages: "
     )
     if phone_number != "":
         print(f"Sending an SMS message directly from SNS to {phone_number}.")
@@ -174,85 +195,85 @@
     # for sub in topic_subs:
     #     sub.delete()
     # sns_resource.Topic(topic_name).delete()
 
     print("Thanks for watching!")
     print("-" * 88)
 
+
 # if __name__ == "__main__":
 #     #usage_demo()
 #     sms = SnsWrapper(boto3.resource('sns'))
 #     sms.publish_text_message('+972545232179',"gfugcuf")
 def send_sms_using_aws_sms_using_api_getaway(self, phone_number, message):
-       
-        example_instance=APIManagementsLocal.get_api
-        external_user_id=None
-        api_type_id=4
-        PRODUCT_USER_IDENTIFIER = os.getenv("PRODUCT_USER_IDENTIFIER")
-        PRODUCT_PASSWORD = os.getenv("PRODUCT_PASSWORD")
-        # user_context._instance = None
-        url_circlez = OurUrl()
-        # authentication_auth_login_endpoint_url = url_circlez.endpoint_url(
-        #         brand_name=BRAND_NAME,
-        #         environment_name=os.getenv('ENVIRONMENT_NAME'),
-        #         component_name=component_name_enum.ComponentName.AUTHENTICATION.value,
-        #         entity_name=entity_name_enum.EntityName.AUTH_LOGIN.value,
-        #         version=AUTHENTICATION_API_VERSION,
-        #         action_name=action_name_enum.ActionName.LOGIN.value
-        #         )
-        authentication_auth_login_endpoint_url = "AWS SNS"
-
-
-        data = {"user_identifier": PRODUCT_USER_IDENTIFIER, "password": PRODUCT_PASSWORD}
-        headers = {"Content-Type": "application/json"}
-        debug_data = {"url": authentication_auth_login_endpoint_url, "data": json.dumps(
-                data, separators=(",", ":")), "headers": headers}
-        Logger.info(json.dumps(debug_data, separators=(",", ":"), indent=4))
-        outgoing_body=(PRODUCT_USER_IDENTIFIER,PRODUCT_PASSWORD)
-        incoming_message=""
-        response_body=""
-        while True:
-                api_check, api_call_id,arr = example_instance.before_call_api(external_user_id=external_user_id,api_type_id=api_type_id,
-                                                                        endpoint=authentication_auth_login_endpoint_url,
-                                                                        outgoing_header=headers,
-                                                                        outgoing_body=outgoing_body
+    example_instance = APIManagementsLocal.get_api
+    external_user_id = None
+    api_type_id = 4
+    PRODUCT_USER_IDENTIFIER = os.getenv("PRODUCT_USER_IDENTIFIER")
+    PRODUCT_PASSWORD = os.getenv("PRODUCT_PASSWORD")
+    # user_context._instance = None
+    url_circlez = OurUrl()
+    # authentication_auth_login_endpoint_url = url_circlez.endpoint_url(
+    #         brand_name=BRAND_NAME,
+    #         environment_name=os.getenv('ENVIRONMENT_NAME'),
+    #         component_name=component_name_enum.ComponentName.AUTHENTICATION.value,
+    #         entity_name=entity_name_enum.EntityName.AUTH_LOGIN.value,
+    #         version=AUTHENTICATION_API_VERSION,
+    #         action_name=action_name_enum.ActionName.LOGIN.value
+    #         )
+    authentication_auth_login_endpoint_url = "AWS SNS"
+
+    data = {"user_identifier": PRODUCT_USER_IDENTIFIER, "password": PRODUCT_PASSWORD}
+    headers = {"Content-Type": "application/json"}
+    debug_data = {"url": authentication_auth_login_endpoint_url, "data": json.dumps(
+        data, separators=(",", ":")), "headers": headers}
+    logger.info(json.dumps(debug_data, separators=(",", ":"), indent=4))
+    outgoing_body = (PRODUCT_USER_IDENTIFIER, PRODUCT_PASSWORD)
+    incoming_message = ""
+    response_body = ""
+    while True:
+        api_check, api_call_id, arr = example_instance.before_call_api(external_user_id=external_user_id,
+                                                                       api_type_id=api_type_id,
+                                                                       endpoint=authentication_auth_login_endpoint_url,
+                                                                       outgoing_header=headers,
+                                                                       outgoing_body=outgoing_body
                                                                        )
-                if arr==None:
-                        used_cache=False
-                        if api_check==BETWEEN_SOFT_AND_HARD:
-                                logger.warn("You excced the soft limit")
-                        if api_check!= MORE_THAN_HARD_LIMIT:   
-                                try: 
-                                    
-                                    response = self.sns_resource.meta.client.publish(
-                                        PhoneNumber=phone_number, Message=message
-                                    )
-                                    message_id = response["MessageId"]
-                                    logger.info("Published message to %s.", phone_number)
-                                except ClientError:
-                                    logger.exception("Couldn't publish message to %s.", phone_number)
-                                    http_status_code=http.HTTPStatus.BAD_REQUEST.value
-                                    raise
-                                else:
-                                     http_status_code=http.HTTPStatus.OK.value                       
-                        else:
-                                print(" You passed the hard limit")    
-                                x=APIManagementsLocal.seconds_to_sleep_after_passing_the_hard_limit(api_type_id=api_type_id)
-                                if x>0:
-                                        print("sleeping : "+ str(x)+ " seconds")
-                                        time.sleep(x)
-                                        # raise PassedTheHardLimitException
+        if arr is None:
+            used_cache = False
+            if api_check == BETWEEN_SOFT_AND_HARD:
+                logger.warn("You excced the soft limit")
+            if api_check != MORE_THAN_HARD_LIMIT:
+                try:
+
+                    response = self.sns_resource.meta.client.publish(
+                        PhoneNumber=phone_number, Message=message
+                    )
+                    message_id = response["MessageId"]
+                    logger.info("Published message to %s.", phone_number)
+                except ClientError:
+                    logger.exception("Couldn't publish message to %s.", phone_number)
+                    http_status_code = http.HTTPStatus.BAD_REQUEST.value
+                    raise
+                else:
+                    http_status_code = http.HTTPStatus.OK.value
+            else:
+                print(" You passed the hard limit")
+                x = APIManagementsLocal.seconds_to_sleep_after_passing_the_hard_limit(api_type_id=api_type_id)
+                if x > 0:
+                    print("sleeping : " + str(x) + " seconds")
+                    time.sleep(x)
+                    # raise PassedTheHardLimitException
 
-                                else:
-                                        print("No sleeping needed : x= "+ str(x)+ " seconds")
                 else:
-                        used_cache=True
-                        print("result from cache")
-                        print(arr)
-                        http_status_code=http.HTTPStatus.OK.value  
-                example_instance.after_call_api(external_user_id=external_user_id,
-                                                api_type_id=api_type_id,
-                                                endpoint=authentication_auth_login_endpoint_url,outgoing_header=headers,
-                                                outgoing_body=outgoing_body,
-                                                incoming_message=incoming_message ,
-                                                http_status_code=http_status_code,
-                                                response_body=response_body,api_call_id=api_call_id,used_cache=used_cache)
+                    print("No sleeping needed : x= " + str(x) + " seconds")
+        else:
+            used_cache = True
+            print("result from cache")
+            print(arr)
+            http_status_code = http.HTTPStatus.OK.value
+        example_instance.after_call_api(external_user_id=external_user_id,
+                                        api_type_id=api_type_id,
+                                        endpoint=authentication_auth_login_endpoint_url, outgoing_header=headers,
+                                        outgoing_body=outgoing_body,
+                                        incoming_message=incoming_message,
+                                        http_status_code=http_status_code,
+                                        response_body=response_body, api_call_id=api_call_id, used_cache=used_cache)
```

