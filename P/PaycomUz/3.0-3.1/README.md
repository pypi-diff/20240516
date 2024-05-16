# Comparing `tmp/PaycomUz-3.0.tar.gz` & `tmp/PaycomUz-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PaycomUz\dist\tmprn4fduk0\PaycomUz-3.0.tar", last modified: Wed Mar  3 20:23:23 2021, max compression
+gzip compressed data, was "PaycomUz-3.1.tar", last modified: Thu May 16 06:03:14 2024, max compression
```

## Comparing `PaycomUz-3.0.tar` & `PaycomUz-3.1.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxrwxrwx   0        0        0        0 2021-03-03 20:23:23.000000 PaycomUz-3.0/
-drwxrwxrwx   0        0        0        0 2021-03-03 20:23:23.000000 PaycomUz-3.0/paycomuz/
--rw-rw-rw-   0        0        0      406 2021-03-03 18:23:43.000000 PaycomUz-3.0/paycomuz/admin.py
--rw-rw-rw-   0        0        0       96 2021-03-03 18:23:43.000000 PaycomUz-3.0/paycomuz/apps.py
--rw-rw-rw-   0        0        0     1430 2021-03-03 18:31:05.000000 PaycomUz-3.0/paycomuz/authentication.py
-drwxrwxrwx   0        0        0        0 2021-03-03 20:23:23.000000 PaycomUz-3.0/paycomuz/management/
-drwxrwxrwx   0        0        0        0 2021-03-03 20:23:23.000000 PaycomUz-3.0/paycomuz/management/commands/
--rw-rw-rw-   0        0        0      858 2021-03-03 18:23:43.000000 PaycomUz-3.0/paycomuz/management/commands/create_paycom_user.py
--rw-rw-rw-   0        0        0        0 2021-03-03 18:23:43.000000 PaycomUz-3.0/paycomuz/management/commands/__init__.py
--rw-rw-rw-   0        0        0        0 2021-03-03 18:23:43.000000 PaycomUz-3.0/paycomuz/management/__init__.py
--rw-rw-rw-   0        0        0     1049 2021-03-03 20:14:09.000000 PaycomUz-3.0/paycomuz/methods_subscribe_api.py
-drwxrwxrwx   0        0        0        0 2021-03-03 20:23:23.000000 PaycomUz-3.0/paycomuz/migrations/
--rw-rw-rw-   0        0        0     1280 2021-03-03 18:23:43.000000 PaycomUz-3.0/paycomuz/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     1289 2021-03-03 18:23:43.000000 PaycomUz-3.0/paycomuz/migrations/0002_auto_20200111_1714.py
--rw-rw-rw-   0        0        0     1615 2021-03-03 18:48:34.000000 PaycomUz-3.0/paycomuz/migrations/0003_auto_20210303_2348.py
--rw-rw-rw-   0        0        0      801 2021-03-03 20:01:14.000000 PaycomUz-3.0/paycomuz/migrations/0004_auto_20210304_0101.py
--rw-rw-rw-   0        0        0        0 2021-03-03 18:23:43.000000 PaycomUz-3.0/paycomuz/migrations/__init__.py
--rw-rw-rw-   0        0        0      983 2021-03-03 20:01:10.000000 PaycomUz-3.0/paycomuz/models.py
-drwxrwxrwx   0        0        0        0 2021-03-03 20:23:23.000000 PaycomUz-3.0/paycomuz/serializers/
--rw-rw-rw-   0        0        0      766 2021-03-03 19:33:58.000000 PaycomUz-3.0/paycomuz/serializers/payme_operation.py
--rw-rw-rw-   0        0        0        0 2021-03-03 18:23:43.000000 PaycomUz-3.0/paycomuz/serializers/__init__.py
--rw-rw-rw-   0        0        0     1139 2021-03-03 18:49:59.000000 PaycomUz-3.0/paycomuz/status.py
--rw-rw-rw-   0        0        0     9066 2021-03-03 20:07:20.000000 PaycomUz-3.0/paycomuz/views.py
--rw-rw-rw-   0        0        0      718 2021-03-03 20:09:48.000000 PaycomUz-3.0/paycomuz/__init__.py
-drwxrwxrwx   0        0        0        0 2021-03-03 20:23:23.000000 PaycomUz-3.0/PaycomUz.egg-info/
--rw-rw-rw-   0        0        0        1 2021-03-03 20:23:23.000000 PaycomUz-3.0/PaycomUz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2869 2021-03-03 20:23:23.000000 PaycomUz-3.0/PaycomUz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       36 2021-03-03 20:23:23.000000 PaycomUz-3.0/PaycomUz.egg-info/requires.txt
--rw-rw-rw-   0        0        0      756 2021-03-03 20:23:23.000000 PaycomUz-3.0/PaycomUz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2021-03-03 20:23:23.000000 PaycomUz-3.0/PaycomUz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2869 2021-03-03 20:23:23.000000 PaycomUz-3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1872 2021-03-03 20:15:25.000000 PaycomUz-3.0/README.md
--rw-rw-rw-   0        0        0       42 2021-03-03 20:23:23.000000 PaycomUz-3.0/setup.cfg
--rw-rw-rw-   0        0        0      660 2021-03-03 20:22:15.000000 PaycomUz-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 06:03:14.325522 PaycomUz-3.1/
+-rw-rw-rw-   0        0        0     1091 2024-04-19 11:20:15.000000 PaycomUz-3.1/LICENSE
+-rw-rw-rw-   0        0        0     2428 2024-05-16 06:03:14.323921 PaycomUz-3.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 06:03:14.280578 PaycomUz-3.1/PaycomUz.egg-info/
+-rw-rw-rw-   0        0        0     2428 2024-05-16 06:03:14.000000 PaycomUz-3.1/PaycomUz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      764 2024-05-16 06:03:14.000000 PaycomUz-3.1/PaycomUz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 06:03:14.000000 PaycomUz-3.1/PaycomUz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-16 06:03:14.000000 PaycomUz-3.1/PaycomUz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-16 06:03:14.000000 PaycomUz-3.1/PaycomUz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2058 2024-04-25 05:30:26.000000 PaycomUz-3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 06:03:14.297307 PaycomUz-3.1/paycomuz/
+-rw-rw-rw-   0        0        0      718 2024-04-19 11:20:15.000000 PaycomUz-3.1/paycomuz/__init__.py
+-rw-rw-rw-   0        0        0      424 2024-04-19 11:20:15.000000 PaycomUz-3.1/paycomuz/admin.py
+-rw-rw-rw-   0        0        0       96 2024-04-19 11:20:15.000000 PaycomUz-3.1/paycomuz/apps.py
+-rw-rw-rw-   0        0        0     1430 2024-04-19 11:20:15.000000 PaycomUz-3.1/paycomuz/authentication.py
+drwxrwxrwx   0        0        0        0 2024-05-16 06:03:14.297307 PaycomUz-3.1/paycomuz/management/
+-rw-rw-rw-   0        0        0        0 2024-04-19 11:20:15.000000 PaycomUz-3.1/paycomuz/management/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 06:03:14.305690 PaycomUz-3.1/paycomuz/management/commands/
+-rw-rw-rw-   0        0        0        0 2024-04-19 11:20:15.000000 PaycomUz-3.1/paycomuz/management/commands/__init__.py
+-rw-rw-rw-   0        0        0      858 2024-04-19 11:20:15.000000 PaycomUz-3.1/paycomuz/management/commands/create_paycom_user.py
+-rw-rw-rw-   0        0        0     1052 2024-04-19 11:20:15.000000 PaycomUz-3.1/paycomuz/methods_subscribe_api.py
+drwxrwxrwx   0        0        0        0 2024-05-16 06:03:14.317504 PaycomUz-3.1/paycomuz/migrations/
+-rw-rw-rw-   0        0        0     1280 2024-04-19 11:20:15.000000 PaycomUz-3.1/paycomuz/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     1289 2024-04-19 11:20:15.000000 PaycomUz-3.1/paycomuz/migrations/0002_auto_20200111_1714.py
+-rw-rw-rw-   0        0        0     1615 2024-04-19 11:20:15.000000 PaycomUz-3.1/paycomuz/migrations/0003_auto_20210303_2348.py
+-rw-rw-rw-   0        0        0      801 2024-04-19 11:20:15.000000 PaycomUz-3.1/paycomuz/migrations/0004_auto_20210304_0101.py
+-rw-rw-rw-   0        0        0        0 2024-04-19 11:20:15.000000 PaycomUz-3.1/paycomuz/migrations/__init__.py
+-rw-rw-rw-   0        0        0      983 2024-04-19 11:20:15.000000 PaycomUz-3.1/paycomuz/models.py
+drwxrwxrwx   0        0        0        0 2024-05-16 06:03:14.322404 PaycomUz-3.1/paycomuz/serializers/
+-rw-rw-rw-   0        0        0        0 2024-04-19 11:20:15.000000 PaycomUz-3.1/paycomuz/serializers/__init__.py
+-rw-rw-rw-   0        0        0      852 2024-04-19 11:39:36.000000 PaycomUz-3.1/paycomuz/serializers/payme_operation.py
+-rw-rw-rw-   0        0        0     1218 2024-04-25 04:44:20.000000 PaycomUz-3.1/paycomuz/status.py
+-rw-rw-rw-   0        0        0    11010 2024-04-25 04:55:25.000000 PaycomUz-3.1/paycomuz/views.py
+-rw-rw-rw-   0        0        0       42 2024-05-16 06:03:14.326571 PaycomUz-3.1/setup.cfg
+-rw-rw-rw-   0        0        0      638 2024-05-16 06:02:38.000000 PaycomUz-3.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PaycomUz-3.0/paycomuz/authentication.py` & `PaycomUz-3.1/paycomuz/authentication.py`

 * *Files identical despite different names*

### Comparing `PaycomUz-3.0/paycomuz/management/commands/create_paycom_user.py` & `PaycomUz-3.1/paycomuz/management/commands/create_paycom_user.py`

 * *Files identical despite different names*

### Comparing `PaycomUz-3.0/paycomuz/methods_subscribe_api.py` & `PaycomUz-3.1/paycomuz/methods_subscribe_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import base64
 from decimal import Decimal
 
 assert settings.PAYCOM_SETTINGS.get('KASSA_ID') != None
 assert settings.PAYCOM_SETTINGS.get('ACCOUNTS') != None
 assert settings.PAYCOM_SETTINGS['ACCOUNTS'].get('KEY') != None
 
