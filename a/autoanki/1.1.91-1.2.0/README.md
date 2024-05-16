# Comparing `tmp/autoanki-1.1.91.tar.gz` & `tmp/autoanki-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoanki-1.1.91.tar", last modified: Sun May 12 03:02:20 2024, max compression
+gzip compressed data, was "autoanki-1.2.0.tar", last modified: Thu May 16 00:50:40 2024, max compression
```

## Comparing `autoanki-1.1.91.tar` & `autoanki-1.2.0.tar`

### file list

```diff
@@ -1,41 +1,46 @@
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.297477 autoanki-1.1.91/
--rw-r--r--   0 owner      (501) staff       (20)     1062 2024-04-04 21:53:37.000000 autoanki-1.1.91/LICENSE.txt
--rw-r--r--   0 owner      (501) staff       (20)      134 2024-05-12 02:29:19.000000 autoanki-1.1.91/MANIFEST.in
--rw-r--r--   0 owner      (501) staff       (20)     5559 2024-05-12 03:02:20.297403 autoanki-1.1.91/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)     5024 2024-04-15 21:45:41.000000 autoanki-1.1.91/README.md
--rw-r--r--   0 owner      (501) staff       (20)      223 2023-05-05 21:35:51.000000 autoanki-1.1.91/pyproject.toml
--rw-r--r--   0 owner      (501) staff       (20)      125 2024-04-14 18:52:00.000000 autoanki-1.1.91/requirements.txt
--rw-r--r--   0 owner      (501) staff       (20)      701 2024-05-12 03:02:20.298227 autoanki-1.1.91/setup.cfg
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.274367 autoanki-1.1.91/src/
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.276563 autoanki-1.1.91/src/autoanki/
--rw-r--r--   0 owner      (501) staff       (20)     6234 2024-05-08 02:45:14.000000 autoanki-1.1.91/src/autoanki/AutoAnki.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.278149 autoanki-1.1.91/src/autoanki/BookCleaner/
--rw-r--r--   0 owner      (501) staff       (20)     4480 2024-05-08 01:47:01.000000 autoanki-1.1.91/src/autoanki/BookCleaner/BookCleaner.py
--rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.1.91/src/autoanki/BookCleaner/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.279513 autoanki-1.1.91/src/autoanki/DatabaseManager/
--rw-r--r--   0 owner      (501) staff       (20)    14271 2024-05-12 01:52:56.000000 autoanki-1.1.91/src/autoanki/DatabaseManager/DatabaseManager.py
--rw-r--r--   0 owner      (501) staff       (20)       45 2023-04-17 16:36:34.000000 autoanki-1.1.91/src/autoanki/DatabaseManager/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.1.91/src/autoanki/DatabaseManager/book_table.sql
--rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.1.91/src/autoanki/DatabaseManager/book_table_view.sql
--rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.1.91/src/autoanki/DatabaseManager/databases_init.sql
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.280603 autoanki-1.1.91/src/autoanki/DeckManager/
--rw-r--r--   0 owner      (501) staff       (20)     4745 2024-05-08 02:25:04.000000 autoanki-1.1.91/src/autoanki/DeckManager/DeckManager.py
--rw-r--r--   0 owner      (501) staff       (20)       67 2024-04-04 22:41:18.000000 autoanki-1.1.91/src/autoanki/DeckManager/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)     2654 2024-04-15 21:12:02.000000 autoanki-1.1.91/src/autoanki/DeckManager/template_decks.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.282433 autoanki-1.1.91/src/autoanki/Dictionary/
--rw-r--r--   0 owner      (501) staff       (20)     6441 2024-05-08 02:44:04.000000 autoanki-1.1.91/src/autoanki/Dictionary/CEDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)      286 2024-04-12 01:17:18.000000 autoanki-1.1.91/src/autoanki/Dictionary/Dictionary.py
--rw-r--r--   0 owner      (501) staff       (20)     5339 2024-04-15 18:03:31.000000 autoanki-1.1.91/src/autoanki/Dictionary/YellowBridgeDictionary.py
--rw-r--r--   0 owner      (501) staff       (20)       40 2024-03-31 20:26:56.000000 autoanki-1.1.91/src/autoanki/Dictionary/__init__.py
--rw-rw-r--   0 owner      (501) staff       (20)  9650508 2024-04-10 22:45:58.000000 autoanki-1.1.91/src/autoanki/Dictionary/cedict_ts.u8
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.296725 autoanki-1.1.91/src/autoanki/Tokenizer/
--rw-r--r--   0 owner      (501) staff       (20)     6669 2024-05-08 02:41:46.000000 autoanki-1.1.91/src/autoanki/Tokenizer/ChineseTokenizer.py
--rw-r--r--   0 owner      (501) staff       (20)      223 2024-04-12 14:29:21.000000 autoanki-1.1.91/src/autoanki/Tokenizer/Tokenizer.py
--rw-r--r--   0 owner      (501) staff       (20)       48 2024-04-11 22:24:23.000000 autoanki-1.1.91/src/autoanki/Tokenizer/__init__.py
--rw-r--r--   0 owner      (501) staff       (20)       30 2023-04-17 17:57:08.000000 autoanki-1.1.91/src/autoanki/__init__.py
-drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-12 03:02:20.297073 autoanki-1.1.91/src/autoanki.egg-info/
--rw-r--r--   0 owner      (501) staff       (20)     5559 2024-05-12 03:02:20.000000 autoanki-1.1.91/src/autoanki.egg-info/PKG-INFO
--rw-r--r--   0 owner      (501) staff       (20)     1046 2024-05-12 03:02:20.000000 autoanki-1.1.91/src/autoanki.egg-info/SOURCES.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2024-05-12 03:02:20.000000 autoanki-1.1.91/src/autoanki.egg-info/dependency_links.txt
--rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.1.91/src/autoanki.egg-info/not-zip-safe
--rw-r--r--   0 owner      (501) staff       (20)        9 2024-05-12 03:02:20.000000 autoanki-1.1.91/src/autoanki.egg-info/top_level.txt
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.083384 autoanki-1.2.0/
+-rw-r--r--   0 owner      (501) staff       (20)     1062 2024-04-04 21:53:37.000000 autoanki-1.2.0/LICENSE.txt
+-rw-r--r--   0 owner      (501) staff       (20)      108 2024-05-14 11:15:45.000000 autoanki-1.2.0/MANIFEST.in
+-rw-r--r--   0 owner      (501) staff       (20)     5810 2024-05-16 00:50:40.083314 autoanki-1.2.0/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)     5053 2024-05-16 00:38:17.000000 autoanki-1.2.0/README.md
+-rw-r--r--   0 owner      (501) staff       (20)      272 2024-05-12 08:57:48.000000 autoanki-1.2.0/pyproject.toml
+-rw-r--r--   0 owner      (501) staff       (20)      119 2024-05-12 09:05:06.000000 autoanki-1.2.0/requirements.txt
+-rw-r--r--   0 owner      (501) staff       (20)      845 2024-05-16 00:50:40.083684 autoanki-1.2.0/setup.cfg
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.068505 autoanki-1.2.0/src/
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.070674 autoanki-1.2.0/src/autoanki/
+-rw-r--r--   0 owner      (501) staff       (20)     9130 2024-05-16 00:05:35.000000 autoanki-1.2.0/src/autoanki/AutoAnki.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.072234 autoanki-1.2.0/src/autoanki/BookCleaner/
+-rw-r--r--   0 owner      (501) staff       (20)     4461 2024-05-14 08:51:38.000000 autoanki-1.2.0/src/autoanki/BookCleaner/BookCleaner.py
+-rw-r--r--   0 owner      (501) staff       (20)       37 2023-04-17 16:36:34.000000 autoanki-1.2.0/src/autoanki/BookCleaner/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.073577 autoanki-1.2.0/src/autoanki/DatabaseManager/
+-rw-r--r--   0 owner      (501) staff       (20)    13253 2024-05-16 00:46:33.000000 autoanki-1.2.0/src/autoanki/DatabaseManager/ChineseDatabaseManager.py
+-rw-r--r--   0 owner      (501) staff       (20)     1873 2024-05-14 10:45:18.000000 autoanki-1.2.0/src/autoanki/DatabaseManager/DatabaseManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       59 2024-05-14 09:37:30.000000 autoanki-1.2.0/src/autoanki/DatabaseManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)      208 2023-04-18 23:52:52.000000 autoanki-1.2.0/src/autoanki/DatabaseManager/book_table.sql
+-rw-r--r--   0 owner      (501) staff       (20)      186 2023-04-17 16:36:34.000000 autoanki-1.2.0/src/autoanki/DatabaseManager/book_table_view.sql
+-rw-r--r--   0 owner      (501) staff       (20)      904 2023-04-17 16:36:34.000000 autoanki-1.2.0/src/autoanki/DatabaseManager/databases_init.sql
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.074223 autoanki-1.2.0/src/autoanki/DeckManager/
+-rw-r--r--   0 owner      (501) staff       (20)     4929 2024-05-16 00:46:57.000000 autoanki-1.2.0/src/autoanki/DeckManager/DeckManager.py
+-rw-r--r--   0 owner      (501) staff       (20)       67 2024-04-04 22:41:18.000000 autoanki-1.2.0/src/autoanki/DeckManager/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)     2829 2024-05-16 00:46:57.000000 autoanki-1.2.0/src/autoanki/DeckManager/template_decks.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.075205 autoanki-1.2.0/src/autoanki/Dictionary/
+-rw-r--r--   0 owner      (501) staff       (20)     6148 2024-05-14 08:26:48.000000 autoanki-1.2.0/src/autoanki/Dictionary/.DS_Store
+-rw-r--r--   0 owner      (501) staff       (20)     6599 2024-05-16 00:46:57.000000 autoanki-1.2.0/src/autoanki/Dictionary/CEDictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)      285 2024-05-14 08:51:38.000000 autoanki-1.2.0/src/autoanki/Dictionary/Dictionary.py
+-rw-r--r--   0 owner      (501) staff       (20)       39 2024-05-14 08:51:38.000000 autoanki-1.2.0/src/autoanki/Dictionary/__init__.py
+-rw-rw-r--   0 owner      (501) staff       (20)  9650508 2024-04-10 22:45:58.000000 autoanki-1.2.0/src/autoanki/Dictionary/cedict_ts.u8
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.082499 autoanki-1.2.0/src/autoanki/Tokenizer/
+-rw-r--r--   0 owner      (501) staff       (20)     6665 2024-05-16 00:46:57.000000 autoanki-1.2.0/src/autoanki/Tokenizer/ChineseTokenizer.py
+-rw-r--r--   0 owner      (501) staff       (20)      222 2024-05-14 08:51:38.000000 autoanki-1.2.0/src/autoanki/Tokenizer/Tokenizer.py
+-rw-r--r--   0 owner      (501) staff       (20)       47 2024-05-14 08:51:38.000000 autoanki-1.2.0/src/autoanki/Tokenizer/__init__.py
+-rw-r--r--   0 owner      (501) staff       (20)       31 2024-05-14 08:51:38.000000 autoanki-1.2.0/src/autoanki/__init__.py
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.082965 autoanki-1.2.0/src/autoanki.egg-info/
+-rw-r--r--   0 owner      (501) staff       (20)     5810 2024-05-16 00:50:40.000000 autoanki-1.2.0/src/autoanki.egg-info/PKG-INFO
+-rw-r--r--   0 owner      (501) staff       (20)     1169 2024-05-16 00:50:40.000000 autoanki-1.2.0/src/autoanki.egg-info/SOURCES.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2024-05-16 00:50:40.000000 autoanki-1.2.0/src/autoanki.egg-info/dependency_links.txt
+-rw-r--r--   0 owner      (501) staff       (20)        1 2023-05-05 21:37:00.000000 autoanki-1.2.0/src/autoanki.egg-info/not-zip-safe
+-rw-r--r--   0 owner      (501) staff       (20)      118 2024-05-16 00:50:40.000000 autoanki-1.2.0/src/autoanki.egg-info/requires.txt
+-rw-r--r--   0 owner      (501) staff       (20)        9 2024-05-16 00:50:40.000000 autoanki-1.2.0/src/autoanki.egg-info/top_level.txt
+drwxr-xr-x   0 owner      (501) staff       (20)        0 2024-05-16 00:50:40.082779 autoanki-1.2.0/tests/
+-rw-r--r--   0 owner      (501) staff       (20)     1294 2024-05-14 10:48:54.000000 autoanki-1.2.0/tests/test_AutoAnki.py
+-rw-r--r--   0 owner      (501) staff       (20)      467 2024-05-14 08:51:38.000000 autoanki-1.2.0/tests/test_DeckManager.py
```

### Comparing `autoanki-1.1.91/LICENSE.txt` & `autoanki-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.91/PKG-INFO` & `autoanki-1.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,98 +1,85 @@
-Metadata-Version: 2.1
-Name: autoanki
-Version: 1.1.91
-Summary: Automatically make Anki Decks for Chinese text
-Home-page: https://github.com/timmy6figures/autoanki
-Author: Jarvis Coghlin
-Author-email: jarviscoghlin@gmail.com
-Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-> **❗️** <br>
-Pull requests welcome! If you think you can improve AA in any way, open a PR!
-
 # autoanki
