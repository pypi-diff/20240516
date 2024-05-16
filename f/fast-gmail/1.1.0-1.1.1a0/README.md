# Comparing `tmp/fast_gmail-1.1.0.tar.gz` & `tmp/fast_gmail-1.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_gmail-1.1.0.tar", last modified: Tue May 14 12:40:14 2024, max compression
+gzip compressed data, was "fast_gmail-1.1.1a0.tar", last modified: Thu May 16 05:50:13 2024, max compression
```

## Comparing `fast_gmail-1.1.0.tar` & `fast_gmail-1.1.1a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-05-14 12:40:14.799512 fast_gmail-1.1.0/
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.1.0/LICENSE
--rw-r--r--   0 aleti     (1000) aleti     (1000)    15624 2024-05-14 12:40:14.799512 fast_gmail-1.1.0/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    14864 2024-04-20 07:12:16.000000 fast_gmail-1.1.0/README.md
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-05-14 12:40:14.795512 fast_gmail-1.1.0/fast_gmail/
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       30 2024-04-15 08:44:02.000000 fast_gmail-1.1.0/fast_gmail/__init__.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      358 2024-04-15 06:27:06.000000 fast_gmail-1.1.0/fast_gmail/draft.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    22531 2024-05-14 12:36:50.000000 fast_gmail-1.1.0/fast_gmail/gmail.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     7203 2024-04-19 12:04:22.000000 fast_gmail-1.1.0/fast_gmail/helpers.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)    25256 2024-04-20 07:20:24.000000 fast_gmail-1.1.0/fast_gmail/message.py
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     3601 2024-04-08 06:37:52.000000 fast_gmail-1.1.0/fast_gmail/search.py
-drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-05-14 12:40:14.799512 fast_gmail-1.1.0/fast_gmail.egg-info/
--rw-r--r--   0 aleti     (1000) aleti     (1000)    15624 2024-05-14 12:40:14.000000 fast_gmail-1.1.0/fast_gmail.egg-info/PKG-INFO
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      323 2024-05-14 12:40:14.000000 fast_gmail-1.1.0/fast_gmail.egg-info/SOURCES.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-05-14 12:40:14.000000 fast_gmail-1.1.0/fast_gmail.egg-info/dependency_links.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-05-14 12:40:14.000000 fast_gmail-1.1.0/fast_gmail.egg-info/requires.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       11 2024-05-14 12:40:14.000000 fast_gmail-1.1.0/fast_gmail.egg-info/top_level.txt
--rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-05-14 12:40:14.799512 fast_gmail-1.1.0/setup.cfg
--rw-rw-r--   0 aleti     (1000) aleti     (1000)     1074 2024-05-14 12:40:06.000000 fast_gmail-1.1.0/setup.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-05-16 05:50:13.446225 fast_gmail-1.1.1a0/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1062 2024-04-08 06:15:40.000000 fast_gmail-1.1.1a0/LICENSE
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    15626 2024-05-16 05:50:13.446225 fast_gmail-1.1.1a0/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    14864 2024-04-20 07:12:16.000000 fast_gmail-1.1.1a0/README.md
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-05-16 05:50:13.446225 fast_gmail-1.1.1a0/fast_gmail/
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       30 2024-04-15 08:44:02.000000 fast_gmail-1.1.1a0/fast_gmail/__init__.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      358 2024-04-15 06:27:06.000000 fast_gmail-1.1.1a0/fast_gmail/draft.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    22222 2024-05-16 05:49:41.000000 fast_gmail-1.1.1a0/fast_gmail/gmail.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     7203 2024-04-19 12:04:22.000000 fast_gmail-1.1.1a0/fast_gmail/helpers.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)    25256 2024-04-20 07:20:24.000000 fast_gmail-1.1.1a0/fast_gmail/message.py
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     3601 2024-04-08 06:37:52.000000 fast_gmail-1.1.1a0/fast_gmail/search.py
+drwxrwxr-x   0 aleti     (1000) aleti     (1000)        0 2024-05-16 05:50:13.446225 fast_gmail-1.1.1a0/fast_gmail.egg-info/
+-rw-r--r--   0 aleti     (1000) aleti     (1000)    15626 2024-05-16 05:50:13.000000 fast_gmail-1.1.1a0/fast_gmail.egg-info/PKG-INFO
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      323 2024-05-16 05:50:13.000000 fast_gmail-1.1.1a0/fast_gmail.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)        1 2024-05-16 05:50:13.000000 fast_gmail-1.1.1a0/fast_gmail.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)      116 2024-05-16 05:50:13.000000 fast_gmail-1.1.1a0/fast_gmail.egg-info/requires.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       11 2024-05-16 05:50:13.000000 fast_gmail-1.1.1a0/fast_gmail.egg-info/top_level.txt
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)       38 2024-05-16 05:50:13.446225 fast_gmail-1.1.1a0/setup.cfg
+-rw-rw-r--   0 aleti     (1000) aleti     (1000)     1075 2024-05-16 05:50:07.000000 fast_gmail-1.1.1a0/setup.py
```

### Comparing `fast_gmail-1.1.0/LICENSE` & `fast_gmail-1.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.1.0/PKG-INFO` & `fast_gmail-1.1.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_gmail
-Version: 1.1.0
+Version: 1.1.1a0
 Summary: GmailApi wrapper
 Home-page: https://github.com/aleti1/fast_gmail
 Author: Aleti
 Author-email: aleti.open.source@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `fast_gmail-1.1.0/README.md` & `fast_gmail-1.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.1.0/fast_gmail/gmail.py` & `fast_gmail-1.1.1a0/fast_gmail/gmail.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,24 +31,24 @@
 	"https://www.googleapis.com/auth/contacts.readonly",
 	"https://www.googleapis.com/auth/contacts.other.readonly"
 ]
 
 
 class GmailApi(object):
 	"""https://googleapis.github.io/google-api-python-client/docs/dyn/gmail_v1.users.html"""
+	auth_token: Optional[dict] = None
 	credentials: Optional[Credentials] = None
 	google_service: GoogleService
 	max_results: int = MAX_RESULTS
 	SEPARATOR_SYMBOL: str
 	profile_data: Optional[GmailProfile] = None
 	redirect_uri: Optional[str] = None
 
 	def __init__(
 		self,
-		token_file_path: str = "token.json",
 		credentials_file_path: str = "credentials.json",
 		port: int = 3000, # set the local server port for Authorized redirect URI
 		separator_symbol: str = ", ",
 		user_id: str = "me",
 		application_type: ApplicationType = ApplicationType.WEB,
 		auth_token: Optional[dict] = None,
 		code: Optional[str] = None
@@ -56,18 +56,15 @@
 		"""https://github.com/googleapis/google-api-python-client/blob/main/docs/oauth-installed.md"""
 
 		# set separator for spliting/joining the array of existing previous_page_tokens for pagination
 		self.SEPARATOR_SYMBOL = separator_symbol
 
 		# The file token.json stores the user's access and refresh tokens, and is
 		# created automatically when the authorization flow completes for the first time.
-		if not auth_token:
-			if os.path.exists(token_file_path):
-				self.credentials = Credentials.from_authorized_user_file(token_file_path, SCOPES)
-		else:
+		if auth_token:
 			self.credentials = Credentials.from_authorized_user_info(auth_token, SCOPES)
 		self.auth_url: str = ""
 		# If there are no (valid) credentials available, let the user log in.
 		if not self.credentials or not self.credentials.valid:
 			if self.credentials and self.credentials.expired and self.credentials.refresh_token:
 				# refresh access token
 				self.credentials = Credentials(
@@ -116,21 +113,16 @@
                         )
 						if code:
 							self.flow.fetch_token(code=code)
 							self.credentials = self.flow.credentials
 						else:
 							self.auth_url = f"{self.flow.authorization_url()[0]}&prompt=consent"
 							return
-			if not auth_token:
-				# Save the credentials for the next run
-				with open(token_file_path, "w") as token:
-					token.write(self.credentials.to_json())
-			else:
-				# save the credentials as a dict
-				self.auth_token = json.loads(self.credentials.to_json())
+			# save the credentials as a dict
+			self.auth_token = json.loads(self.credentials.to_json())
 		try:
 			# Call the Gmail API and set the instance 
 			self.google_service = GoogleService(
 				service = build("gmail", "v1", credentials = self.credentials),
 				user_id = user_id
 			)
 		except HttpError as e:
```