-TOKEN = settings.PAYCOM_SETTINGS['TOKEN']
+TOKEN = settings.PAYCOM_SETTINGS['KASSA_ID']
 KEY = settings.PAYCOM_SETTINGS['ACCOUNTS']['KEY']
 
 
 class PayComResponse(object):
     LINK = 'https://checkout.paycom.uz'
 
     def create_initialization(self, amount: Decimal, order_id: str, return_url: str) -> str:
```

### Comparing `PaycomUz-3.0/paycomuz/migrations/0001_initial.py` & `PaycomUz-3.1/paycomuz/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `PaycomUz-3.0/paycomuz/migrations/0002_auto_20200111_1714.py` & `PaycomUz-3.1/paycomuz/migrations/0002_auto_20200111_1714.py`

 * *Files identical despite different names*

### Comparing `PaycomUz-3.0/paycomuz/migrations/0003_auto_20210303_2348.py` & `PaycomUz-3.1/paycomuz/migrations/0003_auto_20210303_2348.py`

 * *Files identical despite different names*

### Comparing `PaycomUz-3.0/paycomuz/migrations/0004_auto_20210304_0101.py` & `PaycomUz-3.1/paycomuz/migrations/0004_auto_20210304_0101.py`

 * *Files identical despite different names*

### Comparing `PaycomUz-3.0/paycomuz/models.py` & `PaycomUz-3.1/paycomuz/models.py`

 * *Files identical despite different names*

