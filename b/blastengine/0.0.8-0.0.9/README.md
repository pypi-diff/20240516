# Comparing `tmp/blastengine-0.0.8.tar.gz` & `tmp/blastengine-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blastengine-0.0.8.tar", last modified: Tue Feb  6 07:53:26 2024, max compression
+gzip compressed data, was "blastengine-0.0.9.tar", last modified: Thu Apr 18 08:10:53 2024, max compression
```

## Comparing `blastengine-0.0.8.tar` & `blastengine-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 nakatsugawa   (501) staff       (20)        0 2024-02-06 07:53:26.887534 blastengine-0.0.8/
--rw-r--r--   0 nakatsugawa   (501) staff       (20)     1092 2022-10-22 08:37:48.000000 blastengine-0.0.8/LICENSE
--rw-r--r--   0 nakatsugawa   (501) staff       (20)      506 2024-02-06 07:53:26.887358 blastengine-0.0.8/PKG-INFO
--rw-r--r--   0 nakatsugawa   (501) staff       (20)      656 2023-08-21 13:54:02.000000 blastengine-0.0.8/README.md
-drwxr-xr-x   0 nakatsugawa   (501) staff       (20)        0 2024-02-06 07:53:26.886503 blastengine-0.0.8/blastengine/
--rw-r--r--   0 nakatsugawa   (501) staff       (20)     4482 2024-02-06 07:39:09.000000 blastengine-0.0.8/blastengine/Bulk.py
--rw-r--r--   0 nakatsugawa   (501) staff       (20)      463 2022-10-22 08:37:48.000000 blastengine-0.0.8/blastengine/Client.py
--rw-r--r--   0 nakatsugawa   (501) staff       (20)     2242 2023-08-21 13:14:55.000000 blastengine-0.0.8/blastengine/Job.py
--rw-r--r--   0 nakatsugawa   (501) staff       (20)     1562 2023-08-23 02:07:40.000000 blastengine-0.0.8/blastengine/Log.py
--rw-r--r--   0 nakatsugawa   (501) staff       (20)     3221 2024-02-06 07:50:53.000000 blastengine-0.0.8/blastengine/Mail.py
--rw-r--r--   0 nakatsugawa   (501) staff       (20)     4643 2024-02-06 07:49:20.000000 blastengine-0.0.8/blastengine/MailBase.py
--rw-r--r--   0 nakatsugawa   (501) staff       (20)     1943 2024-02-06 07:39:21.000000 blastengine-0.0.8/blastengine/Transaction.py
--rw-r--r--   0 nakatsugawa   (501) staff       (20)        0 2022-10-22 08:37:48.000000 blastengine-0.0.8/blastengine/__init__.py
-drwxr-xr-x   0 nakatsugawa   (501) staff       (20)        0 2024-02-06 07:53:26.887123 blastengine-0.0.8/blastengine.egg-info/
--rw-r--r--   0 nakatsugawa   (501) staff       (20)      506 2024-02-06 07:53:26.000000 blastengine-0.0.8/blastengine.egg-info/PKG-INFO
--rw-r--r--   0 nakatsugawa   (501) staff       (20)      375 2024-02-06 07:53:26.000000 blastengine-0.0.8/blastengine.egg-info/SOURCES.txt
--rw-r--r--   0 nakatsugawa   (501) staff       (20)        1 2024-02-06 07:53:26.000000 blastengine-0.0.8/blastengine.egg-info/dependency_links.txt
--rw-r--r--   0 nakatsugawa   (501) staff       (20)        9 2024-02-06 07:53:26.000000 blastengine-0.0.8/blastengine.egg-info/requires.txt
--rw-r--r--   0 nakatsugawa   (501) staff       (20)       12 2024-02-06 07:53:26.000000 blastengine-0.0.8/blastengine.egg-info/top_level.txt
--rw-r--r--   0 nakatsugawa   (501) staff       (20)       38 2024-02-06 07:53:26.887577 blastengine-0.0.8/setup.cfg
--rw-r--r--   0 nakatsugawa   (501) staff       (20)      656 2024-02-06 07:53:17.000000 blastengine-0.0.8/setup.py
+drwxr-xr-x   0 nakatsugawa   (501) staff       (20)        0 2024-04-18 08:10:53.386378 blastengine-0.0.9/
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)     1092 2022-10-22 08:37:48.000000 blastengine-0.0.9/LICENSE
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)      506 2024-04-18 08:10:53.386199 blastengine-0.0.9/PKG-INFO
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)      738 2024-04-18 07:55:07.000000 blastengine-0.0.9/README.md
+drwxr-xr-x   0 nakatsugawa   (501) staff       (20)        0 2024-04-18 08:10:53.385291 blastengine-0.0.9/blastengine/
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)     4482 2024-02-06 07:39:09.000000 blastengine-0.0.9/blastengine/Bulk.py
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)      463 2022-10-22 08:37:48.000000 blastengine-0.0.9/blastengine/Client.py
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)     2242 2023-08-21 13:14:55.000000 blastengine-0.0.9/blastengine/Job.py
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)     1562 2023-08-23 02:07:40.000000 blastengine-0.0.9/blastengine/Log.py
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)     3278 2024-04-18 08:07:20.000000 blastengine-0.0.9/blastengine/Mail.py
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)     4905 2024-04-18 08:05:50.000000 blastengine-0.0.9/blastengine/MailBase.py
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)     1943 2024-02-06 07:39:21.000000 blastengine-0.0.9/blastengine/Transaction.py
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)        0 2022-10-22 08:37:48.000000 blastengine-0.0.9/blastengine/__init__.py
+drwxr-xr-x   0 nakatsugawa   (501) staff       (20)        0 2024-04-18 08:10:53.386031 blastengine-0.0.9/blastengine.egg-info/
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)      506 2024-04-18 08:10:53.000000 blastengine-0.0.9/blastengine.egg-info/PKG-INFO
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)      375 2024-04-18 08:10:53.000000 blastengine-0.0.9/blastengine.egg-info/SOURCES.txt
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)        1 2024-04-18 08:10:53.000000 blastengine-0.0.9/blastengine.egg-info/dependency_links.txt
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)        9 2024-04-18 08:10:53.000000 blastengine-0.0.9/blastengine.egg-info/requires.txt
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)       12 2024-04-18 08:10:53.000000 blastengine-0.0.9/blastengine.egg-info/top_level.txt
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)       38 2024-04-18 08:10:53.386420 blastengine-0.0.9/setup.cfg
+-rw-r--r--   0 nakatsugawa   (501) staff       (20)      656 2024-04-18 08:10:15.000000 blastengine-0.0.9/setup.py
```

### Comparing `blastengine-0.0.8/LICENSE` & `blastengine-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `blastengine-0.0.8/README.md` & `blastengine-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -33,10 +33,17 @@
 try:
 	delivery_id = transaction.send()
 	print(delivery_id)
 except Exception as e:
 	print(e)
 ```
 