-Tool for generating Anki flashcards to learn Chinese.
+Tool for generating Chinese flashcards for Anki
 
-<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/example.jpg?raw=true" alt="Text to Anki" width="80%"/>
+![PyPI - Version](https://img.shields.io/pypi/v/autoanki)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/timmy6figures/autoanki/python-package.yml)
 
-## Motivation
+## About
 
 When learning Chinese, some common advice is to learn the top X most common words.
 This is good advice, as you can get pretty far with this, however it's [not perfect](https://en.wikipedia.org/wiki/Zipf%27s_law#/media/File:Zipf's_law_on_War_and_Peace.png).
 
 For example, Harry Potter. This book will have normal distribution for most words, however there will be a heavy emphasis on a specialized subset of words such as Wand, Robe, Wizard, Broomstick etc. These words will show up a lot more than they would otherwise.
 
 The intention of this package was to allow Chinese learners to move from beginner books to more advanced material. I found there was a gap in knowledge going from beginner learning books (where there is little specalized terminology), to teen novels, where each novel will generally have its own specialized terminology, making the transition tedious. This is solved by automatically making Anki decks that have this specialized terminology, so that you are able to memorize these words while continuing to make progress
 
 With autoanki, you selectively add words to an Anki file to continue progressing with your lanuage learning skills.
 
 ## Usage
 
-autoanki is both a library and a command-line tool.
-
 To get started, run 
 ```pip install autoanki```
 This should install all the requirements. Then, in a Python file, do ```from autoanki import AutoAnki```
 
-To get started, first, create a database for autoanki to use 
+To get started, create an autoanki instance with the 2-letter code of the language you want to use
+```
+aa = AutoAnki('zh')
+```
+Opitonally, include a path to a database file you want to use:
 ```    
 db_path = "AutoAnki.db"
 if not AutoAnki.is_database(db_path):
     AutoAnki.create_database(db_path)
 ```
-Then create an instance of autoanki using the database
-```
-aa = AutoAnki(db_path)
-```
-Add whatever books you want in your deck. These can be a single file, or a folder
+
+Add whatever books you want in your deck. These can be a single file, or a string
 ```
 bookpath = 'short-story.txt'
-aa.add_book(bookpath, 'My first book🍎')
+aa.add_book_from_string("...", 'My first book🍎')
+aa.add_book_from_string(bookpath, 'My first book🍎')
 ```
+
 Once all of your books are added, the definitions need to be found, and then you can create a deck!
 ```
 aa.complete_unfinished_definitions()
 aa.create_deck("AutoAnki Deck", "output")
 ```
+
 This will automatically have the .apkg extension, which Anki uses. 
 Import this file into Anki, and you're all set.
 
+
 #### Other commands
-If you want to see the status of the database, use:
+If you want to see the information of a database, use:
 ```
 aa.print_database_info()
 ```
-If you would like to create and use your own dictionary, you can pass it in when you 
+
+If you would like to create and use your own dictionary, you can pass it in:
 ```
 aa = AutoAnki(db_path, dictionary=CustomDictionary())
 ```
 This dictionary must implement functions from the abstract class `autoanki/Dictionary.py`
 
 Some settings can be set regarding how cards will be formatted, and what will be shown. They can be seen here:
 ```
 aa.deck_settings(
 include_traditional=True,
 include_part_of_speech=True,
-word_frequency_filter=1e-05 # Float between 0 and 1. Filters using this library: https://pypi.org/project/wordfreq/
+word_frequency_filter=1e-05 # Filters using this library: https://pypi.org/project/wordfreq/
 )
 ```
+The filter is the percentage of words less frequent: 的 shows up 6% of the time in text, so putting a value of 7 will omit it
 
 ## How it works
 AutoAnki interfaces has 4 components on the back end:
-1. BookCleaner: Cleans the input coming in from files that the user supplies 
-2. DatabaseManager: Takes the cleaned input and puts it into the database
-3. Dictionary: Finds definitions for words in the database
-4. DeckManager: Creates Decks
+1. DatabaseManager: Takes the cleaned input and puts it into the database
+2. Dictionary: Finds definitions for words in the database
+3. DeckManager: Creates Decks
 
 ### Dictionary
 This is an abstract class that can be implemented with the following methods
 - `__init__(debug_level)`
 - `find_word(word)` - Returns None, or a list of paramaters that match the input of DatabaseManager.update_definition()
 - `size()` - Number of entries in the dictionary
