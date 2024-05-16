# Comparing `tmp/tikapi-3.1.50.tar.gz` & `tmp/tikapi-3.1.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tikapi-3.1.50.tar", last modified: Tue Apr 16 17:01:41 2024, max compression
+gzip compressed data, was "tikapi-3.1.60.tar", last modified: Thu May 16 11:00:35 2024, max compression
```

## Comparing `tikapi-3.1.50.tar` & `tikapi-3.1.60.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 17:01:41.904266 tikapi-3.1.50/
--rw-rw-rw-   0        0        0       67 2022-12-07 21:27:40.000000 tikapi-3.1.50/MANIFEST.in
--rw-rw-rw-   0        0        0     1861 2024-04-16 17:01:41.904266 tikapi-3.1.50/PKG-INFO
--rw-rw-rw-   0        0        0     1106 2022-08-29 11:23:45.000000 tikapi-3.1.50/README.md
--rw-rw-rw-   0        0        0      121 2024-04-16 17:01:41.905266 tikapi-3.1.50/setup.cfg
--rw-rw-rw-   0        0        0      704 2024-04-16 17:01:19.000000 tikapi-3.1.50/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-16 17:01:41.899266 tikapi-3.1.50/tikapi/
--rw-rw-rw-   0        0        0     3228 2023-09-22 16:50:46.000000 tikapi-3.1.50/tikapi/__init__.py
--rw-rw-rw-   0        0        0    89849 2023-10-17 18:24:12.000000 tikapi-3.1.50/tikapi/api.py
-drwxrwxrwx   0        0        0        0 2024-04-16 17:01:41.903266 tikapi-3.1.50/tikapi.egg-info/
--rw-rw-rw-   0        0        0     1861 2024-04-16 17:01:41.000000 tikapi-3.1.50/tikapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2024-04-16 17:01:41.000000 tikapi-3.1.50/tikapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 17:01:41.000000 tikapi-3.1.50/tikapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-07-07 14:30:05.000000 tikapi-3.1.50/tikapi.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        9 2024-04-16 17:01:41.000000 tikapi-3.1.50/tikapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-16 17:01:41.000000 tikapi-3.1.50/tikapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 11:00:35.045122 tikapi-3.1.60/
+-rw-rw-rw-   0        0        0       67 2022-12-07 21:27:40.000000 tikapi-3.1.60/MANIFEST.in
+-rw-rw-rw-   0        0        0     1861 2024-05-16 11:00:35.045122 tikapi-3.1.60/PKG-INFO
+-rw-rw-rw-   0        0        0     1106 2022-08-29 11:23:45.000000 tikapi-3.1.60/README.md
+-rw-rw-rw-   0        0        0      121 2024-05-16 11:00:35.046121 tikapi-3.1.60/setup.cfg
+-rw-rw-rw-   0        0        0      704 2024-05-16 10:55:24.000000 tikapi-3.1.60/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:00:35.040121 tikapi-3.1.60/tikapi/
+-rw-rw-rw-   0        0        0     3228 2023-09-22 16:50:46.000000 tikapi-3.1.60/tikapi/__init__.py
+-rw-rw-rw-   0        0        0    92547 2024-05-16 10:56:02.000000 tikapi-3.1.60/tikapi/api.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:00:35.045122 tikapi-3.1.60/tikapi.egg-info/
+-rw-rw-rw-   0        0        0     1861 2024-05-16 11:00:34.000000 tikapi-3.1.60/tikapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-05-16 11:00:35.000000 tikapi-3.1.60/tikapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:00:34.000000 tikapi-3.1.60/tikapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-07-07 14:30:05.000000 tikapi-3.1.60/tikapi.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2024-05-16 11:00:34.000000 tikapi-3.1.60/tikapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 11:00:34.000000 tikapi-3.1.60/tikapi.egg-info/top_level.txt
```

### Comparing `tikapi-3.1.50/PKG-INFO` & `tikapi-3.1.60/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikapi
-Version: 3.1.50
+Version: 3.1.60
 Summary: TikAPI | TikTok Unofficial API
 Home-page: https://www.tikapi.io
 Author: TikAPI
 Author-email: contact@tikapi.io
 License: TikAPI
 Description: # Unofficial TikTok API <img src='https://img.shields.io/npm/v/tikapi'> <img src='https://img.shields.io/pypi/v/tikapi'>