+## テスト
+
+```sh
+source venv/bin/activate
+pip install -r requirements.txt
+```
+
 ## License
 
 MIT License
```

### Comparing `blastengine-0.0.8/blastengine/Bulk.py` & `blastengine-0.0.9/blastengine/Bulk.py`

 * *Files identical despite different names*

### Comparing `blastengine-0.0.8/blastengine/Job.py` & `blastengine-0.0.9/blastengine/Job.py`

 * *Files identical despite different names*

### Comparing `blastengine-0.0.8/blastengine/Log.py` & `blastengine-0.0.9/blastengine/Log.py`

 * *Files identical despite different names*

### Comparing `blastengine-0.0.8/blastengine/Mail.py` & `blastengine-0.0.9/blastengine/Mail.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
 	def send(self, date = None):
 		if len(self._cc) > 0 or len(self._bcc) > 0:
 			if date is not None:
 				raise Exception('You can not specify the date when sending CC or BCC.')
 			if len(self._to) > 1:
 				raise Exception('You can not specify the to when sending CC or BCC.')
-		if date is not None or len(self._to) == 1:
+		if date is None:
 			return self.send_transaction_mail()
 		return self.send_bulk_mail()
 
 	def send_transaction_mail(self):
 		transaction = Transaction()
 		self.generate_base(transaction)
 		params = self._to[0]
