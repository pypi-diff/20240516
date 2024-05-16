# Comparing `tmp/pybangla-1.0.9.dev0.tar.gz` & `tmp/pybangla-1.0.9.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybangla-1.0.9.dev0.tar", last modified: Fri May 10 08:11:57 2024, max compression
+gzip compressed data, was "pybangla-1.0.9.dev1.tar", last modified: Thu May 16 18:48:33 2024, max compression
```

## Comparing `pybangla-1.0.9.dev0.tar` & `pybangla-1.0.9.dev1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:11:57.329431 pybangla-1.0.9.dev0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:11:51.000000 pybangla-1.0.9.dev0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    15661 2024-05-10 08:11:57.329431 pybangla-1.0.9.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15098 2024-05-10 08:11:51.000000 pybangla-1.0.9.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:11:57.325431 pybangla-1.0.9.dev0/pybangla/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-10 08:11:51.000000 pybangla-1.0.9.dev0/pybangla/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:11:57.329431 pybangla-1.0.9.dev0/pybangla/module/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 08:11:51.000000 pybangla-1.0.9.dev0/pybangla/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19998 2024-05-10 08:11:51.000000 pybangla-1.0.9.dev0/pybangla/module/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8359 2024-05-10 08:11:51.000000 pybangla-1.0.9.dev0/pybangla/module/date_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-10 08:11:51.000000 pybangla-1.0.9.dev0/pybangla/module/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-10 08:11:51.000000 pybangla-1.0.9.dev0/pybangla/module/number_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    20282 2024-05-10 08:11:51.000000 pybangla-1.0.9.dev0/pybangla/module/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-10 08:11:51.000000 pybangla-1.0.9.dev0/pybangla/module/word_to_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    10137 2024-05-10 08:11:51.000000 pybangla-1.0.9.dev0/pybangla/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:11:57.329431 pybangla-1.0.9.dev0/pybangla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15661 2024-05-10 08:11:57.000000 pybangla-1.0.9.dev0/pybangla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-10 08:11:57.000000 pybangla-1.0.9.dev0/pybangla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 08:11:57.000000 pybangla-1.0.9.dev0/pybangla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-10 08:11:57.000000 pybangla-1.0.9.dev0/pybangla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 08:11:57.000000 pybangla-1.0.9.dev0/pybangla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 08:11:57.329431 pybangla-1.0.9.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-10 08:11:51.000000 pybangla-1.0.9.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 08:11:57.329431 pybangla-1.0.9.dev0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-05-10 08:11:51.000000 pybangla-1.0.9.dev0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:48:33.663015 pybangla-1.0.9.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20323 2024-05-16 18:48:33.663015 pybangla-1.0.9.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:48:33.659016 pybangla-1.0.9.dev1/pybangla/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/matching.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:48:33.663015 pybangla-1.0.9.dev1/pybangla/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/module/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/module/date_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/module/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17040 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/module/number_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27661 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/module/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22922 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/module/word_to_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17489 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/pybangla/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:48:33.663015 pybangla-1.0.9.dev1/pybangla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20323 2024-05-16 18:48:33.000000 pybangla-1.0.9.dev1/pybangla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-16 18:48:33.000000 pybangla-1.0.9.dev1/pybangla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:48:33.000000 pybangla-1.0.9.dev1/pybangla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-16 18:48:33.000000 pybangla-1.0.9.dev1/pybangla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 18:48:33.000000 pybangla-1.0.9.dev1/pybangla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 18:48:33.663015 pybangla-1.0.9.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:48:33.663015 pybangla-1.0.9.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-16 18:48:29.000000 pybangla-1.0.9.dev1/tests/test.py
```

### Comparing `pybangla-1.0.9.dev0/PKG-INFO` & `pybangla-1.0.9.dev1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: pybangla
-Version: 1.0.9.dev0
+Version: 1.0.9.dev1
 Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
 Home-page: https://github.com/saiful9379/pybangla
 Author: saiful
 Author-email: saifulbrur79@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: DateTime
 Requires-Dist: num2words
+Requires-Dist: python-Levenshtein
+Requires-Dist: fuzzywuzzy
 
 
 PYBANGLA is a python3 package for Bangla Number, DateTime and Text Normalizer and Date Extraction. This package can be used Normalize the text number and date (ex: number to text vice versa). This framework  also can be used Django, Flask, FastAPI, and others. PYBANGLA module supported operating system Linux/Unix, Mac OS and Windows.
 Available Features
 
 Features available in PYBANGLA:
 
@@ -35,14 +37,26 @@
 ```
 
 
 # Usage
 
 ## 1. Text Normalization
 ### It supports converting Bangla abbreviations, symbols, and currencies to Bangla textual format.
+<h2 style='color:LightBlue'>(UPDATE) It supports year conversion like </h2>
+
+* "১৯৮৭-র" to "উনিশশো সাতাশি এর"
+* "১৯৯৫ সালে" to "উনিশশো পঁচানব্বই সালে"
+* "২০২৬-২৭" to "দুই হাজার ছাব্বিশ সাতাশ"
+
+<h3 style='color:LightBlue'> Now it also has the abbreviation for units of temperature </h3>
+
+* "৪৪°F" to "চুয়াল্লিশ ডিগ্রী ফারেনহাইট"
+* "৪৪°C" to "চুয়াল্লিশ ডিগ্রী সেলসিয়াস"
+
+<h2> </h2>
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 text = "রাহিম ক্লাস ওয়ান এ ১ম, এন্ড বাসার ক্লাস এ ৩৩ তম, সে জন্য ২০৩০ শতাব্দীতে ¥২০৩০.১২৩৪ দিতে হয়েছে"
 text = nrml.text_normalizer(text)
 
@@ -78,30 +92,97 @@
 text = nrml.text_normalizer(text)
 #output:
 
 সম্মেলনটি পাঁচ সেপ্টেম্বর দুই হাজার তেইশ তারিখে নির্ধারিত করা হয়েছে. এক এপ্রিল দুই হাজার তেইশ
 
 ```
 
+```py
+
+text = "দাড়াবে?না হারিস আনিস জোসেফের মতো খালাস!!!???"
+text = nmlr.text_normalizer(text)    
+
+#output:
+
+দাড়াবে? না হারিস আনিস জোসেফের মতো খালাস!
+```
+
+```py
+
+text = "আজব এক ধর্ম। অবমাননার অর্থ কি ? ? কেউ বলবেন? ? মেধাহীন জাতি তা আর একবার প্রমাণ করলো ।"
+text = nmlr.text_normalizer(text)
+
+#output:
+
+আজব এক ধর্ম। অবমাননার অর্থ কি? কেউ বলবেন? মেধাহীন জাতি তা আর একবার প্রমাণ করলো।
+```
+
+```py
+text = "সে যা-ই হোক, সত্যিকারের এমন পাকা পোনা শেষ বার নেমন্তন্ন বাড়িতে খেয়েছি ১৯৮৭-র এপ্রিলে।"
+text = nrml.text_normalizer(text)
+print(f"{text}")
+
+#output:
+সে যা ই হোক, সত্যিকারের এমন পাকা পোনা শেষ বার নেমন্তন্ন বাড়িতে খেয়েছি উনিশশো সাতাশি এর এপ্রিলে।
+```
+
+```py
+text = "আজকের তাপমাত্রা ৪৪°F"
+text = nrml.text_normalizer(text)
+print(f"{text}")
+
+#output:
+আজকের তাপমাত্রা চুয়াল্লিশ ডিগ্রী ফারেনহাইট
+```
+
+```py
+text = "নতুন নীতিমালায় ২০২৬-২৭ অর্থবছরে দেশের রপ্তানি আয় ১১ হাজার কোটি মার্কিন ডলারে উন্নীত করার ১৯৯৫ সালে লক্ষ্যমাত্রা নির্ধারণ করা হয়েছে।"
+text = nrml.text_normalizer(text)
+print(f"{text}")
+
+#output:
+নতুন নীতিমালায় দুই হাজার ছাব্বিশ সাতাশ অর্থবছরে দেশের রপ্তানি আয় এগারো হাজার কোটি মার্কিন ডলারে উন্নীত করার উনিশশো পঁচানব্বই সালে লক্ষ্যমাত্রা নির্ধারণ করা হয়েছে।
+```
+
+```py
+text = "আজকের তাপমাত্রা ৪৪°F"
+text = nrml.text_normalizer(text)
+print(f"{text}")
+
+#output:
+আজকের তাপমাত্রা চুয়াল্লিশ ডিগ্রী ফারেনহাইট
+```
+
+```py
+text = "আজকের তাপমাত্রা ৪৪°C"
+text = nrml.text_normalizer(text)
+print(f"{text}")
+
+#output:
+আজকের তাপমাত্রা চুয়াল্লিশ ডিগ্রী সেলসিয়াস
+```
+
 Supported
 
 ```
 #abbreviations:
 ("সাঃ", "সাল্লাল্লাহু আলাইহি ওয়া সাল্লাম"),                  
 ("আঃ", "আলাইহিস সালাম"),
 ("রাঃ", "রাদিআল্লাহু আনহু"),
 ("রহঃ", "রহমাতুল্লাহি আলাইহি"),
 ("রহিঃ", "রহিমাহুল্লাহ"),
 ("হাফিঃ", "হাফিযাহুল্লাহ"),
 ("দাঃবাঃ", "দামাত বারাকাতুহুম,দামাত বারাকাতুল্লাহ"),
 ("মোঃ",  "মোহাম্মদ"),
+("মো.",  "মোহাম্মদ"),
 ("মোসাঃ",  "মোসাম্মত"),
 ("মোছাঃ", "মোছাম্মত"),
 ("আ:" , "আব্দুর"),
 ("ডাঃ" , "ডাক্তার"),
+("ড." , "ডক্টর"),
 
 #Symbols:
 ("&", " এবং"),
 ("@", " এট দা রেট"),
 ("%", " পারসেন্ট"),
 ("#", " হ্যাশ"),
 ("°", " ডিগ্রী")
@@ -214,58 +295,54 @@
 ### It supports converting different formats of Bangla date to English date.
 
 ```py
 
 import pybangla
 nrml = pybangla.Normalizer()
 date = "০১-এপ্রিল/২০২৩"
