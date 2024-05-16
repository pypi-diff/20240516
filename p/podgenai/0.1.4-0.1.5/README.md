# Comparing `tmp/podgenai-0.1.4.tar.gz` & `tmp/podgenai-0.1.5.tar.gz`

## Comparing `podgenai-0.1.4.tar` & `podgenai-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 podgenai-0.1.4/.python-version
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 podgenai-0.1.4/requirements-dev.lock
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 podgenai-0.1.4/requirements.lock
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/__init__.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/__main__.py
--rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/config.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/exceptions.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/podgenai.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/work.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/content/audio.py
--rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/content/subtopics.py
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/content/topic.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/content/tts.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/content/voice.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/prompts/continuation_first.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/prompts/continuation_next.txt
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/prompts/generate_subtopic.txt
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/prompts/list_subtopics.txt
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/prompts/select_voice.txt
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/prompts/tts_disclaimer.txt
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/util/binascii.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/util/input.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/util/openai.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/util/semantic_text_splitter.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 podgenai-0.1.4/src/podgenai/util/sys.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 podgenai-0.1.4/.gitignore
--rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 podgenai-0.1.4/LICENSE
--rw-r--r--   0        0        0     9680 2020-02-02 00:00:00.000000 podgenai-0.1.4/README.md
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 podgenai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    10538 2020-02-02 00:00:00.000000 podgenai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 podgenai-0.1.5/.python-version
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 podgenai-0.1.5/requirements-dev.lock
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 podgenai-0.1.5/requirements.lock
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/__init__.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/__main__.py
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/config.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/exceptions.py
+-rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/podgenai.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/work.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/content/audio.py
+-rw-r--r--   0        0        0     6827 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/content/subtopics.py
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/content/topic.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/content/tts.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/content/voice.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/prompts/continuation_first.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/prompts/continuation_next.txt
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/prompts/generate_subtopic.txt
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/prompts/list_subtopics.txt
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/prompts/select_voice.txt
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/prompts/tts_disclaimer.txt
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/util/binascii.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/util/input.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/util/openai.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/util/semantic_text_splitter.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 podgenai-0.1.5/src/podgenai/util/sys.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 podgenai-0.1.5/.gitignore
+-rw-r--r--   0        0        0     7652 2020-02-02 00:00:00.000000 podgenai-0.1.5/LICENSE
+-rw-r--r--   0        0        0     9718 2020-02-02 00:00:00.000000 podgenai-0.1.5/README.md
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 podgenai-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 podgenai-0.1.5/PKG-INFO
```

### Comparing `podgenai-0.1.4/requirements-dev.lock` & `podgenai-0.1.5/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.4/requirements.lock` & `podgenai-0.1.5/requirements.lock`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.4/src/podgenai/__main__.py` & `podgenai-0.1.5/src/podgenai/__main__.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.4/src/podgenai/config.py` & `podgenai-0.1.5/src/podgenai/config.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.4/src/podgenai/podgenai.py` & `podgenai-0.1.5/src/podgenai/podgenai.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.4/src/podgenai/work.py` & `podgenai-0.1.5/src/podgenai/work.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.4/src/podgenai/content/audio.py` & `podgenai-0.1.5/src/podgenai/content/audio.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.4/src/podgenai/content/subtopics.py` & `podgenai-0.1.5/src/podgenai/content/subtopics.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     return True
 
 
 def list_subtopics(topic: str, max_attempts: int = 2) -> list[str]:
     """Return the list of subtopics for the given topic.
 
     Params:
-    * `max_attempts`: If greater than 1, and if the first attempt returns no subtopics, subsequent attempt(s) will be made. Only the first attempt tries to read from the disk cache.
+    * `max_attempts`: If greater than 1, and if the first attempt obtains no subtopics, subsequent attempt(s) will be made. Only the first attempt tries to read from the disk cache.
 
     `LanguageModelOutputError` is raised if the model output is structurally invalid.
     """
     prompt_name = "list_subtopics"
     prompt = PROMPTS[prompt_name].format(topic=topic)
     none_subtopics = ("none", "none.")
```