@@ -63,26 +63,28 @@
 		if len(self._cc) > 0:
 			for cc in self._cc:
 				transaction.cc(cc)
 		if len(self._bcc) > 0:
 			for bcc in self._bcc:
 				transaction.bcc(bcc)
 		transaction.send()
+		self.delivery_id = transaction.delivery_id
 		return transaction.delivery_id
 
 	def send_bulk_mail(self):
 		bulk = Bulk()
 		self.generate_base(bulk)
 		if len(self._to) > 0:
 			for params in self._to:
 				data = {}
 				for insert_code in params['insert_code']:
 					data[re.sub('__(.*)__', '\\1', insert_code['key'])] = insert_code['value']
 				bulk.to(params['email'], data)
 		bulk.begin()
+		self.delivery_id = bulk.delivery_id
 		bulk.update()
 		bulk.send()
 		return bulk.delivery_id
 	
 	def generate_base(self, base):
 		base.subject(self._subject)
 		base.from_address(self._from['email'], self._from['name'])
```

### Comparing `blastengine-0.0.8/blastengine/MailBase.py` & `blastengine-0.0.9/blastengine/MailBase.py`

 * *Files 12% similar despite different names*

```diff
@@ -128,15 +128,23 @@
 		self.job_id = json_body['job_id']
 		return self.job_id
 
 	def handle_response(self, response):
 		json_body = MailBase.handle_error(response)
 		self.delivery_id = json_body['delivery_id']
 		return self.delivery_id
-	
+
+	def cancel(self):
+		headers = {
+			'Authorization': f'Bearer {self.client.token}',
+			'content-type': 'application/json'
+		}
+		response = requests.patch(f'{MailBase.base_url}/{self.delivery_id}/cancel', headers=headers)
+		return self.handle_response(response)
+
 	def delete(self):
 		headers = {
 			'Authorization': f'Bearer {self.client.token}',
 			'content-type': 'application/json'
 		}
 		response = requests.delete(f'{MailBase.base_url}/{self.delivery_id}', headers=headers)
 		return self.handle_response(response)
@@ -146,15 +154,15 @@
 			'Authorization': f'Bearer {self.client.token}',
 			'content-type': 'application/json'
 		}
 		response = requests.get(f'{MailBase.base_url}/{self.delivery_id}', headers=headers)
 		self.handle_response(response)
 		json_body = json.loads(response.content)
 		self.delivery_id = json_body['delivery_id']
-		self.fromAddress(json_body['from']['email'], json_body['from']['name'])
+		self.from_address(json_body['from']['email'], json_body['from']['name'])
 		self.delivery_type = json_body['delivery_type']
 		self.status = json_body['status']
 		self.subject(json_body['subject'])
 		self.text_part(json_body['text_part'])
 		self.html_part(json_body['html_part'])
 		self.total_count = json_body['total_count']
 		self.sent_count = json_body['sent_count']
```

### Comparing `blastengine-0.0.8/blastengine/Transaction.py` & `blastengine-0.0.9/blastengine/Transaction.py`

 * *Files identical despite different names*

### Comparing `blastengine-0.0.8/setup.py` & `blastengine-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="blastengine",
-    version="0.0.8",
+    version="0.0.9",
     author="goofmint",
     author_email="atsushi@moongift.jp",
     description="blastengine is SDK for blastengine",
     long_description="blastengine is SDK for blastengine. It supports text and html email with attachments.",
     long_description_content_type="text/markdown",
     url="https://blastengine.jp/",
     packages=setuptools.find_packages(),
```