### Comparing `PaycomUz-3.0/paycomuz/serializers/payme_operation.py` & `PaycomUz-3.1/paycomuz/serializers/payme_operation.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,17 +3,21 @@
 
 class PaycomOperationSerialzer(serializers.Serializer):
     CHECK_PERFORM_TRANSACTION = 'CheckPerformTransaction'
     CREATE_TRANSACTION = 'CreateTransaction'
     PERFORM_TRANSACTION = 'PerformTransaction'
     CHECK_TRANSACTION = 'CheckTransaction'
     CANCEL_TRANSACTION = 'CancelTransaction'
+    GET_STATEMENT = 'GetStatement'
+
     METHODS = (
         (CHECK_PERFORM_TRANSACTION, CHECK_PERFORM_TRANSACTION),
         (CREATE_TRANSACTION, CREATE_TRANSACTION),
         (PERFORM_TRANSACTION, PERFORM_TRANSACTION),
         (CHECK_TRANSACTION, CHECK_TRANSACTION),
-        (CANCEL_TRANSACTION, CANCEL_TRANSACTION)
+        (CANCEL_TRANSACTION, CANCEL_TRANSACTION),
+        (GET_STATEMENT, GET_STATEMENT),
     )
+    
     id = serializers.IntegerField()
     method = serializers.ChoiceField(choices=METHODS)
     params = serializers.JSONField()