### Comparing `podgenai-0.1.4/src/podgenai/content/topic.py` & `podgenai-0.1.5/src/podgenai/content/topic.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.4/src/podgenai/content/tts.py` & `podgenai-0.1.5/src/podgenai/content/tts.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.4/src/podgenai/prompts/generate_subtopic.txt` & `podgenai-0.1.5/src/podgenai/prompts/generate_subtopic.txt`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.4/src/podgenai/prompts/list_subtopics.txt` & `podgenai-0.1.5/src/podgenai/prompts/list_subtopics.txt`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.4/src/podgenai/util/input.py` & `podgenai-0.1.5/src/podgenai/util/input.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.4/src/podgenai/util/openai.py` & `podgenai-0.1.5/src/podgenai/util/openai.py`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.4/.gitignore` & `podgenai-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.4/LICENSE` & `podgenai-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `podgenai-0.1.4/README.md` & `podgenai-0.1.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 * Ensure that [`rye`](https://rye-up.com/) is installed and available.
 * Clone or download this repo.
 * In the repo directory, run `rye sync` or more narrowly just `rye sync --no-lock` if on Linux.
 * If updating the repo, rerun the `rye sync` step.
 
 ### Setup via PyPI
 * Create and activate a Python 3.12 virtual environment.
-* Install via PyPI: `pip install -U podgenai`.
+* Install via [PyPI](https://pypi.org/project/podgenai/): `pip install -U podgenai`.
 
 ## Usage
 Usage can be as a command-line application or as a Python library. By default, the generated mp3 file will be written to the current working directory. As of 2024, the estimated cost per generation is under 2 USD, more specifically under 0.10 USD per subtopic. The time taken is under three minutes.
 
 ### Usage tips
 * If a requested topic fails to generate subtopics, try rewording it, perhaps to be broader or narrower or more factual. Up to two attempts are made, although the first attempt will use the disk cache if available.
 * For a potentially longer list of covered subtopics, consider appending the "(unabridged)" suffix to the requested topic, e.g. "PyTorch (unabridged)".
```

### Comparing `podgenai-0.1.4/pyproject.toml` & `podgenai-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "podgenai"
-version = "0.1.4"
+version = "0.1.5"
 description = "GPT-4 based informational audiobook/podcast mp3 generator"
 authors = [
     { name = "Ouroboros Chrysopoeia", email = "impredicative@users.noreply.github.com" }
 ]
 dependencies = [
     "fire>=0.6.0",
     "openai>=1.27.0",
@@ -44,18 +44,18 @@
 fix = { chain = ["fix-lint", "fix-fmt" ] }
 "fix-lint" = "rye lint --fix"
 "fix-fmt" = "rye fmt"
 lockup = "rye lock --update-all"
 syncup = "rye sync --update-all"
 build = "rye build --clean --verbose"
 publish = "rye publish --verbose"
-release = { chain = ["build", "publish"]}
+release = { chain = ["check", "build", "publish"]}
 
 [tool.hatch.build]
-exclude = [".env", "archive/", "scripts/", "work/"]
+exclude = [".env", "archive/", "docs/", "scripts/", "work/"]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/podgenai"]
```

### Comparing `podgenai-0.1.4/PKG-INFO` & `podgenai-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: podgenai
-Version: 0.1.4
+Version: 0.1.5
 Summary: GPT-4 based informational audiobook/podcast mp3 generator
 Project-URL: Repository, https://github.com/impredicative/podgenai
 Author-email: Ouroboros Chrysopoeia <impredicative@users.noreply.github.com>
 License-File: LICENSE
 Keywords: GPT-4,aicast,audiobook,mp3,podcast
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -61,15 +61,15 @@
 * Ensure that [`rye`](https://rye-up.com/) is installed and available.
 * Clone or download this repo.
 * In the repo directory, run `rye sync` or more narrowly just `rye sync --no-lock` if on Linux.
 * If updating the repo, rerun the `rye sync` step.
 
 ### Setup via PyPI
 * Create and activate a Python 3.12 virtual environment.
-* Install via PyPI: `pip install -U podgenai`.
+* Install via [PyPI](https://pypi.org/project/podgenai/): `pip install -U podgenai`.
 
 ## Usage
 Usage can be as a command-line application or as a Python library. By default, the generated mp3 file will be written to the current working directory. As of 2024, the estimated cost per generation is under 2 USD, more specifically under 0.10 USD per subtopic. The time taken is under three minutes.
 
 ### Usage tips
 * If a requested topic fails to generate subtopics, try rewording it, perhaps to be broader or narrower or more factual. Up to two attempts are made, although the first attempt will use the disk cache if available.
 * For a potentially longer list of covered subtopics, consider appending the "(unabridged)" suffix to the requested topic, e.g. "PyTorch (unabridged)".
```

