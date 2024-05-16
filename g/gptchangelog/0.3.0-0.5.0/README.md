# Comparing `tmp/gptchangelog-0.3.0.tar.gz` & `tmp/gptchangelog-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptchangelog-0.3.0.tar", last modified: Wed Nov 22 15:39:24 2023, max compression
+gzip compressed data, was "gptchangelog-0.5.0.tar", last modified: Thu May 16 14:10:26 2024, max compression
```

## Comparing `gptchangelog-0.3.0.tar` & `gptchangelog-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-11-22 15:39:24.366244 gptchangelog-0.3.0/
--rw-r--r--   0 xjodoin    (501) staff       (20)     1089 2023-04-13 15:28:44.000000 gptchangelog-0.3.0/LICENSE
--rw-r--r--   0 xjodoin    (501) staff       (20)     1826 2023-11-22 15:39:24.365915 gptchangelog-0.3.0/PKG-INFO
--rw-r--r--   0 xjodoin    (501) staff       (20)     1088 2023-04-13 15:56:57.000000 gptchangelog-0.3.0/README.md
-drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-11-22 15:39:24.362398 gptchangelog-0.3.0/gptchangelog/
--rw-r--r--   0 xjodoin    (501) staff       (20)     4243 2023-11-22 15:34:42.000000 gptchangelog-0.3.0/gptchangelog/__init__.py
-drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-11-22 15:39:24.365431 gptchangelog-0.3.0/gptchangelog/templates/
--rw-r--r--   0 xjodoin    (501) staff       (20)     1311 2023-11-22 15:34:42.000000 gptchangelog-0.3.0/gptchangelog/templates/changelog_prompt.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)      612 2023-11-22 15:34:42.000000 gptchangelog-0.3.0/gptchangelog/templates/version_prompt.txt
-drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2023-11-22 15:39:24.364633 gptchangelog-0.3.0/gptchangelog.egg-info/
--rw-r--r--   0 xjodoin    (501) staff       (20)     1826 2023-11-22 15:39:24.000000 gptchangelog-0.3.0/gptchangelog.egg-info/PKG-INFO
--rw-r--r--   0 xjodoin    (501) staff       (20)      355 2023-11-22 15:39:24.000000 gptchangelog-0.3.0/gptchangelog.egg-info/SOURCES.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)        1 2023-11-22 15:39:24.000000 gptchangelog-0.3.0/gptchangelog.egg-info/dependency_links.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)       51 2023-11-22 15:39:24.000000 gptchangelog-0.3.0/gptchangelog.egg-info/entry_points.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)       30 2023-11-22 15:39:24.000000 gptchangelog-0.3.0/gptchangelog.egg-info/requires.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)       13 2023-11-22 15:39:24.000000 gptchangelog-0.3.0/gptchangelog.egg-info/top_level.txt
--rw-r--r--   0 xjodoin    (501) staff       (20)       38 2023-11-22 15:39:24.366357 gptchangelog-0.3.0/setup.cfg
--rw-r--r--   0 xjodoin    (501) staff       (20)     1231 2023-11-22 15:34:42.000000 gptchangelog-0.3.0/setup.py
+drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2024-05-16 14:10:26.538080 gptchangelog-0.5.0/
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1089 2023-04-13 15:28:44.000000 gptchangelog-0.5.0/LICENSE
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1821 2024-05-16 14:10:26.537697 gptchangelog-0.5.0/PKG-INFO
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1088 2023-04-13 15:56:57.000000 gptchangelog-0.5.0/README.md
+drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2024-05-16 14:10:26.532429 gptchangelog-0.5.0/gptchangelog/
+-rw-r--r--   0 xjodoin    (501) staff       (20)     6519 2024-05-16 13:43:35.000000 gptchangelog-0.5.0/gptchangelog/__init__.py
+drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2024-05-16 14:10:26.536901 gptchangelog-0.5.0/gptchangelog/templates/
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1495 2024-05-16 13:59:38.000000 gptchangelog-0.5.0/gptchangelog/templates/changelog_prompt.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1512 2024-05-16 13:32:53.000000 gptchangelog-0.5.0/gptchangelog/templates/commits_prompt.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)      630 2024-05-16 13:37:56.000000 gptchangelog-0.5.0/gptchangelog/templates/version_prompt.txt
+drwxr-xr-x   0 xjodoin    (501) staff       (20)        0 2024-05-16 14:10:26.535006 gptchangelog-0.5.0/gptchangelog.egg-info/
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1821 2024-05-16 14:10:26.000000 gptchangelog-0.5.0/gptchangelog.egg-info/PKG-INFO
+-rw-r--r--   0 xjodoin    (501) staff       (20)      397 2024-05-16 14:10:26.000000 gptchangelog-0.5.0/gptchangelog.egg-info/SOURCES.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)        1 2024-05-16 14:10:26.000000 gptchangelog-0.5.0/gptchangelog.egg-info/dependency_links.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)       51 2024-05-16 14:10:26.000000 gptchangelog-0.5.0/gptchangelog.egg-info/entry_points.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)       30 2024-05-16 14:10:26.000000 gptchangelog-0.5.0/gptchangelog.egg-info/requires.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)       13 2024-05-16 14:10:26.000000 gptchangelog-0.5.0/gptchangelog.egg-info/top_level.txt
+-rw-r--r--   0 xjodoin    (501) staff       (20)       38 2024-05-16 14:10:26.538188 gptchangelog-0.5.0/setup.cfg
+-rw-r--r--   0 xjodoin    (501) staff       (20)     1226 2024-05-16 13:46:23.000000 gptchangelog-0.5.0/setup.py
```

### Comparing `gptchangelog-0.3.0/LICENSE` & `gptchangelog-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gptchangelog-0.3.0/PKG-INFO` & `gptchangelog-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gptchangelog
-Version: 0.3.0
-Summary: Automatically generate a changelog using GPT-3.5
+Version: 0.5.0
+Summary: Automatically generate a changelog using AI
 Home-page: https://github.com/xjodoin/gptchangelog
 Author: Xavier Jodoin
 Author-email: xavier@jodoin.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gptchangelog-0.3.0/README.md` & `gptchangelog-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `gptchangelog-0.3.0/gptchangelog/__init__.py` & `gptchangelog-0.5.0/gptchangelog/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -22,28 +22,59 @@
     with open(full_template_path, "r") as template_file:
         template_content = template_file.read()
 
     template = Template(template_content)
     return template.safe_substitute(context)
 
 
-def generate_changelog_and_next_version(commit_messages, latest_version):
+def generate_changelog_and_next_version(raw_commit_messages, latest_version):
+    prompt = render_prompt(
+        "templates/commits_prompt.txt",
+        {"commit_messages": raw_commit_messages},
+    )
+
+    response = openai.chat.completions.create(
+        model="gpt-4o",
+        messages=[
+            {
+                "role": "system",
+                "content": (
+                    "You are an expert in refining commit messages. Your task is to analyze, identify redundancies, and improve the clarity and conciseness of the provided commit messages. "
+                    "Combine similar or redundant elements to create a single cohesive message that clearly communicates all relevant changes and updates. "
+                    "Ensure the final message is concise, clear, and follows standard commit message guidelines."
+                ),
+            },
+            {
+                "role": "user",
+                "content": prompt,
+            },
+        ],
+    )
+
+    commit_messages = response.choices[0].message.content
+
+    print(f"Refactor commits: {commit_messages}")
+
     # Assuming render_prompt is a function you've defined elsewhere
     prompt = render_prompt(
         "templates/version_prompt.txt",
         {"commit_messages": commit_messages, "latest_version": latest_version},
     )
 
     # Refactored to use the updated OpenAI API
     response = openai.chat.completions.create(
-        model="gpt-3.5-turbo",
+        model="gpt-4o",
         messages=[
             {
                 "role": "system",
-                "content": "You are a helpful assistant, optimized to provide accurate and concise information.",
+                "content": (
+                    "You are an expert in software versioning. Your task is to determine the next software version number based on semantic versioning principles. "
+                    "Analyze the provided commit messages and increment the version number according to the following rules: "
+                    "MAJOR update for incompatible API changes, MINOR update for new, backwards-compatible functionality, and PATCH update for backwards-compatible bug fixes."
+                ),
             },
             {
                 "role": "user",
                 "content": prompt,
             },
         ],
     )
@@ -58,36 +89,49 @@
             "commit_messages": commit_messages,
             "next_version": next_version,
             "current_date": datetime.today().strftime("%Y-%m-%d"),
         },
     )
 
     response = openai.chat.completions.create(
-        model="gpt-3.5-turbo",
+        model="gpt-4o",
         messages=[
             {
                 "role": "system",
-                "content": "You are a helpful assistant, optimized to provide accurate and concise information.",
+                "content": (
+                    "You are an expert in creating structured and clear changelogs. Your task is to generate a concise and accurate changelog in markdown format based on the provided commit messages. "
+                    "Categorize the changes under appropriate headers such as 'Added', 'Fixed', and 'Changed'. "
+                    "Exclude any empty sections and ensure the changelog adheres to markdown syntax."
+                ),
             },
             {
                 "role": "user",
                 "content": prompt,
             },
         ],
     )
     changelog = response.choices[0].message.content
 
     return changelog
 
 
 # Function to fetch commit messages since the most recent tag
-def get_commit_messages_since_latest_tag(repo_path="."):
+def get_commit_messages_since_latest_tag(repo_path=".", min_length=10, max_length=200):
     repo = git.Repo(repo_path)
     latest_tag = repo.git.describe("--tags", "--abbrev=0")
-    commit_messages = repo.git.log(f"{latest_tag}..HEAD", pretty="%s").split("\n")
+    # Using --no-merges to exclude merge commits and iterating over the log
+    commit_messages = set()
+    for commit in repo.iter_commits(f"{latest_tag}..HEAD", no_merges=True):
+        message = commit.message.strip().split("\n")[0]  # Taking the first line of the commit message
+        # Check if message length is within the specified range
+        if min_length <= len(message) <= max_length:
+            commit_messages.add(message)
+        elif len(message) > max_length:
+            commit_messages.add(message[:max_length] + "...")  # Truncate and add ellipsis
+
     return latest_tag, "\n".join(commit_messages)
 
 
 # Function to prepend changelog to CHANGELOG.md
 def prepend_changelog_to_file(changelog, filepath="CHANGELOG.md"):
     if not os.path.exists(filepath):
         with open(filepath, "w") as file:
```

