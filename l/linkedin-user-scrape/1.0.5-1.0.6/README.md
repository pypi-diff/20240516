# Comparing `tmp/linkedin_user_scrape-1.0.5.tar.gz` & `tmp/linkedin_user_scrape-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkedin_user_scrape-1.0.5.tar", last modified: Tue May 14 17:16:47 2024, max compression
+gzip compressed data, was "linkedin_user_scrape-1.0.6.tar", last modified: Thu May 16 12:13:05 2024, max compression
```

## Comparing `linkedin_user_scrape-1.0.5.tar` & `linkedin_user_scrape-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 17:16:47.229719 linkedin_user_scrape-1.0.5/
--rw-r--r--   0 harikabv   (501) staff       (20)     2311 2024-05-14 17:16:47.229498 linkedin_user_scrape-1.0.5/PKG-INFO
--rw-r--r--   0 harikabv   (501) staff       (20)     1802 2024-05-14 17:09:46.000000 linkedin_user_scrape-1.0.5/README.md
-drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 17:16:47.228363 linkedin_user_scrape-1.0.5/linkedin_user_scrape/
--rw-r--r--   0 harikabv   (501) staff       (20)       43 2024-05-14 11:28:41.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape/__init__.py
--rw-r--r--   0 harikabv   (501) staff       (20)     9913 2024-05-14 17:08:58.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape/scraper.py
--rw-r--r--   0 harikabv   (501) staff       (20)     3368 2024-05-14 16:36:09.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape/utils.py
-drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-14 17:16:47.229286 linkedin_user_scrape-1.0.5/linkedin_user_scrape.egg-info/
--rw-r--r--   0 harikabv   (501) staff       (20)     2311 2024-05-14 17:16:47.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape.egg-info/PKG-INFO
--rw-r--r--   0 harikabv   (501) staff       (20)      332 2024-05-14 17:16:47.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape.egg-info/SOURCES.txt
--rw-r--r--   0 harikabv   (501) staff       (20)        1 2024-05-14 17:16:47.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape.egg-info/dependency_links.txt
--rw-r--r--   0 harikabv   (501) staff       (20)       24 2024-05-14 17:16:47.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape.egg-info/requires.txt
--rw-r--r--   0 harikabv   (501) staff       (20)       21 2024-05-14 17:16:47.000000 linkedin_user_scrape-1.0.5/linkedin_user_scrape.egg-info/top_level.txt
--rw-r--r--   0 harikabv   (501) staff       (20)       38 2024-05-14 17:16:47.229774 linkedin_user_scrape-1.0.5/setup.cfg
--rw-r--r--   0 harikabv   (501) staff       (20)      844 2024-05-14 17:12:34.000000 linkedin_user_scrape-1.0.5/setup.py
+drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-16 12:13:05.227969 linkedin_user_scrape-1.0.6/
+-rw-r--r--   0 harikabv   (501) staff       (20)     2311 2024-05-16 12:13:05.227706 linkedin_user_scrape-1.0.6/PKG-INFO
+-rw-r--r--   0 harikabv   (501) staff       (20)     1802 2024-05-14 17:09:46.000000 linkedin_user_scrape-1.0.6/README.md
+drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-16 12:13:05.226570 linkedin_user_scrape-1.0.6/linkedin_user_scrape/
+-rw-r--r--   0 harikabv   (501) staff       (20)       43 2024-05-14 11:28:41.000000 linkedin_user_scrape-1.0.6/linkedin_user_scrape/__init__.py
+-rw-r--r--   0 harikabv   (501) staff       (20)     9909 2024-05-16 12:12:28.000000 linkedin_user_scrape-1.0.6/linkedin_user_scrape/scraper.py
+-rw-r--r--   0 harikabv   (501) staff       (20)     3368 2024-05-15 09:02:56.000000 linkedin_user_scrape-1.0.6/linkedin_user_scrape/utils.py
+drwxr-xr-x   0 harikabv   (501) staff       (20)        0 2024-05-16 12:13:05.227428 linkedin_user_scrape-1.0.6/linkedin_user_scrape.egg-info/
+-rw-r--r--   0 harikabv   (501) staff       (20)     2311 2024-05-16 12:13:05.000000 linkedin_user_scrape-1.0.6/linkedin_user_scrape.egg-info/PKG-INFO
+-rw-r--r--   0 harikabv   (501) staff       (20)      332 2024-05-16 12:13:05.000000 linkedin_user_scrape-1.0.6/linkedin_user_scrape.egg-info/SOURCES.txt
+-rw-r--r--   0 harikabv   (501) staff       (20)        1 2024-05-16 12:13:05.000000 linkedin_user_scrape-1.0.6/linkedin_user_scrape.egg-info/dependency_links.txt
+-rw-r--r--   0 harikabv   (501) staff       (20)       24 2024-05-16 12:13:05.000000 linkedin_user_scrape-1.0.6/linkedin_user_scrape.egg-info/requires.txt
+-rw-r--r--   0 harikabv   (501) staff       (20)       21 2024-05-16 12:13:05.000000 linkedin_user_scrape-1.0.6/linkedin_user_scrape.egg-info/top_level.txt
+-rw-r--r--   0 harikabv   (501) staff       (20)       38 2024-05-16 12:13:05.228031 linkedin_user_scrape-1.0.6/setup.cfg
+-rw-r--r--   0 harikabv   (501) staff       (20)      844 2024-05-16 12:12:50.000000 linkedin_user_scrape-1.0.6/setup.py
```

### Comparing `linkedin_user_scrape-1.0.5/PKG-INFO` & `linkedin_user_scrape-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedin_user_scrape
-Version: 1.0.5
+Version: 1.0.6
 Summary: LinkedIn scraper to parse user profiles
 Author: Harika B V
 Author-email: harikabv.dev@gmail.com
 Project-URL: Home page, https://github.com/Harika-BV/LinkedIn-User-Scraper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `linkedin_user_scrape-1.0.5/README.md` & `linkedin_user_scrape-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `linkedin_user_scrape-1.0.5/linkedin_user_scrape/scraper.py` & `linkedin_user_scrape-1.0.6/linkedin_user_scrape/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,21 +116,21 @@
 
             try:
                 job_summary = item.find('div', {'class': 'pvs-entity__sub-components'}).text.strip()
             except Exception as e:
                 job_summary = ""
 
             if(bool(match)):