-date = nrml.date_format(date, language="en")
+date = nrml.date_format(date, language="bn")
 print(date)
 #output:
 
-{'date': '01', 'month': 'april', 'year': '2023', 'txt_date': 'one', 'txt_year': 'twenty century twenty-three', 'weekday': 'saturday', 'ls_month': 'apr', 'seasons': 'wet season'}
-
 
+{'date': '০১', 'month': '৪', 'year': '২০২৩', 'txt_date': 'এক', 'txt_month': 'এপ্রিল', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
 ```
 
-```py
-date = nrml.date_format("০১-এপ্রিল/২০২৩", language="bn")
-print(date)
-#output:
-{'date': '০১', 'month': 'এপ্রিল', 'year': '২০২৩', 'txt_date': 'এক', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
 
-```
 
 ```py
-date = nrml.date_format("2023-04-05", language="bn")
+date = nrml.date_format("সেপ্টেম্বর ০৫ ২০২৩", language="bn")
 
 #output
-{'date': '০৫', 'month': 'এপ্রিল', 'year': '২০২৩', 'txt_date': 'পাঁচ', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'বুধবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+
+{'date': '০৫', 'month': '৯', 'year': '২০২৩', 'txt_date': 'পাঁচ', 'txt_month': 'সেপ্টেম্বর', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'মঙ্গলবার', 'ls_month': 'পৌষ', 'seasons': 'শীত'}
+
 
 ```
 
 ```py
 date = nrml.date_format("20230401", language="bn")
 print(date)
 #output
-
-{'date': '০১', 'month': 'এপ্রিল', 'year': '২০২৩', 'txt_date': 'এক', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+{'date': '০১', 'month': '০৪', 'year': '২০২৩', 'txt_date': 'এক', 'txt_month': 'এপ্রিল', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
 
 ```
 
+
 ```py
 
 #input ex. ['dd', "mm", "yyyy"]
 date = nrml.date_format(["1", "4", "2025"], language="bn")
 
 print(date)
 
 #output
 
-{'date': '১', 'month': 'এপ্রিল', 'year': '২০২৫', 'txt_date': 'এক', 'txt_year': 'দুই হাজার পঁচিশ', 'weekday': 'মঙ্গলবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+{'date': '১', 'month': '৪', 'year': '২০২৫', 'txt_date': 'এক', 'txt_month': 'এপ্রিল', 'txt_year': 'দুই হাজার পঁচিশ', 'weekday': 'মঙ্গলবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+
 
 ```
 
 
 
 Supported Date Format:
 
@@ -299,25 +376,27 @@
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 
 date = dt.date_format("01-Apr/2023", language="bn")
 print(f"{date}")
 # Output: 
-{'date': '০১', 'month': 'এপ্রিল', 'year': '২০২৩', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+{'date': '০১', 'month': '৪', 'year': '২০২৩', 'txt_date': 'এক', 'txt_month': 'এপ্রিল', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+
 ```
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 en_date = dt.date_format("01-Apr/2023", language="en")
 print(f"{en_date}")
 
 # Output :
-{'date': '01', 'month': 'April', 'year': '2023', 'weekday': 'Saturday', 'ls_month': 'Apr', 'seasons': 'Wet season'}
+{'date': '01', 'month': '4', 'year': '2023', 'txt_date': 'one', 'txt_month': 'april', 'txt_year': 'twenty century twenty-three', 'weekday': 'saturday', 'ls_month': 'apr', 'seasons': 'wet season'}
+
 ```
 
 ## Date extraction
 
 ```py
 Rule based Date Extraction
 import pybangla
@@ -325,25 +404,50 @@
 
 text = "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে. এপ্রিল ২০২৩"
 dates = nrml.date_extraction(text)
 
 #output:
 
 [
-{'date': '০৫', 'month': 'সেপ্টেম্বর', 'year': '২০২৩', 'txt_date': 'পাঁচ', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'মঙ্গলবার', 'ls_month': 'পৌষ', 'seasons': 'শীত'}, 
+    {'date': '০৫', 'month': '৯', 'year': '২০২৩', 'txt_date': 'পাঁচ', 'txt_month': 'সেপ্টেম্বর', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'মঙ্গলবার', 'ls_month': 'পৌষ', 'seasons': 'শীত'}, 
 
-{'date': '১', 'month': 'এপ্রিল', 'year': '২০২৩', 'txt_date': 'এক', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+{'date': '১৬', 'month': '৫', 'year': '২০২৪', 'txt_date': 'ষোল', 'txt_month': 'মে', 'txt_year': 'দুই হাজার চব্বিশ', 'weekday': 'বৃহস্পতিবার', 'ls_month': 'ভাদ্র', 'seasons': 'শরৎ'}
 ]
 
+
+```
+
+<h1 style='color:LightGreen'> New Feature </h1>
+
+## 4. Emoji Removal
+### Now our normalizer can be used for removing emojis.
+
+```py
+text = 'দয়া করে পবিত্র কুরআনুল কারিম বলেন,,,,পবিত্র কথাটা অবশ্যই বলবেন,,, প্লিজ 😢😥🙏🙏🙏'
+text = nrml.remove_emoji(text)
+print(f"{text}")
+
+#output:
+দয়া করে পবিত্র কুরআনুল কারিম বলেন,,,,পবিত্র কথাটা অবশ্যই বলবেন,,, প্লিজ
+```
+
+
+```py
+text = "😬😬 আর বিভিন্ন চ্যানেল সম্পর্কে কি বলব"
+text = nrml.remove_emoji(text)
+print(f"{text}")
+
+#output:
+ আর বিভিন্ন চ্যানেল সম্পর্কে কি বলব
 ```
 
-## 4. Today, Months, Weekdays, Seasons
+## 5. Today, Months, Weekdays, Seasons
 ### It converts Bangla (today, months, weekdays, and seasons) to English and English to Bangla, and vice versa, in a pair format.
 
-## 1. Today:
+### 1. Today:
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 today = nrml.today()
 print(today)
 
@@ -362,15 +466,15 @@
 today= nrml.today(language="bn")
 print(today)
 #output:
 {'date': '30', 'month': 'april', 'year': '2024', 'txt_date': 'thirty', 'txt_year': 'twenty century twenty-four', 'weekday': 'tuesday', 'ls_month': 'apr', 'seasons': 'wet season'}
 ```
 
 
-# 2. Months
+### 2. Months
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 month = nrml.months()
 print(month)
 
@@ -396,15 +500,15 @@
 print(month)
 
 # output:
 {'march': 'মার্চ', 'bangla': 'আষাঢ়'}
 
 ```
 
-## 3. Weekdays
+### 3. Weekdays
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 weekdays = nrml.weekdays()
 
 print(weekdays)
@@ -446,15 +550,15 @@
 weekdays = nrml.weekdays(day = "Monday")
 print(weekdays)
 #output:
 {'monday': 'সোমবার'}
 ```
 
 
-## 4. Seasons
+### 4. Seasons
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 seasons = nmlr.seasons()
 print(seasons)
```

### Comparing `pybangla-1.0.9.dev0/README.md` & `pybangla-1.0.9.dev1/pybangla.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: pybangla
+Version: 1.0.9.dev1
+Summary: pybangla is the bangla text normalizer tool, it use for text normalization like word to number and date formating purposes
+Home-page: https://github.com/saiful9379/pybangla
+Author: saiful
+Author-email: saifulbrur79@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Requires-Dist: DateTime
+Requires-Dist: num2words
+Requires-Dist: python-Levenshtein
+Requires-Dist: fuzzywuzzy
+
 
 PYBANGLA is a python3 package for Bangla Number, DateTime and Text Normalizer and Date Extraction. This package can be used Normalize the text number and date (ex: number to text vice versa). This framework  also can be used Django, Flask, FastAPI, and others. PYBANGLA module supported operating system Linux/Unix, Mac OS and Windows.
 Available Features
 
 Features available in PYBANGLA:
 
 1. Text Normalization
@@ -19,14 +37,26 @@
 ```
 
 
 # Usage
 
 ## 1. Text Normalization
 ### It supports converting Bangla abbreviations, symbols, and currencies to Bangla textual format.
+<h2 style='color:LightBlue'>(UPDATE) It supports year conversion like </h2>
+
+* "১৯৮৭-র" to "উনিশশো সাতাশি এর"
+* "১৯৯৫ সালে" to "উনিশশো পঁচানব্বই সালে"
+* "২০২৬-২৭" to "দুই হাজার ছাব্বিশ সাতাশ"
+
+<h3 style='color:LightBlue'> Now it also has the abbreviation for units of temperature </h3>
+
+* "৪৪°F" to "চুয়াল্লিশ ডিগ্রী ফারেনহাইট"
+* "৪৪°C" to "চুয়াল্লিশ ডিগ্রী সেলসিয়াস"
+
+<h2> </h2>
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 text = "রাহিম ক্লাস ওয়ান এ ১ম, এন্ড বাসার ক্লাস এ ৩৩ তম, সে জন্য ২০৩০ শতাব্দীতে ¥২০৩০.১২৩৪ দিতে হয়েছে"
 text = nrml.text_normalizer(text)
 
@@ -62,30 +92,97 @@
 text = nrml.text_normalizer(text)
 #output:
 
 সম্মেলনটি পাঁচ সেপ্টেম্বর দুই হাজার তেইশ তারিখে নির্ধারিত করা হয়েছে. এক এপ্রিল দুই হাজার তেইশ
 
 ```
 
+```py
+
+text = "দাড়াবে?না হারিস আনিস জোসেফের মতো খালাস!!!???"
+text = nmlr.text_normalizer(text)    
+
+#output:
+
+দাড়াবে? না হারিস আনিস জোসেফের মতো খালাস!
+```
+
+```py
+
+text = "আজব এক ধর্ম। অবমাননার অর্থ কি ? ? কেউ বলবেন? ? মেধাহীন জাতি তা আর একবার প্রমাণ করলো ।"
+text = nmlr.text_normalizer(text)
+
+#output:
+
+আজব এক ধর্ম। অবমাননার অর্থ কি? কেউ বলবেন? মেধাহীন জাতি তা আর একবার প্রমাণ করলো।
+```
+
+```py
+text = "সে যা-ই হোক, সত্যিকারের এমন পাকা পোনা শেষ বার নেমন্তন্ন বাড়িতে খেয়েছি ১৯৮৭-র এপ্রিলে।"
+text = nrml.text_normalizer(text)
+print(f"{text}")
+
+#output:
+সে যা ই হোক, সত্যিকারের এমন পাকা পোনা শেষ বার নেমন্তন্ন বাড়িতে খেয়েছি উনিশশো সাতাশি এর এপ্রিলে।
+```
+
+```py
+text = "আজকের তাপমাত্রা ৪৪°F"
+text = nrml.text_normalizer(text)
+print(f"{text}")
+
+#output:
+আজকের তাপমাত্রা চুয়াল্লিশ ডিগ্রী ফারেনহাইট
+```
+
+```py
+text = "নতুন নীতিমালায় ২০২৬-২৭ অর্থবছরে দেশের রপ্তানি আয় ১১ হাজার কোটি মার্কিন ডলারে উন্নীত করার ১৯৯৫ সালে লক্ষ্যমাত্রা নির্ধারণ করা হয়েছে।"
+text = nrml.text_normalizer(text)
+print(f"{text}")
+
+#output:
+নতুন নীতিমালায় দুই হাজার ছাব্বিশ সাতাশ অর্থবছরে দেশের রপ্তানি আয় এগারো হাজার কোটি মার্কিন ডলারে উন্নীত করার উনিশশো পঁচানব্বই সালে লক্ষ্যমাত্রা নির্ধারণ করা হয়েছে।
+```
+
+```py
+text = "আজকের তাপমাত্রা ৪৪°F"
+text = nrml.text_normalizer(text)
+print(f"{text}")
+
+#output:
+আজকের তাপমাত্রা চুয়াল্লিশ ডিগ্রী ফারেনহাইট
+```
+
+```py
+text = "আজকের তাপমাত্রা ৪৪°C"
+text = nrml.text_normalizer(text)
+print(f"{text}")
+
+#output:
+আজকের তাপমাত্রা চুয়াল্লিশ ডিগ্রী সেলসিয়াস
+```
+
 Supported
 
 ```
 #abbreviations:
 ("সাঃ", "সাল্লাল্লাহু আলাইহি ওয়া সাল্লাম"),                  
 ("আঃ", "আলাইহিস সালাম"),
 ("রাঃ", "রাদিআল্লাহু আনহু"),
 ("রহঃ", "রহমাতুল্লাহি আলাইহি"),
 ("রহিঃ", "রহিমাহুল্লাহ"),
 ("হাফিঃ", "হাফিযাহুল্লাহ"),
 ("দাঃবাঃ", "দামাত বারাকাতুহুম,দামাত বারাকাতুল্লাহ"),
 ("মোঃ",  "মোহাম্মদ"),
+("মো.",  "মোহাম্মদ"),
 ("মোসাঃ",  "মোসাম্মত"),
 ("মোছাঃ", "মোছাম্মত"),
 ("আ:" , "আব্দুর"),
 ("ডাঃ" , "ডাক্তার"),
+("ড." , "ডক্টর"),
 
 #Symbols:
 ("&", " এবং"),
 ("@", " এট দা রেট"),
 ("%", " পারসেন্ট"),
 ("#", " হ্যাশ"),
 ("°", " ডিগ্রী")
@@ -198,58 +295,54 @@
 ### It supports converting different formats of Bangla date to English date.
 
 ```py
 
 import pybangla
 nrml = pybangla.Normalizer()
 date = "০১-এপ্রিল/২০২৩"
-date = nrml.date_format(date, language="en")
+date = nrml.date_format(date, language="bn")
 print(date)
 #output:
 
-{'date': '01', 'month': 'april', 'year': '2023', 'txt_date': 'one', 'txt_year': 'twenty century twenty-three', 'weekday': 'saturday', 'ls_month': 'apr', 'seasons': 'wet season'}
-
 
+{'date': '০১', 'month': '৪', 'year': '২০২৩', 'txt_date': 'এক', 'txt_month': 'এপ্রিল', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
 ```
 
-```py
-date = nrml.date_format("০১-এপ্রিল/২০২৩", language="bn")
-print(date)
-#output:
-{'date': '০১', 'month': 'এপ্রিল', 'year': '২০২৩', 'txt_date': 'এক', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
 
-```
 
 ```py
-date = nrml.date_format("2023-04-05", language="bn")
+date = nrml.date_format("সেপ্টেম্বর ০৫ ২০২৩", language="bn")
 
 #output
-{'date': '০৫', 'month': 'এপ্রিল', 'year': '২০২৩', 'txt_date': 'পাঁচ', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'বুধবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+
+{'date': '০৫', 'month': '৯', 'year': '২০২৩', 'txt_date': 'পাঁচ', 'txt_month': 'সেপ্টেম্বর', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'মঙ্গলবার', 'ls_month': 'পৌষ', 'seasons': 'শীত'}
+
 
 ```
 
 ```py
 date = nrml.date_format("20230401", language="bn")
 print(date)
 #output
-
-{'date': '০১', 'month': 'এপ্রিল', 'year': '২০২৩', 'txt_date': 'এক', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+{'date': '০১', 'month': '০৪', 'year': '২০২৩', 'txt_date': 'এক', 'txt_month': 'এপ্রিল', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
 
 ```
 
+
 ```py
 
 #input ex. ['dd', "mm", "yyyy"]
 date = nrml.date_format(["1", "4", "2025"], language="bn")
 
 print(date)
 
 #output
 
-{'date': '১', 'month': 'এপ্রিল', 'year': '২০২৫', 'txt_date': 'এক', 'txt_year': 'দুই হাজার পঁচিশ', 'weekday': 'মঙ্গলবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+{'date': '১', 'month': '৪', 'year': '২০২৫', 'txt_date': 'এক', 'txt_month': 'এপ্রিল', 'txt_year': 'দুই হাজার পঁচিশ', 'weekday': 'মঙ্গলবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+
 
 ```
 
 
 
 Supported Date Format:
 
@@ -283,25 +376,27 @@
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 
 date = dt.date_format("01-Apr/2023", language="bn")
 print(f"{date}")
 # Output: 
-{'date': '০১', 'month': 'এপ্রিল', 'year': '২০২৩', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+{'date': '০১', 'month': '৪', 'year': '২০২৩', 'txt_date': 'এক', 'txt_month': 'এপ্রিল', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+
 ```
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 en_date = dt.date_format("01-Apr/2023", language="en")
 print(f"{en_date}")
 
 # Output :
-{'date': '01', 'month': 'April', 'year': '2023', 'weekday': 'Saturday', 'ls_month': 'Apr', 'seasons': 'Wet season'}
+{'date': '01', 'month': '4', 'year': '2023', 'txt_date': 'one', 'txt_month': 'april', 'txt_year': 'twenty century twenty-three', 'weekday': 'saturday', 'ls_month': 'apr', 'seasons': 'wet season'}
+
 ```
 
 ## Date extraction
 
 ```py
 Rule based Date Extraction
 import pybangla
@@ -309,25 +404,50 @@
 
 text = "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে. এপ্রিল ২০২৩"
 dates = nrml.date_extraction(text)
 
 #output:
 
 [
-{'date': '০৫', 'month': 'সেপ্টেম্বর', 'year': '২০২৩', 'txt_date': 'পাঁচ', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'মঙ্গলবার', 'ls_month': 'পৌষ', 'seasons': 'শীত'}, 
+    {'date': '০৫', 'month': '৯', 'year': '২০২৩', 'txt_date': 'পাঁচ', 'txt_month': 'সেপ্টেম্বর', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'মঙ্গলবার', 'ls_month': 'পৌষ', 'seasons': 'শীত'}, 
 
-{'date': '১', 'month': 'এপ্রিল', 'year': '২০২৩', 'txt_date': 'এক', 'txt_year': 'দুই হাজার তেইশ', 'weekday': 'শনিবার', 'ls_month': 'শ্রাবণ', 'seasons': 'বর্ষা'}
+{'date': '১৬', 'month': '৫', 'year': '২০২৪', 'txt_date': 'ষোল', 'txt_month': 'মে', 'txt_year': 'দুই হাজার চব্বিশ', 'weekday': 'বৃহস্পতিবার', 'ls_month': 'ভাদ্র', 'seasons': 'শরৎ'}
 ]
 
+
+```
+
+<h1 style='color:LightGreen'> New Feature </h1>
+
+## 4. Emoji Removal
+### Now our normalizer can be used for removing emojis.
+
+```py
+text = 'দয়া করে পবিত্র কুরআনুল কারিম বলেন,,,,পবিত্র কথাটা অবশ্যই বলবেন,,, প্লিজ 😢😥🙏🙏🙏'
+text = nrml.remove_emoji(text)
+print(f"{text}")
+
+#output:
+দয়া করে পবিত্র কুরআনুল কারিম বলেন,,,,পবিত্র কথাটা অবশ্যই বলবেন,,, প্লিজ
+```
+
+
+```py
+text = "😬😬 আর বিভিন্ন চ্যানেল সম্পর্কে কি বলব"
+text = nrml.remove_emoji(text)
+print(f"{text}")
+
+#output:
+ আর বিভিন্ন চ্যানেল সম্পর্কে কি বলব
 ```
 
-## 4. Today, Months, Weekdays, Seasons
+## 5. Today, Months, Weekdays, Seasons
 ### It converts Bangla (today, months, weekdays, and seasons) to English and English to Bangla, and vice versa, in a pair format.
 
-## 1. Today:
+### 1. Today:
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 today = nrml.today()
 print(today)
 
@@ -346,15 +466,15 @@
 today= nrml.today(language="bn")
 print(today)
 #output:
 {'date': '30', 'month': 'april', 'year': '2024', 'txt_date': 'thirty', 'txt_year': 'twenty century twenty-four', 'weekday': 'tuesday', 'ls_month': 'apr', 'seasons': 'wet season'}
 ```
 
 
-# 2. Months
+### 2. Months
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 month = nrml.months()
 print(month)
 
@@ -380,15 +500,15 @@
 print(month)
 
 # output:
 {'march': 'মার্চ', 'bangla': 'আষাঢ়'}
 
 ```
 
-## 3. Weekdays
+### 3. Weekdays
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 weekdays = nrml.weekdays()
 
 print(weekdays)
@@ -430,15 +550,15 @@
 weekdays = nrml.weekdays(day = "Monday")
 print(weekdays)
 #output:
 {'monday': 'সোমবার'}
 ```
 
 
-## 4. Seasons
+### 4. Seasons
 
 ```py
 import pybangla
 nrml = pybangla.Normalizer()
 seasons = nmlr.seasons()
 print(seasons)
```

### Comparing `pybangla-1.0.9.dev0/pybangla/module/config.py` & `pybangla-1.0.9.dev1/pybangla/module/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,16 @@
     en_regex = r'[0-9]+'
     samples = ["-", ",", "/", " "]
     _currency = {"৳" : "টাকা", "$" : "ডলার", "£" : "পাউন্ড", "€" : "ইউরো", "¥" : "ইয়েন", "₹" : "রুপি", "₽" : "রুবেল", "₺" : "লিরা"}
     en_to_bn_digits_mapping = {e : b for e, b in zip(data["en"]["number"], data["bn"]["number"])}
     bn_to_en_digits_mapping = {v : k for k, v in en_to_bn_digits_mapping.items()}
     en_month_shortname = [i[:3] for i in data["en"]["months"]]
 
+    # ro_adding_in_month = [i+"র" for i in data["bn"]["months"]]
+
     data["bn"]["digits_mapping"] = en_to_bn_digits_mapping
     data["en"]["digits_mapping"] = bn_to_en_digits_mapping
     data["en"]["option_name"] = en_month_shortname
     
     _bangla2english_digits_mapping = {'১':'1', '২':'2', '৩':'3', '৪':'4', '৫':'5', '৬':'6', '৭':'7', '৮':'8', '৯':'9', '০':'0'}
 
     _english2bangla2_digits_mapping = {j:i for i, j in _bangla2english_digits_mapping.items()}
@@ -89,16 +91,14 @@
     checking_adjust = list(adjust_number.keys())
     checking_conjugative_number = list(conjugative_number.keys())
 
     
     
     _abbreviations = {
         "en": [
-            (re.compile("\\b%s\\." % x[0], re.IGNORECASE), x[1])
-            for x in [
                 ("mrs", "misess"),
                 ("mr", "mister"),
                 ("dr", "doctor"),
                 ("st", "saint"),
                 ("co", "company"),
                 ("jr", "junior"),
                 ("maj", "major"),
@@ -109,59 +109,55 @@
                 ("hon", "honorable"),
                 ("sgt", "sergeant"),
                 ("capt", "captain"),
                 ("esq", "esquire"),
                 ("ltd", "limited"),
                 ("col", "colonel"),
                 ("ft", "fort"),
-            ]
-        ],
+            ],
         "bn": [
-            (re.compile(r"%s" % x[0], re.IGNORECASE), x[1])
-            for x in [
-                ("সাঃ", "সাল্লাল্লাহু আলাইহি ওয়া সাল্লাম"),                  
-                ("আঃ", "আলাইহিস সালাম"),
-                ("রাঃ", "রাদিআল্লাহু আনহু"),
-                ("রহঃ", "রহমাতুল্লাহি আলাইহি"),
-                ("রহিঃ", "রহিমাহুল্লাহ"),
-                ("হাফিঃ", "হাফিযাহুল্লাহ"),
-                ("দাঃবাঃ", "দামাত বারাকাতুহুম,দামাত বারাকাতুল্লাহ"),
-                ("মোঃ",  "মোহাম্মদ"),
-                ("মোসাঃ",  "মোসাম্মত"),
-                ("মোছাঃ", "মোছাম্মত"),
-                ("আ:" , "আব্দুর"),
-                ("ডাঃ" , "ডাক্তার"),
-                (" কিমি ", " কিলোমিটার "),
-                (" সেমি ", " সেন্টিমিটার "),
-                (" বিডি ", " বাংলাদেশ ")
-            ]
+            ("সাঃ", "সাল্লাল্লাহু আলাইহি ওয়া সাল্লাম"),
+            ("আঃ", "আলাইহিস সালাম"),
+            ("রাঃ", "রাদিআল্লাহু আনহু"),
+            ("রহঃ", "রহমাতুল্লাহি আলাইহি"),
+            ("রহিঃ", "রহিমাহুল্লাহ"),
+            ("হাফিঃ", "হাফিযাহুল্লাহ"),
+            ("দাঃবাঃ", "দামাত বারাকাতুহুম,দামাত বারাকাতুল্লাহ"),
+            ("মোঃ",  "মোহাম্মদ"),
+            ("মো.",  "মোহাম্মদ"),
+            ("মোসাঃ",  "মোসাম্মত"),
+            ("মোছাঃ", "মোছাম্মত"),
+            ("আ:" , "আব্দুর"),
+            ("ডাঃ" , "ডাক্তার"),
+            ("ড." , "ডক্টর"),
+            (" কিমি ", " কিলোমিটার "),
+            ("কিমি.", " কিলোমিটার "),
+            (" সেমি ", " সেন্টিমিটার "),
+            ("সেমি.", " সেন্টিমিটার "),
+            (" বিডি ", " বাংলাদেশ "),
+            ("মো:", "মোহাম্মদ")
         ]
     }
 
     _symbols = {
             "en": [
-                (re.compile(r"%s" % re.escape(x[0]), re.IGNORECASE), x[1])
-                for x in [
                     ("&", " and "),
                     ("@", " at "),
                     ("%", " percent "),
                     ("#", " hash "),
                     ("°", " degree ")
-                ]
+
             ],
             "bn": [
-                (re.compile(r"%s" % re.escape(x[0]), re.IGNORECASE), x[1])
-                for x in [
                     ("&", " এবং"),
                     ("@", " এট দা রেট"),
                     ("%", " পারসেন্ট"),
                     ("#", " হ্যাশ"),
                     ("°", " ডিগ্রী")
-                ]
-            ],
+                ],
         }
 
     
     _ordinal_re = {
         "en": re.compile(r"([0-9]+)(st|nd|rd|th)"),
         "bn": [
                 (re.compile(r"%s" % re.escape(x[0]), re.IGNORECASE), x[1])
@@ -287,32 +283,36 @@
         "ninety-five" : "পঁচানব্বই",
         "ninety-six" : "ছিয়ানব্বই",
         "ninety-seven" : "সাতানব্বই",
         "ninety-eight" : "আটানব্বই",
         "ninety-nine" : "নিরানব্বই"
     }
     
+    _STANDARDIZE_ZW = re.compile(r'(?<=\u09b0)[\u200c\u200d]+(?=\u09cd\u09af)')
+
+    _DELETE_ZW = re.compile(r'(?<!\u09b0)[\u200c\u200d](?!\u09cd\u09af)')
+    
     _punctuations = {
-        "।": "।",  # won't be replaced
-        ",": ",", # won't be replaced
+        "।": "। ",  # won't be replaced
+        ",": ", ", # won't be replaced
         ".": ".", # won't be replaced
-        "?": "?", # won't be replaced
-        "!": "!", # won't be replaced
-        "⁇": "?", # won't be replaced
-        "’": '"', # won't be replaced
+        "?": "? ", # won't be replaced
+        "!": "! ", # won't be replaced
+        "⁇": "? ", # won't be replaced
+        "’": ' ', 
         '"': '"', # won't be replaced
         "“": '"', # won't be replaced
-        "‘": '"', # won't be replaced
+        "‘": ' ', 
         "”": '"', # won't be replaced
-        "`": '"', # won't be replaced
+        "`": ' ', 
         ";": " ", 
         ":": " ",  
         "'": " ", 
         "\\": " ", 
-        "-": " ", 
+        "-": "-", # won't be replaced
         "[": " ", 
         "]": " ", 
         "{": " ", 
         "}": " ", 
         "(": " ", 
         ")": " ", 
         '–': " ", 
@@ -362,15 +362,14 @@
         '↑': " ",
         '±': " ",
         '¿': " ",
         '▾': " ",
         '═': " ",
         '¦': " ",
         '║': " ",
-        '¥': " ",
         '▓': " ",
         '‹': " ", 
         '─': " ",
         '▒': " ",
         '：': " ",
         '¼': " ",
         '⊕': " ",
```

### Comparing `pybangla-1.0.9.dev0/pybangla/module/date_extractor.py` & `pybangla-1.0.9.dev1/pybangla/module/date_extractor.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,19 @@
         en_month_year = "("+ '|'.join(en_month_name) +")[a-z]{0,6}(( )+)?[-\\/,.;: ](( )+)?\\d{1,4}\\b"
         en_plain_date ='\\d{8}\\b'
 
         bn_dd_mm_yy= "[০-৯]{1,4}(( )+)?[-\\/,.;: ](( )+)?[০-৯]{1,4}(( )+)?[-\\/,.;: ](( )+)?[০-৯]{1,4}"
         bn_number_month_year = "[০-৯]{1,2}[-\\/,.;: ](( )+)?("+ '|'.join(bn_month_name) +")((( )+)?[-\\/,.;: ](( )+)?[০-৯]{1,4})?"
         bn_month_number_year = "("+ '|'.join(bn_month_name) +")(( )+)?[-\\/,.;: ][০-৯]{1,2}(?![০-৯])((( )+)?[-\\/,.;: ](( )+)?[০-৯]{1,4})?"
         bn_month_year = "("+ '|'.join(bn_month_name) +")(( )+)?[-\\/,.;: ](( )+)?[০-৯]{1,4}"
+        bn_year_date_num_month_name = "[০-৯]{1,4}(( )+)?[-\\/,.;: ](( )+)?(সালে|সালের)(( )+)?[-\\/,.;: ]?[০-৯]{1,2}(( )+)?[-\\/,.;: ]?(( )+)?("+ '|'.join(bn_month_name) +")?"
         bn_plain_date = "[০-৯]{8}"
 
-        en_regex = '|'.join([en_dd_mm_yy, en_number_month_year, en_month_number_year,en_month_year, en_plain_date])
-        bn_regex = '|'.join([bn_dd_mm_yy, bn_number_month_year, bn_month_number_year,bn_month_year, bn_plain_date])
+        en_regex = '|'.join([en_dd_mm_yy, en_number_month_year, en_month_number_year, en_month_year, en_plain_date])
+        bn_regex = '|'.join([bn_dd_mm_yy, bn_number_month_year, bn_month_number_year, bn_month_year, bn_year_date_num_month_name, bn_plain_date])
         combined_regex = en_regex + '|' + bn_regex
         return combined_regex
     
     def __init__(self) -> None:
         self.date_regex = self.get_regex_patterns()
         
     def get_dates(self, sentence):
@@ -87,14 +88,16 @@
     "2023/04/01 er", 
     "01-Apr-2023 erv", 
     "01-Apr/2023 sere",  
     "20230401 ",  
     "20042024 ",
 ]
     Bangla_sentences = [
+    "১৯৯৬ সালের ৬তারিখে নির্ধারিত করা হয়েছে.",
+    "১৯৯৬ সালের৬ সেপ্টেম্বর ভ্রমণ পরিকল্পনা করছি.",
     "আমি জুলাই ২০২৩ তে একটি সমুদ্র ভ্রমণ পরিকল্পনা করছি.",
     "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে.",
     "আমরা খ্রীষ্টমাসের জন্য ডিসেম্বর ২৫ ২০২৩ তারিখে পরিবারের সংগঠন করব.",
     "আমার বোনের বিয়ে ১৮ মার্চ, ২০২৩ তারিখে.",
     "আমি আগামী ১২ আগস্ট, ২০২৩ তারিখে আমার জন্মদিনে দেখা করছি.",
     "আমরা ফেব্রুয়ারি ২০২৩ তে স্কিউইং যাব.",
     "আমাদের কোম্পানির পিকনিকটি জুন ৩০ ২০২৩ তারিখে নির্ধারিত হয়েছে.",
@@ -111,18 +114,19 @@
     "আমরা জুন ২০২৩ তে ইউরোপে একটি ভ্রমণ পরিকল্পনা করছি.",
     "আমার ডেন্টিস্টের অ্যাপয়েন্টমেন্ট এপ্রিল ১০, ২০২৩ তারিখে.",
     "কোম্পানির বার্ষিক সভা ফেব্রুয়ারি ২০২৩ তারিখে হয়.",
     "আমার অনুষ্ঠান সমাপন হয়েছে জুন ১৫, ২০২৩ তারিখে.",
     "আমি মার্চ ২০২৩ তারিখে একটি নতুন চাকরি শুরু করছি.",
     "আমি মে ২০২৩ তারিখে পাহাড়ে ট্রেকিং করতে যাচ্ছি.",
     "বিদ্যালয়ের নাটকটি নভেম্বর ২০২৩ তারিখে নির্ধারিত হয়েছে.",
-    "আমরা অক্টোবর ২০২৩ তার"
+    "আমরা অক্টোবর ২০২৩ তার",
+    "১৯৯৬ সালের ৬ সেপ্টেম্বর"
     ]
 
-    combined_sentences = English_sentences + Bangla_sentences + template_provided
+    combined_sentences = English_sentences  + template_provided+Bangla_sentences
     date_extractor = DateExtractor()
     
     for sentence in combined_sentences:
         dates = date_extractor.get_dates(sentence)
         print(f"Input: {sentence}: Output: {dates}")
```

### Comparing `pybangla-1.0.9.dev0/pybangla/module/main.py` & `pybangla-1.0.9.dev1/pybangla/module/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 
 import re
 import time
 import datetime
 from .config import Config as cfg
-from .parser import DateParser, TextParser, NumberParser
+from .parser import DateParser, TextParser, NumberParser, EmojiRemoval
 from .number_parser import Word2NumberMap
 from .date_extractor import DateExtractor
-dp, tp, npr, wnmp = DateParser(), TextParser(), NumberParser(), Word2NumberMap()
+dp, tp, npr, wnmp, emr = DateParser(), TextParser(), NumberParser(), Word2NumberMap(), EmojiRemoval()
 dt = DateExtractor()
 data = cfg.data
 
 class Normalizer:
     def __init__(self):
 
         self.bn_regex = cfg.bn_regex
@@ -138,14 +138,22 @@
     def text_normalizer(self, text):
         """
         this is the text normalizer fucntion
         """
         text = tp.processing(text)
         return text
     
+    def remove_emoji(self, text):
+        text = emr.remove_emoji(text)
+        return text
+    
+    # def emoji2text(self, text):
+    #     text = emrp.replace_emoji(text)
+    #     return text
+    
     def word2number(self, text):
         text = wnmp.convert_word2number(text)
         return text
     
     def date_extraction(self, text):
 
         dates = dt.get_dates(text)
```

### Comparing `pybangla-1.0.9.dev0/pybangla/module/number_parser.py` & `pybangla-1.0.9.dev1/pybangla/module/number_parser.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.9.dev0/pybangla/module/parser.py` & `pybangla-1.0.9.dev1/pybangla/module/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import re
 import datetime
 import string
 from .config import Config as cfg
 from num2words import num2words
 from .date_extractor import DateExtractor
+from fuzzywuzzy import fuzz
+# from bnemo import Translator
 # from .number_parser import Word2NumberMap
 
 
 dt = DateExtractor()
 # nr = Normalizer()
 data = cfg.data
 
@@ -17,14 +19,16 @@
 _whitespace_re = cfg._whitespace_re
 _currency = cfg._currency
 _punctuations = cfg._punctuations
 
 english_digits = cfg._bangla2english_digits_mapping
 bangla_numeric_words = cfg._bangla_numeric_words
 
+_STANDARDIZE_ZW = cfg._STANDARDIZE_ZW
+_DELETE_ZW = cfg._DELETE_ZW
 
 class NumberParser:
     def __init__(self):
         self.english_digits = english_digits
         self.bangla_numeric_words = bangla_numeric_words
         self.en_regex = cfg.en_regex
         self.bn_regex = cfg.bn_regex
@@ -89,35 +93,27 @@
         Args:
             number_string: Bangla year in numbers as string. Example: "১৯৯৪"
 
         Returns:
             Bangla year in words. Example: "উনিশশো চুরানব্বই"
 
         """
-        # print("year_in_number[1]", year_in_number[1])
-        # if (len(year_in_number) == 4 and year_in_number[1] != '০') or \
-        #     (len(year_in_number) == 4 and year_in_number[1] != '0') or len(year_in_number) == 3:
-
-
-
         if language=="bn":
             mid_text = "শো "
         else:
             mid_text = " century "
 
         if (len(year_in_number) == 4 and year_in_number[1] != '০') or len(year_in_number) == 3:
+            # print("year in ")
             
             if year_in_number[1] != '0':
-                return self.number_to_words(year_in_number)
-                
+                year_str = self.number_to_words(year_in_number)
             return self.number_to_words(year_in_number[:-2]) + mid_text + self.number_to_words(year_in_number[-2:])
-        
-        # elif (len(year_in_number) == 4 and year_in_number[1] != '0') or len(year_in_number) == 3:
-        #     return self.number_to_words(year_in_number[:-2]) + mid_text + self.number_to_words(year_in_number[-2:])
         else:
+            # print("+++++++++ else+++++++++++++++")
             return self.number_to_words(year_in_number)
 
     def _replace_starting_zero(self, month):
         """
         Normalize string which start zero first
         
         """
@@ -131,15 +127,19 @@
         
         """
         # print("number  : ", number, language)
 
         if language=="en":
             extracted_number = list(re.finditer(self.bn_regex, str(number), re.UNICODE))
             if extracted_number:
-                number = "".join([cfg._bangla2english_digits_mapping[i.replance(",", "")] for i in number])
+                print("language", number)
+                # [i[1] for i in number if i[0]=="0"]
+                if number[0]=="0":
+                    number = number[1:]
+                number = "".join([cfg._bangla2english_digits_mapping[i.replance(",", "")] for i in number if i[0]=="0"])
                 # print("extracted : ", number)
         c_number = ""
         for n in number:
             n = n.replace(",", "")
             if n:
                 if n in data[language]["number"]:
                     c_number += n
@@ -151,37 +151,31 @@
     
     def get_weekday(self, date_:list=[], language="bn"):
 
         """
         Get weekday name Bangla or English
         
         """
-
-        # print("++++++++++++++++++++ : ", date_)
-
-
-        # print("date_: ", date_)
-
-        d, y = list(re.finditer(self.bn_regex, str(date_[0]), re.UNICODE)), list(re.finditer(self.bn_regex, str(date_[2]), re.UNICODE))
+        if date_[0] is None or date_[1] is None or  date_[2] is None:
+            return None
         
-        # print("d, y : ", d, y)
+        d, y = list(re.finditer(self.bn_regex, str(date_[0]), re.UNICODE)), list(re.finditer(self.bn_regex, str(date_[2]), re.UNICODE))
         
         if d:
             date_[0] = self._digit_converter(date_[0], language="bn")
         if y:
             date_[2] = self._digit_converter(date_[2], language="bn")
 
-        # print("date_", date_)
-
         current_date_object = datetime.datetime(int(date_[2]), int(date_[1]), int(date_[0]))
         if language in data:
             weekday = data[language]["weekdays"][current_date_object.weekday()]
         else:
             print("language not handel")
             weekday = ""
+        # print("weekday : ", weekday)
         return weekday
     
     def search_month(self, search_key, language="bn"):
         """
         Search for a month or month abbreviation in the month_data dictionary.
         
         Args:
@@ -278,14 +272,16 @@
         return re.split(separator_pattern, date_string)
 
 
     def month_convert_to_number(self, month):
         """
         
         """
+        index= None
+        # print("month", month)
         key = month.lower().strip()
         if key in data["en"]["months"]:
             index = data["en"]["months"].index(key)+1
         elif key in data["bn"]["months"]:
             index = data["bn"]["months"].index(key)+1
         elif key in  data["bn"]["option_name"]:
             index = data["bn"]["option_name"].index(key)+1
@@ -343,96 +339,153 @@
         else:
             print("Date format not handled yet")
         return None, None
 
 
     def get_date_indexes(self, date_list):
         """
-        
-        
+        Get Date index  
         """
         day, month, year = None, None, None
         for idx, elem in enumerate(date_list):
             if elem.isdigit() and len(elem) == 4:
                 year_idx = idx
                 year = date_list[idx]
-                # print(date_list)
+                # print(year)
                 day, month = self.get_day_and_month(year_idx, idx, date_list)
+                # print(day, month)
         return [day, month, year]
     
     def date_processing(self, date_, language="bn"):
-
         if isinstance(date_, list):
             if len(date_):
                 formatted_date = date_
         else:
             split_date = self.data_splitter(date_)
+            # print("split_date : ", split_date)
             split_date = [i for i in split_date if i]
-
+            # print("split_date : ", split_date)
             if len(split_date)==2:
                 adding_date = ["1"] if language=="en" else ["১"]
                 split_date = adding_date +split_date
 
-            # print("split_date : ", split_date)
 
             if len(split_date) == 1:
                 formatted_date = self.format_non_punctuation(split_date)
             else:
+                # print("hello")
                 formatted_date = self.get_date_indexes(split_date)
 
-        if formatted_date[0] == None and formatted_date[1] == None and formatted_date[2] == None:
+                # print("formatted_date :", formatted_date)
+
+        if formatted_date[0] is None and formatted_date[1] is None and formatted_date[2] is None:
             current_date_object = datetime.date.today()
             formatted_date = [current_date_object.day, current_date_object.month, current_date_object.year]
 
-        weekday = self.npr.get_weekday(formatted_date, language)
-        day   = self.npr._digit_converter(str(formatted_date[0]), language)
-        month = self.npr.search_month(str(formatted_date[1]), language)
-        year  =  self.npr._digit_converter(str(formatted_date[2]), language)
-
-        txt_date = self.npr.number_to_words(day)
-        txt_year = self.npr.year_in_number(year, language=language)
+        elif formatted_date[1] == None:
+            for i in split_date:
+                if formatted_date[0] == i or formatted_date[2] == i:
+                    continue
+                m_numeric = self.month_convert_to_number(i)
+                if m_numeric:
+                    formatted_date[1] = cfg._english2bangla2_digits_mapping[str(m_numeric)]
 
+        # print("final formated date : ", formatted_date)
 
-        return {"date":day, "month": month[0], "year": year, "txt_date":txt_date, "txt_year": txt_year, "weekday" : weekday, "ls_month": month[1], "seasons" : month[2]}
+        if formatted_date[0] is not None and formatted_date[1] is not None and formatted_date[2] is not None:
+            weekday = self.npr.get_weekday(formatted_date, language)
+        else:
+            weekday = None
 
+        if formatted_date[0] is None:
+            day = None
+            txt_date = None
+        else:
+            day   = self.npr._digit_converter(str(formatted_date[0]), language)
+            txt_date = self.npr.number_to_words(day)
+        if formatted_date[1] is None:
+            month = [None, None, None]
+            m_n = None
+        else:
+            m_n = self.npr._digit_converter(str(formatted_date[1]), language)
+            month = self.npr.search_month(str(formatted_date[1]), language)
+        if formatted_date[2] is None:
+            year = None
+            txt_year = None
+        else:
+            year  =  self.npr._digit_converter(str(formatted_date[2]), language)
+            txt_year = self.npr.year_in_number(year, language=language)
+            
+        return {"date":day, "month": m_n, "year": year, "txt_date":txt_date, "txt_month":month[0] ,"txt_year": txt_year, "weekday" : weekday, "ls_month": month[1], "seasons" : month[2]}
 
 
 class TextParser:
 
     def __init__(self):
         self.year_patterns  =["সালের","সালে", "শতাব্দী", "শতাব্দীর", "শতাব্দীতে"]
-        self.year_pattern = r'(?:\b|^\d+)(\d{4})\s*(?:সালে?র?|শতাব্দী(?:র)?|শতাব্দীতে)+'
+        self.year_pattern = r'(?:\b|^\d+)(\d{4})\s*(?:সালে?র?|শতাব্দী(?:র)?|শতাব্দীতে|এর)+'
         self.currency_pattern = r'(?:\$|£|৳|€|¥|₹|₽|₺)?(?:\d+(?:,\d{3})*(?:\.\d+)?|\d+(?:\.\d+)?)'
         self.npr = NumberParser()
         self.dp = DateParser() 
 
     def collapse_whitespace(self, text):
         return re.sub(_whitespace_re, " ", text)
     
+    def exception_year_processing(self, text):
+        _year_with_hyphen = re.findall(r'(\d{4}(?:-|–|—|―)\d{2})', text)
+        # print(_year_with_hyphen)
+        replce_map = {}
+        for year in _year_with_hyphen:
+            # print(year)
+            rep_year = year.replace('–', '-')
+            rep_year = rep_year.replace('—', '-')
+            rep_year = rep_year.replace('―', '-')
+            four_digit_year, two_digit_year = rep_year.split('-')
+            rep_year = self.npr.year_in_number(four_digit_year) + " " + self.npr.number_to_words(two_digit_year)
+            text = text.replace(year, rep_year)
+        return text
+    
     def unwanted_puntuation_removing(self, text):
+        
+        # https://stackoverflow.com/questions/63256077/how-to-remove-redundant-punctuations-keep-only-the-first-one-in-text
+        def my_replace(match): 
+            match = match.group()
+            return match[0] + (" " if " " in match else "")
+
+        _redundent_punc_removal = r"[!\"#$%&\'()*+,\-.\/:;<=>?@\[\\\]^_`।{|}~ ]{2,}"
+        
+        text = _STANDARDIZE_ZW.sub('\u200D', text)
+        text = re.sub(r'\u200d', '', text)
+        text = _DELETE_ZW.sub('', text)
+        
         text = text.replace("'র" , " এর")
         text = text.replace("-র" , " এর")
+        text = text.replace("-" , " ")
+        text = text.replace("°F", "° ফারেনহাইট")
+        text = text.replace("° F", "° ফারেনহাইট")
+        text = text.replace("°C", "° সেলসিয়াস")
+        text = text.replace("° C", "° সেলসিয়াস")
+        
+        
+        text = re.sub(r'(?<=[^\w\s])\s+(?=[^\w\s])', '', text) # deleting space between two punctuations
+        text = re.sub(_redundent_punc_removal, my_replace, text, 0) # only keep the first punctuation
+        
         translation_table = str.maketrans(_punctuations)
-        return text.translate(translation_table)
-        # unwanted_symbols = ["-", "_", ":", "[", "]", "(", ")", "{", "}", "^", "~"]
-        # pattern = "[" + re.escape("".join(unwanted_symbols)) + "]"
-        # text = re.sub(pattern, " ", text)
-        # return text
+        text = text.translate(translation_table)
+        return text
+
 
-    
     def expand_symbols(self, text, lang="bn"):
-        for regex, replacement in _symbols[lang]:
-            # print("regex : ", regex)
-            text = re.sub(regex, replacement, text)
-            text = text.replace("  ", " ")  # Ensure there are no double spaces
+        for key, replacement in  _symbols[lang]:
+            text = text.replace(key, replacement)
         return text.strip()
 
     def expand_abbreviations(self, text, lang="bn"):
-        for regex, replacement in _abbreviations[lang]:
-            text = re.sub(regex, replacement, text)
+        for key, replacement in _abbreviations[lang]:
+            text = text.replace(key, replacement)
         return text
     
     def expand_position(self, text, lang="bn"):
 
         """
         Replace : 
             ("১ম", "প্রথম"),
@@ -474,70 +527,172 @@
 
     def extract_currency_amounts(self, text):
 
         matches = re.findall(self.currency_pattern, text)
         pattern = r'[৳$£€¥₹₽₺]'
 
         for m in matches:
-            # Use findall to extract matches
             currency = re.findall(pattern, m)
-
-            # print(currency)
             if currency:
-                # print("m : ", m)
                 n_m = m.replace(currency[0], "")
                 n_m = n_m.replace(",", "")
                 language = "en" if self.npr.contains_only_english(n_m) else "bn"
                 if "." in n_m:
                     word = self.npr.fraction_number_conversion(n_m, language=language)
-                    r_word =  word+" "+_currency[currency[0]]
+                    r_word =  " " + word+" "+_currency[currency[0]] + " "
                     text = text.replace(m, r_word)
                 else:
                     word = self.npr.number_to_words(n_m)
-                    n_word = word + " "+_currency[currency[0]]
+                    n_word = " " + word + " "+_currency[currency[0]] + " "
                     text = text.replace(m, n_word)
         return text
     
-    def date_formate_validation(self, date):
-        n_data = date.strip().split(" ")
-        month_name = data["en"]["months"]+ data["en"]["months"] + data["en"]["option_name"] + data["bn"]["option_name"]
+    def matching_similariy_of_months(self, input_word):
+        month_name = data["en"]["months"]+ data["bn"]["months"] + data["en"]["option_name"] + data["bn"]["option_name"]
+        similarity_threshold = 90  # Adjust this threshold as needed
+        similar_months = []
+        status = False
+        for month in month_name:
+            similarity_score = fuzz.partial_ratio(input_word, month)
+            if similarity_score >= similarity_threshold:
+                similar_months.append((month, input_word, similarity_score))
+
+        # print("Similar months:")
+        for month, input_word, similarity_score in similar_months:
+            # print(f"{input_word} {month}: Similarity Score = {similarity_score}")
+            status = True
+        # return True
+        if similar_months:
+            sorted_similar_months = sorted(similar_months, key=lambda x: x[2], reverse=True)
+            # print("+++++++", sorted_similar_months)
+            return status, (sorted_similar_months[0][0], sorted_similar_months[0][1])
+        return status, (None, None)
+    
+    def date_formate_validation(self, date, text):
+        n_data =date.strip().split(" ")
         for n_d in n_data:
-            if n_d in month_name:
-                return True
-        return False
-
-
+            status, text_replacer = self.matching_similariy_of_months(n_d)
+            if status:
+                for t in text_replacer:
+                    text = text.replace(t[0], t[1])
+                return status, text
+            if n_d in self.year_patterns:
+                return True, text
+        return False, text
+    
+    def add_spaces_to_numbers(self, text):
+        # Define a regular expression pattern to match both Bangla and English digits without spaces around them
+        pattern = r'(?<![০-৯0-9])[\u09E6-\u09EF0-9]+(?![০-৯0-9])'
+        # Use re.sub to find and replace matches with spaces around them
+        result = re.sub(pattern, lambda x: ' ' + x.group(0) + ' ', text)
+        # print(result)
+        result = " ".join([i for i in result.split(" ") if i.strip()]).strip()
+        return result
+    
+
+    def extract_year(self, text):
+        pattern = re.findall(self.year_pattern, text)
+        for p in pattern:
+            text = text.replace(p, f" {p} ")
+        return text
     
     def replance_date_processing(self, text):
+        text = self.extract_year(text)
+        original_text = text
+        r_text = text
+        # print("original_text : ", original_text)
         dates = dt.get_dates(text)
-        # print()
+        # print("+++++++++++++++++++++++++++ date :++++++++++++++++++++++++", dates)
         for date in dates:
+            r_date = date
+            # spanning_position = self.npr.find_word_index(text, date)
+            # print(spanning_position)
+            date = self.add_spaces_to_numbers(date)
+            # print("date:", date)
             status = True
             if " " in date:
-                status = self.date_formate_validation(date)
+                status, text = self.date_formate_validation(date, text)
             if status:
-                position = self.npr.find_word_index(text, date)
                 formated_date = self.dp.date_processing(date)
-                f_d_string = formated_date["txt_date"]+" "+formated_date["month"]+" "+formated_date["txt_year"]
-                text = self.npr.replace_text_at_position(text, f_d_string, position[0], position[1])
-        return text
+                original_date = date
+                date_list = [i for i in date.split(" ") if i.strip()]
+                # print(date_list)
+                for k, v in formated_date.items():
+                    if v in date_list:
+                        key = k if "txt" in k else f"txt_{k}"
+                        index = date_list.index(v)
+                        date_list[index] = formated_date[key]
+
+                process_date = " ".join(date_list).strip()
+                original_text = original_text.replace(r_date, " "+process_date+" ")
+                # search for only year
+        
+        _only_years = re.findall(self.year_pattern, original_text)
+        # print(_only_years)
+        for y in _only_years:
+            original_text = original_text.replace(y, " " +self.npr.year_in_number(y) + " ")
+        return original_text
 
     
 
     def processing(self, text):
+        text = self.exception_year_processing(text)
         text = self.unwanted_puntuation_removing(text)
         text = self.expand_symbols(text)
         text = self.expand_abbreviations(text)
         text = self.expand_position(text)
         text = self.extract_currency_amounts(text)
         text = self.replance_date_processing(text)
+        # handel the exception year like 2017-18
+        
+
         text = self.npr.number_processing(text)
         text = self.collapse_whitespace(text)
         return text
     
+
+class EmojiRemoval:
+    
+    def __init__(self):
+        self.regex_to_remove_emoji = re.compile("["
+                                                u"\U0001F600-\U0001F64F"  # emoticons
+                                                u"\U0001F300-\U0001F5FF"  # symbols & pictographs
+                                                u"\U0001F680-\U0001F6FF"  # transport & map symbols
+                                                u"\U0001F1E0-\U0001F1FF"  # flags (iOS)
+                                                u"\U00002500-\U00002BEF"  # chinese char
+                                                u"\U00002702-\U000027B0"
+                                                u"\U00002702-\U000027B0"
+                                                u"\U000024C2-\U0001F251"
+                                                u"\U0001f926-\U0001f937"
+                                                u"\U00010000-\U0010ffff"
+                                                u"\u2640-\u2642"
+                                                u"\u2600-\u2B55"
+                                                u"\u200d"
+                                                u"\u23cf"
+                                                u"\u23e9"
+                                                u"\u231a"
+                                                u"\ufe0f"  # dingbats
+                                                u"\u3030"
+                                                            "]+", re.UNICODE)
+        self.tp = TextParser()
+    
+    def remove_emoji(self, text):
+        text = re.sub(self.regex_to_remove_emoji, ' ', text)
+        text = self.tp.collapse_whitespace(text)
+        return text
+
+# class EmojiReplacer:
+#     def __init__(self):
+#         self.translator = Translator()
+        
+#     def replace_emoji(self, text):
+#         txt = self.translator.translate(text).text
+#         # print(txt)
+#         return text if len(txt)==0 else txt
+
 if __name__ =="__main__":
 
     text = "রাহিম ক্লাস ওয়ান এ ১ম, ১১তম ২২ তম ৩৩ তম, ১২৩৪ শতাব্দীতে ¥২০৩০.১২৩৪ বিবিধ  বাকেরগঞ্জ উপজেলার প্রায় 40 ভাগের পেশাই চাষাবাদ 80 and 40 ২২"
     tp = TextParser()
     text = tp.processing(text)
     print(text)
```

### Comparing `pybangla-1.0.9.dev0/pybangla/module/word_to_number.py` & `pybangla-1.0.9.dev1/pybangla/module/word_to_number.py`

 * *Files identical despite different names*

### Comparing `pybangla-1.0.9.dev0/pybangla/test.py` & `pybangla-1.0.9.dev1/pybangla/test.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,47 +1,52 @@
 import time
 from module.main import Normalizer
 
 if __name__ == "__main__":
 
 
     # # Testing Date format
-    # date_list = [
+    date_list = [
+    #     "০১-এপ্রিল/২০২৩",
     #     "সেপ্টেম্বর ০৫ ২০২৩",
-    #     "এপ্রিল ২০২৩" 
-    #     "2023-04-05",  
-    #     "06-04-2023", 
-    #     "04/01/2023",  
-    #     "07 April, 2023", 
-    #     "Apr 1, 2023",  
-    #     "2023/04/01", 
-    #     "01-Apr-2023", 
-    #     "01-Apr/2023",  
-    #     "20230401",  
-    #     "20042024",
-    #     ["1", "4", "2025"]
-    # ]
+        "01-Apr/2023"
+        # "এপ্রিল ২০২৩" 
+        # "2023-04-05",  
+        # "06-04-2023", 
+        # "04/01/2023",  
+        # "07 April, 2023", 
+        # "Apr 1, 2023",  
+        # "2023/04/01", 
+        # "01-Apr-2023", 
+        # "01-Apr/2023",  
+        # "20230401",  
+        # "20042024",
+        # "20230401",
+        # ["1", "4", "2025"]
+    ]
     # # # # number = "123456" or "২০২৩"
     # # number = "২০২৩"
     nrml = Normalizer()
-    # # # print("++++++++++++++++++++ Date testing ++++++++++++++++++++++")
-    # # print("Date format Testing : ", end ="", flush=True)
-    # for date_ in date_list:
-    #     start_time = time.time()
-    #     formated_date = nrml.date_format(date_, language="bn")
-    #     print(formated_date)
+    # # # # print("++++++++++++++++++++ Date testing ++++++++++++++++++++++")
+    # # # print("Date format Testing : ", end ="", flush=True)
+    for date_ in date_list:
+        start_time = time.time()
+        print("date_:", date_)
+        formated_date = nrml.date_format(date_, language="en")
+        print(formated_date)
     # print("++++++++++++++++++++ end of Date testing ++++++++++++++++++++++")
 
     # print("++++++++++++++++++++ en number to bn number convert ++++++++++++++++++++++")
-    # number = nrml.number_convert(number, language="bn")
+    number = "1234"
+    number = nrml.number_convert(number, language="en")
     
     
     # number = nrml.number_convert(number, language="bn")
 
-    # print("Bn Number : ", number)
+    print("Bn Number : ", number)
     # print("++++++++++++++++++++ stop number convert ++++++++++++++++++++++")
 
     # # print("++++++++++++++++ Today +++++++++++++++++++++")
     # today_date = nrml.today(language="bn")
     # # today_date = nrml.today(language="en")
     # print(today_date)
 
@@ -150,32 +155,86 @@
     #     "তিনশ পঁচিশ পাঁচশ এক",
     #     "চা-পুন",
     #     "ওকে",
     #     "ডের আউটস্ট্যান্ডিং কত",
     #     "ডাবল",
     #     "নাইন ডাবল এইট",
     #     "দশ বারো এ এগুলা একশ একশ দুই",
-    #     "এক লক্ষ তেত্রিশ চার"
+    #     "এক লক্ষ তেত্রিশ চার",
+    #     "আমাকে এক লক্ষ দুই হাজার এক টাকা দেয় এন্ড তুমি বিশ হাজার টাকা নিও এন্ড এক লক্ষ চার হাজার দুইশ এক টাকা এক ডবল দুই"
     #     ]
     # for i in input_texts:
     #     print("="*40)
     #     print("input : ", i)
     #     text = nrml.word2number(i)
     #     print("output : ", text)
     #     print("="*40)
     # text = "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে. এপ্রিল ২,০২৩"
     # formated_date = nrml.date_extraction(text)
 
     # print(formated_date)
 
-    # text = "৫ বছরে নন-ক্যাডার পদে ৭,৪৪৭ জনকে নিয়োগের সুপারিশ করা হয়েছে 1,230"
-    text = "৫ বছরে নন-ক্যাডার পদে ৭,৪৪৭ জনকে নিয়োগের সুপারিশ করা হয়েছে"
+    # # text = "৫ বছরে নন-ক্যাডার পদে ৭,৪৪৭ জনকে নিয়োগের সুপারিশ করা হয়েছে 1,230"
+    # text = "৫ বছরে নন-ক্যাডার পদে ৭,৪৪৭ জনকে নিয়োগের সুপারিশ করা হয়েছে"
 
     # text = "শীঘ্রই ভিক্টোরিয়ার এক প্রতিনিধিদল আসছেন,শিলংয়ের ব্রুকসাইড হাউসে"
 
     # text = "The numbers are 10 নন-ক্যাডার 20.5  30, and 40.75. সুপারিশ ২০৩০.৩০ 12 23 45"
-    # text = "This_is-a:test~sentence^with{some}unwanted[symbols]"
 
-    print("input : ", text)
-    text = nrml.text_normalizer(text)
-    print("output : ", text)
+    # bangla_sentences = [
+    # "১৯৯৬ সালের ৬ তারিখে নির্ধারিত করা হয়েছে.",
+    # "১৯৯৬ সালের ৬ সেপ্টেম্বর ভ্রমণ পরিকল্পনা করছি.",
+    # "আমি জুলাই ২০২৩ তে একটি সমুদ্র ভ্রমণ পরিকল্পনা করছি.",
+    # "সম্মেলনটি সেপ্টেম্বর ০৫ ২০২৩ তারিখে নির্ধারিত করা হয়েছে.",
+    # "আমরা খ্রীষ্টমাসের জন্য ডিসেম্বর ২৫ ২০২৩ তারিখে পরিবারের সংগঠন করব.",
+    # "আমার বোনের বিয়ে ১৮ মার্চ, ২০২৩ তারিখে.",
+    # "আমি আগামী ১২ আগস্ট, ২০২৩ তারিখে আমার জন্মদিনে দেখা করছি.",
+    # "আমরা ফেব্রুয়ারি ২০২৩ তে স্কিউইং যাব.",
+    # "আমাদের কোম্পানির পিকনিকটি জুন ৩০ ২০২৩ তারিখে নির্ধারিত হয়েছে.",
+    # "আমার গুরুত্বপূর্ণ পরীক্ষা ১০ মে, ২০২৩ তারিখে.",
+    # "নতুন সেমিস্টার শুরু হয় জানুয়ারি ২০২৩ তারিখে.",
+    # "আমরা এপ্রিল ২০২৩ তে একটি রোড ট্রিপ পরিকল্পনা করছি.",
+    # "আমি অক্টোবর ২০২৩ তারিখে একটি নতুন অ্যাপার্টমেন্টে যাচ্ছি.",
+    # "আপনার ক্যালেন্ডারের মার্ক নভেম্বর ০৫, ২০২৩, এটি দীপাবলি.",
+    # "আমি জুলাই ২০২৩ তারিখে গরম শিবিরের জন্য উৎসাহিত.",
+    # "মার্চ ২৫, ২০২৩ তারিখের কনসার্ট টিকেটগুলি দ্রুত বিক্রয় হচ্ছে.",
+    # "আগস্ট ২০২৩ তারিখে একটি বারবিকিউ পার্টি আয়োজন করা হবে.",
+    # "আমি মে ২০২৩ তারিখে আমার নানা-নানির কাছে যাচ্ছি.",
+    # "আমি সেপ্টেম্বর ২০২৩ তারিখে একটি বিয়ে অনুষ্ঠানে যাচ্ছি.",
+    # "আমরা জুন ২০২৩ তে ইউরোপে একটি ভ্রমণ পরিকল্পনা করছি.",
+    # "আমার ডেন্টিস্টের অ্যাপয়েন্টমেন্ট এপ্রিল ১০, ২০২৩ তারিখে.",
+    # "কোম্পানির বার্ষিক সভা ফেব্রুয়ারি ২০২৩ তারিখে হয়.",
+    # "আমার অনুষ্ঠান সমাপন হয়েছে জুন ১৫, ২০২৩ তারিখে.",
+    # "আমি মার্চ ২০২৩ তারিখে একটি নতুন চাকরি শুরু করছি.",
+    # "আমি মে ২০২৩ তারিখে পাহাড়ে ট্রেকিং করতে যাচ্ছি.",
+    # "বিদ্যালয়ের নাটকটি নভেম্বর ২০২৩ তারিখে নির্ধারিত হয়েছে.",
+    # "আমরা অক্টোবর ২০২৩ তার",
+    # "১৯৯৬ সালের ৬ সেপ্টেম্বর",
+    # "২০৩০ সালের ৬ সেপ্টেম্বর",
+    # "১৯৯৬ সালের৬ তারিখে নির্ধারিত করা হয়েছে.",
+    # "১৯৯৬সালের ৬ সেপ্টেম্বররণ ভ্রমণ পরিকল্পনা করছি ২০৩০সালের ৬সেপ্টেম্বর",
+    # "এয়ারলাইনসসহ তিনটি এয়ারলাইনসের ৫১টি ফ্লাইটে মো: ২০ হাজার ২৯১ জন হজযাত্রী সৌদি আরবে গেছেন। এ বছর হজ করতে ৮৫ হাজার ২৫৭ জনের সৌদি আরবে যাওয়ার কথা রয়েছে।",
+    # " সাঃ কিমি হাফিক বিডিটি এয়ারলাইনসসহ তিনটি এয়ারলাইনসের ৫১টি কিমি. ফ্লাইটে মোট ২০ হাজার ২৯১ জন হজযাত্রী সৌদি আরবে গেছেন। এ বছর হজ করতে ৮৫ হাজার ২৫৭ জনের সৌদি আরবে যাওয়ার কথা রয়েছে। ৫ম",
+    # "প্রদর্শনীটি চলার কথা ছিল ১২ মে পর্যন্ত, তবে দর্শকদের ব্যাপক আগ্রহের কারণে তিন দিন সময় বাড়িয়ে ১৫ মে পর্যন্ত করা হয়েছিল ১৫.১৫",
+    # "The numbers are 10 নন-ক্যাডার 20.5  30, and 40.75. সুপারিশ ২০৩০.৩০ 12 23 45",
+    # "[১৯৯৬]-সালের-৬:তারিখে-নির্ধারিত করা হয়েছে"
+    # ]
+
+    # # solving steps is have number need to give extra space both side
+    # issue = [
+    # "[১৯৯৬]-সালের-৬:তারিখে-নির্ধারিত করা হয়েছে.",
+    # "১৯৯৬সালের ৬ সেপ্টেম্বররণ ভ্রমণ পরিকল্পনা করছি ২০৩০সালের ৬সেপ্টেম্বর",
+    # "আজকের তাপমাত্রা ৪৪°F",
+    # "আজকের তাপমাত্রা ৪৪°C",
+    # "যেমন ১৯৬১ সালে দেশটির তৎকালীন প্রেসিডেন্ট ডোয়াইট ডি আইজেনহাওয়ার শিক্ষা খাতে সামরিক শিল্পের প্রবেশের বিপদ নিয়ে সতর্ক করেছিলেন।",
+    # "১৯৯৬সালের ৬ সেপ্টেম্বররণ ভ্রমণ পরিকল্পনা করছি ২০৩০সালের ৬সেপ্টেম্বর"
+    # ]
+
+
+
+    # for i in issue:
+
+    #     print("input : ", i)
+    #     text = nrml.text_normalizer(i)
+    #     print("output : ", text)
+    #     print("+"*40)
```

### Comparing `pybangla-1.0.9.dev0/setup.py` & `pybangla-1.0.9.dev1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 import codecs
 from setuptools import setup, find_packages
 
 setup(
     name='pybangla',
-    version='1.0.9-dev',
+    version='1.0.9-dev1',
     packages=find_packages(),
     # entry_points={
     #     'console_scripts': [
     #         'pybangla = pybangla.main:Normalizer'
     #     ]
     # },
     author='saiful',
@@ -23,11 +23,13 @@
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "DateTime",
-        "num2words"
+        "num2words",
+        "python-Levenshtein",
+        "fuzzywuzzy"
     ],
     python_requires = ">=3.6"
 )
```