### Comparing `fast_gmail-1.1.0/fast_gmail/helpers.py` & `fast_gmail-1.1.1a0/fast_gmail/helpers.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.1.0/fast_gmail/message.py` & `fast_gmail-1.1.1a0/fast_gmail/message.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.1.0/fast_gmail/search.py` & `fast_gmail-1.1.1a0/fast_gmail/search.py`

 * *Files identical despite different names*

### Comparing `fast_gmail-1.1.0/fast_gmail.egg-info/PKG-INFO` & `fast_gmail-1.1.1a0/fast_gmail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_gmail
-Version: 1.1.0
+Version: 1.1.1a0
 Summary: GmailApi wrapper
 Home-page: https://github.com/aleti1/fast_gmail
 Author: Aleti
 Author-email: aleti.open.source@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

### Comparing `fast_gmail-1.1.0/setup.py` & `fast_gmail-1.1.1a0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages
 
 with open("README.md", "r") as f:
     long_descrition=f.read()
 
 setup(
     name="fast_gmail",
-    version="1.1.0",
+    version="1.1.1a",
     description="GmailApi wrapper",
     long_description=long_descrition,
     long_description_content_type='text/markdown',
     author="Aleti",
     author_email="aleti.open.source@gmail.com",
     url="https://github.com/aleti1/fast_gmail",
     license="MIT",
```