### Comparing `gptchangelog-0.3.0/gptchangelog/templates/version_prompt.txt` & `gptchangelog-0.5.0/gptchangelog/templates/version_prompt.txt`

 * *Files 26% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 Commit Messages:
 ```
 $commit_messages
 ```
 
 Rules for Incrementing:
 
-    MAJOR Update: When there are incompatible API changes.
-    MINOR Update: When new, backwards-compatible functionality is added.
-    PATCH Update: For backwards-compatible bug fixes.
+    MAJOR Update: Increment for incompatible API changes.
+    MINOR Update: Increment for new, backwards-compatible functionality.
+    PATCH Update: Increment for backwards-compatible bug fixes.
 
-Objective: Determine the next version number based on the above commit messages, adhering to semantic versioning principles.
+Objective:
 
-Output Format: Provide the next version number in the format MAJOR.MINOR.PATCH.
+Determine the next version number based on the provided commit messages, following the principles of semantic versioning.
+Output Format:
+
+Provide the next version number in the format MAJOR.MINOR.PATCH.
 
 Example Output: 1.2.3
```

### Comparing `gptchangelog-0.3.0/gptchangelog.egg-info/PKG-INFO` & `gptchangelog-0.5.0/gptchangelog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gptchangelog
-Version: 0.3.0
-Summary: Automatically generate a changelog using GPT-3.5
+Version: 0.5.0
+Summary: Automatically generate a changelog using AI
 Home-page: https://github.com/xjodoin/gptchangelog
 Author: Xavier Jodoin
 Author-email: xavier@jodoin.me
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gptchangelog-0.3.0/setup.py` & `gptchangelog-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="gptchangelog",
-    version="0.3.0",
+    version="0.5.0",
     author="Xavier Jodoin",
     author_email="xavier@jodoin.me",
-    description="Automatically generate a changelog using GPT-3.5",
+    description="Automatically generate a changelog using AI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/xjodoin/gptchangelog",
     packages=find_packages(),
     package_data={"gptchangelog": ["templates/*.txt"]},
     classifiers=[
         "Development Status :: 3 - Alpha",
```