```

### Comparing `PaycomUz-3.0/paycomuz/status.py` & `PaycomUz-3.1/paycomuz/status.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-ORDER_NOT_FOND = -31050
-TRANSACTION_NOT_FOND = -31003
+ORDER_NOT_FOUND = -31050
+TRANSACTION_NOT_FOUND = -31003
 UNABLE_TO_PERFORM_OPERATION = -31008
 INVALID_AMOUNT = -31001
+ON_PROCESS = -31099
 ORDER_FOUND = 200
 
 CREATE_TRANSACTION = 1
 CLOSE_TRANSACTION = 2
 CANCEL_TRANSACTION_CODE = -1
 PERFORM_CANCELED_CODE = -2
-ORDER_NOT_FOND_MESSAGE = {
+ORDER_NOT_FOUND_MESSAGE = {
     "uz": "Buyurtma topilmadi",
     "ru": "Заказ не найден",
     "en": "Order not fond"
 }
-TRANSACTION_NOT_FOND_MESSAGE = {
+TRANSACTION_NOT_FOUND_MESSAGE = {
     "uz": "Tranzaksiya topilmadi",
     "ru": "Транзакция не найдена",
-    "en": "Transaction not fond"
+    "en": "Transaction not found"
 }
 UNABLE_TO_PERFORM_OPERATION_MESSAGE = {
     "uz": "Ushbu amalni bajarib bo'lmaydi",
     "ru": "Невозможно выполнить данную операцию",
     "en": "Unable to perform operation"
 }
 INVALID_AMOUNT_MESSAGE = {
@@ -29,14 +30,14 @@
     "en": "Invalid amount"
 }
 
 AUTH_ERROR = {
     "error": {
         "code": -32504,
         "message": {
-            "ru": "user not exists",
-            "uz": "user not exists",
-            "en": "user not exists"
+            "ru": "пользователь не существует",
+            "uz": "foydalanuvchi mavjud emas",
+            "en": "user does not exist"
         },
-        "data": "user not exists"
+        "data": "user does not exist"
     }
 }
```

### Comparing `PaycomUz-3.0/paycomuz/views.py` & `PaycomUz-3.1/paycomuz/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,33 +18,38 @@
 class MerchantAPIView(APIView):
     permission_classes = [AllowAny]
     CHECK_PERFORM_TRANSACTION = 'CheckPerformTransaction'
     CREATE_TRANSACTION = 'CreateTransaction'
     PERFORM_TRANSACTION = 'PerformTransaction'
     CHECK_TRANSACTION = 'CheckTransaction'
     CANCEL_TRANSACTION = 'CancelTransaction'
+    GET_STATEMENT = 'GetStatement'
+
     http_method_names = ['post']
     authentication_classes = []
     VALIDATE_CLASS: Paycom = None
     reply = None
     ORDER_KEY = KEY = settings.PAYCOM_SETTINGS['ACCOUNTS']['KEY']
 
     def __init__(self):
         self.METHODS = {
             self.CHECK_PERFORM_TRANSACTION: self.check_perform_transaction,
             self.CREATE_TRANSACTION: self.create_transaction,
             self.PERFORM_TRANSACTION: self.perform_transaction,
             self.CHECK_TRANSACTION: self.check_transaction,
-            self.CANCEL_TRANSACTION: self.cancel_transaction
+            self.CANCEL_TRANSACTION: self.cancel_transaction,
+            self.GET_STATEMENT: self.get_statement
         }
+
         self.REPLY_RESPONSE = {
             ORDER_FOUND: self.order_found,
-            ORDER_NOT_FOND: self.order_not_found,
+            ORDER_NOT_FOUND: self.order_not_found,
             INVALID_AMOUNT: self.invalid_amount
         }
+
         super(MerchantAPIView, self).__init__()
 
     def post(self, request):
         check = authentication(request)
         if check is False or not check:
             return Response(AUTH_ERROR)
         serializer = PaycomOperationSerialzer(data=request.data, many=False)
@@ -86,19 +91,33 @@
             transaction = check_transaction.first()
             if transaction.status != Transaction.CANCELED and transaction._id == _id:
                 self.reply = dict(result=dict(
                     create_time=int(transaction.created_datetime),
                     transaction=str(transaction.id),
                     state=CREATE_TRANSACTION
                 ))
+
+            elif transaction.status == Transaction.PROCESSING:
+                self.reply = dict(
+                    id=validated_data['id'],
+                    error=dict(
+                        code=ON_PROCESS,
+                        message=dict(
+                            uz="Buyurtma to'lo'vi hozirda amalga oshirilmoqda",
+                            ru="Платеж на этот заказ на данный момент в процессе",
+                            en="Payment for this order is currently on process"
+                        )
+                    )
+                )
+
             else:
                 self.reply = dict(error=dict(
                     id=validated_data['id'],
-                    code=ORDER_NOT_FOND,
-                    message=ORDER_NOT_FOND_MESSAGE
+                    code=ORDER_NOT_FOUND,
+                    message=ORDER_NOT_FOUND_MESSAGE
                 ))
         else:
             current_time = datetime.now()
             current_time_to_string = int(round(current_time.timestamp()) * 1000)
             obj = Transaction.objects.create(
                 request_id=validated_data['id'],
                 _id=validated_data['params']['id'],
@@ -143,16 +162,16 @@
                     code=UNABLE_TO_PERFORM_OPERATION,
                     message=UNABLE_TO_PERFORM_OPERATION_MESSAGE
                 ))
             obj.save()
         except Transaction.DoesNotExist:
             self.reply = dict(error=dict(
                 id=request_id,
-                code=TRANSACTION_NOT_FOND,
-                message=TRANSACTION_NOT_FOND_MESSAGE
+                code=TRANSACTION_NOT_FOUND,
+                message=TRANSACTION_NOT_FOUND_MESSAGE
             ))
 
     def check_transaction(self, validated_data):
         """
         >>> self.check_transaction(validated_data)
         """
         id = validated_data['params']['id']
@@ -160,16 +179,16 @@
 
         try:
             transaction = Transaction.objects.get(_id=id)
             self.response_check_transaction(transaction)
         except Transaction.DoesNotExist:
             self.reply = dict(error=dict(
                 id=request_id,
-                code=TRANSACTION_NOT_FOND,
-                message=TRANSACTION_NOT_FOND_MESSAGE
+                code=TRANSACTION_NOT_FOUND,
+                message=TRANSACTION_NOT_FOUND_MESSAGE
             ))
 
     def cancel_transaction(self, validated_data):
         id = validated_data['params']['id']
         reason = validated_data['params']['reason']
         request_id = validated_data['id']
 
@@ -189,26 +208,61 @@
                 transaction.cancel_datetime = current_time_to_string
             transaction.save()
 
             self.response_check_transaction(transaction)
         except Transaction.DoesNotExist:
             self.reply = dict(error=dict(
                 id=request_id,
-                code=TRANSACTION_NOT_FOND,
-                message=TRANSACTION_NOT_FOND_MESSAGE
+                code=TRANSACTION_NOT_FOUND,
+                message=TRANSACTION_NOT_FOUND_MESSAGE
             ))
 
+    def get_statement(self, validated_data):
+        from_d = validated_data.get('params').get('from')
+        to_d = validated_data.get('params').get('to')
+
+        filtered_transactions = Transaction.objects.filter(
+            created_datetime__gte=from_d,
+            created_datetime__lte=to_d
+        )
+
+        transactions_json = [
+            dict(
+                id = obj._id,
+                time = int(obj.created_datetime),
+                amount = obj.amount,
+                account = dict(
+                    order_id = obj.order_key
+                ),
+                create_time = int(obj.created_datetime) if obj.created_datetime else 0,
+                perform_time = int(obj.perform_datetime) if obj.perform_datetime else 0,
+                cancel_time = int(obj.cancel_datetime) if obj.cancel_datetime else 0,
+                transaction = obj.request_id,
+                state = obj.state,
+                reason = obj.reason,
+            ) 
+            
+            for obj in filtered_transactions]
+
+        response = dict(
+            result = dict(
+                transactions = transactions_json
+            )
+        )
+
+        self.reply = response
+
     def order_found(self, validated_data):
         self.reply = dict(result=dict(allow=True))
 
     def order_not_found(self, validated_data):
         self.reply = dict(error=dict(
             id=validated_data['id'],
-            code=ORDER_NOT_FOND,
-            message=ORDER_NOT_FOND_MESSAGE
+            code=ORDER_NOT_FOUND,
+            message=ORDER_NOT_FOUND_MESSAGE
         ))
 
     def invalid_amount(self, validated_data):
         self.reply = dict(error=dict(
             id=validated_data['id'],
             code=INVALID_AMOUNT,
             message=INVALID_AMOUNT_MESSAGE
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `PaycomUz-3.0/paycomuz/__init__.py` & `PaycomUz-3.1/paycomuz/__init__.py`

 * *Files identical despite different names*

### Comparing `PaycomUz-3.0/PaycomUz.egg-info/PKG-INFO` & `PaycomUz-3.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,89 +1,95 @@
 Metadata-Version: 2.1
 Name: PaycomUz
-Version: 3.0
+Version: 3.1
 Summary: Paycomuz
 Home-page: https://github.com/begyy/PaycomUz
 Author: Sadullayev Bekhzod
 Author-email: begymrx@gmail.com
-License: UNKNOWN
-Description: ![alt text](https://i.imgur.com/bmVCvl8.jpg)
-        
-        [![Downloads](https://pepy.tech/badge/paycomuz)](https://pepy.tech/project/paycomuz)
-        ![alt text](https://img.shields.io/badge/code%20style-black-000000.svg)
-        [![Downloads](https://img.shields.io/pypi/v/paycomuz)](https://pypi.org/project/PaycomUz)
-        [![Downloads](https://black.readthedocs.io/en/stable/_static/license.svg)](https://github.com/begyy/PaycomUz/blob/master/LICENSE)
-        
-        ### Requirements
-        ````
-        pip install django
-        pip install djangorestframework
-        pip install PaycomUz 
-        pip install requests
-        
-        # supported versions
-        python 3.5 +
-        django 2 +
-        djangorestframework 3.7 +
-        PaycomUz 2 +
-        ````
-        
-        **settings.py**
-        
-        ```python
-        PAYCOM_SETTINGS = {
-            "KASSA_ID": "KASSA ID",  # token
-            "SECRET_KEY": "TEST KEY OR PRODUCTIN KEY",  # password
-            "ACCOUNTS": {
-                "KEY": "order_id"
-            }
-        }
-        
-        INSTALLED_APPS = [
-            'rest_framework',
-            'paycomuz',
-            ...
-        ]
-        ```
-        
-        ```
-        python manage.py migrate
-        ```
-        
-        ### Create paycom user
-        ```python
-        python manage.py create_paycom_user
-        ```
-        
-        ### view.py
-        ```python
-        from paycomuz.views import MerchantAPIView
-        from paycomuz.methods_subscribe_api import Paycom
-        from django.urls import path
-        
-        class CheckOrder(Paycom):
-            def check_order(self, amount, account):
-                return self.ORDER_FOUND
-        
-        class TestView(MerchantAPIView):
-            VALIDATE_CLASS = CheckOrder
-        
-        urlpatterns = [
-            path('paycom/', TestView.as_view())
-        ]
-        ```
-        
-        ### create_initialization.py
-        https://help.paycom.uz/uz/initsializatsiya-platezhey/otpravka-cheka-po-metodu-get
-        ```python
-        from paycomuz.methods_subscribe_api import Paycom
-        paycom = Paycom()
-        url = paycom.create_initialization(amount=5.00, order_id='197', return_url='https://example.com/success/')
-        print(url)
-        ```
-        ![alt text](https://help.paycom.uz/images/ru/payment_initialization/checkout-get-method-response.png)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![alt text](https://i.imgur.com/bmVCvl8.jpg)
+
+[![Downloads](https://pepy.tech/badge/paycomuz)](https://pepy.tech/project/paycomuz)
+![alt text](https://img.shields.io/badge/code%20style-black-000000.svg)
+[![Downloads](https://img.shields.io/pypi/v/paycomuz)](https://pypi.org/project/PaycomUz)
+[![Downloads](https://black.readthedocs.io/en/stable/_static/license.svg)](https://github.com/begyy/PaycomUz/blob/master/LICENSE)
+
+### Requirements
+````
+pip install django
+pip install djangorestframework
+pip install PaycomUz 
+pip install requests
+
+# supported versions
+python 3.5 +
+django 2 +
+djangorestframework 3.7 +
+PaycomUz 2 +
+````
+
+**settings.py**
+
+```python
+PAYCOM_SETTINGS = {
+    "KASSA_ID": "KASSA ID",  # token
+    "SECRET_KEY": "TEST KEY OR PRODUCTIN KEY",  # password
+    "ACCOUNTS": {
+        "KEY": "order_id"
+    },
+}
+
+INSTALLED_APPS = [
+    'rest_framework',
+    'paycomuz',
+    ...
+]
+```
+
+```
+python manage.py migrate
+```
+
+### Create paycom user
+```python
+python manage.py create_paycom_user
+```
+
+### view.py
+```python
+from paycomuz.views import MerchantAPIView
+from paycomuz import Paycom
+from django.urls import path
+
+class CheckOrder(Paycom):
+    def check_order(self, amount, account, *args, **kwargs):
+        return self.ORDER_FOUND
+        
+   def successfully_payment(self, account, transaction, *args, **kwargs):
+        print(account)
+
+   def cancel_payment(self, account, transaction, *args, **kwargs):
+        print(account)
+      
+
+class TestView(MerchantAPIView):
+    VALIDATE_CLASS = CheckOrder
+
+urlpatterns = [
+    path('paycom/', TestView.as_view())
+]
+```
+
+### create_initialization.py
+https://help.paycom.uz/uz/initsializatsiya-platezhey/otpravka-cheka-po-metodu-get
+```python
+from paycomuz import Paycom
+paycom = Paycom()
+url = paycom.create_initialization(amount=5.00, order_id='197', return_url='https://example.com/success/')
+print(url)
+```
+![alt text](https://help.paycom.uz/images/ru/payment_initialization/checkout-get-method-response.png)
```

### Comparing `PaycomUz-3.0/PaycomUz.egg-info/SOURCES.txt` & `PaycomUz-3.1/PaycomUz.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 PaycomUz.egg-info/PKG-INFO
 PaycomUz.egg-info/SOURCES.txt
 PaycomUz.egg-info/dependency_links.txt
 PaycomUz.egg-info/requires.txt
 PaycomUz.egg-info/top_level.txt
```

### Comparing `PaycomUz-3.0/PKG-INFO` & `PaycomUz-3.1/PaycomUz.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,89 +1,95 @@
 Metadata-Version: 2.1
 Name: PaycomUz
-Version: 3.0
+Version: 3.1
 Summary: Paycomuz
 Home-page: https://github.com/begyy/PaycomUz
 Author: Sadullayev Bekhzod
 Author-email: begymrx@gmail.com
-License: UNKNOWN
-Description: ![alt text](https://i.imgur.com/bmVCvl8.jpg)
-        
-        [![Downloads](https://pepy.tech/badge/paycomuz)](https://pepy.tech/project/paycomuz)
-        ![alt text](https://img.shields.io/badge/code%20style-black-000000.svg)
-        [![Downloads](https://img.shields.io/pypi/v/paycomuz)](https://pypi.org/project/PaycomUz)
-        [![Downloads](https://black.readthedocs.io/en/stable/_static/license.svg)](https://github.com/begyy/PaycomUz/blob/master/LICENSE)
-        
-        ### Requirements
-        ````
-        pip install django
-        pip install djangorestframework
-        pip install PaycomUz 
-        pip install requests
-        
-        # supported versions
-        python 3.5 +
-        django 2 +
-        djangorestframework 3.7 +
-        PaycomUz 2 +
-        ````
-        
-        **settings.py**
-        
-        ```python
-        PAYCOM_SETTINGS = {
-            "KASSA_ID": "KASSA ID",  # token
-            "SECRET_KEY": "TEST KEY OR PRODUCTIN KEY",  # password
-            "ACCOUNTS": {
-                "KEY": "order_id"
-            }
-        }
-        
-        INSTALLED_APPS = [
-            'rest_framework',
-            'paycomuz',
-            ...
-        ]
-        ```
-        
-        ```
-        python manage.py migrate
-        ```
-        
-        ### Create paycom user
-        ```python
-        python manage.py create_paycom_user
-        ```
-        
-        ### view.py
-        ```python
-        from paycomuz.views import MerchantAPIView
-        from paycomuz.methods_subscribe_api import Paycom
-        from django.urls import path
-        
-        class CheckOrder(Paycom):
-            def check_order(self, amount, account):
-                return self.ORDER_FOUND
-        
-        class TestView(MerchantAPIView):
-            VALIDATE_CLASS = CheckOrder
-        
-        urlpatterns = [
-            path('paycom/', TestView.as_view())
-        ]
-        ```
-        
-        ### create_initialization.py
-        https://help.paycom.uz/uz/initsializatsiya-platezhey/otpravka-cheka-po-metodu-get
-        ```python
-        from paycomuz.methods_subscribe_api import Paycom
-        paycom = Paycom()
-        url = paycom.create_initialization(amount=5.00, order_id='197', return_url='https://example.com/success/')
-        print(url)
-        ```
-        ![alt text](https://help.paycom.uz/images/ru/payment_initialization/checkout-get-method-response.png)
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+![alt text](https://i.imgur.com/bmVCvl8.jpg)
+
+[![Downloads](https://pepy.tech/badge/paycomuz)](https://pepy.tech/project/paycomuz)
+![alt text](https://img.shields.io/badge/code%20style-black-000000.svg)
+[![Downloads](https://img.shields.io/pypi/v/paycomuz)](https://pypi.org/project/PaycomUz)
+[![Downloads](https://black.readthedocs.io/en/stable/_static/license.svg)](https://github.com/begyy/PaycomUz/blob/master/LICENSE)
+
+### Requirements
+````
+pip install django
+pip install djangorestframework
+pip install PaycomUz 
+pip install requests
+
+# supported versions
+python 3.5 +
+django 2 +
+djangorestframework 3.7 +
+PaycomUz 2 +
+````
+
+**settings.py**
+
+```python
+PAYCOM_SETTINGS = {
+    "KASSA_ID": "KASSA ID",  # token
+    "SECRET_KEY": "TEST KEY OR PRODUCTIN KEY",  # password
+    "ACCOUNTS": {
+        "KEY": "order_id"
+    },
+}
+
+INSTALLED_APPS = [
+    'rest_framework',
+    'paycomuz',
+    ...
+]
+```
+
+```
+python manage.py migrate
+```
+
+### Create paycom user
+```python
+python manage.py create_paycom_user
+```
+
+### view.py
+```python
+from paycomuz.views import MerchantAPIView
+from paycomuz import Paycom
+from django.urls import path
+
+class CheckOrder(Paycom):
+    def check_order(self, amount, account, *args, **kwargs):
+        return self.ORDER_FOUND
+        
+   def successfully_payment(self, account, transaction, *args, **kwargs):
+        print(account)
+
+   def cancel_payment(self, account, transaction, *args, **kwargs):
+        print(account)
+      
+
+class TestView(MerchantAPIView):
+    VALIDATE_CLASS = CheckOrder
+
+urlpatterns = [
+    path('paycom/', TestView.as_view())
+]
+```
+
+### create_initialization.py
+https://help.paycom.uz/uz/initsializatsiya-platezhey/otpravka-cheka-po-metodu-get
+```python
+from paycomuz import Paycom
+paycom = Paycom()
+url = paycom.create_initialization(amount=5.00, order_id='197', return_url='https://example.com/success/')
+print(url)
+```
+![alt text](https://help.paycom.uz/images/ru/payment_initialization/checkout-get-method-response.png)
```

### Comparing `PaycomUz-3.0/README.md` & `PaycomUz-3.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 ```python
 PAYCOM_SETTINGS = {
     "KASSA_ID": "KASSA ID",  # token
     "SECRET_KEY": "TEST KEY OR PRODUCTIN KEY",  # password
     "ACCOUNTS": {
         "KEY": "order_id"
-    }
+    },
 }
 
 INSTALLED_APPS = [
     'rest_framework',
     'paycomuz',
     ...
 ]
@@ -45,31 +45,38 @@
 ```python
 python manage.py create_paycom_user
 ```
 
 ### view.py
 ```python
 from paycomuz.views import MerchantAPIView
-from paycomuz.methods_subscribe_api import Paycom
+from paycomuz import Paycom
 from django.urls import path
 
 class CheckOrder(Paycom):
-    def check_order(self, amount, account):
+    def check_order(self, amount, account, *args, **kwargs):
         return self.ORDER_FOUND
+        
+   def successfully_payment(self, account, transaction, *args, **kwargs):
+        print(account)
+
+   def cancel_payment(self, account, transaction, *args, **kwargs):
+        print(account)
+      
 
 class TestView(MerchantAPIView):
     VALIDATE_CLASS = CheckOrder
 
 urlpatterns = [
     path('paycom/', TestView.as_view())
 ]
 ```
 
 ### create_initialization.py
 https://help.paycom.uz/uz/initsializatsiya-platezhey/otpravka-cheka-po-metodu-get
 ```python
-from paycomuz.methods_subscribe_api import Paycom
+from paycomuz import Paycom
 paycom = Paycom()
 url = paycom.create_initialization(amount=5.00, order_id='197', return_url='https://example.com/success/')
 print(url)
 ```
 ![alt text](https://help.paycom.uz/images/ru/payment_initialization/checkout-get-method-response.png)
```

### Comparing `PaycomUz-3.0/setup.py` & `PaycomUz-3.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PaycomUz",
-    version="3.0",
+    version="3.1",
     author="Sadullayev Bekhzod",
     author_email="begymrx@gmail.com",
     description="Paycomuz",
     long_description=long_description,
     long_description_content_type="text/markdown",
     python_requires=">=3.5",
-    install_requires=['requests', 'django','djangorestframework'],
+    install_requires=['requests', 'django'],
     url="https://github.com/begyy/PaycomUz",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ]
 )
```

