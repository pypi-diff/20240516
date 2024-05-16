# Comparing `tmp/cururo-1.1.1.tar.gz` & `tmp/cururo-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cururo-1.1.1.tar", last modified: Thu May 16 19:23:21 2024, max compression
+gzip compressed data, was "cururo-1.1.2.tar", last modified: Thu May 16 19:30:36 2024, max compression
```

## Comparing `cururo-1.1.1.tar` & `cururo-1.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:21.953410 cururo-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:17.000000 cururo-1.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-16 19:23:17.000000 cururo-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 19:23:17.000000 cururo-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-16 19:23:21.953410 cururo-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-16 19:23:17.000000 cururo-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:21.949410 cururo-1.1.1/cururo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:17.000000 cururo-1.1.1/cururo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-16 19:23:17.000000 cururo-1.1.1/cururo/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:21.953410 cururo-1.1.1/cururo/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:17.000000 cururo-1.1.1/cururo/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-16 19:23:17.000000 cururo-1.1.1/cururo/lib/ai_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-16 19:23:17.000000 cururo-1.1.1/cururo/lib/env_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-16 19:23:17.000000 cururo-1.1.1/cururo/lib/openai_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-16 19:23:17.000000 cururo-1.1.1/cururo/lib/web_publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-16 19:23:17.000000 cururo-1.1.1/cururo/reviewer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:21.953410 cururo-1.1.1/cururo/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:17.000000 cururo-1.1.1/cururo/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-16 19:23:17.000000 cururo-1.1.1/cururo/util/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-16 19:23:17.000000 cururo-1.1.1/cururo/util/processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-16 19:23:17.000000 cururo-1.1.1/cururo/util/publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-16 19:23:17.000000 cururo-1.1.1/cururo/util/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:21.953410 cururo-1.1.1/cururo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-16 19:23:21.000000 cururo-1.1.1/cururo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-16 19:23:21.000000 cururo-1.1.1/cururo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:23:21.000000 cururo-1.1.1/cururo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 19:23:21.000000 cururo-1.1.1/cururo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 19:23:21.000000 cururo-1.1.1/cururo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 19:23:21.000000 cururo-1.1.1/cururo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 19:23:17.000000 cururo-1.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:23:21.953410 cururo-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-16 19:23:17.000000 cururo-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:21.953410 cururo-1.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:17.000000 cururo-1.1.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:21.953410 cururo-1.1.1/test/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:17.000000 cururo-1.1.1/test/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 19:23:17.000000 cururo-1.1.1/test/lib/test_env_modes.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-16 19:23:17.000000 cururo-1.1.1/test/linter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:17.000000 cururo-1.1.1/test/test_openai_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-16 19:23:17.000000 cururo-1.1.1/test/test_publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:17.000000 cururo-1.1.1/test/test_response_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:23:17.000000 cururo-1.1.1/test/test_response_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-16 19:23:17.000000 cururo-1.1.1/test/test_reviewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:36.476067 cururo-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:32.000000 cururo-1.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-16 19:30:32.000000 cururo-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 19:30:32.000000 cururo-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-16 19:30:36.476067 cururo-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-16 19:30:32.000000 cururo-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:36.472067 cururo-1.1.2/cururo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:32.000000 cururo-1.1.2/cururo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-16 19:30:32.000000 cururo-1.1.2/cururo/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:36.472067 cururo-1.1.2/cururo/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:32.000000 cururo-1.1.2/cururo/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-16 19:30:32.000000 cururo-1.1.2/cururo/lib/ai_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-16 19:30:32.000000 cururo-1.1.2/cururo/lib/env_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-16 19:30:32.000000 cururo-1.1.2/cururo/lib/openai_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-16 19:30:32.000000 cururo-1.1.2/cururo/lib/web_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-16 19:30:32.000000 cururo-1.1.2/cururo/reviewer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:36.472067 cururo-1.1.2/cururo/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:32.000000 cururo-1.1.2/cururo/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-16 19:30:32.000000 cururo-1.1.2/cururo/util/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-16 19:30:32.000000 cururo-1.1.2/cururo/util/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-16 19:30:32.000000 cururo-1.1.2/cururo/util/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-16 19:30:32.000000 cururo-1.1.2/cururo/util/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:36.472067 cururo-1.1.2/cururo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-16 19:30:36.000000 cururo-1.1.2/cururo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-16 19:30:36.000000 cururo-1.1.2/cururo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:30:36.000000 cururo-1.1.2/cururo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 19:30:36.000000 cururo-1.1.2/cururo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 19:30:36.000000 cururo-1.1.2/cururo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 19:30:36.000000 cururo-1.1.2/cururo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 19:30:32.000000 cururo-1.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:30:36.476067 cururo-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-16 19:30:32.000000 cururo-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:36.472067 cururo-1.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:32.000000 cururo-1.1.2/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:36.472067 cururo-1.1.2/test/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:32.000000 cururo-1.1.2/test/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 19:30:32.000000 cururo-1.1.2/test/lib/test_env_modes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-16 19:30:32.000000 cururo-1.1.2/test/linter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:32.000000 cururo-1.1.2/test/test_openai_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-16 19:30:32.000000 cururo-1.1.2/test/test_publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:32.000000 cururo-1.1.2/test/test_response_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:30:32.000000 cururo-1.1.2/test/test_response_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-16 19:30:32.000000 cururo-1.1.2/test/test_reviewer.py
```

### Comparing `cururo-1.1.1/LICENSE` & `cururo-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cururo-1.1.1/PKG-INFO` & `cururo-1.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cururo
-Version: 1.1.1
+Version: 1.1.2
 Summary: Review an item using OpenAI.
 Author: Agustin Rios
 Author-email: arios6@uc.cl
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `cururo-1.1.1/README.md` & `cururo-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cururo-1.1.1/cururo/cli.py` & `cururo-1.1.2/cururo/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     parser.add_argument('--item', type=str, required=True, help='Item to add to the review.')
     parser.add_argument('--openai-key', type=str, default=DEFAULT_OPENAI_KEY, help='OpenAI API key.', required=DEFAULT_OPENAI_KEY is None)
     parser.add_argument('--assistant-id', type=str, default=DEFAULT_ASSISTANT_ID, help='OpenAI assistant ID.', required=DEFAULT_ASSISTANT_ID is None)
     parser.add_argument('--mode', type=str, default=DEFAULT_MODE, help='Mode to run the review in.', choices=EnvModes.allowed_modes)
     parser.add_argument('--web-url', type=str, help='URL to post the response to.', default=None)
     parser.add_argument('--web-secret', type=str, help='Secret to use when posting the response to the URL.', default=None)
     parser.add_argument('--web-processor', type=str, help='Processor to use when posting the response to the URL.', default=None)
-    parser.add_argument('--version', action='version', version='%(prog)s 1.1.1')
+    parser.add_argument('--version', action='version', version='%(prog)s 1.1.2')
     
     args = parser.parse_args()
 
     if args.web_url and not args.web_secret:
         parser.error('--web-secret is required when using --web-url')
 
     if args.web_processor:
@@ -39,14 +39,14 @@
 
     # check url
     if args.web_url:
         publisher = WebPublisher(web_url=args.web_url, web_secret=args.web_secret, processor=args.web_processor)
     else:
         publisher = DEFAULT_PUBLISHER
 
-    handler = ResponseHandler(publisher=publisher, additional_actions=[args.action])
+    handler = ResponseHandler(publisher=publisher, additional_actions=[custom_action])
     reviewer = Reviewer(openai_api_key=args.openai_key, assistant_id=args.assistant_id, mode=args.mode)
     reviewer.append_item(args.item)
     reviewer.execute(handler.handle_response)
 
 if __name__ == '__main__':
     main()
```