```

### Comparing `tikapi-3.1.50/README.md` & `tikapi-3.1.60/README.md`

 * *Files identical despite different names*

### Comparing `tikapi-3.1.50/setup.py` & `tikapi-3.1.60/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 INSTALL_REQUIRES = [
    'requests',
 ]
 
 setup(
     name='tikapi',
-    version='3.1.50',
+    version='3.1.60',
     description='TikAPI | TikTok Unofficial API',
     long_description_content_type="text/markdown",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     license='TikAPI',
     author='TikAPI',
     author_email='contact@tikapi.io',
     url='https://www.tikapi.io',
```

### Comparing `tikapi-3.1.50/tikapi/__init__.py` & `tikapi-3.1.60/tikapi/__init__.py`

 * *Files identical despite different names*

### Comparing `tikapi-3.1.50/tikapi/api.py` & `tikapi-3.1.60/tikapi/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -565,14 +565,30 @@
 			'''
 				Get hashtag posts 
 			'''
 			count = None if count is cls.hashtag.__defaults__[2] else count
 			return wrap({"help":"Get hashtag posts","comment":"Your first request should be using the hashtag `name` parameter, then the following requests should be using the `id` parameter which you have stored from the first request (returned in response `challengeInfo > challenge > id`). <br/><a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","path":"/public/hashtag","params":{"id":{"validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","help":"The hashtag ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","example":"4655293"},"name":{"type":"string","help":"The hashtag name"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.hashtag")(id=id, name=name, count=count, cursor=cursor, country=country, session_id=session_id, **otherParams)
 	
 		@classmethod
+		def commentsList(cls, media_id: str = None, count: int = Default(30), cursor: int = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
+			'''
+				Get a video comments list 
+			'''
+			count = None if count is cls.commentsList.__defaults__[1] else count
+			return wrap({"help":"Get a video comments list","path":"/public/comment/list","params":{"media_id":{"help":"The video ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","type":"string","validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","required":True,"example":"7109178205151464746"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"number","validate":"^[0-9]+$"}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "Public.commentsList")(media_id=media_id, count=count, cursor=cursor, country=country, session_id=session_id, **otherParams)
+	
+		@classmethod
+		def commentRepliesList(cls, media_id: str = None, comment_id: str = None, count: int = Default(30), cursor: int = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
+			'''
+				Get a comment replies list 
+			'''
+			count = None if count is cls.commentRepliesList.__defaults__[2] else count
+			return wrap({"help":"Get a comment replies list","path":"/public/comment/reply/list","params":{"media_id":{"help":"The video ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","type":"string","validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","required":True,"example":"7109178205151464746"},"comment_id":{"validate":"^[0-9]+$","help":"The comment ID","type":"string","required":True,"example":"7109185042560680750"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"number","validate":"^[0-9]+$"}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "Public.commentRepliesList")(media_id=media_id, comment_id=comment_id, count=count, cursor=cursor, country=country, session_id=session_id, **otherParams)
+	
+		@classmethod
 		def music(cls, id: str = None, count: int = Default(30), cursor: str = None, country: str = None, session_id: int = None, **otherParams) -> APIResponse:
 			'''
 				Get music posts 
 			'''
 			count = None if count is cls.music.__defaults__[1] else count
 			return wrap({"help":"Get music posts","comment":"Get a list of posts that are using this music. <br/><a target=\"_blank\" href='https://helpdesk.tikapi.io/portal/en/kb/articles/how-to-download-tiktok-videos'>\nLearn more about downloading videos</a>\n\n","path":"/public/music","params":{"id":{"validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","type":"string","help":"The music ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","required":True,"example":"28459463"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"string","validate":"^[0-9]+$"}},"$other":{"openapi":{"hideParams":["session_id"]}},"method":"GET"}, cls.__get_options__(), "Public.music")(id=id, count=count, cursor=cursor, country=country, session_id=session_id, **otherParams)
 	
@@ -632,23 +648,23 @@
 	
 		@classmethod
 		def list(cls, media_id: str = None, count: int = Default(30), cursor: int = None, **otherParams) -> APIResponse:
 			'''
 				Get a video comments list 
 			'''
 			count = None if count is cls.list.__defaults__[1] else count
-			return wrap({"help":"Get a video comments list","path":"/comment/list","params":{"media_id":{"help":"The video ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","type":"string","validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","required":True,"example":"7109178205151464746"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"number","validate":"^[0-9]+$"}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "UserPostsComments.list")(media_id=media_id, count=count, cursor=cursor, **otherParams)
+			return wrap({"help":"Get a video comments list","path":"/user/comment/list","params":{"media_id":{"help":"The video ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","type":"string","validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","required":True,"example":"7109178205151464746"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"number","validate":"^[0-9]+$"}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "UserPostsComments.list")(media_id=media_id, count=count, cursor=cursor, **otherParams)
 	
 		@classmethod
 		def replies(cls, media_id: str = None, comment_id: str = None, count: int = Default(30), cursor: int = None, **otherParams) -> APIResponse:
 			'''
 				Get a comment reply list 
 			'''
 			count = None if count is cls.replies.__defaults__[2] else count
-			return wrap({"help":"Get a comment reply list","path":"/comment/reply/list","params":{"media_id":{"help":"The video ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","type":"string","validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","required":True,"example":"7109178205151464746"},"comment_id":{"validate":"^[0-9]+$","help":"The comment ID","type":"string","required":True,"example":"7109185042560680750"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"number","validate":"^[0-9]+$"}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "UserPostsComments.replies")(media_id=media_id, comment_id=comment_id, count=count, cursor=cursor, **otherParams)
+			return wrap({"help":"Get a comment reply list","path":"/user/comment/reply/list","params":{"media_id":{"help":"The video ID. Can also be a short TikTok link (e.g. vm.tiktok.com/UwU)","type":"string","validate":"^([0-9]+|https?://vm.tiktok.com/[a-zA-Z0-9]+/?)$","required":True,"example":"7109178205151464746"},"comment_id":{"validate":"^[0-9]+$","help":"The comment ID","type":"string","required":True,"example":"7109185042560680750"},"count":{"example":30,"default":30,"max":30,"type":"number","help":"Maximum amount of items for one request","validate":"^[0-9]{1,2}$"},"cursor":{"help":"The starting point of the items list. Returned in every response, should be included in the next request for iteration.<br><br> *(A simple iteration method is already implemented in the Javascript & Python libraries as seen in the request samples)*","type":"number","validate":"^[0-9]+$"}},"$other":{"openapi":{}},"method":"GET"}, cls.__get_options__(), "UserPostsComments.replies")(media_id=media_id, comment_id=comment_id, count=count, cursor=cursor, **otherParams)
 	
 		@classmethod
 		def post(cls, media_id: str = None, text: str = None, reply_comment_id: str = None, has_tags: bool = None, **otherParams) -> APIResponse:
 			'''
 				Post a new comment 
 			'''
```

### Comparing `tikapi-3.1.50/tikapi.egg-info/PKG-INFO` & `tikapi-3.1.60/tikapi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tikapi
-Version: 3.1.50
+Version: 3.1.60
 Summary: TikAPI | TikTok Unofficial API
 Home-page: https://www.tikapi.io
 Author: TikAPI
 Author-email: contact@tikapi.io
 License: TikAPI
 Description: # Unofficial TikTok API <img src='https://img.shields.io/npm/v/tikapi'> <img src='https://img.shields.io/pypi/v/tikapi'>
```

