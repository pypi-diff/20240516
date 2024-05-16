# Comparing `tmp/jzchatbot-59.83.99.tar.gz` & `tmp/jzchatbot-59.84.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzchatbot-59.83.99.tar", last modified: Mon May 13 00:43:42 2024, max compression
+gzip compressed data, was "jzchatbot-59.84.0.tar", last modified: Thu May 16 03:09:49 2024, max compression
```

## Comparing `jzchatbot-59.83.99.tar` & `jzchatbot-59.84.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 00:43:42.556788 jzchatbot-59.83.99/
--rw-rw-rw-   0        0        0     1067 2024-05-09 03:25:46.000000 jzchatbot-59.83.99/LICENSE
--rw-rw-rw-   0        0        0      343 2024-05-13 00:43:42.552958 jzchatbot-59.83.99/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-10 01:46:29.000000 jzchatbot-59.83.99/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 00:43:42.499894 jzchatbot-59.83.99/jzchatbot/
--rw-rw-rw-   0        0        0     3868 2024-05-13 00:43:22.000000 jzchatbot-59.83.99/jzchatbot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 00:43:42.550068 jzchatbot-59.83.99/jzchatbot.egg-info/
--rw-rw-rw-   0        0        0      343 2024-05-13 00:43:42.000000 jzchatbot-59.83.99/jzchatbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2024-05-13 00:43:42.000000 jzchatbot-59.83.99/jzchatbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 00:43:42.000000 jzchatbot-59.83.99/jzchatbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2024-05-13 00:43:42.000000 jzchatbot-59.83.99/jzchatbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-13 00:43:42.000000 jzchatbot-59.83.99/jzchatbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 00:43:42.556788 jzchatbot-59.83.99/setup.cfg
--rw-rw-rw-   0        0        0      530 2024-05-13 00:43:33.000000 jzchatbot-59.83.99/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 03:09:49.361069 jzchatbot-59.84.0/
+-rw-rw-rw-   0        0        0     1067 2024-05-09 03:25:46.000000 jzchatbot-59.84.0/LICENSE
+-rw-rw-rw-   0        0        0      342 2024-05-16 03:09:49.358065 jzchatbot-59.84.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-10 01:46:29.000000 jzchatbot-59.84.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 03:09:49.316141 jzchatbot-59.84.0/jzchatbot/
+-rw-rw-rw-   0        0        0     5227 2024-05-16 03:09:29.000000 jzchatbot-59.84.0/jzchatbot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 03:09:49.356080 jzchatbot-59.84.0/jzchatbot.egg-info/
+-rw-rw-rw-   0        0        0      342 2024-05-16 03:09:49.000000 jzchatbot-59.84.0/jzchatbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2024-05-16 03:09:49.000000 jzchatbot-59.84.0/jzchatbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 03:09:49.000000 jzchatbot-59.84.0/jzchatbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-16 03:09:49.000000 jzchatbot-59.84.0/jzchatbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-16 03:09:49.000000 jzchatbot-59.84.0/jzchatbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 03:09:49.362065 jzchatbot-59.84.0/setup.cfg
+-rw-rw-rw-   0        0        0      530 2024-05-16 03:09:39.000000 jzchatbot-59.84.0/setup.py
```

### Comparing `jzchatbot-59.83.99/LICENSE` & `jzchatbot-59.84.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jzchatbot-59.83.99/jzchatbot/__init__.py` & `jzchatbot-59.84.0/jzchatbot/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,20 +3,26 @@
 import re
 import json
 import pyttsx3
 import speech_recognition as sr
 from nltk.tokenize import word_tokenize
 from nltk.corpus import stopwords
 from textblob import TextBlob
+import nltk
+
+# Ensure necessary NLTK data is downloaded
+nltk.download('punkt')
+nltk.download('stopwords')
 
 class Bot:
     def __init__(self, name, jsonfile):
         self.name = name
         self.conversations = self.load_conversations(jsonfile)
         self.engine = pyttsx3.init()