```

### Comparing `autoanki-1.1.91/README.md` & `autoanki-1.2.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,107 @@
-> **❗️** <br>
-Pull requests welcome! If you think you can improve AA in any way, open a PR!
+Metadata-Version: 2.1
+Name: autoanki
+Version: 1.2.0
+Summary: Automatically make Anki Decks for Chinese text
+Home-page: https://github.com/timmy6figures/autoanki
+Author: Jarvis Coghlin
+Author-email: jarviscoghlin@gmail.com
+Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: chinese-converter>=1.1.1
+Requires-Dist: beautifulsoup4~=4.12.2
+Requires-Dist: genanki~=0.13.0
+Requires-Dist: jieba~=0.42.1
+Requires-Dist: pinyin~=0.4.0
+Requires-Dist: requests~=2.31.0
+Requires-Dist: wordfreq
 
 # autoanki
-Tool for generating Anki flashcards to learn Chinese.
+Tool for generating Chinese flashcards for Anki
 
-<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/example.jpg?raw=true" alt="Text to Anki" width="80%"/>
+![PyPI - Version](https://img.shields.io/pypi/v/autoanki)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/timmy6figures/autoanki/python-package.yml)
 
-## Motivation
+## About
 
 When learning Chinese, some common advice is to learn the top X most common words.
 This is good advice, as you can get pretty far with this, however it's [not perfect](https://en.wikipedia.org/wiki/Zipf%27s_law#/media/File:Zipf's_law_on_War_and_Peace.png).
 
 For example, Harry Potter. This book will have normal distribution for most words, however there will be a heavy emphasis on a specialized subset of words such as Wand, Robe, Wizard, Broomstick etc. These words will show up a lot more than they would otherwise.
 
 The intention of this package was to allow Chinese learners to move from beginner books to more advanced material. I found there was a gap in knowledge going from beginner learning books (where there is little specalized terminology), to teen novels, where each novel will generally have its own specialized terminology, making the transition tedious. This is solved by automatically making Anki decks that have this specialized terminology, so that you are able to memorize these words while continuing to make progress
 
 With autoanki, you selectively add words to an Anki file to continue progressing with your lanuage learning skills.
 
 ## Usage
 
-autoanki is both a library and a command-line tool.
-
 To get started, run 
 ```pip install autoanki```
 This should install all the requirements. Then, in a Python file, do ```from autoanki import AutoAnki```
 
-To get started, first, create a database for autoanki to use 
+To get started, create an autoanki instance with the 2-letter code of the language you want to use
+```
+aa = AutoAnki('zh')
+```
+Opitonally, include a path to a database file you want to use:
 ```    
 db_path = "AutoAnki.db"
 if not AutoAnki.is_database(db_path):
     AutoAnki.create_database(db_path)
 ```
-Then create an instance of autoanki using the database
-```
-aa = AutoAnki(db_path)
-```
-Add whatever books you want in your deck. These can be a single file, or a folder
+
+Add whatever books you want in your deck. These can be a single file, or a string
 ```
 bookpath = 'short-story.txt'
-aa.add_book(bookpath, 'My first book🍎')
+aa.add_book_from_string("...", 'My first book🍎')
+aa.add_book_from_string(bookpath, 'My first book🍎')
 ```
+
 Once all of your books are added, the definitions need to be found, and then you can create a deck!
 ```
 aa.complete_unfinished_definitions()
 aa.create_deck("AutoAnki Deck", "output")
 ```
+
 This will automatically have the .apkg extension, which Anki uses. 
 Import this file into Anki, and you're all set.
 
+
 #### Other commands
-If you want to see the status of the database, use:
+If you want to see the information of a database, use:
 ```
 aa.print_database_info()
 ```
-If you would like to create and use your own dictionary, you can pass it in when you 
+
+If you would like to create and use your own dictionary, you can pass it in:
 ```
 aa = AutoAnki(db_path, dictionary=CustomDictionary())
 ```
 This dictionary must implement functions from the abstract class `autoanki/Dictionary.py`
 
 Some settings can be set regarding how cards will be formatted, and what will be shown. They can be seen here:
 ```
 aa.deck_settings(
 include_traditional=True,
 include_part_of_speech=True,
-word_frequency_filter=1e-05 # Float between 0 and 1. Filters using this library: https://pypi.org/project/wordfreq/
+word_frequency_filter=1e-05 # Filters using this library: https://pypi.org/project/wordfreq/
 )
 ```
+The filter is the percentage of words less frequent: 的 shows up 6% of the time in text, so putting a value of 7 will omit it
 
 ## How it works
 AutoAnki interfaces has 4 components on the back end:
-1. BookCleaner: Cleans the input coming in from files that the user supplies 
-2. DatabaseManager: Takes the cleaned input and puts it into the database
-3. Dictionary: Finds definitions for words in the database
-4. DeckManager: Creates Decks
+1. DatabaseManager: Takes the cleaned input and puts it into the database
+2. Dictionary: Finds definitions for words in the database
+3. DeckManager: Creates Decks
 
 ### Dictionary
 This is an abstract class that can be implemented with the following methods
 - `__init__(debug_level)`
 - `find_word(word)` - Returns None, or a list of paramaters that match the input of DatabaseManager.update_definition()
 - `size()` - Number of entries in the dictionary
```

### Comparing `autoanki-1.1.91/setup.cfg` & `autoanki-1.2.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = autoanki
-version = 1.1.91
+version = 1.2.0
 author = Jarvis Coghlin
 author_email = jarviscoghlin@gmail.com
 description = Automatically make Anki Decks for Chinese text
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/timmy6figures/autoanki
 project_urls = 
@@ -17,14 +17,22 @@
 [options]
 include_package_data = True
 zip_safe = False
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
+install_requires = 
+	chinese-converter>=1.1.1
+	beautifulsoup4~=4.12.2
+	genanki~=0.13.0
+	jieba~=0.42.1
+	pinyin~=0.4.0
+	requests~=2.31.0
+	wordfreq
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `autoanki-1.1.91/src/autoanki/BookCleaner/BookCleaner.py` & `autoanki-1.2.0/src/autoanki/BookCleaner/BookCleaner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,37 @@
 import logging
 import os
 
-# TODO: I think that the entire book cleaner file is not needed. 
+# TODO: I think that the entire book cleaner file is not needed.
 #   Words should not be written back to a file. This is slow
-CLEANED_FILES_DIRECTORY = 'cleaned_files'
-CLEANED_FILES_SUFFIX = '_cleaned'
+CLEANED_FILES_DIRECTORY = "cleaned_files"
+CLEANED_FILES_SUFFIX = "_cleaned"
 # Sentences That should not be added to the completed file.
-GARBAGE_SENTENCES = ['',
-                     "",
-                     ".",
-                     "。",
-                     "\n"]
+GARBAGE_SENTENCES = ["", "", ".", "。", "\n"]
 
 
 class BookCleaner:
-
     def __init__(self, debug_level, force=False):
-        """ Internal tool used to sanatize input
+        """Internal tool used to sanatize input
         Use `clean(bookpath)` to sanatize files and remove junk data
         Args:
             `force`: Ignore confirmations on if you want to clean >50 files
         """
-        self.logger = logging.getLogger('autoanki.bookcleaner')
+        self.logger = logging.getLogger("autoanki.bookcleaner")
         self.logger.setLevel(debug_level)
         self.file_list = []
         self.bookpath = ""
         self.force = force
 
     def clean(self, bookpath: str) -> None | list[str]:
         """
         Cleans the files contained in the bookpath. If bookpath is a single file, clean it.
-        Args: 
+        Args:
             `bookpath: filepath of files to be cleaned`
-        Return: 
+        Return:
             `str: list of cleaned file(s)`
         """
         if not os.path.exists(bookpath):
             self.logger.warning("Cannot find path [" + str(bookpath) + "]")
             return None
         self.logger.info("Bookpath: " + bookpath)
 
@@ -47,33 +42,37 @@
         else:
             dirty_files = []
             for root, dirs, files in os.walk(bookpath):
                 for file in files:
                     # Only clean files that are not in cleaned_files directory
                     in_cleaned = str(root).find(CLEANED_FILES_DIRECTORY) != -1
                     if not in_cleaned:
-                        if '.txt' in file:
+                        if ".txt" in file:
                             dirty_files.append(os.path.join(root, file))
 
             # Check this cleaning won't be mean to the CPU
             if len(dirty_files) > 50 and not self.force:
-                yn = input("Over 50 files. Are you sure you want to convert this many files? (Y/N)")
-                if yn.lower() != 'y':
+                yn = input(
+                    "Over 50 files. Are you sure you want to convert this many files? (Y/N)"
+                )
+                if yn.lower() != "y":
                     return None
 
         # Now we have a list of files to convert in a list
         cleaned_files = []
 
         # Create directory for files
         cleaned_files_root = os.path.join(bookpath, CLEANED_FILES_DIRECTORY)
         if not os.path.exists(cleaned_files_root):
             os.mkdir(cleaned_files_root)
 
         for file in dirty_files:
-            cleaned_filepath = self._clean_file(file, cleaned_files_root=cleaned_files_root)
+            cleaned_filepath = self._clean_file(
+                file, cleaned_files_root=cleaned_files_root
+            )
             if cleaned_filepath:
                 cleaned_files.append(cleaned_filepath)
 
         return cleaned_files
 
     def _clean_file(self, filepath: str, cleaned_files_root: str):
         """
@@ -86,34 +85,34 @@
         # TODO: This will not work for books with nested files that share the same name
         filename = os.path.basename(filepath)
         new_filepath = os.path.join(cleaned_files_root, filename)
         self.logger.debug("Filepath:     " + filepath)
         self.logger.debug("New filepath: " + new_filepath)
 
         # Clean page file of characters that may cause issues.
-        page_file = open(filepath, encoding='utf-8')
-        try: 
+        page_file = open(filepath, encoding="utf-8")
+        try:
             page_sentences = page_file.read().split("。")
         except:
             self.logger.error(f"Critical error cleaning file: [{filepath}]")
             return
-        cleaned_file = open(new_filepath, "w", encoding='utf-8')
+        cleaned_file = open(new_filepath, "w", encoding="utf-8")
 
         for page_sentence in page_sentences:
             # Clean string
-            page_sentence = page_sentence\
-                .lstrip()\
-                .rstrip()\
-                .replace("  ", " ")\
-                .lstrip("\"")\
-                .rstrip("\"")\
-                .replace("”","'")\
-                .replace("　", "")\
-                .replace("“","")\
-                .rstrip("。")\
-                .strip("'")\
+            page_sentence = (
+                page_sentence.lstrip()
+                .rstrip()
+                .replace("  ", " ")
+                .lstrip('"')
+                .rstrip('"')
+                .replace("”", "'")
+                .replace("　", "")
+                .replace("“", "")
+                .rstrip("。")
                 .strip("'")
+                .strip("'")
+            )
             if page_sentence not in GARBAGE_SENTENCES:
                 cleaned_file.write(page_sentence + "。" + "\n")
 
         return new_filepath
-
```