-                workExperience.append([
+                workExperience.append(
                     {
                         "Title" : titleUnique,
                         "Company" : companyUnique,
                         "Duration" : duration,
                         "Summary" : job_summary
-                    }]
+                    }
                 )
             else:
                 companyCache = titleUnique
 
     return workExperience
 
 def get_education_details(driver, userId, cookie, email, password):
@@ -192,21 +192,21 @@
             except:
                 summaryDetails = ""
 
             summaryDetailsData = ""
             for data in summaryDetails:
                 summaryDetailsData = summaryDetailsData + " " + data.text.strip()
             
-            education.append([
+            education.append(
                 {
                     "Institute" : instituteDetails,
                     "Course" : courseDetails,
                     "Duration" : duration,
                     "Summary" : summaryDetailsData
-                }]
+                }
             )
     return education
 
 def get_project_details(driver, userId, cookie, email, password):
     projects = []
     return projects
```

### Comparing `linkedin_user_scrape-1.0.5/linkedin_user_scrape/utils.py` & `linkedin_user_scrape-1.0.6/linkedin_user_scrape/utils.py`

 * *Files identical despite different names*

### Comparing `linkedin_user_scrape-1.0.5/linkedin_user_scrape.egg-info/PKG-INFO` & `linkedin_user_scrape-1.0.6/linkedin_user_scrape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkedin_user_scrape
-Version: 1.0.5
+Version: 1.0.6
 Summary: LinkedIn scraper to parse user profiles
 Author: Harika B V
 Author-email: harikabv.dev@gmail.com
 Project-URL: Home page, https://github.com/Harika-BV/LinkedIn-User-Scraper
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `linkedin_user_scrape-1.0.5/setup.py` & `linkedin_user_scrape-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='linkedin_user_scrape',
-    version='1.0.5',
+    version='1.0.6',
     author='Harika B V',
     author_email='harikabv.dev@gmail.com',
     description='LinkedIn scraper to parse user profiles',
     packages=find_packages(),
     classifiers=[
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
```