+        self.user_name = None
 
     def preprocess_text(self, text):
         # Correct spelling mistakes using TextBlob
         corrected_text = str(TextBlob(text).correct())
 
         # Tokenization
         tokens = word_tokenize(corrected_text)
@@ -62,41 +68,68 @@
         self.engine.say(text)
         self.engine.runAndWait()
 
     def load_conversations(self, file_path):
         with open(file_path, 'r') as file:
             return json.load(file)
 
-    def run(self):
-        while True:
-            user_input = input("You: ")  # Wait for user to input command
-            if user_input.lower() == '/m on':
-                self.listen_for_input()  # Start listening for speech input
-            elif user_input.lower() == 'exit':
-                break
+    def get_user_name(self):
+        if not self.user_name:
+            self.user_name = input("Hi! What's your name? ")
+        return self.user_name
+
+    def set_user_name(self, new_name=None):
+        if not new_name:
+            new_name = input("What's your new name? ")
+        self.user_name = new_name
+        print(f"Got it! I'll call you {self.user_name} from now on.")
+
+    def process_input(self, user_input):
+        user_input_lower = user_input.lower()
+        if user_input_lower == "what's my name?":
+            if self.user_name:
+                print(f"Your name is {self.user_name}.")
             else:
-                bot_response = self.generate_response(user_input)
-                print(f"{self.name}: {bot_response}")
-                self.speak(bot_response)
+                print("I don't know your name yet.")
+        elif user_input_lower.startswith("change my name to "):
+            new_name = user_input[17:].strip()  # Extract the new name from the input
+            self.set_user_name(new_name)
+        elif user_input_lower == "change my name":
+            self.set_user_name()
+        else:
+            bot_response = self.generate_response(user_input)
+            print(f"{self.name}: {bot_response}")
+            self.speak(bot_response)
+
+    def run(self):
+        self.get_user_name()
+        try:
+            while True:
+                user_input = input(f"{self.user_name if self.user_name else 'You'}: ")  # Wait for user to input command
+                if user_input.lower() == '/m on':
+                    self.listen_for_input()  # Start listening for speech input
+                elif user_input.lower() == 'exit':
+                    break
+                else:
+                    self.process_input(user_input)
+        except KeyboardInterrupt:
+            print("\nExiting...")
+        finally:
+            self.engine.stop()
 
     def listen_for_input(self):
         recognizer = sr.Recognizer()
         with sr.Microphone() as source:
             print("Listening...")
             recognizer.adjust_for_ambient_noise(source)  # Adjust microphone for ambient noise
             audio = recognizer.listen(source)  # Listen for audio input
 
         try:
             print("Recognizing...")
             user_input = recognizer.recognize_google(audio)  # Recognize speech using Google Speech Recognition
-            print("You:", user_input)  # Print "You: " before the recognized user input
+            print(f"{self.user_name if self.user_name else 'You'}: {user_input}")  # Print "You: " before the recognized user input
             # Process the recognized user input here
-            bot_response = self.generate_response(user_input)
-            print(f"{self.name}: {bot_response}")
-            self.speak(bot_response)
+            self.process_input(user_input)
         except sr.UnknownValueError:
-            print("JZ: Sorry, I could not understand your speech.")
+            print(f"{self.name}: Sorry, I could not understand your speech.")
         except sr.RequestError as e:
-            print("JZ: Speech recognition request failed:", e)
-
-
-
+            print(f"{self.name}: Speech recognition request failed:", e)
```

### Comparing `jzchatbot-59.83.99/setup.py` & `jzchatbot-59.84.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
 
 with open("README.md", "r") as fh: 
 	description = fh.read() 
 
 setuptools.setup( 
 	name="jzchatbot", 
-	version="59.83.99", 
+	version="59.84.00", 
 	author="JZ Enterprises", 
 	packages=setuptools.find_packages(), 
 	description="A package that creates advanced AI chatbots", 
 	long_description=description, 
 	long_description_content_type="text/markdown", 
 	license='MIT', 
 	python_requires='>=3.8',
```