### Comparing `autoanki-1.1.91/src/autoanki/DatabaseManager/DatabaseManager.py` & `autoanki-1.2.0/src/autoanki/DatabaseManager/ChineseDatabaseManager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,173 +1,136 @@
 import os
-import re
 import sqlite3
 import logging
-import unicodedata
 
-from glob import glob
 from pathlib import Path
 
-from autoanki.BookCleaner.BookCleaner import CLEANED_FILES_DIRECTORY
 from autoanki.Tokenizer.ChineseTokenizer import ChineseTokenizer
+from autoanki.DatabaseManager.DatabaseManager import DatabaseManager
 
 
-class DatabaseManager:
-
-    def __init__(self, database_path, debug_level):
-        """Interfaces with an SQLLite database containing information on words, definitions, and more
-
-        """
-        self.logger = logging.getLogger('autoanki.dbmngr')
+class ChineseDatabaseManager(DatabaseManager):
+    def __init__(self, database_path, debug_level, dictionary=None):
+        """Interfaces with an SQLLite database containing information on words, definitions, and more"""
+        self.logger = logging.getLogger("autoanki.dbmngr")
         self.logger.setLevel(debug_level)
 
         # Init database
         if not os.path.exists(database_path):
             self.logger.warning("The database [", database_path, "] does not exist.")
             raise Exception("Cannot create DatabaseManager with invalid database path.")
         self.database_path = database_path
 
         # Text segmenter
-        self.tokenizer = ChineseTokenizer(debug_level)
+        self.tokenizer = ChineseTokenizer(debug_level, dictionary=dictionary)
 
         # Sql connection
         path = os.path.join(os.getcwd(), self.database_path)
         self.connection = sqlite3.connect(path)
         self.cursor = self.connection.cursor()
 
         self.books = []
 
     @staticmethod
-    def convert_to_tablename(name: str) -> str:
-        """
-        Converts a string to a sql-valid table name.
-        Args:
-            `name`: The name to convert
-        Return:
-            A valid sql table name
-        """
-        value = unicodedata.normalize('NFKC', name)
-        # value.replace("：",":")
-        value = value.replace("：", "__")
-        value = re.sub(r'[^\w\s-]', '', value.lower())
-        return re.sub(r'[-\s]+', '_', value).strip('-_')
-
-    @staticmethod
-    def is_database(database_name:str):
-        """ Verifies integrity of AutoAnki database
-        Args:
-            `database_name`: Filepath of database
-        """
-        if not database_name.endswith(".db"):
-            return False
-        if not os.path.exists(database_name):
-            return False
-        try:
-            connection = sqlite3.connect(database_name)
-            cursor = connection.cursor()
-            # This will fail if dictionary table does not exist
-            cursor.execute("SELECT word FROM dictionary")
-            connection.close()
-        except sqlite3.OperationalError:
-            return False
-        return True
-
-    @staticmethod
     def create_database(database_path: str):
-        """ Creates autoanki database file, including all tables needed
+        """Creates autoanki database file, including all tables needed
         Args:
             `database_path`: The path to the database to create
         """
-        logger = logging.getLogger('autoanki.dbmngr')
+        logger = logging.getLogger("autoanki.dbmngr")
         logger.info("Creating database [" + database_path + "]")
-        # TODO Fix this logger
-        path = os.path.join(os.path.dirname(__file__), 'databases_init.sql')
+        path = os.path.join(os.path.dirname(__file__), "databases_init.sql")
         try:
-            with open(path, 'r') as sql_file:
+            with open(path, "r") as sql_file:
                 sql_script = sql_file.read()
             connection = sqlite3.connect(database_path)
             cursor = connection.cursor()
             cursor.executescript(sql_script)
             connection.commit()
+            return True
         except FileNotFoundError:
             logger.warning("Could not create database: Missing SQL files")
             return False
 
     def _create_book_table(self, book_name, table_name) -> bool:
-        """ Creates a new entry in the book_list table
+        """Creates a new entry in the book_list table
         Args:
             `table_name`: The name of the new entry to create
         Return:
             False if error
         """
         self.cursor.execute("SELECT table_name FROM book_list")
         book_list = self.cursor.fetchall()
 
         if (table_name,) in book_list:
             self.logger.warning("The book is already in database. Not adding")
             return False
 
         # self.logger.debug("Inserting")
-        self.cursor.execute(f"INSERT INTO book_list VALUES(\"{book_name}\",\"{table_name}\",'cn')")
+        self.cursor.execute(
+            f'INSERT INTO book_list VALUES("{book_name}","{table_name}",\'cn\')'
+        )
         self.connection.commit()
-        fname = 'book_table.sql'
+        fname = "book_table.sql"
         this_file = os.path.abspath(__file__)
         this_dir = os.path.dirname(this_file)
         wanted_file = os.path.join(this_dir, fname)
-        fd = open(wanted_file, 'r')
+        fd = open(wanted_file, "r")
         book_table_file = fd.read()
         book_table_file = book_table_file.replace("BOOK_NAME", table_name)
         fd.close()
         # Create the new table
         self.cursor.execute(book_table_file)
         self.connection.commit()
         return True
 