### Comparing `cururo-1.1.1/cururo/lib/ai_env.py` & `cururo-1.1.2/cururo/lib/ai_env.py`

 * *Files identical despite different names*

### Comparing `cururo-1.1.1/cururo/lib/env_modes.py` & `cururo-1.1.2/cururo/lib/env_modes.py`

 * *Files identical despite different names*

### Comparing `cururo-1.1.1/cururo/lib/openai_assistant.py` & `cururo-1.1.2/cururo/lib/openai_assistant.py`

 * *Files identical despite different names*

### Comparing `cururo-1.1.1/cururo/lib/web_publisher.py` & `cururo-1.1.2/cururo/lib/web_publisher.py`

 * *Files identical despite different names*

### Comparing `cururo-1.1.1/cururo/reviewer.py` & `cururo-1.1.2/cururo/reviewer.py`

 * *Files identical despite different names*

### Comparing `cururo-1.1.1/cururo/util/handler.py` & `cururo-1.1.2/cururo/util/handler.py`

 * *Files identical despite different names*

### Comparing `cururo-1.1.1/cururo/util/processor.py` & `cururo-1.1.2/cururo/util/processor.py`

 * *Files identical despite different names*

### Comparing `cururo-1.1.1/cururo/util/publisher.py` & `cururo-1.1.2/cururo/util/publisher.py`

 * *Files identical despite different names*

### Comparing `cururo-1.1.1/cururo/util/util.py` & `cururo-1.1.2/cururo/util/util.py`

 * *Files identical despite different names*

### Comparing `cururo-1.1.1/cururo.egg-info/PKG-INFO` & `cururo-1.1.2/cururo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cururo
-Version: 1.1.1
+Version: 1.1.2
 Summary: Review an item using OpenAI.
 Author: Agustin Rios
 Author-email: arios6@uc.cl
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `cururo-1.1.1/cururo.egg-info/SOURCES.txt` & `cururo-1.1.2/cururo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cururo-1.1.1/setup.py` & `cururo-1.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cururo',
-    version='1.1.1',
+    version='1.1.2',
     author='Agustin Rios',
     author_email='arios6@uc.cl',
     description='Review an item using OpenAI.',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=open("./requirements.txt").read().splitlines(),
```

### Comparing `cururo-1.1.1/test/lib/test_env_modes.py` & `cururo-1.1.2/test/lib/test_env_modes.py`

 * *Files identical despite different names*

### Comparing `cururo-1.1.1/test/test_publisher.py` & `cururo-1.1.2/test/test_publisher.py`

 * *Files identical despite different names*