-    def add_file_to_database(self, filepath: str, table_name: str):
-        """ Adds every word in a file to both the dictionary table and the book's table
+    def add_contents_to_database(self, contents: str, table_name: str):
+        """Adds every word in a file to both the dictionary table and the book's table
         Args:
             `filepath`: The path to the file
             `table_name`: The name of the table to add the words to.
                 This should be the same for every wile in a given book
         """
-        self.logger.info(f"Adding [{filepath}] to database...")
+        self.logger.info(f"Adding contents to database...")
         word_appearances = {}
-        with open(filepath,'r',encoding='utf-8') as f:
-            line = " "
-            while line:
-                line = f.readline().strip(" ")
-                if not line:
-                    continue
-                words = self.tokenizer.tokenize(line)
-                if not words:
-                    continue
-                for word in words:
-                    if word_appearances.get(word) == None:
-                        word_appearances[word] = 1
-                    else:
-                        word_appearances[word] += 1
+        lines = contents.splitlines()
+        for line in lines:
+            if not line:
+                continue
+            words = self.tokenizer.tokenize(line)
+            if not words:
+                continue
+            for word in words:
+                if word_appearances.get(word) == None:
+                    word_appearances[word] = 1
+                else:
+                    word_appearances[word] += 1
 
         # Add the words to the dictionary if they are not already there
         self.cursor.execute(f"SELECT word FROM dictionary")
         self.connection.commit()
         dictionary_words = self.cursor.fetchall()
-        self.logger.info(f"{len(word_appearances.items())} words in file. {len(dictionary_words)} in dictionary.")
+        self.logger.info(
+            f"{len(word_appearances.items())} words in file. {len(dictionary_words)} in dictionary."
+        )
 
         for word, appearances in word_appearances.items():
             if (word,) not in dictionary_words:
                 self.insert_word(word)
 
         # Make a dictionary of word ids from dictionary
         self.cursor.execute(f"SELECT word_id, word FROM dictionary")
         result = self.cursor.fetchall()
         word_id_dict = {}
         for line in result:
             word_id_dict[line[1]] = line[0]
 
-        self.cursor.execute(f"SELECT dictionary_word_id, number_of_appearances FROM {table_name}")
+        self.cursor.execute(
+            f"SELECT dictionary_word_id, number_of_appearances FROM {table_name}"
+        )
         self.connection.commit()
         book_table_response = self.cursor.fetchall()
         book_table_appearances = {}
         # Get the number of appearances in the book table
         for i in book_table_response:
             book_table_appearances[i[0]] = i[1]
         # pprint.pprint(book_table_appearances)
@@ -180,108 +143,125 @@
             # If the word is already in the dictionary, add the number of appearances to it
             if dictionary_word_id in book_table_appearances:
                 file_appearances = word_appearances[word]
                 db_appearances = book_table_appearances[dictionary_word_id]
                 # print("File app:", file_appearances)
                 # print("Book app:", book_table_appearances[dictionary_word_id])
                 sum = file_appearances + db_appearances
-                self.cursor.execute(f"UPDATE {table_name} SET number_of_appearances = ? "
-                                    f"WHERE dictionary_word_id = ?", [sum, dictionary_word_id])
+                self.cursor.execute(
+                    f"UPDATE {table_name} SET number_of_appearances = ? "
+                    f"WHERE dictionary_word_id = ?",
+                    [sum, dictionary_word_id],
+                )
                 self.connection.commit()
 
             else:
-                self.cursor.execute(f"INSERT INTO {table_name} (dictionary_word_id, number_of_appearances) "
-                                    f"VALUES (?,?)", [dictionary_word_id, word_appearances[word]])
+                self.cursor.execute(
+                    f"INSERT INTO {table_name} (dictionary_word_id, number_of_appearances) "
+                    f"VALUES (?,?)",
+                    [dictionary_word_id, word_appearances[word]],
+                )
                 self.connection.commit()
 
         # self.logger.debug("Done adding file to database")
 
     def insert_word(self, word):
         # TODO Doing this breaks the `number_of_appearances`. This is a temporary fix
         # TODO This is really ineficcient
-        #   Either contain an internal dict of words in the dictionary, 
+        #   Either contain an internal dict of words in the dictionary,
         #   or wrap this with a try catch
         self.cursor.execute("SELECT word FROM dictionary WHERE word = ?", [word])
         all_rows = self.cursor.fetchall()
         if len(all_rows) == 0:
             # self.logger.info("  Inserting")
             self.cursor.execute(f"INSERT INTO dictionary (word) VALUES (?)", [word])
             self.connection.commit()
 
-    def remove_word(self, word:str):
+    def remove_word(self, word: str):
         # TODO: Make more stringent constraints on removing words. This should be extremely rare
-        if '*' in word:
+        if "*" in word:
             self.logger.info(f"Not executing: [{word}]. Star in command")
             return
         self.cursor.execute(f"DELETE FROM dictionary WHERE word=(?)", [word])
         self.connection.commit()
 
-    def add_book(self, bookpath: str, book_name: str):
-        """ Adds a file to the autoanki database. 
+    def add_book_from_string(self, contents: str, book_name: str) -> bool:
+        return self._add_book(contents, book_name)
+
+    def add_book_from_file(self, filepath: str, book_name: str) -> bool:
+        if not os.path.isfile(filepath):
+            self.logger.info(f"File does not exist: [{filepath}]")
+            return False
+
+        with open(filepath, "r") as file:
+            contents = file.read()
+            return self._add_book(contents, book_name)
+
+    # def add_book_from_folder(directory):
+    # TODO This
+
+    # Legacy code from _add_book()
+    # self.logger.debug("Bookpath: " + filepath)
+    # if os.path.isdir(filepath):
+    #     self.logger.debug("Directory found:")
+    #     result = [y for x in os.walk(filepath + '/' + CLEANED_FILES_DIRECTORY) for y in glob(os.path.join(x[0], '*.txt'))]
+    #     for path in result:
+    #         self.logger.debug(path)
+    #         self.add_file_to_database(path, book_tablename)
+
+    def _add_book(self, contents: str, book_name: str) -> bool:
+        """Adds a file to the autoanki database.
         This involves the following steps:\n
         1 - Add book to the `book_list` table
         2 - Add all the files in "bookpath" to the definitions table and book table
-        3 - Add book to book_list property
-
-        If given a directory, it will recursively search for all files in the directory and add them.
-
-        if not already there, adding the
         Args:
             `bookpath`: The filepath to the book. This is file, or a directory of files
             `book_name: The name of the book. This will show up in the Anki deck
         """
         self.logger.info("Adding book...")
         # Get a 'table name' clean version of the book name
         book_tablename = self.convert_to_tablename(book_name)
-
         # Add the name of the book to the book_list table
         success = self._create_book_table(book_name, book_tablename)
         if not success:
-            self.logger.error("Failed to create book table")
-            return
-
-        self.logger.debug("Bookpath: " + bookpath)
-        if os.path.isdir(bookpath):
-            self.logger.debug("Directory found:")
-            result = [y for x in os.walk(bookpath + '/' + CLEANED_FILES_DIRECTORY) for y in glob(os.path.join(x[0], '*.txt'))]
-            for path in result:
-                self.logger.debug(path)
-                self.add_file_to_database(path, book_tablename)
-
-        elif os.path.isfile(bookpath):
-            self.logger.debug("File found:")
-            # Add all the words in the book to the `definitions` table
-            self.add_file_to_database(bookpath, book_tablename)
-
-        else:
-            self.logger.warning(f"Incorrect bookpath: [{bookpath}]")
+            self.logger.error(f"Failed to create book table: [{book_tablename}]")
             return False
 
+        # Add all the words in the book to the `definitions` table
+        self.add_contents_to_database(contents, book_tablename)
+
         self.logger.info("Done adding book.")
         return True
 
     def print_info(self):
-        """ Print basic information about the database """
+        """Print basic information about the database"""
         self.cursor.execute("SELECT word FROM dictionary")
         all_rows = self.cursor.fetchall()
         self.cursor.execute("SELECT word FROM dictionary WHERE definition IS NULL")
         unfinished_rows = self.cursor.fetchall()
         format_string_int = "{:<30} | {:>8}"
         format_string_dec = "{:<30} | {:>8.2}"
         print("------------------------")
         print(self.database_path)
         print("------------------------")
         print(format_string_int.format("Number of books:", len(self.books)))
-        print(format_string_dec.format("Database size (MB):", Path(self.database_path).stat().st_size / (1024 * 1024)))
+        print(
+            format_string_dec.format(
+                "Database size (MB):",
+                Path(self.database_path).stat().st_size / (1024 * 1024),
+            )
+        )
         print("Dictionary Table:")
         print(format_string_int.format("Number of rows:", len(all_rows)))
-        print(format_string_int.format("Number of unfinished rows:", len(unfinished_rows)))
+        print(
+            format_string_int.format("Number of unfinished rows:", len(unfinished_rows))
+        )
 
     def update_definition(self, params: list):
-        f""" Complete a definition for one word in the dictionary table\n
+        f"""Complete a definition for one word in the dictionary table\n
         traditional_script = params[0]\n
         word_type = params[1]\n
         pinyin = params[2]\n
         pinyin_numbers = params[3]\n
         sub_components = params[4]\n
         hsk_level = params[5]\n
         top_level = params[6]\n
@@ -289,26 +269,28 @@
         frequency = params[8]
         word = params[9]
         :param params: A list of params for the database:
         :return:
         """
         # TODO Some sanatization here might be a good idea
         #   Make sure junk data can't crash this function
-        self.cursor.execute("UPDATE dictionary "
-                            "SET word_traditional = ?, "
-                            "word_type = ?,"
-                            "pinyin = ?, "
-                            "pinyin_numbers = ?,"
-                            "sub_components = ?,"
-                            "hsk_level = ?,"
-                            "top_level = ?,"
-                            "definition = ?,"
-                            "frequency = ?"
-                            "WHERE word = ?",
-                            params)
+        self.cursor.execute(
+            "UPDATE dictionary "
+            "SET word_traditional = ?, "
+            "word_type = ?,"
+            "pinyin = ?, "
+            "pinyin_numbers = ?,"
+            "sub_components = ?,"
+            "hsk_level = ?,"
+            "top_level = ?,"
+            "definition = ?,"
+            "frequency = ?"
+            "WHERE word = ?",
+            params,
+        )
         self.connection.commit()
 
     def get_all_completed_definitions(self):
 
         self.cursor.execute("SELECT * FROM dictionary WHERE definition IS NOT NULL")
         raw_words = self.cursor.fetchall()
 
@@ -325,15 +307,15 @@
                 "number_of_strokes": row[6],
                 "sub_components": row[7],
                 "frequency": row[8],
                 "hsk_level": row[9],
                 "top_level": row[10],
                 "audio_path": row[11],
                 "image_path": row[12],
-                "definition": row[13]
+                "definition": row[13],
             }
             # print(word["word"])
             # pprint.pp(word)
             # words.append(word)
             words.append(word)
         # pprint.pp(words)
         return words
@@ -351,8 +333,8 @@
         return_array = []
         for table in cursor.fetchall():
             return_array.append(table[0])
         return return_array
 
     @books.setter
     def books(self, value):
-        self._books= value
+        self._books = value
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `autoanki-1.1.91/src/autoanki/DatabaseManager/databases_init.sql` & `autoanki-1.2.0/src/autoanki/DatabaseManager/databases_init.sql`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.91/src/autoanki/DeckManager/DeckManager.py` & `autoanki-1.2.0/src/autoanki/DeckManager/DeckManager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,89 +1,86 @@
 import logging
 
 import genanki
 from wordfreq import word_frequency
 
 from autoanki.DeckManager import template_decks
 
+
 class DeckManager:
     """
     The class to make anki decks. Create the file using generate_deck_file()
     One of the most important concepts is the id. No matter what deck the word is in, it should have the same id so the
     same card in different decks can be remembered.
     This class makes extensive use of genanki, so understanding how genanki works
         is pretty significant for understanding this.
     """
 
-    def __init__(self, debug_level,
-                include_traditional=True,
-                 include_part_of_speech=True
-                 ):
-        self.logger = logging.getLogger('autoanki.dckmngr')
+    def __init__(
+        self, debug_level, include_traditional=True, include_part_of_speech=True
+    ):
+        self.logger = logging.getLogger("autoanki.dckmngr")
         self.logger.setLevel(debug_level)
-        self.deck = genanki.Deck(
-            2020000110,
-            "autoankiTesting"
-        )
+        self.deck = genanki.Deck(2020000110, "autoankiTesting")
         self.include_pinyin_numbers = False
         self.include_number_of_strokes = False
-        self.include_traditional = include_traditional 
+        self.include_traditional = include_traditional
         self.include_part_of_speech = include_part_of_speech
 
         self.word_frequency_filter = None
 
         self.book_list = []
 
-    def settings(self,
-                 include_traditional,
-                 include_part_of_speech,
-                 word_frequency_filter
-                 ):
+    def settings(
+        self,
+        include_traditional,
+        include_part_of_speech,
+        word_frequency_filter,
+    ):
         """
         Configures settings for what's in the deck, and how it looks
         """
         self.include_traditional = include_traditional
-        self.include_part_of_speech = include_part_of_speech 
-        self.word_frequency_filter = word_frequency_filter 
+        self.include_part_of_speech = include_part_of_speech
+        self.word_frequency_filter = word_frequency_filter
 
     def generate_deck_file(self, words, deck_name: str, filename: str):
         """
         Generates a deck file from the database
         :param deck_name: The name of the deck to be created
         :param definitions_filename: The name of the file containing the definitions.
         :return:
         """
 
         # Number of valid cards that have been added to the deck
         num_of_valid_cards_added = 0
 
         # length = general_functions.file_len(definitions_filename)
         # self.deck.add_note()
-        self.deck = genanki.Deck(
-            2020000110,
-            deck_name
-        )
+        self.deck = genanki.Deck(2020000110, deck_name)
 
         for row in words:
 
             if self.word_frequency_filter:
-                if self.word_frequency_filter < row['frequency']:
+                if self.word_frequency_filter < row["frequency"]:
                     continue
 
             word = row["word"]
 
             if self.include_traditional:
                 word_traditional = row["word_traditional"]
             else:
                 word_traditional = ""
 
             if len(word) != len(word_traditional):
-                self.logger.error(f"{word} and {word_traditional} should be the same length")
+                self.logger.error(
+                    f"{word} and {word_traditional} should be the same length"
+                )
 
-            # Replace all matching characters with a dash 
+            # Replace all matching characters with a dash
             formatted_word_traditional = ""
             for i in range(len(word)):
                 if word[i] == word_traditional[i]:
                     formatted_word_traditional += "-"
                 else:
                     formatted_word_traditional += word_traditional[i]
 
@@ -102,36 +99,49 @@
             # word["sub_components"]
             # word["frequency"]
             # word["hsk_level"]
             # word["top_level"]]
             # word["audio_path"]
             # word["image_path"]
             # word["definition"]
+            part_of_speech = row["word_type"]
 
             if not word:
                 word = "Not found"
             if not word_traditional:
                 word_traditional = "Not found"
             if not pinyin:
                 pinyin = "Not found"
             if not definition:
                 definition = "Not found"
 
+            card_tags = ["autoanki"]
+
             note = genanki.Note(
                 model=template_decks.CHINESE_CARD_MODEL,
-                tags=['autoanki'],
-                fields=[word, formatted_word_traditional, pinyin, definition],
+                tags=card_tags,
+                fields=[
+                    word,
+                    formatted_word_traditional,
+                    pinyin,
+                    part_of_speech,
+                    definition,
+                ],
                 # sort_field can be used to sort when the cards appear.
                 # By default they are shown in the order they are addeed, so this is not currently used
                 sort_field=1,
-
             )
             self.deck.add_note(note)
             num_of_valid_cards_added += 1
 
         if not filename.endswith(".apkg"):
             filename += ".apkg"
 
         genanki.Package(self.deck).write_to_file(filename)
-        self.logger.info("Deck " + deck_name + " created with " + str(num_of_valid_cards_added) + " cards")
+        self.logger.info(
+            "Deck "
+            + deck_name
+            + " created with "
+            + str(num_of_valid_cards_added)
+            + " cards"
+        )
         return filename
-
```

### Comparing `autoanki-1.1.91/src/autoanki/Dictionary/CEDictionary.py` & `autoanki-1.2.0/src/autoanki/Dictionary/CEDictionary.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,68 @@
 from os import path
 import logging
 
 import pinyin
 import jieba
+
 logging.getLogger("jieba").setLevel(logging.WARNING)
 import jieba.posseg as pseg
 import chinese_converter
 from wordfreq import word_frequency
 
 from autoanki.Dictionary.Dictionary import Dictionary
 
-PATH_TO_FILE = path.join(path.dirname(__file__), 'cedict_ts.u8')
+PATH_TO_FILE = path.join(path.dirname(__file__), "cedict_ts.u8")
 
 # Use the lookup table here: https://github.com/fxsjy/jieba
-NOUN = ['n', 'nt', 'nrt', 'ORG', 'nr', 'PER', 'ns', 'nw', 'nz', 'f', 's', 'an', 'zg', 'j']
-TIME = ['t', 'TIME', 'tg', 'g']
-ADPOSITION = ['p']
-PRONOUN = ['r', 'rz', 'rg']
-QUANTIFIER = ['q', 'm']
-VERB = ['v', 'vd', 'vn', 'e', 'vg', 'h']
-ADVERB = ['ad', 'd', 'aq', 'df']
-OTHER = ['vn', 'xc', 'x']
-ADJECTIVE = ['a', 'b', 'ng', 'ag']
-CONJUNCTION = ['c']
-PARTICLE = ['y', 'u', 'uj', 'uz', 'ul', 'uv', 'ud', 'ug']
-PUNCTUATION = ['w']
-IDIOM = ['i', 'l']
-SUFFIX = ['k']
-OTHER = ['z', 'o', 'x']
+NOUN = [
+    "n",
+    "nt",
+    "nrt",
+    "ORG",
+    "nr",
+    "PER",
+    "ns",
+    "nw",
+    "nz",
+    "f",
+    "s",
+    "an",
+    "zg",
+    "j",
+]
+TIME = ["t", "TIME", "tg", "g"]
+ADPOSITION = ["p"]
+PRONOUN = ["r", "rz", "rg"]
+QUANTIFIER = ["q", "m"]
+VERB = ["v", "vd", "vn", "e", "vg", "h"]
+ADVERB = ["ad", "d", "aq", "df"]
+OTHER = ["vn", "xc", "x"]
+ADJECTIVE = ["a", "b", "ng", "ag"]
+CONJUNCTION = ["c"]
+PARTICLE = ["y", "u", "uj", "uz", "ul", "uv", "ud", "ug"]
+PUNCTUATION = ["w"]
+IDIOM = ["i", "l"]
+SUFFIX = ["k"]
+OTHER = ["z", "o", "x"]
 
 
 class CEDictionary(Dictionary):
-
     def __init__(self, debug_level):
         """Chinese to English Dictionary
         Parser for the CC-CEDICT Dictionary:
             https://www.mdbg.net/chinese/dictionary?page=cedict
         This is a file containing 122,839 entries
         """
-        self.logger = logging.getLogger('autoanki.cedict') 
+        self.logger = logging.getLogger("autoanki.cedict")
         self.logger.setLevel(debug_level)
         self.logger.info("Loading Chinese Dictionary (CEDictionary)")
         self.dict = self._parse_file()
         self.logger.debug("Done!")
-        
+
         pass
 
     def _parse_file(self) -> dict[str, dict]:
         """Parse dictionary file on load
         `return` A dictionary of the information, the key being the Chinese word
         """
         self.logger.debug("Parsing CE-DICT file...")
@@ -59,53 +74,58 @@
         #   this does not currently match
         definitions = {}
         last_word = "~"
         current_word = ""
 
         with open(PATH_TO_FILE, "r") as dict_file:
             for line in dict_file:
-                if line[0] == '#':
+                if line[0] == "#":
                     continue
                 parts = line.split(" ")
                 trad_word = parts[0]
                 current_word = parts[1]
 
-                definition = line[line.find("]")+2:]
+                definition = line[line.find("]") + 2 :]
 
                 if current_word != last_word:
                     # self.logger.debug(f"Creating entry: {current_word}")
                     definitions[current_word] = {
-                        'trad_word': "", 
-                        'pinyin_numbers':"", 
-                        'definition':"", 
-                        'pinyin':"",
-                        'frequency':"",
+                        "trad_word": "",
+                        "pinyin_numbers": "",
+                        "definition": "",
+                        "pinyin": "",
+                        "frequency": "",
                     }
-                
+
                 # These only need to be done the first time the word is seen
                 if last_word != current_word:
-                    definitions[current_word]['trad_word'] = trad_word
-                    definitions[current_word]['pinyin'] = pinyin.get(current_word)
-                    definitions[current_word]['pinyin_numbers'] = pinyin.get(current_word, format="numerical")
-                    definitions[current_word]['frequency'] = str(word_frequency(current_word, 'zh'))
+                    definitions[current_word]["trad_word"] = trad_word
+                    definitions[current_word]["pinyin"] = pinyin.get(current_word)
+                    definitions[current_word]["pinyin_numbers"] = pinyin.get(
+                        current_word, format="numerical"
+                    )
+                    definitions[current_word]["frequency"] = str(
+                        100 * word_frequency(current_word, "zh")
+                    )
 
-                definitions[current_word]['definition'] += '<br>' + definition 
+                definitions[current_word]["definition"] += "<br>" + definition
                 last_word = current_word
 
         for key, _ in definitions.items():
-            definitions[key]['definition'].strip('\n')
-            definitions[key]['definition'] = definitions[key]['definition'].lstrip('<br>')
-            definitions[key]['definition'] = definitions[key]['definition'].lstrip('/')
+            definitions[key]["definition"].strip("\n")
+            definitions[key]["definition"] = definitions[key]["definition"].lstrip(
+                "<br>"
+            )
+            definitions[key]["definition"] = definitions[key]["definition"].lstrip("/")
 
-            definitions[key]['definition'] = definitions[key]['definition'].rstrip('\n')
-            definitions[key]['definition'] = definitions[key]['definition'].rstrip('/')
+            definitions[key]["definition"] = definitions[key]["definition"].rstrip("\n")
+            definitions[key]["definition"] = definitions[key]["definition"].rstrip("/")
             # self.logger.info('[' + definitions[key]['definition'] + ']')
         return definitions
 
-
     def find_word(self, word: str) -> None | list[str]:
         """
         Find a word in the dictionary. This can be simplified, or traditional
         `return` Paramaters that get passed to the database
         """
         # Convert the word to simplified if needed
         word = chinese_converter.to_simplified(word)
@@ -128,28 +148,28 @@
         params = ["", "", "", "", "", "", "", "", "", ""]
 
         slice = next(pseg.cut(word))
         part_of_speech = self.get_part_of_speech(word, slice.flag)
         if part_of_speech != None:
             params[1] = part_of_speech
 
-        params[0] = self.dict[word]['trad_word'] 
-        params[2] = self.dict[word]['pinyin'] 
-        params[3] = self.dict[word]['pinyin_numbers'] 
-        params[7] = self.dict[word]['definition'] 
+        params[0] = self.dict[word]["trad_word"]
+        params[2] = self.dict[word]["pinyin"]
+        params[3] = self.dict[word]["pinyin_numbers"]
+        params[7] = self.dict[word]["definition"]
         # self.logger.debug(f"Word: {word}")
-        params[8] = self.dict[word]['frequency'] 
+        params[8] = self.dict[word]["frequency"]
         params[9] = word
         return params
 
     def size(self):
-        with open(PATH_TO_FILE,"r") as f:
-            return len(f.readlines()) 
+        with open(PATH_TO_FILE, "r") as f:
+            return len(f.readlines())
 
-    def get_part_of_speech(self, word:str, code:str) -> str:
+    def get_part_of_speech(self, word: str, code: str) -> str:
         if code in NOUN:
             return "noun"
         if code in TIME:
             return "time"
         if code in ADPOSITION:
             return "adposition"
         if code in PRONOUN:
@@ -177,10 +197,7 @@
         if code in OTHER:
             return "other"
         if code in SUFFIX:
             return "suffix"
 
         self.logger.warning(f"Part of speech code not covered: {word}:{code}")
         return "other"
-
-
-
```

### Comparing `autoanki-1.1.91/src/autoanki/Dictionary/cedict_ts.u8` & `autoanki-1.2.0/src/autoanki/Dictionary/cedict_ts.u8`

 * *Files identical despite different names*

### Comparing `autoanki-1.1.91/src/autoanki/Tokenizer/ChineseTokenizer.py` & `autoanki-1.2.0/src/autoanki/Tokenizer/ChineseTokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 import logging
 
 import jieba
+
 logging.getLogger("jieba").setLevel(logging.WARNING)
 import chinese_converter
 from string import punctuation
 
-from autoanki.Dictionary.CEDictionary import CEDictionary
 
 # TODO Is there a way to do this in a smarter way? Maybe check if the characters are in a certian UTF-8 block?
 PUNCTUATION = """
 +,;:'()[]{}&*^%$#@!◇♦•·■◎∞=™©×
 """
 CHINESE_PUNC = "！？｡。．.…、＂＃＄％＆＇（）＊＋，－／：；＜＝＞＠［＼］＾＿｀｛｜｝～｟｠｢｣､、〃《》「」『』【】〔〕〖〗〘〙〚〛〜〝〞〟〰〾〿–—‘’‛“”„‟…‧﹏  ① ② ③ ④ ⑽ "
 
 # TODO: This can be extened and implemented
 OTHER = "ｗ９ｌｉｔｂｎｅｐｈⅠ Ⅱ Ⅲ Ⅳ "
 
 # TODO Remove straight numbers and english words
 
-class ChineseTokenizer():
 
+class ChineseTokenizer:
     def __init__(self, debug_level=20, dictionary=None):
-        self.logger = logging.getLogger('autoanki.dbmngr')
+        self.logger = logging.getLogger("autoanki.dbmngr")
         self.logger.setLevel(debug_level)
 
-        # Currently, each element tokenized will be checked against the dictionary, 
+        # Currently, each element tokenized will be checked against the dictionary,
         #   and shortented if there is not a match
-        # TODO It's silly how much processing power this might use in worst-case. 
+        # TODO It's silly how much processing power this might use in worst-case.
         #   Can we improve on this?
         if dictionary:
             self.dictionary = dictionary
         else:
+            from autoanki.Dictionary.CEDictionary import CEDictionary
+
             self.dictionary = CEDictionary(debug_level=20)
 
-    def tokenize(self, line:str) -> None | list[str]:
-        
+    def tokenize(self, line: str) -> None | list[str]:
+
         # TODO jieba has more features that we should take advantage of to get better tokenizing
         dirty_words = jieba.lcut(line)
         clean_words = []
         self.logger.debug("Dirty words:")
         self.logger.debug(dirty_words)
         for word in dirty_words:
-            word = word.strip('\n')
+            word = word.strip("\n")
             if not word:
                 continue
             # Convert the word to simplified if needed
             word = chinese_converter.to_simplified(word)
             if len(word) == 1:
                 if word in PUNCTUATION:
                     continue
@@ -57,26 +59,25 @@
             # If there is a definition in the dictionary, skip any more processing
             if not word:
                 continue
             if self.dictionary.find_word(word):
                 clean_words.append(word)
                 continue
 
-
             # Try tokenizing again?
             subwords = jieba.lcut(word)
             if len(subwords) > 1:
                 for subword in subwords:
                     clean_words.append(subword)
                 continue
 
             # Remove all ascii
-            new_word = ''.join(i for i in word if ord(i)>128)
+            new_word = "".join(i for i in word if ord(i) > 128)
             # if word != new_word:
-                # self.logger.info(f"{word} -> {new_word}", )
+            # self.logger.info(f"{word} -> {new_word}", )
             word = new_word
             if not word:
                 continue
             if self.dictionary.find_word(word):
                 clean_words.append(word)
                 continue
 
@@ -147,42 +148,39 @@
                 continue
 
             clean_words.append(word)
 
         if clean_words:
             self.logger.debug("Clean words")
             self.logger.debug(clean_words)
-        return clean_words 
+        return clean_words
 
-
-    def remove_numbers(self, word:str):
+    def remove_numbers(self, word: str):
         # Remove all numbers from the front
         # Lots of the words follow the following format:
         #   Number + Subject
         CHINESE_NUMBERS = "第一二两三四五五六七八九十百千万满"
-        old_word = "" 
+        old_word = ""
         temp_word = word
         while old_word != temp_word:
-            old_word = temp_word 
+            old_word = temp_word
             if len(temp_word) == 0:
                 break
             if temp_word[0] in CHINESE_NUMBERS:
                 temp_word = temp_word[1:]
         return temp_word
 
-    def remove_modifiers(self, word:str):
-        stripped_word = word.lstrip('小')
-        stripped_word = stripped_word.lstrip('大')
-        stripped_word = stripped_word.lstrip('这')
-        stripped_word = stripped_word.lstrip('那')
-        stripped_word = stripped_word.lstrip('不')
-        stripped_word = stripped_word.lstrip('几')
-        stripped_word = stripped_word.lstrip('无')
-        stripped_word = stripped_word.lstrip('没')
-        stripped_word = stripped_word.lstrip('全')
-        stripped_word = stripped_word.lstrip('上')
-        stripped_word = stripped_word.lstrip('下')
-        stripped_word = stripped_word.lstrip('太')
-        stripped_word = stripped_word.lstrip('一个')
+    def remove_modifiers(self, word: str):
+        stripped_word = word.lstrip("小")
+        stripped_word = stripped_word.lstrip("大")
+        stripped_word = stripped_word.lstrip("这")
+        stripped_word = stripped_word.lstrip("那")
+        stripped_word = stripped_word.lstrip("不")
+        stripped_word = stripped_word.lstrip("几")
+        stripped_word = stripped_word.lstrip("无")
+        stripped_word = stripped_word.lstrip("没")
+        stripped_word = stripped_word.lstrip("全")
+        stripped_word = stripped_word.lstrip("上")
+        stripped_word = stripped_word.lstrip("下")
+        stripped_word = stripped_word.lstrip("太")
+        stripped_word = stripped_word.lstrip("一个")
         return stripped_word
-
-
```

### Comparing `autoanki-1.1.91/src/autoanki.egg-info/PKG-INFO` & `autoanki-1.2.0/src/autoanki.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,98 +1,107 @@
 Metadata-Version: 2.1
 Name: autoanki
-Version: 1.1.91
+Version: 1.2.0
 Summary: Automatically make Anki Decks for Chinese text
 Home-page: https://github.com/timmy6figures/autoanki
 Author: Jarvis Coghlin
 Author-email: jarviscoghlin@gmail.com
 Project-URL: Bug Tracker, https://github.com/timmy6figures/autoanki/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-
-> **❗️** <br>
-Pull requests welcome! If you think you can improve AA in any way, open a PR!
+Requires-Dist: chinese-converter>=1.1.1
+Requires-Dist: beautifulsoup4~=4.12.2
+Requires-Dist: genanki~=0.13.0
+Requires-Dist: jieba~=0.42.1
+Requires-Dist: pinyin~=0.4.0
+Requires-Dist: requests~=2.31.0
+Requires-Dist: wordfreq
 
 # autoanki
-Tool for generating Anki flashcards to learn Chinese.
+Tool for generating Chinese flashcards for Anki
 
-<img src="https://github.com/timmy6figures/autoanki/blob/main/media/images/example.jpg?raw=true" alt="Text to Anki" width="80%"/>
+![PyPI - Version](https://img.shields.io/pypi/v/autoanki)
+![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/timmy6figures/autoanki/python-package.yml)
 
-## Motivation
+## About
 
 When learning Chinese, some common advice is to learn the top X most common words.
 This is good advice, as you can get pretty far with this, however it's [not perfect](https://en.wikipedia.org/wiki/Zipf%27s_law#/media/File:Zipf's_law_on_War_and_Peace.png).
 
 For example, Harry Potter. This book will have normal distribution for most words, however there will be a heavy emphasis on a specialized subset of words such as Wand, Robe, Wizard, Broomstick etc. These words will show up a lot more than they would otherwise.
 
 The intention of this package was to allow Chinese learners to move from beginner books to more advanced material. I found there was a gap in knowledge going from beginner learning books (where there is little specalized terminology), to teen novels, where each novel will generally have its own specialized terminology, making the transition tedious. This is solved by automatically making Anki decks that have this specialized terminology, so that you are able to memorize these words while continuing to make progress
 
 With autoanki, you selectively add words to an Anki file to continue progressing with your lanuage learning skills.
 
 ## Usage
 
-autoanki is both a library and a command-line tool.
-
 To get started, run 
 ```pip install autoanki```
 This should install all the requirements. Then, in a Python file, do ```from autoanki import AutoAnki```
 
-To get started, first, create a database for autoanki to use 
+To get started, create an autoanki instance with the 2-letter code of the language you want to use
+```
+aa = AutoAnki('zh')
+```
+Opitonally, include a path to a database file you want to use:
 ```    
 db_path = "AutoAnki.db"
 if not AutoAnki.is_database(db_path):
     AutoAnki.create_database(db_path)
 ```
-Then create an instance of autoanki using the database
-```
-aa = AutoAnki(db_path)
-```
-Add whatever books you want in your deck. These can be a single file, or a folder
+
+Add whatever books you want in your deck. These can be a single file, or a string
 ```
 bookpath = 'short-story.txt'
-aa.add_book(bookpath, 'My first book🍎')
+aa.add_book_from_string("...", 'My first book🍎')
+aa.add_book_from_string(bookpath, 'My first book🍎')
 ```
+
 Once all of your books are added, the definitions need to be found, and then you can create a deck!
 ```
 aa.complete_unfinished_definitions()
 aa.create_deck("AutoAnki Deck", "output")
 ```
+
 This will automatically have the .apkg extension, which Anki uses. 
 Import this file into Anki, and you're all set.
 
+
 #### Other commands
-If you want to see the status of the database, use:
+If you want to see the information of a database, use:
 ```
 aa.print_database_info()
 ```
-If you would like to create and use your own dictionary, you can pass it in when you 
+
+If you would like to create and use your own dictionary, you can pass it in:
 ```
 aa = AutoAnki(db_path, dictionary=CustomDictionary())
 ```
 This dictionary must implement functions from the abstract class `autoanki/Dictionary.py`
 
 Some settings can be set regarding how cards will be formatted, and what will be shown. They can be seen here:
 ```
 aa.deck_settings(
 include_traditional=True,
 include_part_of_speech=True,
-word_frequency_filter=1e-05 # Float between 0 and 1. Filters using this library: https://pypi.org/project/wordfreq/
+word_frequency_filter=1e-05 # Filters using this library: https://pypi.org/project/wordfreq/
 )
 ```
+The filter is the percentage of words less frequent: 的 shows up 6% of the time in text, so putting a value of 7 will omit it
 
 ## How it works
 AutoAnki interfaces has 4 components on the back end:
-1. BookCleaner: Cleans the input coming in from files that the user supplies 
-2. DatabaseManager: Takes the cleaned input and puts it into the database
-3. Dictionary: Finds definitions for words in the database
-4. DeckManager: Creates Decks
+1. DatabaseManager: Takes the cleaned input and puts it into the database
+2. Dictionary: Finds definitions for words in the database
+3. DeckManager: Creates Decks
 
 ### Dictionary
 This is an abstract class that can be implemented with the following methods
 - `__init__(debug_level)`
 - `find_word(word)` - Returns None, or a list of paramaters that match the input of DatabaseManager.update_definition()
 - `size()` - Number of entries in the dictionary
```

### Comparing `autoanki-1.1.91/src/autoanki.egg-info/SOURCES.txt` & `autoanki-1.2.0/src/autoanki.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -6,26 +6,30 @@
 setup.cfg
 src/autoanki/AutoAnki.py
 src/autoanki/__init__.py
 src/autoanki.egg-info/PKG-INFO
 src/autoanki.egg-info/SOURCES.txt
 src/autoanki.egg-info/dependency_links.txt
 src/autoanki.egg-info/not-zip-safe
+src/autoanki.egg-info/requires.txt
 src/autoanki.egg-info/top_level.txt
 src/autoanki/BookCleaner/BookCleaner.py
 src/autoanki/BookCleaner/__init__.py
+src/autoanki/DatabaseManager/ChineseDatabaseManager.py
 src/autoanki/DatabaseManager/DatabaseManager.py
 src/autoanki/DatabaseManager/__init__.py
 src/autoanki/DatabaseManager/book_table.sql
 src/autoanki/DatabaseManager/book_table_view.sql
 src/autoanki/DatabaseManager/databases_init.sql
 src/autoanki/DeckManager/DeckManager.py
 src/autoanki/DeckManager/__init__.py
 src/autoanki/DeckManager/template_decks.py
+src/autoanki/Dictionary/.DS_Store
 src/autoanki/Dictionary/CEDictionary.py
 src/autoanki/Dictionary/Dictionary.py
-src/autoanki/Dictionary/YellowBridgeDictionary.py
 src/autoanki/Dictionary/__init__.py
 src/autoanki/Dictionary/cedict_ts.u8
 src/autoanki/Tokenizer/ChineseTokenizer.py
 src/autoanki/Tokenizer/Tokenizer.py
-src/autoanki/Tokenizer/__init__.py
+src/autoanki/Tokenizer/__init__.py
+tests/test_AutoAnki.py
+tests/test_DeckManager.py
```

