# Comparing `tmp/noveler-0.1.0.tar.gz` & `tmp/noveler-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noveler-0.1.0.tar", max compression
+gzip compressed data, was "noveler-0.1.1.tar", max compression
```

## Comparing `noveler-0.1.0.tar` & `noveler-0.1.1.tar`

### file list

```diff
@@ -1,68 +1,67 @@
--rw-r--r--   0        0        0     1073 2024-04-05 16:46:40.584169 noveler-0.1.0/LICENSE
--rw-r--r--   0        0        0     2640 2024-04-05 20:59:45.723726 noveler-0.1.0/README.md
--rw-r--r--   0        0        0       72 2024-03-27 02:28:45.063002 noveler-0.1.0/noveler/__init__.py
--rw-r--r--   0        0        0     7397 2024-04-05 21:32:21.031031 noveler-0.1.0/noveler/application.py
--rw-r--r--   0        0        0     3647 2024-04-05 19:23:44.195456 noveler-0.1.0/noveler/controllers/ActivityController.py
--rw-r--r--   0        0        0    26690 2024-04-05 19:38:01.686143 noveler-0.1.0/noveler/controllers/AssistantController.py
--rw-r--r--   0        0        0    10928 2024-04-05 19:26:56.572996 noveler-0.1.0/noveler/controllers/AuthorController.py
--rw-r--r--   0        0        0      970 2024-04-05 21:23:15.458026 noveler-0.1.0/noveler/controllers/BaseController.py
--rw-r--r--   0        0        0    13429 2024-04-05 19:27:04.015211 noveler-0.1.0/noveler/controllers/BibliographyController.py
--rw-r--r--   0        0        0    25189 2024-04-05 19:27:14.270506 noveler-0.1.0/noveler/controllers/ChapterController.py
--rw-r--r--   0        0        0    68774 2024-04-05 19:27:25.487829 noveler-0.1.0/noveler/controllers/CharacterController.py
--rw-r--r--   0        0        0    19205 2024-04-05 19:27:34.869099 noveler-0.1.0/noveler/controllers/EventController.py
--rw-r--r--   0        0        0    15052 2024-04-05 19:38:01.714144 noveler-0.1.0/noveler/controllers/ExportController.py
--rw-r--r--   0        0        0    10143 2024-04-05 19:27:51.147568 noveler-0.1.0/noveler/controllers/ImageController.py
--rw-r--r--   0        0        0     6997 2024-04-05 19:28:28.300638 noveler-0.1.0/noveler/controllers/LinkController.py
--rw-r--r--   0        0        0    22881 2024-04-05 19:28:37.059890 noveler-0.1.0/noveler/controllers/LocationController.py
--rw-r--r--   0        0        0     6513 2024-04-05 19:28:47.641195 noveler-0.1.0/noveler/controllers/NoteController.py
--rw-r--r--   0        0        0     2772 2024-04-05 19:28:57.470478 noveler-0.1.0/noveler/controllers/OllamaModelController.py
--rw-r--r--   0        0        0    21100 2024-04-05 19:29:06.568740 noveler-0.1.0/noveler/controllers/SceneController.py
--rw-r--r--   0        0        0    22172 2024-04-05 19:29:13.642943 noveler-0.1.0/noveler/controllers/StoryController.py
--rw-r--r--   0        0        0     9049 2024-04-05 19:29:20.038128 noveler-0.1.0/noveler/controllers/SubmissionController.py
--rw-r--r--   0        0        0    17329 2024-04-05 19:29:27.950355 noveler-0.1.0/noveler/controllers/UserController.py
--rw-r--r--   0        0        0     1221 2024-03-30 00:37:25.669229 noveler-0.1.0/noveler/controllers/__init__.py
--rw-r--r--   0        0        0     3297 2024-03-26 17:54:38.616466 noveler-0.1.0/noveler/models/Activity.py
--rw-r--r--   0        0        0     6354 2024-03-26 17:54:48.082733 noveler-0.1.0/noveler/models/Assistance.py
--rw-r--r--   0        0        0     4790 2024-03-26 17:54:58.737034 noveler-0.1.0/noveler/models/Author.py
--rw-r--r--   0        0        0     3316 2024-04-03 23:34:03.335534 noveler-0.1.0/noveler/models/AuthorStory.py
--rw-r--r--   0        0        0       70 2024-03-24 02:35:40.239112 noveler-0.1.0/noveler/models/Base.py
--rw-r--r--   0        0        0     7167 2024-03-26 22:58:11.040491 noveler-0.1.0/noveler/models/Bibliography.py
--rw-r--r--   0        0        0     4789 2024-03-26 17:55:27.028835 noveler-0.1.0/noveler/models/BibliographyAuthor.py
--rw-r--r--   0        0        0     6709 2024-03-30 20:19:56.562647 noveler-0.1.0/noveler/models/Chapter.py
--rw-r--r--   0        0        0     3799 2024-03-30 15:06:41.382174 noveler-0.1.0/noveler/models/ChapterLink.py
--rw-r--r--   0        0        0     3798 2024-03-30 15:06:11.516345 noveler-0.1.0/noveler/models/ChapterNote.py
--rw-r--r--   0        0        0    16242 2024-04-03 17:15:36.661748 noveler-0.1.0/noveler/models/Character.py
--rw-r--r--   0        0        0     3594 2024-04-03 17:49:52.714571 noveler-0.1.0/noveler/models/CharacterEvent.py
--rw-r--r--   0        0        0     4529 2024-04-03 04:05:10.789780 noveler-0.1.0/noveler/models/CharacterImage.py
--rw-r--r--   0        0        0     3483 2024-04-03 04:06:41.377737 noveler-0.1.0/noveler/models/CharacterLink.py
--rw-r--r--   0        0        0     3609 2024-04-03 04:05:52.527628 noveler-0.1.0/noveler/models/CharacterNote.py
--rw-r--r--   0        0        0     7615 2024-04-03 16:14:05.483259 noveler-0.1.0/noveler/models/CharacterRelationship.py
--rw-r--r--   0        0        0      649 2024-03-23 23:08:42.545496 noveler-0.1.0/noveler/models/CharacterRelationshipTypes.py
--rw-r--r--   0        0        0     3589 2024-04-03 17:54:57.531181 noveler-0.1.0/noveler/models/CharacterStory.py
--rw-r--r--   0        0        0     5186 2024-03-26 17:58:57.654914 noveler-0.1.0/noveler/models/CharacterTrait.py
--rw-r--r--   0        0        0     6088 2024-03-26 17:59:15.113426 noveler-0.1.0/noveler/models/Event.py
--rw-r--r--   0        0        0     3366 2024-03-26 17:59:36.066040 noveler-0.1.0/noveler/models/EventLink.py
--rw-r--r--   0        0        0     3492 2024-03-26 17:59:57.234663 noveler-0.1.0/noveler/models/EventLocation.py
--rw-r--r--   0        0        0     3353 2024-03-26 18:00:15.887213 noveler-0.1.0/noveler/models/EventNote.py
--rw-r--r--   0        0        0     7572 2024-03-26 18:00:34.923775 noveler-0.1.0/noveler/models/Image.py
--rw-r--r--   0        0        0     4309 2024-03-26 18:00:46.640121 noveler-0.1.0/noveler/models/ImageLocation.py
--rw-r--r--   0        0        0      403 2024-03-24 00:00:16.388632 noveler-0.1.0/noveler/models/ImageMimeTypes.py
--rw-r--r--   0        0        0     6181 2024-03-30 19:28:02.451016 noveler-0.1.0/noveler/models/Link.py
--rw-r--r--   0        0        0     3414 2024-03-24 02:51:56.610270 noveler-0.1.0/noveler/models/LinkLocation.py
--rw-r--r--   0        0        0     3366 2024-03-30 14:28:11.555374 noveler-0.1.0/noveler/models/LinkScene.py
--rw-r--r--   0        0        0     3397 2024-03-30 15:15:20.441603 noveler-0.1.0/noveler/models/LinkStory.py
--rw-r--r--   0        0        0    11003 2024-03-24 02:52:42.980518 noveler-0.1.0/noveler/models/Location.py
--rw-r--r--   0        0        0     3311 2024-03-24 02:53:02.016031 noveler-0.1.0/noveler/models/LocationNote.py
--rw-r--r--   0        0        0     6040 2024-03-30 19:27:13.713012 noveler-0.1.0/noveler/models/Note.py
--rw-r--r--   0        0        0     3366 2024-03-30 14:29:01.876861 noveler-0.1.0/noveler/models/NoteScene.py
--rw-r--r--   0        0        0     3397 2024-03-30 15:16:00.109707 noveler-0.1.0/noveler/models/NoteStory.py
--rw-r--r--   0        0        0     5647 2024-03-28 01:41:58.811177 noveler-0.1.0/noveler/models/OllamaModel.py
--rw-r--r--   0        0        0     7196 2024-03-30 20:19:45.055313 noveler-0.1.0/noveler/models/Scene.py
--rw-r--r--   0        0        0     7243 2024-03-30 20:20:13.551141 noveler-0.1.0/noveler/models/Story.py
--rw-r--r--   0        0        0     9696 2024-03-26 23:02:54.011348 noveler-0.1.0/noveler/models/Submission.py
--rw-r--r--   0        0        0      752 2024-03-24 00:39:22.749618 noveler-0.1.0/noveler/models/SubmissionResultType.py
--rw-r--r--   0        0        0     9002 2024-03-26 18:01:38.321653 noveler-0.1.0/noveler/models/User.py
--rw-r--r--   0        0        0     2059 2024-03-27 21:58:27.857198 noveler-0.1.0/noveler/models/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 19:38:44.012362 noveler-0.1.0/noveler/tmp/empty
--rw-r--r--   0        0        0      781 2024-04-05 21:39:17.546345 noveler-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3034 1970-01-01 00:00:00.000000 noveler-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-05 16:46:40.584169 noveler-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2812 2024-04-05 23:46:41.029817 noveler-0.1.1/README.md
+-rw-r--r--   0        0        0       72 2024-03-27 02:28:45.063002 noveler-0.1.1/noveler/__init__.py
+-rw-r--r--   0        0        0     7397 2024-05-16 16:29:47.881622 noveler-0.1.1/noveler/application.py
+-rw-r--r--   0        0        0     5138 2024-04-26 23:37:57.167329 noveler-0.1.1/noveler/controllers/ActivityController.py
+-rw-r--r--   0        0        0    26678 2024-04-26 23:26:37.587556 noveler-0.1.1/noveler/controllers/AssistantController.py
+-rw-r--r--   0        0        0    11098 2024-04-26 23:42:46.902640 noveler-0.1.1/noveler/controllers/AuthorController.py
+-rw-r--r--   0        0        0      984 2024-04-29 20:02:53.981822 noveler-0.1.1/noveler/controllers/BaseController.py
+-rw-r--r--   0        0        0    13579 2024-04-29 20:07:01.963452 noveler-0.1.1/noveler/controllers/BibliographyController.py
+-rw-r--r--   0        0        0    25404 2024-04-29 23:40:17.360757 noveler-0.1.1/noveler/controllers/ChapterController.py
+-rw-r--r--   0        0        0    75357 2024-04-30 18:57:39.408452 noveler-0.1.1/noveler/controllers/CharacterController.py
+-rw-r--r--   0        0        0    20297 2024-04-29 22:11:35.716251 noveler-0.1.1/noveler/controllers/EventController.py
+-rw-r--r--   0        0        0    16728 2024-04-30 18:44:07.987106 noveler-0.1.1/noveler/controllers/ExportController.py
+-rw-r--r--   0        0        0    10472 2024-04-29 22:15:45.985866 noveler-0.1.1/noveler/controllers/ImageController.py
+-rw-r--r--   0        0        0     7221 2024-04-29 23:00:47.199253 noveler-0.1.1/noveler/controllers/LinkController.py
+-rw-r--r--   0        0        0    23864 2024-04-29 23:07:38.798422 noveler-0.1.1/noveler/controllers/LocationController.py
+-rw-r--r--   0        0        0     6655 2024-04-29 23:14:13.518805 noveler-0.1.1/noveler/controllers/NoteController.py
+-rw-r--r--   0        0        0     2865 2024-04-29 23:14:38.879658 noveler-0.1.1/noveler/controllers/OllamaModelController.py
+-rw-r--r--   0        0        0    21926 2024-04-29 23:22:47.753481 noveler-0.1.1/noveler/controllers/SceneController.py
+-rw-r--r--   0        0        0    23049 2024-04-29 23:29:10.431386 noveler-0.1.1/noveler/controllers/StoryController.py
+-rw-r--r--   0        0        0     9149 2024-04-29 23:31:13.876182 noveler-0.1.1/noveler/controllers/SubmissionController.py
+-rw-r--r--   0        0        0    17444 2024-04-29 23:31:13.774179 noveler-0.1.1/noveler/controllers/UserController.py
+-rw-r--r--   0        0        0     1221 2024-03-30 00:37:25.669229 noveler-0.1.1/noveler/controllers/__init__.py
+-rw-r--r--   0        0        0     3374 2024-04-18 17:39:28.714791 noveler-0.1.1/noveler/models/Activity.py
+-rw-r--r--   0        0        0     6358 2024-05-03 01:08:29.388098 noveler-0.1.1/noveler/models/Assistance.py
+-rw-r--r--   0        0        0     4790 2024-03-26 17:54:58.737034 noveler-0.1.1/noveler/models/Author.py
+-rw-r--r--   0        0        0     3316 2024-05-05 19:32:49.704937 noveler-0.1.1/noveler/models/AuthorStory.py
+-rw-r--r--   0        0        0       70 2024-03-24 02:35:40.239112 noveler-0.1.1/noveler/models/Base.py
+-rw-r--r--   0        0        0     7430 2024-05-05 18:44:03.133809 noveler-0.1.1/noveler/models/Bibliography.py
+-rw-r--r--   0        0        0     4817 2024-05-05 19:15:35.689588 noveler-0.1.1/noveler/models/BibliographyAuthor.py
+-rw-r--r--   0        0        0     6709 2024-03-30 20:19:56.562647 noveler-0.1.1/noveler/models/Chapter.py
+-rw-r--r--   0        0        0     3799 2024-03-30 15:06:41.382174 noveler-0.1.1/noveler/models/ChapterLink.py
+-rw-r--r--   0        0        0     3798 2024-03-30 15:06:11.516345 noveler-0.1.1/noveler/models/ChapterNote.py
+-rw-r--r--   0        0        0    27269 2024-05-15 04:11:34.202461 noveler-0.1.1/noveler/models/Character.py
+-rw-r--r--   0        0        0     3594 2024-04-03 17:49:52.714571 noveler-0.1.1/noveler/models/CharacterEvent.py
+-rw-r--r--   0        0        0     4529 2024-04-03 04:05:10.789780 noveler-0.1.1/noveler/models/CharacterImage.py
+-rw-r--r--   0        0        0     3483 2024-04-03 04:06:41.377737 noveler-0.1.1/noveler/models/CharacterLink.py
+-rw-r--r--   0        0        0     3609 2024-04-03 04:05:52.527628 noveler-0.1.1/noveler/models/CharacterNote.py
+-rw-r--r--   0        0        0     7615 2024-04-03 16:14:05.483259 noveler-0.1.1/noveler/models/CharacterRelationship.py
+-rw-r--r--   0        0        0      649 2024-03-23 23:08:42.545496 noveler-0.1.1/noveler/models/CharacterRelationshipTypes.py
+-rw-r--r--   0        0        0     3589 2024-04-03 17:54:57.531181 noveler-0.1.1/noveler/models/CharacterStory.py
+-rw-r--r--   0        0        0     5186 2024-03-26 17:58:57.654914 noveler-0.1.1/noveler/models/CharacterTrait.py
+-rw-r--r--   0        0        0     6119 2024-05-15 17:30:41.019205 noveler-0.1.1/noveler/models/Event.py
+-rw-r--r--   0        0        0     3366 2024-03-26 17:59:36.066040 noveler-0.1.1/noveler/models/EventLink.py
+-rw-r--r--   0        0        0     3353 2024-03-26 18:00:15.887213 noveler-0.1.1/noveler/models/EventNote.py
+-rw-r--r--   0        0        0     7577 2024-05-15 17:34:54.008689 noveler-0.1.1/noveler/models/Image.py
+-rw-r--r--   0        0        0     4309 2024-03-26 18:00:46.640121 noveler-0.1.1/noveler/models/ImageLocation.py
+-rw-r--r--   0        0        0      403 2024-03-24 00:00:16.388632 noveler-0.1.1/noveler/models/ImageMimeTypes.py
+-rw-r--r--   0        0        0     6190 2024-05-15 17:41:06.577136 noveler-0.1.1/noveler/models/Link.py
+-rw-r--r--   0        0        0     3414 2024-03-24 02:51:56.610270 noveler-0.1.1/noveler/models/LinkLocation.py
+-rw-r--r--   0        0        0     3366 2024-03-30 14:28:11.555374 noveler-0.1.1/noveler/models/LinkScene.py
+-rw-r--r--   0        0        0     3397 2024-03-30 15:15:20.441603 noveler-0.1.1/noveler/models/LinkStory.py
+-rw-r--r--   0        0        0    11025 2024-05-15 17:44:44.416398 noveler-0.1.1/noveler/models/Location.py
+-rw-r--r--   0        0        0     3311 2024-03-24 02:53:02.016031 noveler-0.1.1/noveler/models/LocationNote.py
+-rw-r--r--   0        0        0     6026 2024-05-15 18:39:18.266390 noveler-0.1.1/noveler/models/Note.py
+-rw-r--r--   0        0        0     3366 2024-03-30 14:29:01.876861 noveler-0.1.1/noveler/models/NoteScene.py
+-rw-r--r--   0        0        0     3397 2024-03-30 15:16:00.109707 noveler-0.1.1/noveler/models/NoteStory.py
+-rw-r--r--   0        0        0     5644 2024-05-15 18:41:45.146555 noveler-0.1.1/noveler/models/OllamaModel.py
+-rw-r--r--   0        0        0     7206 2024-05-15 18:42:51.323681 noveler-0.1.1/noveler/models/Scene.py
+-rw-r--r--   0        0        0     7248 2024-05-15 18:44:18.920291 noveler-0.1.1/noveler/models/Story.py
+-rw-r--r--   0        0        0     9722 2024-05-15 18:45:30.881700 noveler-0.1.1/noveler/models/Submission.py
+-rw-r--r--   0        0        0      768 2024-05-15 18:46:35.155017 noveler-0.1.1/noveler/models/SubmissionResultType.py
+-rw-r--r--   0        0        0     9026 2024-05-15 18:47:38.667364 noveler-0.1.1/noveler/models/User.py
+-rw-r--r--   0        0        0     2059 2024-03-27 21:58:27.857198 noveler-0.1.1/noveler/models/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 19:38:44.012362 noveler-0.1.1/noveler/tmp/empty
+-rw-r--r--   0        0        0      781 2024-05-16 16:44:12.587280 noveler-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3206 1970-01-01 00:00:00.000000 noveler-0.1.1/PKG-INFO
```

### Comparing `noveler-0.1.0/LICENSE` & `noveler-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/README.md` & `noveler-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 needed.
 
 Using pip:
 From within your activated project, run `pip install noveler`.
 
 ### Usage
 Import the `Noveler` class from the `noveler` module and create a new 
-instance:
+instance. Pass in the path to the configuration file as the only argument.
 
     from noveler import Noveler
 
-    noveler = Noveler()
+    noveler = Noveler('path/to/noveler.cfg')
 
 To use a controller, pass a controller name to the noveler instance. For 
 example, to create a story do the following:
 
     story = noveler("story").create_story('title', 'description')
 
 You also create Chapter and Scene objects separately, and then append them to
@@ -54,8 +54,8 @@
 
 Noveler also exports Story and Character objects to plain text files, mainly to 
 use as input for the LLM tools. Noveler uses the Ollama ecosystem and supporting
 libraries to deliver a Retrieval-Augmented Generation session wherein the user 
 may talk to the LLM about a story and/or characters. The ability to export Events and
 Locations is not yet supported but will be in future releases.
 
-More documentation will be forthcoming.
+More documentation can be found in [this project's wiki](https://github.com/applebiter/noveler/wiki/Introduction-to-Noveler).
```

### Comparing `noveler-0.1.0/noveler/application.py` & `noveler-0.1.1/noveler/application.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,11 +195,11 @@
             )
         }
 
     def __call__(self, *args, **kwargs):
         return self._controllers[args[0]]
 
     def __str__(self):
-        return "Noveler Application [Version 0.1.0]"
+        return "Noveler Application [Version 0.1.1]"
 
     def __repr__(self):
         return f"{self.__class__.__name__}()"
```

### Comparing `noveler-0.1.0/noveler/controllers/ActivityController.py` & `noveler-0.1.1/noveler/controllers/ActivityController.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,42 @@
-from typing import Type
+from typing import Type, List
 from sqlalchemy import func
 from sqlalchemy.orm import Session
 from noveler.controllers import BaseController
 from noveler.models import User, Activity
 
 
 class ActivityController(BaseController):
     """Activity controller encapsulates activity management functionality
 
+    Attributes
+    ----------
+    _instance : ActivityController
+        The instance of the activity controller
+    _path_to_config : str
+        The path to the configuration file
+    _session : Session
+        The database session object
+    _owner : Type[User]
+        The current user of the controller
+
     Methods
     -------
     get_activity_by_id(activity_id: int)
         Get an activity by id
     get_activities()
         Get all activities associated with a user, sorted by created date with most recent first
     get_activities_page(user_id: int, page: int, per_page: int)
         Get a single page of activities associated with a user, sorted by created date with most recent first
     get_activity_count()
         Get activity count associated with a user
     search_activities(search: str)
         Search for activities by summary
+    search_activities_page(search: str, page: int, per_page: int)
+        Search for activities by summary and get a single page of activities associated with a user, sorted by created date with most recent first
     """
 
     def __init__(
             self, path_to_config: str, session: Session, owner: Type[User]
     ):
         """Initialize the class"""
 
@@ -48,30 +61,32 @@
             activity = session.query(Activity).filter(
                 Activity.id == activity_id,
                 Activity.user_id == self._owner.id
             ).first()
 
             return activity if activity else None
 
-    def get_activities(self) -> list:
+    def get_activities(self) -> List[Type[Activity]]:
         """Get all activities associated with a user, sorted by created date with most recent first
 
         Returns
         -------
         list
             A list of activity objects
         """
 
         with self._session as session:
 
             return session.query(Activity).filter(
                 Activity.user_id == self._owner.id
             ).order_by(Activity.created.desc()).all()
 
-    def get_activities_page(self, page: int, per_page: int) -> list:
+    def get_activities_page(
+        self, page: int, per_page: int
+    ) -> List[Type[Activity]]:
         """Get a single page of activities associated with a user, sorted by created date with most recent first
 
         Parameters
         ----------
         page : int
             The page number
         per_page : int
@@ -85,15 +100,17 @@
 
         with self._session as session:
 
             offset = (page - 1) * per_page
 
             return session.query(Activity).filter(
                 Activity.user_id == self._owner.id
-            ).order_by(Activity.created.desc()).offset(offset).limit(per_page).all()
+            ).order_by(
+                Activity.created.desc()
+            ).offset(offset).limit(per_page).all()
 
     def get_activity_count(self) -> int:
         """Get activity count associated with a user
 
         Returns
         -------
         int
@@ -102,15 +119,15 @@
 
         with self._session as session:
 
             return session.query(func.count(Activity.id)).filter(
                 Activity.user_id == self._owner.id
             ).scalar()
 
-    def search_activities(self, search: str) -> list:
+    def search_activities(self, search: str) -> List[Type[Activity]]:
         """Search for activities by summary
 
         Parameters
         ----------
         search : str
             The search string
 
@@ -123,7 +140,37 @@
         with self._session as session:
 
             return session.query(Activity).filter(
                 Activity.summary.like(f'%{search}%'),
                 Activity.user_id == self._owner.id
             ).all()
 
+    def search_activities_page(
+        self, search: str, page: int, per_page: int
+    ) -> List[Type[Activity]]:
+        """Search for activities by summary and get a single page of activities associated with a user
+
+        Parameters
+        ----------
+        search : str
+            The search string
+        page : int
+            The page number
+        per_page : int
+            The number of rows per page
+
+        Returns
+        -------
+        list
+            A list of activity objects
+        """
+
+        with self._session as session:
+
+            offset = (page - 1) * per_page
+
+            return session.query(Activity).filter(
+                Activity.summary.like(f'%{search}%'),
+                Activity.user_id == self._owner.id
+            ).order_by(
+                Activity.created.desc()
+            ).offset(offset).limit(per_page).all()
```

### Comparing `noveler-0.1.0/noveler/controllers/AssistantController.py` & `noveler-0.1.1/noveler/controllers/AssistantController.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import base64
 import os
 import shutil
 import uuid
 from configparser import ConfigParser
 from datetime import datetime
 from typing import Type, Optional, Union, List, Literal, Mapping, Any
-
 from langchain_community.document_loaders.directory import DirectoryLoader
 from langchain_community.document_loaders.text import TextLoader
 from langchain_community.embeddings.ollama import OllamaEmbeddings
 from langchain_community.vectorstores.chroma import Chroma
 from langchain_text_splitters import RecursiveCharacterTextSplitter
 from ollama import Client, Message
 from sqlalchemy.orm import Session
@@ -323,15 +322,15 @@
             else:
                 session.commit()
                 return response
 
     def rag_chat(
         self,
         prompt: str,
-        documents: List[str],  #
+        documents: List[str],
         temperature: Optional[float] = 0.5,
         seed: Optional[int] = None,
         priming: str = None,
         options: Optional[dict] = None,
         session_uuid: str = None,
         keep_alive: Optional[Union[float, str]] = None
     ):
@@ -689,12 +688,12 @@
 
     def show_model(self, model: str) -> Mapping[str, Any]:
         """Show the details of a specific model."""
         return self._client.show(model)
 
     def __str__(self):
         """Return the class string representation."""
-        return f"Noveler Application [alpha] Assistant Controller"
+        return f"Noveler Application Assistant Controller"
 
     def __repr__(self):
         """Return the class representation."""
         return f"{self.__class__.__name__}()"
```

### Comparing `noveler-0.1.0/noveler/controllers/AuthorController.py` & `noveler-0.1.1/noveler/controllers/AuthorController.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from datetime import datetime
-from typing import Type
+from typing import Type, List
 from sqlalchemy import func
 from sqlalchemy.orm import Session
 from noveler.controllers.BaseController import BaseController
 from noveler.models import User, Author, Activity, Story
 
 
 class AuthorController(BaseController):
     """Author controller encapsulates author management functionality
 
     Attributes
     ----------
-    _self : AuthorController
+    _instance : AuthorController
         The instance of the author controller
-    _owner : User
-        The current user of the author controller
+    _path_to_config : str
+        The path to the configuration file
     _session : Session
-        The database session
+        The database session object
+    _owner : User
+        The current user of the controller
 
     Methods
     -------
     create_author(name: str, initials: str, is_pseudonym: bool)
         Create a new author
     update_author(author_id: int, name: str, initials: str)
         Update an author
@@ -315,15 +317,15 @@
 
         with self._session as session:
 
             return session.query(func.count(Author.id)).filter(
                 Author.user_id == self._owner.id
             ).scalar()
 
-    def get_all_authors(self) -> list:
+    def get_all_authors(self) -> List[Type[Author]]:
         """Get all authors associated with a user
 
         Returns
         -------
         list
             A list of author objects
         """
@@ -354,38 +356,40 @@
 
             offset = (page - 1) * per_page
 
             return session.query(Author).filter(
                 Author.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def get_authors_by_story_id(self, story_id: int) -> list:
+    def get_authors_by_story_id(
+        self, story_id: int
+    ) -> List[Type[Author]] | None:
         """Get all authors associated with a story
 
         Parameters
         ----------
         story_id : int
             The id of the story
 
         Returns
         -------
-        list
-            A list of author objects
+        list | None
+            A list of author objects or None if not found
         """
 
         with self._session as session:
 
             story = session.query(Story).filter(
                 Story.id == story_id,
                 Story.user_id == self._owner.id
             ).first()
 
             return story.authors if story else None
 
-    def search_authors(self, search: str) -> list:
+    def search_authors(self, search: str) -> List[Type[Author]]:
         """Search for authors by name
 
         Parameters
         ----------
         search : str
             The search string
```

### Comparing `noveler-0.1.0/noveler/controllers/BaseController.py` & `noveler-0.1.1/noveler/controllers/BaseController.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,13 +24,15 @@
         """Enforce Singleton pattern"""
 
         if cls._instance is None:
             cls._instance = super().__new__(cls)
 
         return cls._instance
 
-    def __init__(self, path_to_config: str, session: Session, owner: Type[User]):
+    def __init__(
+        self, path_to_config: str, session: Session, owner: Type[User]
+    ):
         """Initialize the class"""
 
         self._path_to_config = path_to_config
         self._session = session
         self._owner = owner
```

### Comparing `noveler-0.1.0/noveler/controllers/BibliographyController.py` & `noveler-0.1.1/noveler/controllers/BibliographyController.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from datetime import datetime
-from typing import Type
+from typing import Type, List
 from sqlalchemy import func
 from sqlalchemy.orm import Session
 from noveler.controllers.BaseController import BaseController
 from noveler.models import User, Bibliography, Activity
 
 
 class BibliographyController(BaseController):
     """Bibliography controller encapsulates bibliography management functionality
 
     Attributes
     ----------
-    _self : BibliographyController
+    _instance : BibliographyController
         The instance of the bibliography controller
     _owner : User
         The current user of the bibliography controller
     _session : Session
         The database session
 
     Methods
@@ -232,15 +232,15 @@
                 raise e
 
             else:
                 session.commit()
                 return True
 
     def get_bibliography_by_id(
-            self, bibliography_id: int
+        self, bibliography_id: int
     ) -> Type[Bibliography] | None:
         """Get a bibliography by id
 
         Parameters
         ----------
         bibliography_id : int
             The id of the bibliography to get
@@ -257,15 +257,15 @@
                 Bibliography.id == bibliography_id,
                 Bibliography.user_id == self._owner.id
             ).first()
 
             return bibliography if bibliography else None
 
     def get_bibliography_by_title(
-            self, title: str
+        self, title: str
     ) -> Type[Bibliography] | None:
         """Get a bibliography by title
 
         Parameters
         ----------
         title : str
             The title of the referenced work
@@ -296,30 +296,32 @@
 
         with self._session as session:
 
             return session.query(func.count(Bibliography.id)).filter(
                 Bibliography.user_id == self._owner.id
             ).scalar()
 
-    def get_all_bibliographies(self) -> list:
+    def get_all_bibliographies(self) -> List[Type[Bibliography]]:
         """Get all bibliographies associated with a user
 
         Returns
         -------
         list
             A list of bibliography objects
         """
 
         with self._session as session:
 
             return session.query(Bibliography).filter(
                 Bibliography.user_id == self._owner.id
             ).all()
 
-    def get_bibliographies_page(self, page: int, per_page: int) -> list:
+    def get_bibliographies_page(
+        self, page: int, per_page: int
+    ) -> List[Type[Bibliography]]:
         """Get a single page of bibliographies from the database associated with a user
 
         Parameters
         ----------
         page : int
             The page number
         per_page : int
@@ -335,15 +337,17 @@
 
             offset = (page - 1) * per_page
 
             return session.query(Bibliography).filter(
                 Bibliography.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def get_bibliographies_by_story_id(self, story_id: int) -> list:
+    def get_bibliographies_by_story_id(
+        self, story_id: int
+    ) -> List[Type[Bibliography]]:
         """Get all bibliographies associated with a story
 
         Parameters
         ----------
         story_id : int
             The id of the story
 
@@ -360,15 +364,15 @@
                 Bibliography.user_id == self._owner.id
             ).all()
 
             return bibliographies if bibliographies else None
 
     def get_bibliographies_page_by_story_id(
         self, story_id: int, page: int, per_page: int
-    ) -> list:
+    ) -> List[Type[Bibliography]]:
         """Get a single page of bibliographies associated with a story from the database
 
         Parameters
         ----------
         story_id : int
             The id of the story
         page : int
@@ -389,15 +393,15 @@
             bibliographies = session.query(Bibliography).filter(
                 Bibliography.story_id == story_id,
                 Bibliography.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
             return bibliographies if bibliographies else None
 
-    def search_bibliographies(self, search: str) -> list:
+    def search_bibliographies(self, search: str) -> List[Type[Bibliography]]:
         """Search for bibliographies by title associated with a user
 
         Parameters
         ----------
         search : str
             The search string
 
@@ -412,15 +416,15 @@
             return session.query(Bibliography).filter(
                 Bibliography.title.like(f'%{search}%'),
                 Bibliography.user_id == self._owner.id
             ).all()
 
     def search_bibliographies_by_story_id(
         self, story_id: int, search: str
-    ) -> list:
+    ) -> List[Type[Bibliography]]:
         """Search for bibliographies by title associated with a story
 
         Parameters
         ----------
         story_id : int
             The id of the story
         search : str
```

### Comparing `noveler-0.1.0/noveler/controllers/ChapterController.py` & `noveler-0.1.1/noveler/controllers/ChapterController.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 from configparser import ConfigParser
 from datetime import datetime
-from typing import Type
+from typing import Type, List
 from sqlalchemy import func, or_
 from sqlalchemy.orm import Session
 from noveler.controllers import BaseController
 from noveler.models import User, Chapter, Activity, Scene, Link, ChapterLink, Note, ChapterNote
 
 
 class ChapterController(BaseController):
     """Chapter controller encapsulates chapter management functionality
 
     Attributes
     ----------
-    _self : ChapterController
+    _instance : ChapterController
         The instance of the chapter controller
     _owner : User
         The current user of the chapter controller
 
     Methods
     -------
     create_chapter(story_id: int, title: str, description: str)
@@ -57,15 +57,15 @@
     append_notes_to_chapter(chapter_id: int, notes: list)
         Append notes to a chapter
     get_notes_by_chapter_id(chapter_id: int)
         Get all notes associated with a chapter
     """
 
     def __init__(
-            self, path_to_config: str, session: Session, owner: Type[User]
+        self, path_to_config: str, session: Session, owner: Type[User]
     ):
         """Initialize the class"""
 
         super().__init__(path_to_config, session, owner)
 
     def create_chapter(
         self, story_id: int, title: str, description: str = None
@@ -385,15 +385,15 @@
             chapter = session.query(Chapter).filter(
                 Chapter.id == chapter_id,
                 Chapter.user_id == self._owner.id
             ).first()
 
             return chapter if chapter else None
 
-    def get_all_chapters(self) -> list | None:
+    def get_all_chapters(self) -> List[Type[Chapter]]:
         """Get all chapters associated with a user
 
         Chapters are sorted by story id and position.
 
         Returns
         -------
         list | None
@@ -402,15 +402,17 @@
 
         with self._session as session:
 
             return session.query(Chapter).filter(
                 Chapter.user_id == self._owner.id
             ).order_by(Chapter.story_id, Chapter.position).all()
 
-    def get_all_chapters_page(self, page: int, per_page: int) -> list | None:
+    def get_all_chapters_page(
+        self, page: int, per_page: int
+    ) -> List[Type[Chapter]]:
         """Get a single page of chapters from the database associated with a user
 
         Chapters are sorted by story id and position.
 
         Parameters
         ----------
         page : int
@@ -430,15 +432,15 @@
 
             return session.query(Chapter).filter(
                 Chapter.user_id == self._owner.id
             ).order_by(
                 Chapter.story_id, Chapter.position
             ).offset(offset).limit(per_page).all()
 
-    def get_chapters_by_story_id(self, story_id: int) -> list | None:
+    def get_chapters_by_story_id(self, story_id: int) -> List[Type[Chapter]]:
         """Get all chapters associated with a story
 
         The returned list will be sorted by the position.
 
         Parameters
         ----------
         story_id : int
@@ -455,15 +457,15 @@
             return session.query(Chapter).filter(
                 Chapter.story_id == story_id,
                 Chapter.user_id == self._owner.id
             ).order_by(Chapter.position).all()
 
     def get_chapters_page_by_story_id(
         self, story_id: int, page: int, per_page: int
-    ) -> list | None:
+    ) -> List[Type[Chapter]] | None:
         """Get a single page of chapters associated with a story from the database
 
         The returned list will be sorted by the position.
 
         Parameters
         ----------
         story_id : int
@@ -507,15 +509,15 @@
         with self._session as session:
 
             return session.query(func.count(Chapter.id)).filter(
                 Chapter.story_id == story_id,
                 Chapter.user_id == self._owner.id
             ).scalar()
 
-    def search_chapters(self, search: str) -> list:
+    def search_chapters(self, search: str) -> List[Type[Chapter]]:
         """Search for chapters by title and description belonging to a specific user
 
         Parameters
         ----------
         search : str
             The search string
 
@@ -524,20 +526,24 @@
         list
             A list of chapter objects
         """
 
         with self._session as session:
 
             return session.query(Chapter).filter(
-                or_(Chapter.title.like(f'%{search}%'),
-                Chapter.description.like(f'%{search}%')),
+                or_(
+                    Chapter.title.like(f'%{search}%'),
+                    Chapter.description.like(f'%{search}%')
+                ),
                 Chapter.user_id == self._owner.id
             ).all()
 
-    def search_chapters_by_story_id(self, story_id: int, search: str) -> list:
+    def search_chapters_by_story_id(
+        self, story_id: int, search: str
+    ) -> List[Type[Chapter]]:
         """Search for chapters by title and description belonging to a specific story
 
         Parameters
         ----------
         story_id : int
             The id of the story
         search : str
@@ -548,16 +554,18 @@
         list
             A list of chapter objects
         """
 
         with self._session as session:
 
             return session.query(Chapter).filter(
-                or_(Chapter.title.like(f'%{search}%'),
-                Chapter.description.like(f'%{search}%')),
+                or_(
+                    Chapter.title.like(f'%{search}%'),
+                    Chapter.description.like(f'%{search}%')
+                ),
                 Chapter.story_id == story_id,
                 Chapter.user_id == self._owner.id
             ).all()
 
     def has_scenes(self, chapter_id: int) -> bool:
         """Check if a chapter has scenes
 
@@ -575,15 +583,17 @@
         with self._session as session:
 
             return session.query(Scene).filter(
                 Scene.chapter_id == chapter_id,
                 Scene.user_id == self._owner.id
             ).count() > 0
 
-    def get_scene_by_position(self, chapter_id: int, position: int) -> Type[Scene] | None:
+    def get_scene_by_position(
+        self, chapter_id: int, position: int
+    ) -> Type[Scene] | None:
         """Get a scene by position
 
         Parameters
         ----------
         chapter_id : int
             The id of the chapter
         position : int
@@ -601,15 +611,17 @@
                 Scene.chapter_id == chapter_id,
                 Scene.position == position,
                 Scene.user_id == self._owner.id
             ).first()
 
             return scene if scene else None
 
-    def get_all_scenes_by_chapter_id(self, chapter_id: int) -> list[Type[Scene]]:
+    def get_all_scenes_by_chapter_id(
+        self, chapter_id: int
+    ) -> List[Type[Scene]]:
         """Get all scenes associated with a chapter
 
         Parameters
         ----------
         chapter_id : int
             The id of the chapter
 
@@ -682,15 +694,15 @@
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return chapter
 
-    def get_links_by_chapter_id(self, chapter_id: int) -> list[Type[Link]]:
+    def get_links_by_chapter_id(self, chapter_id: int) -> List[Type[Link]]:
         """Get all links associated with a chapter
 
         Parameters
         ----------
         chapter_id : int
             The id of the chapter
 
@@ -768,15 +780,15 @@
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return chapter
 
-    def get_notes_by_chapter_id(self, chapter_id: int) -> list[Type[Note]]:
+    def get_notes_by_chapter_id(self, chapter_id: int) -> List[Type[Note]]:
         """Get all notes associated with a chapter
 
         Parameters
         ----------
         chapter_id : int
             The id of the chapter
```

### Comparing `noveler-0.1.0/noveler/controllers/CharacterController.py` & `noveler-0.1.1/noveler/controllers/CharacterController.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 from datetime import datetime
-from typing import Type
+from typing import Type, List
 from sqlalchemy import func, or_
 from sqlalchemy.orm import Session
 from noveler.controllers.BaseController import BaseController
 from noveler.models import User, Character, CharacterStory, Activity, CharacterRelationship, CharacterTrait, Event, \
     CharacterEvent, Link, CharacterLink, Note, CharacterNote, Image, CharacterImage
 from configparser import ConfigParser
 
 
 class CharacterController(BaseController):
     """Character controller encapsulates characters management functionality
 
     Attributes
     ----------
-    _self : CharacterController
+    _instance : CharacterController
         The instance of the characters controller
     _owner : User
         The current user of the characters controller
     _session : Session
         The database session
 
     Methods
     -------
-    create_character(title: str, first_name: str, middle_name: str, last_name: str, nickname: str, gender: str, \
-                     sex: str, description: str, date_of_birth: str, date_of_death: str)
+    create_character(title: str, first_name: str, middle_name: str, last_name: str, honorific: str, nickname: str, \
+                     gender: str, sex: str, ethnicity: str, race: str, tribe_or_clan: str, nationality: str, \
+                     date_of_birth: str, date_of_death: str, description: str, mbti: str, enneagram: str, wounds: str)
         Create a new character
-    update_character(character_id: int, title: str, first_name: str, middle_name: str, last_name: str, nickname: str, \
-                     gender: str, sex: str, description: str, date_of_birth: str, date_of_death: str)
+    update_character(character_id: int, title: str, first_name: str, middle_name: str, last_name: str, honorific: str, \
+                     nickname: str, gender: str, sex: str, ethnicity: str, race: str, tribe_or_clan: str, \
+                     nationality: str, date_of_birth: str, date_of_death: str, description: str, mbti: str, \
+                     enneagram: str, wounds: str)
         Update a character
     delete_character(character_id: int)
         Delete a character
     get_character_by_id(character_id: int)
         Get a character by id
     get_character_count()
         Get character count associated with a user
@@ -111,53 +114,84 @@
     get_images_by_character_id(character_id: int)
         Get all images associated with a character
     get_images_page_by_character_id(character_id: int, page: int, per_page: int)
         Get a single page of images associated with a character from the database
     """
 
     def __init__(
-            self, path_to_config: str, session: Session, owner: Type[User]
+        self, path_to_config: str, session: Session, owner: Type[User]
     ):
         """Initialize the class"""
 
         super().__init__(path_to_config, session, owner)
 
     def create_character(
-            self, title: str = None, first_name: str = None,
-            middle_name: str = None, last_name: str = None, nickname: str = None,
-            gender: str = None, sex: str = None, date_of_birth: str = None,
-            date_of_death: str = None, description: str = None
+        self, title: str = None, honorific: str = None, first_name: str = None,
+        middle_name: str = None, last_name: str = None, nickname: str = None,
+        gender: str = None, sex: str = None, ethnicity: str = None,
+        race: str = None, tribe_or_clan: str = None, nationality: str = None,
+        religion: str = None, occupation: str = None, education: str = None,
+        marital_status: str = None, children: bool = None,
+        date_of_birth: str = None, date_of_death: str = None,
+        description: str = None, mbti: str = None, enneagram: str = None,
+        wounds: str = None
     ) -> Character:
         """Create a new character
 
         Although all the attributes are technically optional, at least one of the following fields must be provided:
         title, first name, middle name, last name, or nickname.
 
         Parameters
         ----------
         title : str
             The title of the character, optional
+        honorific : str
+            The honorific of the character, optional
         first_name : str
             The first name of the character, optional
         middle_name : str
             The middle name of the character, optional
         last_name : str
             The last name of the character, optional
         nickname : str
             The nickname of the character, optional
         gender: str
             The gender of the character, optional
         sex: str
             The sex of the character, optional
+        ethnicity: str
+            The ethnicity of the character, optional
+        race: str
+            The race of the character, optional
+        tribe_or_clan: str
+            The tribe or clan of the character, optional
+        nationality: str
+            The nationality of the character, optional
+        religion: str
+            The religion of the character, optional
+        occupation: str
+            The occupation of the character, optional
+        education: str
+            The education of the character, optional
+        marital_status: str
+            The marital status of the character, optional
+        children: bool
+            Whether the character has children, optional
         date_of_birth: str
             The date of birth of the character, optional
         date_of_death: str
             The date of death of the character, optional
         description
             The description of the character, optional
+        mbti: str
+            The Myers-Briggs Type Indicator of the character, optional
+        enneagram: str
+            The Enneagram type of the character, optional
+        wounds: str
+            The wounds of the character, optional
 
         Returns
         -------
         Character
             The new character object
         """
 
@@ -171,17 +205,23 @@
                     nickname.""")
 
                 created = datetime.now()
                 modified = created
                 character = Character(
                     user_id=self._owner.id, title=title, first_name=first_name,
                     middle_name=middle_name, last_name=last_name,
-                    nickname=nickname, gender=gender, sex=sex,
-                    date_of_birth=date_of_birth, date_of_death=date_of_death,
-                    description=description, created=created, modified=modified
+                    honorific=honorific, nickname=nickname, gender=gender,
+                    sex=sex, ethnicity=ethnicity, race=race,
+                    tribe_or_clan=tribe_or_clan, nationality=nationality,
+                    religion=religion, occupation=occupation,
+                    education=education, marital_status=marital_status,
+                    children=children, date_of_birth=date_of_birth,
+                    date_of_death=date_of_death, description=description,
+                    mbti=mbti, enneagram=enneagram, wounds=wounds,
+                    created=created, modified=modified
                 )
 
                 activity = Activity(
                     user_id=self._owner.id, summary=f'{character.__str__} \
                     created by {self._owner.username}', created=datetime.now()
                 )
 
@@ -193,46 +233,76 @@
                 raise e
 
             else:
                 session.commit()
                 return character
 
     def update_character(
-            self, character_id: int = None, title: str = None,
-            first_name: str = None, middle_name: str = None, last_name: str = None,
-            nickname: str = None, gender: str = None, sex: str = None,
-            date_of_birth: str = None, date_of_death: str = None,
-            description: str = None
+        self, character_id: int = None, title: str = None, honorific: str = None,
+        first_name: str = None, middle_name: str = None, last_name: str = None,
+        nickname: str = None, gender: str = None, sex: str = None,
+        ethnicity: str = None, race: str = None, tribe_or_clan: str = None,
+        nationality: str = None, religion: str = None, occupation: str = None,
+        education: str = None, marital_status: str = None, children: bool = None,
+        date_of_birth: str = None, date_of_death: str = None,
+        description: str = None, mbti: str = None, enneagram: str = None,
+        wounds: str = None
     ) -> Type[Character]:
         """Update a character
 
         Parameters
         ----------
         character_id : int
             The id of the character to update
         title : str
             The title of the character
+        honorific : str
+            The honorific of the character
         first_name : str
             The first name of the character
         middle_name : str
             The middle name of the character
         last_name : str
             The last name of the character
         nickname : str
             The nickname of the character
         gender : str
             The gender of the character
         sex : str
             The sex of the character
+        ethnicity : str
+            The ethnicity of the character
+        race : str
+            The race of the character
+        tribe_or_clan : str
+            The tribe or clan of the character
+        nationality : str
+            The nationality of the character
+        religion : str
+            The religion of the character
+        occupation : str
+            The occupation of the character
+        education : str
+            The education of the character
+        marital_status : str
+            The marital status of the character
+        children : bool
+            Whether the character has children
         date_of_birth : str
             The date of birth of the character
         date_of_death : str
             The date of death of the character
         description : str
             The description of the character
+        mbti : str
+            The Myers-Briggs Type Indicator of the character
+        enneagram : str
+            The Enneagram type of the character
+        wounds : str
+            The wounds of the character
 
         Returns
         -------
         Character
             The updated character object
         """
 
@@ -245,23 +315,36 @@
                     Character.user_id == self._owner.id
                 ).first()
 
                 if not character:
                     raise ValueError('Character not found.')
 
                 character.title = title
+                character.honorific = honorific
                 character.first_name = first_name
                 character.middle_name = middle_name
                 character.last_name = last_name
                 character.nickname = nickname
                 character.gender = gender
                 character.sex = sex
+                character.ethnicity = ethnicity
+                character.race = race
+                character.tribe_or_clan = tribe_or_clan
+                character.nationality = nationality
+                character.religion = religion
+                character.occupation = occupation
+                character.education = education
+                character.marital_status = marital_status
+                character.children = children
                 character.date_of_birth = date_of_birth
                 character.date_of_death = date_of_death
                 character.description = description
+                character.mbti = mbti
+                character.enneagram = enneagram
+                character.wounds = wounds
                 character.modified = datetime.now()
 
                 activity = Activity(
                     user_id=self._owner.id, summary=f'{character.__str__} \
                     updated by {self._owner.username}', created=datetime.now()
                 )
 
@@ -336,15 +419,16 @@
         -------
         Type[Character] | None
             The character if found, otherwise None
         """
 
         with self._session as session:
             character = session.query(Character).filter(
-                Character.id == character_id, Character.user_id == self._owner.id
+                Character.id == character_id,
+                Character.user_id == self._owner.id
             ).first()
             return character if character else None
 
     def get_character_count(self) -> int:
         """Get character count associated with a user
 
         Returns
@@ -354,29 +438,31 @@
         """
 
         with self._session as session:
             return session.query(func.count(Character.id)).filter(
                 Character.user_id == self._owner.id
             ).scalar()
 
-    def get_all_characters(self) -> list:
+    def get_all_characters(self) -> List[Type[Character]]:
         """Get all characters associated with a user
 
         Returns
         -------
         list
             The list of characters associated with the user
         """
 
         with self._session as session:
             return session.query(Character).filter(
                 Character.user_id == self._owner.id
             ).all()
 
-    def get_all_characters_page(self, page: int, per_page: int) -> list:
+    def get_all_characters_page(
+        self, page: int, per_page: int
+    ) -> List[Type[Character]]:
         """Get a single page of characters from the database associated with a user
 
         Parameters
         ----------
         page : int
             The page number
         per_page : int
@@ -407,19 +493,24 @@
         Returns
         -------
         int
             The count of characters associated with the story
         """
 
         with self._session as session:
-            return session.query(func.count(CharacterStory.character_id)).filter(
-                CharacterStory.story_id == story_id, CharacterStory.user_id == self._owner.id
+            return session.query(
+                func.count(CharacterStory.character_id)
+            ).filter(
+                CharacterStory.story_id == story_id,
+                CharacterStory.user_id == self._owner.id
             ).scalar()
 
-    def get_characters_by_story_id(self, story_id: int) -> list:
+    def get_characters_by_story_id(
+        self, story_id: int
+    ) -> List[Type[Character]]:
         """Get characters by story id
 
         The characters and stories are associated in the CharacterStory table.
 
         Parameters
         ----------
         story_id : int
@@ -429,21 +520,25 @@
         -------
         list
             The list of characters associated with the story
         """
 
         with self._session as session:
             for character_story in session.query(CharacterStory).filter(
-                    CharacterStory.story_id == story_id, CharacterStory.user_id == self._owner.id
+                CharacterStory.story_id == story_id,
+                CharacterStory.user_id == self._owner.id
             ).all():
                 yield session.query(Character).filter(
-                    Character.id == character_story.character_id, Character.user_id == self._owner.id
+                    Character.id == character_story.character_id,
+                    Character.user_id == self._owner.id
                 ).first()
 
-    def get_characters_page_by_story_id(self, story_id: int, page: int, per_page: int) -> list:
+    def get_characters_page_by_story_id(
+        self, story_id: int, page: int, per_page: int
+    ) -> List[Type[Character]]:
         """Get a single page of characters by story id
 
         The characters and stories are associated in the CharacterStory table.
 
         Parameters
         ----------
         story_id : int
@@ -458,21 +553,23 @@
         list
             The list of characters associated with the story
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             for character_story in session.query(CharacterStory).filter(
-                    CharacterStory.story_id == story_id, CharacterStory.user_id == self._owner.id
+                CharacterStory.story_id == story_id,
+                    CharacterStory.user_id == self._owner.id
             ).offset(offset).limit(per_page).all():
                 yield session.query(Character).filter(
-                    Character.id == character_story.character_id, Character.user_id == self._owner.id
+                    Character.id == character_story.character_id,
+                    Character.user_id == self._owner.id
                 ).first()
 
-    def search_characters(self, search: str) -> list:
+    def search_characters(self, search: str) -> List[Type[Character]]:
         """Search for characters by title, first name, middle name, last name, nickname, and description belonging to \
         a specific user
 
         Parameters
         ----------
         search : str
             The search string
@@ -481,21 +578,28 @@
         -------
         list
             The list of characters associated with the user
         """
 
         with self._session as session:
             return session.query(Character).filter(
-                or_(Character.title.like(f'%{search}%'), Character.first_name.like(f'%{search}%'),
-                    Character.middle_name.like(f'%{search}%'), Character.last_name.like(f'%{search}%'),
-                    Character.nickname.like(f'%{search}%'), Character.description.like(f'%{search}%')),
+                or_(
+                    Character.title.like(f'%{search}%'),
+                    Character.first_name.like(f'%{search}%'),
+                    Character.middle_name.like(f'%{search}%'),
+                    Character.last_name.like(f'%{search}%'),
+                    Character.nickname.like(f'%{search}%'),
+                    Character.description.like(f'%{search}%')
+                ),
                 Character.user_id == self._owner.id
             ).all()
 
-    def search_characters_by_story_id(self, story_id: int, search: str) -> list:
+    def search_characters_by_story_id(
+        self, story_id: int, search: str
+    ) -> List[Type[Character]]:
         """Search for characters by title, first name, middle name, last name, nickname, and description belonging to \
         a specific story
 
         Parameters
         ----------
         story_id : int
             The id of the story
@@ -521,16 +625,18 @@
                     Character.nickname.like(f'%{search}%'),
                     Character.description.like(f'%{search}%')
                 ),
                 CharacterStory.story_id == story_id,
                 CharacterStory.user_id == self._owner.id
             ).all()
 
-    def create_relationship(self, parent_id: int, related_id: int, relationship_type: str, description: str = None,
-                            start_date: str = None, end_date: str = None) -> CharacterRelationship:
+    def create_relationship(
+        self, parent_id: int, related_id: int, relationship_type: str,
+        description: str = None, start_date: str = None, end_date: str = None
+    ) -> CharacterRelationship:
         """Create a new character relationship
 
         There are many relationships for each character, and the linking class, CharacterRelationship, is used to
         define the relationship between two characters. The relationship type is defined in the
         CharacterRelationshipTypes and elaborated upon in the description. Before insertion, in order to determine
         the correct position, the highest position among sibling CharacterRelationship objects is first determined.
         The new position is set to the highest position plus one. The created and modified fields are set to the
@@ -583,38 +689,43 @@
                     CharacterRelationship.parent_id == parent_id,
                     CharacterRelationship.user_id == self._owner.id
                 ).scalar()
 
                 position = 1 if not position else position + 1
                 created = datetime.now()
                 modified = created
-                character_relationship = CharacterRelationship(user_id=self._owner.id, parent_id=parent.id,
-                                                               related_id=related.id, position=position,
-                                                               relationship_type=relationship_type,
-                                                               description=description, start_date=start_date,
-                                                               end_date=end_date, created=created,
-                                                               modified=modified)
+                character_relationship = CharacterRelationship(
+                    user_id=self._owner.id, parent_id=parent.id,
+                    related_id=related.id, position=position,
+                    relationship_type=relationship_type,
+                    description=description, start_date=start_date,
+                    end_date=end_date, created=created, modified=modified
+                )
 
-                activity = Activity(user_id=self._owner.id, summary=f'Character relationship created by \
-                                        {self._owner.username}', created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Character relationship \
+                    created by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(character_relationship)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return character_relationship
 
-    def update_relationship(self, relationship_id: int, parent_id: int, related_id: int, relationship_type: str,
-                            description: str = None, start_date: str = None, end_date: str = None) \
-            -> Type[CharacterRelationship]:
+    def update_relationship(
+        self, relationship_id: int, parent_id: int, related_id: int,
+        relationship_type: str, description: str = None, start_date: str = None,
+        end_date: str = None
+    ) -> Type[CharacterRelationship]:
         """Update a character relationship
 
         Parameters
         ----------
         relationship_id : int
             The id of the relationship to update
         parent_id : int
@@ -634,43 +745,50 @@
         -------
         CharacterRelationship
             The updated character relationship object
         """
 
         with self._session as session:
             try:
-                character_relationship = session.query(CharacterRelationship).filter(
-                    CharacterRelationship.id == relationship_id, CharacterRelationship.user_id == self._owner.id
+                character_relationship = session.query(
+                    CharacterRelationship
+                ).filter(
+                    CharacterRelationship.id == relationship_id,
+                    CharacterRelationship.user_id == self._owner.id
                 ).first()
 
                 if not character_relationship:
                     raise ValueError('Character relationship not found.')
 
                 character_relationship.parent_id = parent_id
                 character_relationship.related_id = related_id
                 character_relationship.relationship_type = relationship_type
                 character_relationship.description = description
                 character_relationship.start_date = start_date
                 character_relationship.end_date = end_date
                 character_relationship.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id, summary=f'Character relationship updated by \
-                                    {self._owner.username}', created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Character relationship \
+                    updated by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return character_relationship
 
-    def change_relationship_position(self, relationship_id: int, position: int) -> Type[CharacterRelationship]:
+    def change_relationship_position(
+        self, relationship_id: int, position: int
+    ) -> Type[CharacterRelationship]:
         """Set the position of a character relationship
 
         First, determine whether the new position is closer to 1 or further from 1. If closer to one, get all sibling
         CharacterRelationship objects with positions greater than or equal to the new position but less than the current
         position, and increment those position values by 1. If the target position is further away from 1 than the
         current position, get all sibling CharacterRelationship objects with positions greater than the current position
         but less than or equal to the new position, and decrement those position values by 1. Finally, set the position
@@ -702,34 +820,38 @@
                     raise ValueError('Position must be greater than 0.')
 
                 if position == character_relationship.position:
                     return character_relationship
 
                 if position < character_relationship.position:
                     for sibling in session.query(CharacterRelationship).filter(
-                            CharacterRelationship.parent_id == character_relationship.parent_id,
-                            CharacterRelationship.position >= position,
-                            CharacterRelationship.position < character_relationship.position,
-                            CharacterRelationship.user_id == self._owner.id
+                        CharacterRelationship.parent_id == character_relationship.parent_id,
+                        CharacterRelationship.position >= position,
+                        CharacterRelationship.position < character_relationship.position,
+                        CharacterRelationship.user_id == self._owner.id
                     ).all():
                         sibling.position += 1
 
                 else:
                     for sibling in session.query(CharacterRelationship).filter(
-                            CharacterRelationship.parent_id == character_relationship.parent_id,
-                            CharacterRelationship.position > character_relationship.position,
-                            CharacterRelationship.position <= position, CharacterRelationship.user_id == self._owner.id
+                        CharacterRelationship.parent_id == character_relationship.parent_id,
+                        CharacterRelationship.position > character_relationship.position,
+                        CharacterRelationship.position <= position,
+                        CharacterRelationship.user_id == self._owner.id
                     ).all():
                         sibling.position -= 1
 
                 character_relationship.position = position
                 character_relationship.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id, summary=f'Character relationship position updated by \
-                                    {self._owner.username}', created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Character relationship \
+                    position updated by {self._owner.username}',
+                    created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
@@ -752,63 +874,75 @@
         -------
         bool
             True on success
         """
 
         with self._session as session:
             try:
-                character_relationship = session.query(CharacterRelationship).filter(
-                    CharacterRelationship.id == relationship_id, CharacterRelationship.user_id == self._owner.id
+                character_relationship = session.query(
+                    CharacterRelationship
+                ).filter(
+                    CharacterRelationship.id == relationship_id,
+                    CharacterRelationship.user_id == self._owner.id
                 ).first()
 
                 if not character_relationship:
                     raise ValueError('Character relationship not found.')
 
                 for sibling in session.query(CharacterRelationship).filter(
-                        CharacterRelationship.parent_id == character_relationship.parent_id,
-                        CharacterRelationship.position > character_relationship.position,
-                        CharacterRelationship.user_id == self._owner.id
+                    CharacterRelationship.parent_id == character_relationship.parent_id,
+                    CharacterRelationship.position > character_relationship.position,
+                    CharacterRelationship.user_id == self._owner.id
                 ).all():
                     sibling.position -= 1
 
-                activity = Activity(user_id=self._owner.id, summary=f'Character relationship deleted by \
-                                    {self._owner.username}', created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Character relationship \
+                    deleted by {self._owner.username}', created=datetime.now()
+                )
 
                 session.delete(character_relationship)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return True
 
-    def get_relationship_by_id(self, relationship_id: int) -> Type[CharacterRelationship] | None:
+    def get_relationship_by_id(
+        self, relationship_id: int
+    ) -> Type[CharacterRelationship] | None:
         """Get a character relationship by id
 
         Parameters
         ----------
         relationship_id : int
             The id of the relationship to get
 
         Returns
         -------
         Type[CharacterRelationship] | None
             The character relationship if found, otherwise None
         """
 
         with self._session as session:
-            character_relationship = session.query(CharacterRelationship).filter(
-                CharacterRelationship.id == relationship_id, CharacterRelationship.user_id == self._owner.id
+            character_relationship = session.query(
+                CharacterRelationship
+            ).filter(
+                CharacterRelationship.id == relationship_id,
+                CharacterRelationship.user_id == self._owner.id
             ).first()
             return character_relationship if character_relationship else None
 
-    def get_relationships_by_character_id(self, parent_id: int) -> list:
+    def get_relationships_by_character_id(
+        self, parent_id: int
+    ) -> List[Type[CharacterRelationship]]:
         """Get character relationships by character id, from that character's perspective
 
         Parameters
         ----------
         parent_id : int
             The id of the character
 
@@ -816,18 +950,21 @@
         -------
         list
             The list of character relationships
         """
 
         with self._session as session:
             return session.query(CharacterRelationship).filter(
-                CharacterRelationship.parent_id == parent_id, CharacterRelationship.user_id == self._owner.id
+                CharacterRelationship.parent_id == parent_id,
+                CharacterRelationship.user_id == self._owner.id
             ).all()
 
-    def get_relationships_page_by_character_id(self, parent_id: int, page: int, per_page: int) -> list:
+    def get_relationships_page_by_character_id(
+        self, parent_id: int, page: int, per_page: int
+    ) -> List[Type[CharacterRelationship]]:
         """Get a single page of character relationships by character id, from that character's perspective
 
         Parameters
         ----------
         parent_id : int
             The id of the character
         page : int
@@ -840,18 +977,21 @@
         list
             The list of character relationships
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(CharacterRelationship).filter(
-                CharacterRelationship.parent_id == parent_id, CharacterRelationship.user_id == self._owner.id
+                CharacterRelationship.parent_id == parent_id,
+                CharacterRelationship.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def create_trait(self, character_id: int, name: str, magnitude: int) -> CharacterTrait:
+    def create_trait(
+        self, character_id: int, name: str, magnitude: int
+    ) -> CharacterTrait:
         """Create a new character trait
 
         The position of the new trait must be determined by first finding the highest existing position among siblings,
         if any. Any other CharacterTrait objects associated with the same character are those siblings.
 
         Parameters
         ----------
@@ -870,46 +1010,57 @@
 
         with self._session as session:
             try:
                 if not character_id or not name or not magnitude:
                     raise ValueError('Character id, name, and magnitude must be provided.')
 
                 character = session.query(Character).filter(
-                    Character.id == character_id, Character.user_id == self._owner.id
+                    Character.id == character_id,
+                    Character.user_id == self._owner.id
                 ).first()
 
                 if not character:
                     raise ValueError('Character not found.')
 
-                position = session.query(func.max(CharacterTrait.position)).filter(
-                    CharacterTrait.character_id == character_id, CharacterTrait.user_id == self._owner.id
+                position = session.query(
+                    func.max(CharacterTrait.position)
+                ).filter(
+                    CharacterTrait.character_id == character_id,
+                    CharacterTrait.user_id == self._owner.id
                 ).scalar()
 
                 position = 1 if not position else position + 1
                 created = datetime.now()
                 modified = created
-                character_trait = CharacterTrait(user_id=self._owner.id, character_id=character_id, position=position,
-                                                 name=name, magnitude=magnitude, created=created, modified=modified)
+                character_trait = CharacterTrait(
+                    user_id=self._owner.id, character_id=character_id,
+                    position=position, name=name, magnitude=magnitude,
+                    created=created, modified=modified
+                )
 
-                activity = Activity(user_id=self._owner.id, summary=f'Character trait {name} \
-                                    created by {self._owner.username} for "{character.__str__}"',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Character trait {name} \
+                    created by {self._owner.username} for "{character.__str__}"',
+                    created=datetime.now()
+                )
 
                 session.add(character_trait)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return character_trait
 
-    def update_trait(self, trait_id: int, name: str, magnitude: int) -> Type[CharacterTrait]:
+    def update_trait(
+        self, trait_id: int, name: str, magnitude: int
+    ) -> Type[CharacterTrait]:
         """Update a character trait
 
         Parameters
         ----------
         trait_id : int
             The id of the trait to update
         name : str
@@ -922,38 +1073,44 @@
         CharacterTrait
             The updated character trait object
         """
 
         with self._session as session:
             try:
                 character_trait = session.query(CharacterTrait).filter(
-                    CharacterTrait.id == trait_id, CharacterTrait.user_id == self._owner.id
+                    CharacterTrait.id == trait_id,
+                    CharacterTrait.user_id == self._owner.id
                 ).first()
 
                 if not character_trait:
                     raise ValueError('Character trait not found.')
 
                 character_trait.name = name
                 character_trait.magnitude = magnitude
                 character_trait.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id, summary=f'Character trait {character_trait.__str__} \
-                                    updated by {self._owner.username}', created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Character trait \
+                    {character_trait.__str__} updated by {self._owner.username}',
+                    created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return character_trait
 
-    def change_trait_position(self, trait_id: int, position: int) -> Type[CharacterTrait]:
+    def change_trait_position(
+        self, trait_id: int, position: int
+    ) -> Type[CharacterTrait]:
         """Set the position of a character trait
 
         First, determine whether the new position is closer to 1 or further from 1. If closer to one, get all sibling
         CharacterTraits with positions greater than or equal to the new position but less than the current position, and
         increment those position values by 1. If the target position is further away from 1 than the current position,
         get all sibling CharacterTraits with positions greater than the current position but less than or equal to the
         new position, and decrement those position values by 1. Finally, set the position of the target chapter to the
@@ -998,39 +1155,48 @@
 
                 if position == character_trait.position:
                     return character_trait.position
 
                 if position < character_trait.position:
                     siblings = session.query(CharacterTrait).filter(
                         CharacterTrait.character_id == character_trait.character_id,
-                        CharacterTrait.position >= position, CharacterTrait.user_id == self._owner.id,
+                        CharacterTrait.position >= position,
+                        CharacterTrait.user_id == self._owner.id,
                         CharacterTrait.position < character_trait.position
                     ).all()
 
                     for sibling in siblings:
                         sibling.position += 1
-                        sibling.created = datetime.strptime(str(sibling.created), datetime_format)
+                        sibling.created = datetime.strptime(
+                            str(sibling.created), datetime_format
+                        )
                         sibling.modified = datetime.now()
 
                 else:
                     siblings = session.query(CharacterTrait).filter(
                         CharacterTrait.character_id == character_trait.character_id,
                         CharacterTrait.position > character_trait.position,
-                        CharacterTrait.position <= position, CharacterTrait.user_id == self._owner.id
+                        CharacterTrait.position <= position,
+                        CharacterTrait.user_id == self._owner.id
                     ).all()
 
                     for sibling in siblings:
                         sibling.position -= 1
-                        sibling.created = datetime.strptime(str(sibling.created), datetime_format)
+                        sibling.created = datetime.strptime(
+                            str(sibling.created), datetime_format
+                        )
                         sibling.modified = datetime.now()
 
                 character_trait.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id, summary=f'Character trait {character_trait.__str__} \
-                                    position changed by {self._owner.username}', created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Character trait \
+                    {character_trait.__str__} position changed by \
+                    {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
@@ -1059,30 +1225,37 @@
             try:
 
                 config = ConfigParser()
                 config.read("config.cfg")
                 datetime_format = config.get("formats", "datetime")
 
                 character_trait = session.query(CharacterTrait).filter(
-                    CharacterTrait.id == trait_id, CharacterTrait.user_id == self._owner.id
+                    CharacterTrait.id == trait_id,
+                    CharacterTrait.user_id == self._owner.id
                 ).first()
 
                 if not character_trait:
                     raise ValueError('Character trait not found.')
 
                 for sibling in session.query(CharacterTrait).filter(
-                        CharacterTrait.character_id == character_trait.character_id,
-                        CharacterTrait.position > character_trait.position, CharacterTrait.user_id == self._owner.id
+                    CharacterTrait.character_id == character_trait.character_id,
+                    CharacterTrait.position > character_trait.position,
+                    CharacterTrait.user_id == self._owner.id
                 ).all():
                     sibling.position -= 1
-                    sibling.created = datetime.strptime(str(sibling.created), datetime_format)
+                    sibling.created = datetime.strptime(
+                        str(sibling.created), datetime_format
+                    )
                     sibling.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id, summary=f'Character trait {character_trait.__str__} \
-                                    deleted by {self._owner.username}', created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Character trait \
+                    {character_trait.__str__} deleted by \
+                    {self._owner.username}', created=datetime.now()
+                )
 
                 session.delete(character_trait)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
@@ -1103,19 +1276,22 @@
         -------
         Type[CharacterTrait] | None
             The character trait if found, otherwise None
         """
 
         with self._session as session:
             character_trait = session.query(CharacterTrait).filter(
-                CharacterTrait.id == trait_id, CharacterTrait.user_id == self._owner.id
+                CharacterTrait.id == trait_id,
+                CharacterTrait.user_id == self._owner.id
             ).first()
             return character_trait if character_trait else None
 
-    def get_traits_by_character_id(self, character_id: int) -> list:
+    def get_traits_by_character_id(
+        self, character_id: int
+    ) -> List[Type[CharacterTrait]]:
         """Get character traits by character id
 
         Parameters
         ----------
         character_id : int
             The id of the character
 
@@ -1123,18 +1299,21 @@
         -------
         list
             The list of character traits
         """
 
         with self._session as session:
             return session.query(CharacterTrait).filter(
-                CharacterTrait.character_id == character_id, CharacterTrait.user_id == self._owner.id
+                CharacterTrait.character_id == character_id,
+                CharacterTrait.user_id == self._owner.id
             ).all()
 
-    def get_traits_page_by_character_id(self, character_id: int, page: int, per_page: int) -> list:
+    def get_traits_page_by_character_id(
+        self, character_id: int, page: int, per_page: int
+    ) -> List[Type[CharacterTrait]]:
         """Get a single page of character traits by character id
 
         Parameters
         ----------
         character_id : int
             The id of the character
         page : int
@@ -1147,19 +1326,22 @@
         list
             The list of character traits
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(CharacterTrait).filter(
-                CharacterTrait.character_id == character_id, CharacterTrait.user_id == self._owner.id
+                CharacterTrait.character_id == character_id,
+                CharacterTrait.user_id == self._owner.id
             ).offset(
                 offset).limit(per_page).all()
 
-    def append_events_to_character(self, character_id: int, event_ids: list) -> Type[Character]:
+    def append_events_to_character(
+        self, character_id: int, event_ids: list
+    ) -> Type[Character]:
         """Append events to a character
 
         Parameters
         ----------
         character_id : int
             The id of the character
         event_ids : list
@@ -1170,46 +1352,54 @@
         Character
             The updated character object
         """
 
         with self._session as session:
             try:
                 character = session.query(Character).filter(
-                    Character.id == character_id, Character.user_id == self._owner.id
+                    Character.id == character_id,
+                    Character.user_id == self._owner.id
                 ).first()
 
                 if not character:
                     raise ValueError('Character not found.')
 
                 for event_id in event_ids:
                     event = session.query(Event).filter(
                         Event.id == event_id, Event.user_id == self._owner.id
                     ).first()
 
                     if not event:
                         raise ValueError('Event not found.')
 
-                    character_event = CharacterEvent(user_id=self._owner.id, character_id=character_id,
-                                                     event_id=event_id, created=datetime.now())
-
-                    activity = Activity(user_id=self._owner.id, summary=f'Event {event.title[:50]} associated with \
-                                        {character.__str__} by {self._owner.username}', created=datetime.now())
+                    character_event = CharacterEvent(
+                        user_id=self._owner.id, character_id=character_id,
+                        event_id=event_id, created=datetime.now()
+                    )
+
+                    activity = Activity(
+                        user_id=self._owner.id, summary=f'Event \
+                        {event.title[:50]} associated with {character.__str__} \
+                        by {self._owner.username}', created=datetime.now()
+                    )
 
                     session.add(character_event)
                     session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return character
 
-    def get_events_by_character_id(self, character_id: int) -> list:
+    def get_events_by_character_id(
+        self, character_id: int
+    ) -> List[Type[Event]]:
         """Get all events associated with a character
 
         Using the association of the CharacterEvent table, get all events from teh Event table associated with a
         character.
 
         Parameters
         ----------
@@ -1220,21 +1410,25 @@
         -------
         list
             The list of events
         """
 
         with self._session as session:
             for character_event in session.query(CharacterEvent).filter(
-                    CharacterEvent.character_id == character_id, CharacterEvent.user_id == self._owner.id
+                CharacterEvent.character_id == character_id,
+                    CharacterEvent.user_id == self._owner.id
             ).all():
                 yield session.query(Event).filter(
-                    Event.id == character_event.event_id, Event.user_id == self._owner.id
+                    Event.id == character_event.event_id,
+                    Event.user_id == self._owner.id
                 ).first()
 
-    def get_events_page_by_character_id(self, character_id: int, page: int, per_page: int) -> list:
+    def get_events_page_by_character_id(
+        self, character_id: int, page: int, per_page: int
+    ) -> List[Type[Event]]:
         """Get a single page of events associated with a character from the database
 
         Parameters
         ----------
         character_id : int
             The id of the character
         page : int
@@ -1247,18 +1441,21 @@
         list
             The list of events
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(CharacterEvent).filter(
-                CharacterEvent.character_id == character_id, CharacterEvent.user_id == self._owner.id
+                CharacterEvent.character_id == character_id,
+                CharacterEvent.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def append_links_to_character(self, character_id: int, link_ids: list) -> Type[Character]:
+    def append_links_to_character(
+        self, character_id: int, link_ids: list
+    ) -> Type[Character]:
         """Append links to a character
 
         Parameters
         ----------
         character_id : int
             The id of the character
         link_ids : list
@@ -1269,46 +1466,53 @@
         Character
             The updated character object
         """
 
         with self._session as session:
             try:
                 character = session.query(Character).filter(
-                    Character.id == character_id, Character.user_id == self._owner.id
+                    Character.id == character_id,
+                    Character.user_id == self._owner.id
                 ).first()
 
                 if not character:
                     raise ValueError('Character not found.')
 
                 for link_id in link_ids:
                     link = session.query(Link).filter(
-                        Link.id == link_id, Link.user_id == self._owner.id
+                        Link.id == link_id,
+                        Link.user_id == self._owner.id
                     ).first()
 
                     if not link:
                         raise ValueError('Link not found.')
 
-                    character_link = CharacterLink(user_id=self._owner.id, character_id=character_id, link_id=link_id,
-                                                   created=datetime.now())
-
-                    activity = Activity(user_id=self._owner.id, summary=f'Link {link.title[:50]} associated with \
-                                        {character.__str__} by {self._owner.username}', created=datetime.now())
+                    character_link = CharacterLink(
+                        user_id=self._owner.id, character_id=character_id,
+                        link_id=link_id, created=datetime.now()
+                    )
+
+                    activity = Activity(
+                        user_id=self._owner.id, summary=f'Link \
+                        {link.title[:50]} associated with {character.__str__} \
+                        by {self._owner.username}', created=datetime.now()
+                    )
 
                     session.add(character_link)
                     session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return character
 
-    def get_links_by_character_id(self, character_id: int) -> list:
+    def get_links_by_character_id(self, character_id: int) -> List[Type[Link]]:
         """Get all links associated with a character
 
         Parameters
         ----------
         character_id : int
             The id of the character
 
@@ -1316,21 +1520,25 @@
         -------
         list
             The list of links
         """
 
         with self._session as session:
             for character_link in session.query(CharacterLink).filter(
-                    CharacterLink.character_id == character_id, CharacterLink.user_id == self._owner.id
+                CharacterLink.character_id == character_id,
+                CharacterLink.user_id == self._owner.id
             ).all():
                 yield session.query(Link).filter(
-                    Link.id == character_link.link_id, Link.user_id == self._owner.id
+                    Link.id == character_link.link_id,
+                    Link.user_id == self._owner.id
                 ).first()
 
-    def get_links_page_by_character_id(self, character_id: int, page: int, per_page: int) -> list:
+    def get_links_page_by_character_id(
+        self, character_id: int, page: int, per_page: int
+    ) -> List[Type[Link]]:
         """Get a single page of links associated with a character from the database
 
         Parameters
         ----------
         character_id : int
             The id of the character
         page : int
@@ -1343,18 +1551,21 @@
         list
             The list of links
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(CharacterLink).filter(
-                CharacterLink.character_id == character_id, CharacterLink.user_id == self._owner.id
+                CharacterLink.character_id == character_id,
+                CharacterLink.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def append_notes_to_character(self, character_id: int, note_ids: list) -> Type[Character]:
+    def append_notes_to_character(
+        self, character_id: int, note_ids: list
+    ) -> Type[Character]:
         """Append notes to a character
 
         Parameters
         ----------
         character_id : int
             The id of the character
         note_ids : list
@@ -1365,46 +1576,53 @@
         Character
             The updated character object
         """
 
         with self._session as session:
             try:
                 character = session.query(Character).filter(
-                    Character.id == character_id, Character.user_id == self._owner.id
+                    Character.id == character_id,
+                    Character.user_id == self._owner.id
                 ).first()
 
                 if not character:
                     raise ValueError('Character not found.')
 
                 for note_id in note_ids:
                     note = session.query(Note).filter(
-                        Note.id == note_id, Note.user_id == self._owner.id
+                        Note.id == note_id,
+                        Note.user_id == self._owner.id
                     ).first()
 
                     if not note:
                         raise ValueError('Note not found.')
 
-                    character_note = CharacterNote(user_id=self._owner.id, character_id=character_id, note_id=note_id,
-                                                   created=datetime.now())
-
-                    activity = Activity(user_id=self._owner.id, summary=f'Note {note.title[:50]} associated with \
-                                        {character.__str__} by {self._owner.username}', created=datetime.now())
+                    character_note = CharacterNote(
+                        user_id=self._owner.id, character_id=character_id,
+                        note_id=note_id, created=datetime.now()
+                    )
+
+                    activity = Activity(
+                        user_id=self._owner.id, summary=f'Note \
+                        {note.title[:50]} associated with {character.__str__} \
+                        by {self._owner.username}', created=datetime.now()
+                    )
 
                     session.add(character_note)
                     session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return character
 
-    def get_notes_by_character_id(self, character_id: int) -> list:
+    def get_notes_by_character_id(self, character_id: int) -> List[Type[Note]]:
         """Get all notes associated with a character
 
         Parameters
         ----------
         character_id : int
             The id of the character
 
@@ -1412,21 +1630,25 @@
         -------
         list
             The list of notes
         """
 
         with self._session as session:
             for character_note in session.query(CharacterNote).filter(
-                    CharacterNote.character_id == character_id, CharacterNote.user_id == self._owner.id
+                CharacterNote.character_id == character_id,
+                CharacterNote.user_id == self._owner.id
             ).all():
                 yield session.query(Note).filter(
-                    Note.id == character_note.note_id, Note.user_id == self._owner.id
+                    Note.id == character_note.note_id,
+                    Note.user_id == self._owner.id
                 ).first()
 
-    def get_notes_page_by_character_id(self, character_id: int, page: int, per_page: int) -> list:
+    def get_notes_page_by_character_id(
+        self, character_id: int, page: int, per_page: int
+    ) -> List[Type[Note]]:
         """Get a single page of notes associated with a character from the database
 
         Parameters
         ----------
         character_id : int
             The id of the character
         page : int
@@ -1439,18 +1661,21 @@
         list
             The list of notes
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(CharacterNote).filter(
-                CharacterNote.character_id == character_id, CharacterNote.user_id == self._owner.id
+                CharacterNote.character_id == character_id,
+                CharacterNote.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def append_images_to_character(self, character_id: int, image_ids: list) -> Type[Character]:
+    def append_images_to_character(
+        self, character_id: int, image_ids: list
+    ) -> Type[Character]:
         """Append images to a character
 
         As images are appended to the character, before each image is appended, the highest position among other images
         associated with this object is found and the new image is appended with a position one higher than the highest
         position.
 
         Parameters
@@ -1465,56 +1690,69 @@
         Character
             The updated character object
         """
 
         with self._session as session:
             try:
                 character = session.query(Character).filter(
-                    Character.id == character_id, Character.user_id == self._owner.id
+                    Character.id == character_id,
+                    Character.user_id == self._owner.id
                 ).first()
 
                 if not character:
                     raise ValueError('Character not found.')
 
                 for image_id in image_ids:
                     image = session.query(Image).filter(
-                        Image.id == image_id, Image.user_id == self._owner.id
+                        Image.id == image_id,
+                        Image.user_id == self._owner.id
                     ).first()
 
                     if not image:
                         raise ValueError('Image not found.')
 
-                    position = session.query(func.max(CharacterImage.position)).filter(
-                        CharacterImage.character_id == character_id, CharacterImage.user_id == self._owner.id
+                    position = session.query(
+                        func.max(CharacterImage.position)
+                    ).filter(
+                        CharacterImage.character_id == character_id,
+                        CharacterImage.user_id == self._owner.id
                     ).scalar()
 
                     position = 1 if not position else position + 1
                     is_default = False
                     created = datetime.now()
                     modified = created
-                    character_image = CharacterImage(user_id=self._owner.id, character_id=character_id,
-                                                     image_id=image_id, position=position, is_default=is_default,
-                                                     created=created, modified=modified)
-
-                    activity = Activity(user_id=self._owner.id, summary=f'Image {image.filename[:50]} associated with \
-                                        character {str(character)[:50]} by {self._owner.username}',
-                                        created=datetime.now())
+                    character_image = CharacterImage(
+                        user_id=self._owner.id, character_id=character_id,
+                        image_id=image_id, position=position,
+                        is_default=is_default, created=created,
+                        modified=modified
+                    )
+
+                    activity = Activity(
+                        user_id=self._owner.id, summary=f'Image \
+                        {image.filename[:50]} associated with character \
+                        {str(character)[:50]} by {self._owner.username}',
+                        created=datetime.now()
+                    )
 
                     session.add(character_image)
                     session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return character
 
-    def change_image_position(self, image_id: int, position: int) -> Type[CharacterImage]:
+    def change_image_position(
+        self, image_id: int, position: int
+    ) -> Type[CharacterImage]:
         """Set the position of a character image
 
         First, determine whether the new position is closer to 1 or further from 1. If closer to one, get all sibling
         CharacterImage objects with positions greater than or equal to the new position but less than the current
         position, and increment those position values by 1. If the target position is further away from 1 than the
         current position, get all sibling CharacterImage objects with positions greater than the current position but
         less than or equal to the new position, and decrement those position values by 1. Finally, set the position of
@@ -1537,75 +1775,89 @@
             try:
 
                 config = ConfigParser()
                 config.read("config.cfg")
                 datetime_format = config.get("formats", "datetime")
 
                 character_image = session.query(CharacterImage).filter(
-                    CharacterImage.id == image_id, CharacterImage.user_id == self._owner.id
+                    CharacterImage.id == image_id,
+                    CharacterImage.user_id == self._owner.id
                 ).first()
 
                 if not character_image:
                     raise ValueError('Character image not found.')
 
                 if position < 1:
                     raise ValueError('Position must be greater than 0.')
 
-                highest_position = session.query(func.max(CharacterImage.position)).filter(
+                highest_position = session.query(
+                    func.max(CharacterImage.position)
+                ).filter(
                     CharacterImage.character_id == character_image.character_id,
                     CharacterImage.user_id == self._owner.id
                 ).scalar()
 
                 if position > highest_position:
                     raise ValueError(f'Position must be less than or equal to {highest_position}.')
 
                 if position == character_image.position:
                     return character_image.position
 
                 if position < character_image.position:
                     siblings = session.query(CharacterImage).filter(
                         CharacterImage.character_id == character_image.character_id,
-                        CharacterImage.position >= position, CharacterImage.user_id == self._owner.id,
+                        CharacterImage.position >= position,
+                        CharacterImage.user_id == self._owner.id,
                         CharacterImage.position < character_image.position
                     ).all()
 
                     for sibling in siblings:
                         sibling.position += 1
-                        sibling.created = datetime.strptime(str(sibling.created), datetime_format)
+                        sibling.created = datetime.strptime(
+                            str(sibling.created), datetime_format
+                        )
                         sibling.modified = datetime.now()
 
                 else:
                     siblings = session.query(CharacterImage).filter(
                         CharacterImage.character_id == character_image.character_id,
                         CharacterImage.position > character_image.position,
-                        CharacterImage.position <= position, CharacterImage.user_id == self._owner.id
+                        CharacterImage.position <= position,
+                        CharacterImage.user_id == self._owner.id
                     ).all()
 
                     for sibling in siblings:
                         sibling.position -= 1
-                        sibling.created = datetime.strptime(str(sibling.created), datetime_format)
+                        sibling.created = datetime.strptime(
+                            str(sibling.created), datetime_format
+                        )
                         sibling.modified = datetime.now()
 
                 character_image.position = position
                 character_image.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id, summary=f'Character image {character_image.__str__} \
-                                    position changed by {self._owner.username}', created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Character image \
+                    {character_image.__str__} position changed by \
+                    {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return character_image
 
-    def change_image_default_status(self, image_id: int, is_default: bool) -> Type[CharacterImage]:
+    def change_image_default_status(
+        self, image_id: int, is_default: bool
+    ) -> Type[CharacterImage]:
         """Set the default status of a character image
 
         If changing the value from true to false, it is straightforward - make the value change and save the object.
         However, if the value is changed from false to true, then before saving that new value in the object, the same
         attribute must first be set to false in all sibling CharacterImage objects. This is because only one image can
         be the default image for a character. The activity is then logged and the CharacterImage object is saved.
 
@@ -1621,36 +1873,40 @@
         CharacterImage
             The updated character image object
         """
 
         with self._session as session:
             try:
                 character_image = session.query(CharacterImage).filter(
-                    CharacterImage.id == image_id, CharacterImage.user_id == self._owner.id
+                    CharacterImage.id == image_id,
+                    CharacterImage.user_id == self._owner.id
                 ).first()
 
                 if not character_image:
                     raise ValueError('Character image not found.')
 
                 if is_default == character_image.is_default:
                     return character_image
 
                 if is_default:
                     for sibling in session.query(CharacterImage).filter(
-                            CharacterImage.character_id == character_image.character_id,
-                            CharacterImage.user_id == self._owner.id
+                        CharacterImage.character_id == character_image.character_id,
+                        CharacterImage.user_id == self._owner.id
                     ).all():
                         sibling.is_default = False
                         sibling.modified = datetime.now()
 
                 character_image.is_default = is_default
                 character_image.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id, summary=f'Character image {character_image.__str__} \
-                                    default status changed by {self._owner.username}', created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Character image \
+                    {character_image.__str__} default status changed by \
+                    {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
@@ -1680,33 +1936,41 @@
             try:
 
                 config = ConfigParser()
                 config.read("config.cfg")
                 datetime_format = config.get("formats", "datetime")
 
                 character_image = session.query(CharacterImage).filter(
-                    CharacterImage.id == image_id, CharacterImage.user_id == self._owner.id
+                    CharacterImage.id == image_id,
+                    CharacterImage.user_id == self._owner.id
                 ).first()
                 image = session.query(Image).filter(
-                    Image.id == character_image.image_id, Image.user_id == self._owner.id
+                    Image.id == character_image.image_id,
+                    Image.user_id == self._owner.id
                 ).first()
 
                 if not character_image:
                     raise ValueError('Character image not found.')
 
                 for sibling in session.query(CharacterImage).filter(
-                        CharacterImage.character_id == character_image.character_id,
-                        CharacterImage.position > character_image.position, CharacterImage.user_id == self._owner.id
+                    CharacterImage.character_id == character_image.character_id,
+                    CharacterImage.position > character_image.position,
+                        CharacterImage.user_id == self._owner.id
                 ).all():
                     sibling.position -= 1
-                    sibling.created = datetime.strptime(str(sibling.created), datetime_format)
+                    sibling.created = datetime.strptime(
+                        str(sibling.created), datetime_format
+                    )
                     sibling.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id, summary=f'Character image {image.caption[:50]} \
-                                    deleted by {self._owner.username}', created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Character image \
+                    {image.caption[:50]} deleted by {self._owner.username}',
+                    created=datetime.now()
+                )
 
                 session.delete(character_image)
                 session.delete(image)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
@@ -1728,18 +1992,21 @@
         -------
         int
             The count of images
         """
 
         with self._session as session:
             return session.query(func.count(CharacterImage.id)).filter(
-                CharacterImage.character_id == character_id, CharacterImage.user_id == self._owner.id
+                CharacterImage.character_id == character_id,
+                CharacterImage.user_id == self._owner.id
             ).scalar()
 
-    def get_images_by_character_id(self, character_id: int) -> list:
+    def get_images_by_character_id(
+        self, character_id: int
+    ) -> List[Type[Image]]:
         """Get all images associated with a character
 
         The images will be returned in the order of their position. A yield is used to return the images one at a time.
 
         Parameters
         ----------
         character_id : int
@@ -1749,21 +2016,25 @@
         -------
         list
             The list of images
         """
 
         with self._session as session:
             for character_image in session.query(CharacterImage).filter(
-                    CharacterImage.character_id == character_id, CharacterImage.user_id == self._owner.id
+                CharacterImage.character_id == character_id,
+                    CharacterImage.user_id == self._owner.id
             ).order_by(CharacterImage.position).all():
                 yield session.query(Image).filter(
-                    Image.id == character_image.image_id, Image.user_id == self._owner.id
+                    Image.id == character_image.image_id,
+                    Image.user_id == self._owner.id
                 ).first()
 
-    def get_images_page_by_character_id(self, character_id: int, page: int, per_page: int) -> list:
+    def get_images_page_by_character_id(
+        self, character_id: int, page: int, per_page: int
+    ) -> List[Type[Image]]:
         """Get a single page of images associated with a character from the database
 
         The images will be returned in the order of their position. A yield is used to return the images one at a time.
 
         Parameters
         ----------
         character_id : int
@@ -1778,12 +2049,16 @@
         list
             The list of images
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             for character_image in session.query(CharacterImage).filter(
-                    CharacterImage.character_id == character_id, CharacterImage.user_id == self._owner.id
-            ).order_by(CharacterImage.position).offset(offset).limit(per_page).all():
+                CharacterImage.character_id == character_id,
+                    CharacterImage.user_id == self._owner.id
+            ).order_by(
+                CharacterImage.position
+            ).offset(offset).limit(per_page).all():
                 yield session.query(Image).filter(
-                    Image.id == character_image.image_id, Image.user_id == self._owner.id
+                    Image.id == character_image.image_id,
+                    Image.user_id == self._owner.id
                 ).first()
```

### Comparing `noveler-0.1.0/noveler/controllers/EventController.py` & `noveler-0.1.1/noveler/controllers/EventController.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from datetime import datetime
-from typing import Type
+from typing import Type, List
 from sqlalchemy.orm import Session
 from noveler.controllers.BaseController import BaseController
 from noveler.models import User, Event, CharacterEvent, Character, Activity, EventLocation, Location, Link, EventLink, \
     Note, EventNote
 
 
 class EventController(BaseController):
     """Event controller encapsulates event management functionality
 
     Attributes
     ----------
-    _self : EventController
+    _instance : EventController
         The instance of the event controller
     _owner : User
         The current user of the event controller
     _session : Session
         The database session
 
     Methods
@@ -49,22 +49,24 @@
     get_notes_by_event_id(event_id: int)
         Get all notes associated with an event
     get_notes_page_by_event_id(event_id: int, page: int, per_page: int)
         Get a single page of notes associated with an event from the database
     """
 
     def __init__(
-            self, path_to_config: str, session: Session, owner: Type[User]
+        self, path_to_config: str, session: Session, owner: Type[User]
     ):
         """Initialize the class"""
 
         super().__init__(path_to_config, session, owner)
 
-    def create_event(self, title: str, description: str = None, start_datetime: str = None,
-                     end_datetime: str = None) -> Event:
+    def create_event(
+        self, title: str, description: str = None, start_datetime: str = None,
+        end_datetime: str = None
+    ) -> Event:
         """Create a new event
 
         Parameters
         ----------
         title : str
             The title of the event
         description : str
@@ -81,35 +83,40 @@
         """
 
         with self._session as session:
             try:
                 created = datetime.now()
                 modified = created
 
-                event = Event(user_id=self._owner.id, title=title, description=description,
-                              start_datetime=start_datetime, end_datetime=end_datetime, created=created,
-                              modified=modified)
-
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Event {event.title[:50]} created by {self._owner.username}',
-                                    created=datetime.now())
+                event = Event(
+                    user_id=self._owner.id, title=title, description=description,
+                    start_datetime=start_datetime, end_datetime=end_datetime,
+                    created=created, modified=modified
+                )
+
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Event {event.title[:50]} \
+                    created by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(event)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return event
 
-    def update_event(self, event_id: int, title: str, description: str, start_datetime: str,
-                     end_datetime: str) -> Type[Event]:
+    def update_event(
+        self, event_id: int, title: str, description: str, start_datetime: str,
+        end_datetime: str
+    ) -> Type[Event]:
         """Update an event
 
         Parameters
         ----------
         event_id : int
             The id of the event
         title : str
@@ -136,17 +143,18 @@
 
                 event.title = title
                 event.description = description
                 event.start_datetime = start_datetime
                 event.end_datetime = end_datetime
                 event.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Event {event.id} updated by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Event {event.id} updated \
+                    by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
@@ -167,50 +175,54 @@
         bool
             True on success
         """
 
         with self._session as session:
             try:
                 event = session.query(Event).filter(
-                    Event.id == event_id, Event.user_id == self._owner.id
+                    Event.id == event_id,
+                    Event.user_id == self._owner.id
                 ).first()
 
                 if not event:
                     raise ValueError('Event not found.')
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Event {event.id} deleted by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Event {event.id} deleted \
+                    by {self._owner.username}', created=datetime.now()
+                )
 
                 session.delete(event)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return True
 
-    def get_all_events(self) -> list:
+    def get_all_events(self) -> List[Type[Event]]:
         """Get all events associated with a user
 
         Returns
         -------
         list
             A list of event objects
         """
 
         with self._session as session:
             return session.query(Event).filter(
                 Event.user_id == self._owner.id
             ).all()
 
-    def get_all_events_page(self, page: int, per_page: int) -> list:
+    def get_all_events_page(
+        self, page: int, per_page: int
+    ) -> List[Type[Event]]:
         """Get a single page of events associated with a user from the database
 
         Parameters
         ----------
         page : int
             The page number
         per_page : int
@@ -224,15 +236,17 @@
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(Event).filter(
                 Event.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def append_characters_to_event(self, event_id: int, character_ids: list) -> Type[Event]:
+    def append_characters_to_event(
+        self, event_id: int, character_ids: list
+    ) -> Type[Event]:
         """Append characters to an event
 
         Parameters
         ----------
         event_id : int
             The id of the event
         character_ids : list
@@ -243,46 +257,56 @@
         Event
             The updated event object
         """
 
         with self._session as session:
             try:
                 event = session.query(Event).filter(
-                    Event.id == event_id, Event.user_id == self._owner.id
+                    Event.id == event_id,
+                    Event.user_id == self._owner.id
                 ).first()
 
                 if not event:
                     raise ValueError('Event not found.')
 
                 for character_id in character_ids:
                     character = session.query(Character).filter(
-                        Character.id == character_id, Character.user_id == self._owner.id
+                        Character.id == character_id,
+                        Character.user_id == self._owner.id
                     ).first()
 
                     if not character:
                         raise ValueError('Character not found.')
 
-                    character_event = CharacterEvent(user_id=self._owner.id, event_id=event_id,
-                                                     character_id=character_id, created=datetime.now())
-
-                    activity = Activity(user_id=self._owner.id, summary=f'Character {character.__str__} associated with\
-                                         event {event.title[:50]} by {self._owner.username}', created=datetime.now())
+                    character_event = CharacterEvent(
+                        user_id=self._owner.id, event_id=event_id,
+                        character_id=character_id, created=datetime.now()
+                    )
+
+                    activity = Activity(
+                        user_id=self._owner.id, summary=f'Character \
+                        {character.__str__} associated with event \
+                        {event.title[:50]} by {self._owner.username}',
+                        created=datetime.now()
+                    )
 
                     session.add(character_event)
                     session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return event
 
-    def get_characters_by_event_id(self, event_id: int) -> list:
+    def get_characters_by_event_id(
+        self, event_id: int
+    ) -> List[Type[Character]]:
         """Get all characters associated with an event
 
         Parameters
         ----------
         event_id : int
             The id of the event
 
@@ -290,19 +314,24 @@
         -------
         list
             A list of character objects
         """
 
         with self._session as session:
             for character_event in session.query(CharacterEvent).filter(
-                CharacterEvent.event_id == event_id, CharacterEvent.user_id == self._owner.id
+                CharacterEvent.event_id == event_id,
+                    CharacterEvent.user_id == self._owner.id
             ).all():
-                yield session.query(Character).filter(Character.id == character_event.character_id).first()
+                yield session.query(Character).filter(
+                    Character.id == character_event.character_id
+                ).first()
 
-    def get_characters_page_by_event_id(self, event_id: int, page: int, per_page: int) -> list:
+    def get_characters_page_by_event_id(
+        self, event_id: int, page: int, per_page: int
+    ) -> List[Type[Character]]:
         """Get a single page of characters associated with an event from the database
 
         Parameters
         ----------
         event_id : int
             The id of the event
         page : int
@@ -315,21 +344,25 @@
         list
             A list of character objects
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             for character_event in session.query(CharacterEvent).filter(
-                CharacterEvent.event_id == event_id, CharacterEvent.user_id == self._owner.id
+                CharacterEvent.event_id == event_id,
+                CharacterEvent.user_id == self._owner.id
             ).offset(offset).limit(per_page).all():
                 yield session.query(Character).filter(
-                    Character.id == character_event.character_id, Character.user_id == self._owner.id
+                    Character.id == character_event.character_id,
+                    Character.user_id == self._owner.id
                 ).first()
 
-    def append_locations_to_event(self, event_id: int, location_ids: list) -> Type[Event]:
+    def append_locations_to_event(
+        self, event_id: int, location_ids: list
+    ) -> Type[Event]:
         """Append locations to an event
 
         Parameters
         ----------
         event_id : int
             The id of the event
         location_ids : list
@@ -340,46 +373,54 @@
         Event
             The updated event object
         """
 
         with self._session as session:
             try:
                 event = session.query(Event).filter(
-                    Event.id == event_id, Event.user_id == self._owner.id
+                    Event.id == event_id,
+                    Event.user_id == self._owner.id
                 ).first()
 
                 if not event:
                     raise ValueError('Event not found.')
 
                 for location_id in location_ids:
                     location = session.query(Location).filter(
-                        Location.id == location_id, Location.user_id == self._owner.id
+                        Location.id == location_id,
+                        Location.user_id == self._owner.id
                     ).first()
 
                     if not location:
                         raise ValueError('Location not found.')
 
-                    event_location = EventLocation(user_id=self._owner.id, event_id=event_id, location_id=location_id,
-                                                   created=datetime.now())
-
-                    activity = Activity(user_id=self._owner.id, summary=f'Location {location.name[:50]} associated with\
-                                         event {event.title[:50]} by {self._owner.username}', created=datetime.now())
+                    event_location = EventLocation(
+                        user_id=self._owner.id, event_id=event_id,
+                        location_id=location_id, created=datetime.now()
+                    )
+
+                    activity = Activity(
+                        user_id=self._owner.id, summary=f'Location \
+                        {location.name[:50]} associated with event \
+                        {event.title[:50]} by {self._owner.username}',
+                        created=datetime.now()
+                    )
 
                     session.add(event_location)
                     session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return event
 
-    def get_locations_by_event_id(self, event_id: int) -> list:
+    def get_locations_by_event_id(self, event_id: int) -> List[Type[Location]]:
         """Get all locations associated with an event
 
         Parameters
         ----------
         event_id : int
             The id of the event
 
@@ -387,21 +428,25 @@
         -------
         list
             A list of location objects
         """
 
         with self._session as session:
             for event_location in session.query(EventLocation).filter(
-                EventLocation.event_id == event_id, EventLocation.user_id == self._owner.id
+                EventLocation.event_id == event_id,
+                    EventLocation.user_id == self._owner.id
             ).all():
                 yield session.query(Location).filter(
-                    Location.id == event_location.location_id, Location.user_id == self._owner.id
+                    Location.id == event_location.location_id,
+                    Location.user_id == self._owner.id
                 ).first()
 
-    def append_links_to_event(self, event_id: int, link_ids: list) -> Type[Event]:
+    def append_links_to_event(
+        self, event_id: int, link_ids: list
+    ) -> Type[Event]:
         """Append links to an event
 
         Parameters
         ----------
         event_id : int
             The id of the event
         link_ids : list
@@ -412,46 +457,54 @@
         Event
             The updated event object
         """
 
         with self._session as session:
             try:
                 event = session.query(Event).filter(
-                    Event.id == event_id, Event.user_id == self._owner.id
+                    Event.id == event_id,
+                    Event.user_id == self._owner.id
                 ).first()
 
                 if not event:
                     raise ValueError('Event not found.')
 
                 for link_id in link_ids:
                     link = session.query(Link).filter(
-                        Link.id == link_id, Link.user_id == self._owner.id
+                        Link.id == link_id,
+                        Link.user_id == self._owner.id
                     ).first()
 
                     if not link:
                         raise ValueError('Link not found.')
 
-                    event_link = EventLink(user_id=self._owner.id, event_id=event_id, link_id=link_id,
-                                           created=datetime.now())
-
-                    activity = Activity(user_id=self._owner.id, summary=f'Link {link.title[:50]} associated with \
-                                        event {event.title[:50]} by {self._owner.username}', created=datetime.now())
+                    event_link = EventLink(
+                        user_id=self._owner.id, event_id=event_id,
+                        link_id=link_id, created=datetime.now()
+                    )
+
+                    activity = Activity(
+                        user_id=self._owner.id, summary=f'Link\
+                        {link.title[:50]} associated with event \
+                        {event.title[:50]} by {self._owner.username}',
+                        created=datetime.now()
+                    )
 
                     session.add(event_link)
                     session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return event
 
-    def get_links_by_event_id(self, event_id: int) -> list:
+    def get_links_by_event_id(self, event_id: int) -> List[Type[Link]]:
         """Get all links associated with an event
 
         Parameters
         ----------
         event_id : int
             The id of the event
 
@@ -459,21 +512,26 @@
         -------
         list
             A list of link objects
         """
 
         with self._session as session:
             for event_link in session.query(EventLink).filter(
-                EventLink.event_id == event_id, EventLink.user_id == self._owner.id
+                EventLink.event_id == event_id,
+                    EventLink.user_id == self._owner.id
             ).all():
                 yield session.query(Link).filter(
-                    Link.id == event_link.link_id, Link.user_id == self._owner.id
+                    Link.id == event_link.link_id,
+                    Link.user_id == self._owner.id
                 ).first()
 
-    def get_links_page_by_event_id(self, event_id: int, page: int, per_page: int) -> list:
+    def get_links_page_by_event_id(
+        self, event_id: int, page: int, per_page: int
+    ) -> List[Type[Link]]:
+
         """Get a single page of links associated with an event from the database
 
         Parameters
         ----------
         event_id : int
             The id of the event
         page : int
@@ -486,18 +544,21 @@
         list
             A list of link objects
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(EventLink).filter(
-                EventLink.event_id == event_id, EventLink.user_id == self._owner.id
+                EventLink.event_id == event_id,
+                EventLink.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def append_notes_to_event(self, event_id: int, note_ids: list) -> Type[Event]:
+    def append_notes_to_event(
+        self, event_id: int, note_ids: list
+    ) -> Type[Event]:
         """Append notes to an event
 
         Parameters
         ----------
         event_id : int
             The id of the event
         note_ids : list
@@ -508,46 +569,54 @@
         Event
             The updated event object
         """
 
         with self._session as session:
             try:
                 event = session.query(Event).filter(
-                    Event.id == event_id, Event.user_id == self._owner.id
+                    Event.id == event_id,
+                    Event.user_id == self._owner.id
                 ).first()
 
                 if not event:
                     raise ValueError('Event not found.')
 
                 for note_id in note_ids:
                     note = session.query(Note).filter(
-                        Note.id == note_id, Note.user_id == self._owner.id
+                        Note.id == note_id,
+                        Note.user_id == self._owner.id
                     ).first()
 
                     if not note:
                         raise ValueError('Note not found.')
 
-                    event_note = EventNote(user_id=self._owner.id, event_id=event_id, note_id=note_id,
-                                           created=datetime.now())
-
-                    activity = Activity(user_id=self._owner.id, summary=f'Note {note.title[:50]} associated with \
-                                        event {event.title[:50]} by {self._owner.username}', created=datetime.now())
+                    event_note = EventNote(
+                        user_id=self._owner.id, event_id=event_id,
+                        note_id=note_id, created=datetime.now()
+                    )
+
+                    activity = Activity(
+                        user_id=self._owner.id, summary=f'Note \
+                        {note.title[:50]} associated with event \
+                        {event.title[:50]} by {self._owner.username}',
+                        created=datetime.now()
+                    )
 
                     session.add(event_note)
                     session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return event
 
-    def get_notes_by_event_id(self, event_id: int) -> list:
+    def get_notes_by_event_id(self, event_id: int) -> List[Type[Note]]:
         """Get all notes associated with an event
 
         Parameters
         ----------
         event_id : int
             The id of the event
 
@@ -555,21 +624,25 @@
         -------
         list
             A list of note objects
         """
 
         with self._session as session:
             for event_note in session.query(EventNote).filter(
-                EventNote.event_id == event_id, EventNote.user_id == self._owner.id
+                EventNote.event_id == event_id,
+                    EventNote.user_id == self._owner.id
             ).all():
                 yield session.query(Note).filter(
-                    Note.id == event_note.note_id, Note.user_id == self._owner.id
+                    Note.id == event_note.note_id,
+                    Note.user_id == self._owner.id
                 ).first()
 
-    def get_notes_page_by_event_id(self, event_id: int, page: int, per_page: int) -> list:
+    def get_notes_page_by_event_id(
+        self, event_id: int, page: int, per_page: int
+    ) -> List[Type[Note]]:
         """Get a single page of notes associated with an event from the database
 
         Parameters
         ----------
         event_id : int
             The id of the event
         page : int
@@ -582,9 +655,10 @@
         list
             A list of note objects
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(EventNote).filter(
-                EventNote.event_id == event_id, EventNote.user_id == self._owner.id
+                EventNote.event_id == event_id,
+                EventNote.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
```

### Comparing `noveler-0.1.0/noveler/controllers/ExportController.py` & `noveler-0.1.1/noveler/controllers/ExportController.py`

 * *Files 5% similar despite different names*

```diff
@@ -301,20 +301,58 @@
                 output.write(
                     f"Character Profile for {dict_character['full_name']}"
                 )
 
                 if dict_character['description']:
                     output.write(f"\n\n{dict_character['description']}")
 
+                if dict_character['wounds']:
+                    output.write(f"\n\nThe character's wounds:\n{dict_character['wounds']}")
+
                 if dict_character["gender"]:
                     output.write(f"\n\nGender: {dict_character['gender']}")
 
                 if dict_character["sex"]:
                     output.write(f"\nSex: {dict_character['sex']}")
 
+                if dict_character["ethnicity"]:
+                    output.write(f"\nEthnicity: {dict_character['ethnicity']}")
+
+                if dict_character["race"]:
+                    output.write(f"\nRace: {dict_character['race']}")
+
+                if dict_character["tribe_or_clan"]:
+                    output.write(f"\nTribe or Clan: {dict_character['tribe_or_clan']}")
+
+                if dict_character["nationality"]:
+                    output.write(f"\nNationality: {dict_character['nationality']}")
+
+                if dict_character["religion"]:
+                    output.write(f"\nReligion: {dict_character['religion']}")
+
+                if dict_character["mbti"]:
+                    output.write(f"\nMyers-Briggs Type Indicator: {dict_character['mbti']}")
+
+                if dict_character["enneagram"]:
+                    output.write(f"\nEnneagram Type: {dict_character['enneagram']}")
+
+                if dict_character["occupation"]:
+                    output.write(f"\nOccupation: {dict_character['occupation']}")
+
+                if dict_character["education"]:
+                    output.write(f"\nEducation: {dict_character['education']}")
+
+                if dict_character["marital_status"]:
+                    output.write(f"\nMarital Status: {dict_character['marital_status']}")
+
+                if dict_character["children"]:
+                    output.write(f"\nThis character has or had children.")
+                else:
+                    output.write(f"\nThis character has no children.")
+
                 if dict_character["age"]:
                     output.write(f"\nAge: {dict_character['age']}")
 
                 if dict_character["date_of_birth"]:
                     output.write(f"\nDate of Birth: {dict_character['date_of_birth']}")
 
                 if dict_character["date_of_death"]:
```

### Comparing `noveler-0.1.0/noveler/controllers/ImageController.py` & `noveler-0.1.1/noveler/controllers/ImageController.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Type
+from typing import Type, List
 from sqlalchemy.orm import Session
 from noveler.controllers.BaseController import BaseController
 from noveler.models import User, Image, Activity, ImageLocation
 
 
 class ImageController(BaseController):
     """Image controller encapsulates image management functionality
@@ -38,22 +38,23 @@
     get_images_by_location_id(location_id: int)
         Get all images associated with a location
     get_images_page_by_location_id(location_id: int, page: int, per_page: int)
         Get a single page of images associated with a location from the database
     """
 
     def __init__(
-            self, path_to_config: str, session: Session, owner: Type[User]
+        self, path_to_config: str, session: Session, owner: Type[User]
     ):
         """Initialize the class"""
 
         super().__init__(path_to_config, session, owner)
 
     def create_image(
-            self, filename: str, dirname: str, size_in_bytes: int, mime_type: str, caption: str = None
+        self, filename: str, dirname: str, size_in_bytes: int, mime_type: str,
+        caption: str = None
     ) -> Image:
         """Create a new image
 
         Parameters
         ----------
         filename : str
             The filename of the image
@@ -73,20 +74,24 @@
         """
 
         with self._session as session:
             try:
                 created = datetime.now()
                 modified = created
 
-                image = Image(user_id=self._owner.id, caption=caption, filename=filename, dirname=dirname,
-                              size_in_bytes=size_in_bytes, mime_type=mime_type, created=created, modified=modified)
-
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Image {image.id} created by {self._owner.username}',
-                                    created=datetime.now())
+                image = Image(
+                    user_id=self._owner.id, caption=caption, filename=filename,
+                    dirname=dirname, size_in_bytes=size_in_bytes,
+                    mime_type=mime_type, created=created, modified=modified
+                )
+
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Image {image.id} created \
+                    by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(image)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
@@ -110,26 +115,28 @@
         Image
             The updated image object
         """
 
         with self._session as session:
             try:
                 image = session.query(Image).filter(
-                    Image.id == image_id, Image.user_id == self._owner.id
+                    Image.id == image_id,
+                    Image.user_id == self._owner.id
                 ).first()
 
                 if not image:
                     raise ValueError('Image not found.')
 
                 image.caption = caption
                 image.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Image {image.id} updated by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Image {image.id} updated \
+                    by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
@@ -150,50 +157,54 @@
         bool
             True on success
         """
 
         with self._session as session:
             try:
                 image = session.query(Image).filter(
-                    Image.id == image_id, Image.user_id == self._owner.id
+                    Image.id == image_id,
+                    Image.user_id == self._owner.id
                 ).first()
 
                 if not image:
                     raise ValueError('Image not found.')
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Image {image.id} deleted by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Image {image.id} deleted \
+                    by {self._owner.username}', created=datetime.now()
+                )
 
                 session.delete(image)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return True
 
-    def get_all_images(self) -> list:
+    def get_all_images(self) -> List[Type[Image]]:
         """Get all images associated with a user
 
         Returns
         -------
         list
             A list of image objects
         """
 
         with self._session as session:
             return session.query(Image).filter(
                 Image.user_id == self._owner.id
             ).all()
 
-    def get_all_images_page(self, page: int, per_page: int) -> list:
+    def get_all_images_page(
+        self, page: int, per_page: int
+    ) -> List[Type[Image]]:
         """Get a single page of images associated with a user from the database
 
         Parameters
         ----------
         page : int
             The page number
         per_page : int
@@ -207,15 +218,15 @@
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(Image).filter(
                 Image.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def search_images(self, search: str) -> list:
+    def search_images(self, search: str) -> List[Type[Image]]:
         """Search for images by caption
 
         Parameters
         ----------
         search : str
             The search string
 
@@ -223,18 +234,21 @@
         -------
         list
             A list of image objects
         """
 
         with self._session as session:
             return session.query(Image).filter(
-                Image.caption.like(f'%{search}%'), Image.user_id == self._owner.id
+                Image.caption.like(f'%{search}%'),
+                Image.user_id == self._owner.id
             ).all()
 
-    def get_images_by_character_id(self, character_id: int) -> list:
+    def get_images_by_character_id(
+        self, character_id: int
+    ) -> List[Type[Image]]:
         """Get all images associated with a character
 
         Parameters
         ----------
         character_id : int
             The id of the character
 
@@ -242,18 +256,21 @@
         -------
         list
             A list of image objects
         """
 
         with self._session as session:
             return session.query(Image).filter(
-                Image.character_id == character_id, Image.user_id == self._owner.id
+                Image.character_id == character_id,
+                Image.user_id == self._owner.id
             ).all()
 
-    def get_images_page_by_character_id(self, character_id: int, page: int, per_page: int) -> list:
+    def get_images_page_by_character_id(
+        self, character_id: int, page: int, per_page: int
+    ) -> List[Type[Image]]:
         """Get a single page of images associated with a character from the database
 
         Parameters
         ----------
         character_id : int
             The id of the character
         page : int
@@ -266,18 +283,19 @@
         list
             A list of image objects
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(Image).filter(
-                Image.character_id == character_id, Image.user_id == self._owner.id
+                Image.character_id == character_id,
+                Image.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def get_images_by_location_id(self, location_id: int) -> list:
+    def get_images_by_location_id(self, location_id: int) -> List[Type[Image]]:
         """Get all images associated with a location
 
         Images and Locations are associated through ImageLocation objects. This method will use yield to return the
         images one at a time.
 
         Parameters
         ----------
@@ -288,21 +306,25 @@
         -------
         list
             A list of image objects
         """
 
         with self._session as session:
             for image_location in session.query(ImageLocation).filter(
-                ImageLocation.location_id == location_id, ImageLocation.user_id == self._owner.id
+                ImageLocation.location_id == location_id,
+                    ImageLocation.user_id == self._owner.id
             ).all():
                 yield session.query(Image).filter(
-                    Image.id == image_location.image_id, Image.user_id == self._owner.id
+                    Image.id == image_location.image_id,
+                    Image.user_id == self._owner.id
                 ).first()
 
-    def get_images_page_by_location_id(self, location_id: int, page: int, per_page: int) -> list:
+    def get_images_page_by_location_id(
+        self, location_id: int, page: int, per_page: int
+    ) -> List[Type[Image]]:
         """Get a single page of images associated with a location from the database
 
         Images and Locations are associated through ImageLocation objects. This method will use yield to return the
         images one at a time.
 
         Parameters
         ----------
@@ -318,12 +340,14 @@
         list
             A list of image objects
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             for image_location in session.query(ImageLocation).filter(
-                ImageLocation.location_id == location_id, ImageLocation.user_id == self._owner.id
+                ImageLocation.location_id == location_id,
+                ImageLocation.user_id == self._owner.id
             ).offset(offset).limit(per_page).all():
                 yield session.query(Image).filter(
-                    Image.id == image_location.image_id, Image.user_id == self._owner.id
+                    Image.id == image_location.image_id,
+                    Image.user_id == self._owner.id
                 ).first()
```

### Comparing `noveler-0.1.0/noveler/controllers/LinkController.py` & `noveler-0.1.1/noveler/controllers/LinkController.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from datetime import datetime
-from typing import Type
+from typing import Type, List
 from sqlalchemy.orm import Session
 from noveler.controllers.BaseController import BaseController
 from noveler.models import User, Link, Activity, LinkStory
 
 
 class LinkController(BaseController):
     """Link controller encapsulates link management functionality
 
     Attributes
     ----------
-    _self : LinkController
+    _instance : LinkController
         The instance of the link controller
     _owner : User
         The current user of the link controller
     _session : Session
         The database session
 
     Methods
@@ -32,15 +32,15 @@
     get_all_links_page(page: int, per_page: int)
         Get a single page of links associated with a user from the database
     search_links(search: str)
         Search for links by title
     """
 
     def __init__(
-            self, path_to_config: str, session: Session, owner: Type[User]
+        self, path_to_config: str, session: Session, owner: Type[User]
     ):
         """Initialize the class"""
 
         super().__init__(path_to_config, session, owner)
 
     def create_link(self, url: str, title: str) -> Link:
         """Create a new link
@@ -59,19 +59,23 @@
         """
 
         with self._session as session:
             try:
                 created = datetime.now()
                 modified = created
 
-                link = Link(user_id=self._owner.id, url=url, title=title, created=created, modified=modified)
-
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Link {link.title[:50]} created by {self._owner.username}',
-                                    created=datetime.now())
+                link = Link(
+                    user_id=self._owner.id, url=url, title=title,
+                    created=created, modified=modified
+                )
+
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Link {link.title[:50]} \
+                    created by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(link)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
@@ -97,27 +101,29 @@
         Link
             The updated link object
         """
 
         with self._session as session:
             try:
                 link = session.query(Link).filter(
-                    Link.id == link_id, Link.user_id == self._owner.id
+                    Link.id == link_id,
+                    Link.user_id == self._owner.id
                 ).first()
 
                 if not link:
                     raise ValueError('Link not found.')
 
                 link.url = url
                 link.title = title
                 link.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Link {link.id} updated by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Link {link.id} updated \
+                    by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
@@ -138,23 +144,25 @@
         bool
             True on success
         """
 
         with self._session as session:
             try:
                 link = session.query(Link).filter(
-                    Link.id == link_id, Link.user_id == self._owner.id
+                    Link.id == link_id,
+                    Link.user_id == self._owner.id
                 ).first()
 
                 if not link:
                     raise ValueError('Link not found.')
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Link {link.id} deleted by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Link {link.id} deleted \
+                    by {self._owner.username}', created=datetime.now()
+                )
 
                 session.delete(link)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
@@ -175,18 +183,19 @@
         -------
         Link
             The link object
         """
 
         with self._session as session:
             return session.query(Link).filter(
-                Link.id == link_id, Link.user_id == self._owner.id
+                Link.id == link_id,
+                Link.user_id == self._owner.id
             ).first()
 
-    def get_links_by_story_id(self, story_id: int) -> list:
+    def get_links_by_story_id(self, story_id: int) -> List[Type[Link]]:
         """Get all links associated with a story
 
         The LinkStory objects are the associations between links and stories. This method returns a list of links
         associated with a story.
 
         Parameters
         ----------
@@ -197,30 +206,33 @@
         -------
         list
             A list of link objects
         """
 
         with self._session as session:
             return session.query(Link).join(LinkStory).filter(
-                LinkStory.story_id == story_id, LinkStory.user_id == self._owner.id
+                LinkStory.story_id == story_id,
+                LinkStory.user_id == self._owner.id
             ).all()
 
-    def get_all_links(self) -> list:
+    def get_all_links(self) -> List[Type[Link]]:
         """Get all links associated with an owner
 
         Returns
         -------
         list
             A list of link objects
         """
 
         with self._session as session:
-            return session.query(Link).filter(Link.user_id == self._owner.id).all()
+            return session.query(Link).filter(
+                Link.user_id == self._owner.id
+            ).all()
 
-    def get_all_links_page(self, page: int, per_page: int) -> list:
+    def get_all_links_page(self, page: int, per_page: int) -> List[Type[Link]]:
         """Get a single page of links associated with an owner from the database
 
         Parameters
         ----------
         page : int
             The page number
         per_page : int
@@ -230,17 +242,19 @@
         -------
         list
             A list of link objects
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
-            return session.query(Link).filter(Link.user_id == self._owner.id).offset(offset).limit(per_page).all()
+            return session.query(Link).filter(
+                Link.user_id == self._owner.id
+            ).offset(offset).limit(per_page).all()
 
-    def search_links(self, search: str) -> list:
+    def search_links(self, search: str) -> List[Type[Link]]:
         """Search for links by title
 
         Parameters
         ----------
         search : str
             The search string
 
@@ -248,9 +262,10 @@
         -------
         list
             A list of link objects
         """
 
         with self._session as session:
             return session.query(Link).filter(
-                Link.title.like(f'%{search}%'), Link.user_id == self._owner.id
+                Link.title.like(f'%{search}%'),
+                Link.user_id == self._owner.id
             ).all()
```

### Comparing `noveler-0.1.0/noveler/controllers/LocationController.py` & `noveler-0.1.1/noveler/controllers/LocationController.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from datetime import datetime
-from typing import Type
+from typing import Type, List
 from sqlalchemy import or_, func
 from sqlalchemy.orm import Session
 from noveler.controllers.BaseController import BaseController
 from noveler.models import User, Location, Activity, Image, ImageLocation, Link, LinkLocation, Note, LocationNote
 
 
 class LocationController(BaseController):
     """Location controller encapsulates location management functionality
 
     Attributes
     ----------
-    _self : LocationController
+    _instance : LocationController
         The instance of the location controller
     _owner : User
         The current user of the location controller
     _session : Session
         The database session
 
     Methods
@@ -61,23 +61,25 @@
     get_notes_by_location_id(location_id: int)
         Get all notes associated with a location
     get_notes_page_by_location_id(location_id: int, page: int, per_page: int)
         Get a single page of notes associated with a location from the database
     """
 
     def __init__(
-            self, path_to_config: str, session: Session, owner: Type[User]
+        self, path_to_config: str, session: Session, owner: Type[User]
     ):
         """Initialize the class"""
 
         super().__init__(path_to_config, session, owner)
 
-    def create_location(self, title: str, description: str = None, address: str = None, city: str = None,
-                        state: str = None, country: str = None, zip_code: str = None, latitude: float = None,
-                        longitude: float = None) -> Location:
+    def create_location(
+        self, title: str, description: str = None, address: str = None,
+        city: str = None, state: str = None, country: str = None,
+        zip_code: str = None, latitude: float = None, longitude: float = None
+    ) -> Location:
         """Create a new location
 
         Parameters
         ----------
         title : str
             The title of the location
         description : str
@@ -104,36 +106,44 @@
         """
 
         with self._session as session:
             try:
                 created = datetime.now()
                 modified = created
 
-                location = Location(user_id=self._owner.id, title=title, description=description, address=address,
-                                    city=city, state=state, country=country, zip_code=zip_code, latitude=latitude,
-                                    longitude=longitude, created=created, modified=modified)
-
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Location {location.id} created by {self._owner.username}',
-                                    created=datetime.now())
+                location = Location(
+                    user_id=self._owner.id, title=title,
+                    description=description, address=address, city=city,
+                    state=state, country=country, zip_code=zip_code,
+                    latitude=latitude, longitude=longitude, created=created,
+                    modified=modified
+                )
+
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Location {location.id} \
+                    created by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(location)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return location
 
-    def update_location(self, location_id: int, title: str, description: str = None, address: str = None,
-                        city: str = None, state: str = None, country: str = None, zip_code: str = None,
-                        latitude: float = None, longitude: float = None) -> Type[Location]:
+    def update_location(
+        self, location_id: int, title: str, description: str = None,
+        address: str = None, city: str = None, state: str = None,
+        country: str = None, zip_code: str = None, latitude: float = None,
+        longitude: float = None
+    ) -> Type[Location]:
         """Update a location
 
         Parameters
         ----------
         location_id : int
             The id of the location
         title : str
@@ -160,15 +170,16 @@
         bool
             True on success
         """
 
         with self._session as session:
             try:
                 location = session.query(Location).filter(
-                    Location.id == location_id, Location.user_id == self._owner.id
+                    Location.id == location_id,
+                    Location.user_id == self._owner.id
                 ).first()
 
                 if not location:
                     raise ValueError('Location not found.')
 
                 location.title = title
                 location.description = description
@@ -177,17 +188,18 @@
                 location.state = state
                 location.country = country
                 location.zip_code = zip_code
                 location.latitude = latitude
                 location.longitude = longitude
                 location.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Location {location.id} updated by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Location {location.id} \
+                    updated by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
@@ -208,48 +220,54 @@
         bool
             True on success
         """
 
         with self._session as session:
             try:
                 location = session.query(Location).filter(
-                    Location.id == location_id, Location.user_id == self._owner.id
+                    Location.id == location_id,
+                    Location.user_id == self._owner.id
                 ).first()
 
                 if not location:
                     raise ValueError('Location not found.')
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Location {location.id} deleted by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Location {location.id} \
+                    deleted by {self._owner.username}', created=datetime.now()
+                )
 
                 session.delete(location)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return True
 
-    def get_all_locations(self) -> list:
+    def get_all_locations(self) -> List[Type[Location]]:
         """Get all locations associated with an owner
 
         Returns
         -------
         list
             A list of location objects
         """
 
         with self._session as session:
-            return session.query(Location).filter(Location.user_id == self._owner.id).all()
+            return session.query(Location).filter(
+                Location.user_id == self._owner.id
+            ).all()
 
-    def get_all_locations_page(self, page: int, per_page: int) -> list:
+    def get_all_locations_page(
+        self, page: int, per_page: int
+    ) -> List[Type[Location]]:
         """Get a single page of locations associated with an owner from the database
 
         Parameters
         ----------
         page : int
             The page number
         per_page : int
@@ -263,15 +281,17 @@
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(Location).filter(
                 Location.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def search_locations_by_title_and_description(self, search: str) -> list:
+    def search_locations_by_title_and_description(
+        self, search: str
+    ) -> List[Type[Location]]:
         """Search for locations by title and description
 
         Parameters
         ----------
         search : str
             The search string
 
@@ -280,18 +300,21 @@
         list
             A list of location objects
         """
 
         with self._session as session:
             return session.query(Location).filter(
                 Location.user_id == self._owner.id,
-                or_(Location.title.like(f'%{search}%'), Location.description.like(f'%{search}%'))
+                or_(
+                    Location.title.like(f'%{search}%'),
+                    Location.description.like(f'%{search}%')
+                )
             ).all()
 
-    def search_locations_by_address(self, search: str) -> list:
+    def search_locations_by_address(self, search: str) -> List[Type[Location]]:
         """Search for locations by address
 
         Parameters
         ----------
         search : str
             The search string
 
@@ -299,18 +322,19 @@
         -------
         list
             A list of location objects
         """
 
         with self._session as session:
             return session.query(Location).filter(
-                Location.address.like(f'%{search}%'), Location.user_id == self._owner.id
+                Location.address.like(f'%{search}%'),
+                Location.user_id == self._owner.id
             ).all()
 
-    def search_locations_by_city(self, search: str) -> list:
+    def search_locations_by_city(self, search: str) -> List[Type[Location]]:
         """Search for locations by city
 
         Parameters
         ----------
         search : str
             The search string
 
@@ -318,18 +342,19 @@
         -------
         list
             A list of location objects
         """
 
         with self._session as session:
             return session.query(Location).filter(
-                Location.city.like(f'%{search}%'), Location.user_id == self._owner.id
+                Location.city.like(f'%{search}%'),
+                Location.user_id == self._owner.id
             ).all()
 
-    def search_locations_by_state(self, search: str) -> list:
+    def search_locations_by_state(self, search: str) -> List[Type[Location]]:
         """Search for locations by state
 
         Parameters
         ----------
         search : str
             The search string
 
@@ -337,18 +362,19 @@
         -------
         list
             A list of location objects
         """
 
         with self._session as session:
             return session.query(Location).filter(
-                Location.state.like(f'%{search}%'), Location.user_id == self._owner.id
+                Location.state.like(f'%{search}%'),
+                Location.user_id == self._owner.id
             ).all()
 
-    def search_locations_by_country(self, search: str) -> list:
+    def search_locations_by_country(self, search: str) -> List[Type[Location]]:
         """Search for locations by country
 
         Parameters
         ----------
         search : str
             The search string
 
@@ -356,18 +382,19 @@
         -------
         list
             A list of location objects
         """
 
         with self._session as session:
             return session.query(Location).filter(
-                Location.country.like(f'%{search}%'), Location.user_id == self._owner.id
+                Location.country.like(f'%{search}%'),
+                Location.user_id == self._owner.id
             ).all()
 
-    def search_locations_by_zip_code(self, search: str) -> list:
+    def search_locations_by_zip_code(self, search: str) -> List[Type[Location]]:
         """Search for locations by zip code
 
         Parameters
         ----------
         search : str
             The search string
 
@@ -375,18 +402,21 @@
         -------
         list
             A list of location objects
         """
 
         with self._session as session:
             return session.query(Location).filter(
-                Location.zip_code.like(f'%{search}%'), Location.user_id == self._owner.id
+                Location.zip_code.like(f'%{search}%'),
+                Location.user_id == self._owner.id
             ).all()
 
-    def append_images_to_location(self, location_id: int, image_ids: list) -> Type[Location]:
+    def append_images_to_location(
+        self, location_id: int, image_ids: list
+    ) -> Type[Location]:
         """Append images to a location
 
         Parameters
         ----------
         location_id : int
             The id of the location
         image_ids : list
@@ -397,55 +427,66 @@
         Location
             The updated location object
         """
 
         with self._session as session:
             try:
                 location = session.query(Location).filter(
-                    Location.id == location_id, Location.user_id == self._owner.id
+                    Location.id == location_id,
+                    Location.user_id == self._owner.id
                 ).first()
 
                 if not location:
                     raise ValueError('Location not found.')
 
                 for image_id in image_ids:
                     image = session.query(Image).filter(
-                        Image.id == image_id, Image.user_id == self._owner.id
+                        Image.id == image_id,
+                        Image.user_id == self._owner.id
                     ).first()
 
                     if not image:
                         raise ValueError('Image not found.')
 
-                    position = session.query(func.max(ImageLocation.position)).filter(
+                    position = session.query(
+                        func.max(ImageLocation.position)
+                    ).filter(
                         ImageLocation.location_id == location_id
                     ).scalar()
                     position = position + 1 if position else 1
                     is_default = False
                     created = datetime.now()
                     modified = created
-                    image_location = ImageLocation(user_id=self._owner.id, location_id=location_id, image_id=image_id,
-                                                   position=position, is_default=is_default, created=created,
-                                                   modified=modified)
-
-                    activity = Activity(user_id=self._owner.id, summary=f'Image {image.caption[:50]} associated with \
-                                        location {location.title[:50]} by {self._owner.username}',
-                                        created=datetime.now())
+
+                    image_location = ImageLocation(
+                        user_id=self._owner.id, location_id=location_id,
+                        image_id=image_id, position=position,
+                        is_default=is_default, created=created,
+                        modified=modified
+                    )
+
+                    activity = Activity(
+                        user_id=self._owner.id, summary=f'Image \
+                        {image.caption[:50]} associated with location \
+                        {location.title[:50]} by {self._owner.username}',
+                        created=datetime.now()
+                    )
 
                     session.add(image_location)
                     session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return location
 
-    def get_images_by_location_id(self, location_id: int) -> list:
+    def get_images_by_location_id(self, location_id: int) -> List[Type[Image]]:
         """Get all images associated with a location
 
         The images should be returned in the order determined by the position field in the ImageLocation table.
 
         Parameters
         ----------
         location_id : int
@@ -457,23 +498,25 @@
             A list of image objects
         """
 
         with self._session as session:
 
             for image_location in session.query(ImageLocation).filter(
                 ImageLocation.location_id == location_id,
-                    ImageLocation.user_id == self._owner.id
+                ImageLocation.user_id == self._owner.id
             ).order_by(ImageLocation.position).all():
 
                 yield session.query(Image).filter(
                     Image.id == image_location.image_id,
                     Image.user_id == self._owner.id
                 ).first()
 
-    def get_images_page_by_location_id(self, location_id: int, page: int, per_page: int) -> list:
+    def get_images_page_by_location_id(
+        self, location_id: int, page: int, per_page: int
+    ) -> List[Type[Image]]:
         """Get a single page of images associated with a location from the database
 
         Parameters
         ----------
         location_id : int
             The id of the location
         page : int
@@ -486,18 +529,21 @@
         list
             A list of image objects
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(ImageLocation).filter(
-                ImageLocation.location_id == location_id, ImageLocation.user_id == self._owner.id
+                ImageLocation.location_id == location_id,
+                ImageLocation.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def append_links_to_location(self, location_id: int, link_ids: list) -> Type[Location]:
+    def append_links_to_location(
+        self, location_id: int, link_ids: list
+    ) -> Type[Location]:
         """Append links to a location
 
         Parameters
         ----------
         location_id : int
             The id of the location
         link_ids : list
@@ -508,47 +554,54 @@
         Location
             The updated location object
         """
 
         with self._session as session:
             try:
                 location = session.query(Location).filter(
-                    Location.id == location_id, Location.user_id == self._owner.id
+                    Location.id == location_id,
+                    Location.user_id == self._owner.id
                 ).first()
 
                 if not location:
                     raise ValueError('Location not found.')
 
                 for link_id in link_ids:
                     link = session.query(Link).filter(
-                        Link.id == link_id, Link.user_id == self._owner.id
+                        Link.id == link_id,
+                        Link.user_id == self._owner.id
                     ).first()
 
                     if not link:
                         raise ValueError('Link not found.')
 
-                    link_location = LinkLocation(user_id=self._owner.id, location_id=location_id, link_id=link_id,
-                                                 created=datetime.now())
-
-                    activity = Activity(user_id=self._owner.id, summary=f'Link {link.title[:50]} associated with \
-                                        location {location.title[:50]} by {self._owner.username}',
-                                        created=datetime.now())
+                    link_location = LinkLocation(
+                        user_id=self._owner.id, location_id=location_id,
+                        link_id=link_id, created=datetime.now()
+                    )
+
+                    activity = Activity(
+                        user_id=self._owner.id, summary=f'Link \
+                        {link.title[:50]} associated with location \
+                        {location.title[:50]} by {self._owner.username}',
+                        created=datetime.now()
+                    )
 
                     session.add(link_location)
                     session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return location
 
-    def get_links_by_location_id(self, location_id: int) -> list:
+    def get_links_by_location_id(self, location_id: int) -> List[Type[Link]]:
         """Get all links associated with a location
 
         Parameters
         ----------
         location_id : int
             The id of the location
 
@@ -556,21 +609,25 @@
         -------
         list
             A list of link objects
         """
 
         with self._session as session:
             for link_location in session.query(LinkLocation).filter(
-                LinkLocation.location_id == location_id, LinkLocation.user_id == self._owner.id
+                LinkLocation.location_id == location_id,
+                LinkLocation.user_id == self._owner.id
             ).all():
                 yield session.query(Link).filter(
-                    Link.id == link_location.link_id, Link.user_id == self._owner.id
+                    Link.id == link_location.link_id,
+                    Link.user_id == self._owner.id
                 ).first()
 
-    def get_links_page_by_location_id(self, location_id: int, page: int, per_page: int) -> list:
+    def get_links_page_by_location_id(
+        self, location_id: int, page: int, per_page: int
+    ) -> List[Type[Link]]:
         """Get a single page of links associated with a location from the database
 
         Parameters
         ----------
         location_id : int
             The id of the location
         page : int
@@ -583,18 +640,21 @@
         list
             A list of link objects
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(LinkLocation).filter(
-                LinkLocation.location_id == location_id, LinkLocation.user_id == self._owner.id
+                LinkLocation.location_id == location_id,
+                LinkLocation.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def append_notes_to_location(self, location_id: int, note_ids: list) -> Type[Location]:
+    def append_notes_to_location(
+        self, location_id: int, note_ids: list
+    ) -> Type[Location]:
         """Append notes to a location
 
         Parameters
         ----------
         location_id : int
             The id of the location
         note_ids : list
@@ -605,47 +665,54 @@
         Location
             The updated location object
         """
 
         with self._session as session:
             try:
                 location = session.query(Location).filter(
-                    Location.id == location_id, Location.user_id == self._owner.id
+                    Location.id == location_id,
+                    Location.user_id == self._owner.id
                 ).first()
 
                 if not location:
                     raise ValueError('Location not found.')
 
                 for note_id in note_ids:
                     note = session.query(Note).filter(
-                        Note.id == note_id, Note.user_id == self._owner.id
+                        Note.id == note_id,
+                        Note.user_id == self._owner.id
                     ).first()
 
                     if not note:
                         raise ValueError('Note not found.')
 
-                    location_note = LocationNote(user_id=self._owner.id, location_id=location_id, note_id=note_id,
-                                                 created=datetime.now())
-
-                    activity = Activity(user_id=self._owner.id, summary=f'Note {note.title[:50]} associated with \
-                                        location {location.title[:50]} by {self._owner.username}',
-                                        created=datetime.now())
+                    location_note = LocationNote(
+                        user_id=self._owner.id, location_id=location_id,
+                        note_id=note_id, created=datetime.now()
+                    )
+
+                    activity = Activity(
+                        user_id=self._owner.id, summary=f'Note \
+                        {note.title[:50]} associated with location \
+                        {location.title[:50]} by {self._owner.username}',
+                        created=datetime.now()
+                    )
 
                     session.add(location_note)
                     session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return location
 
-    def get_notes_by_location_id(self, location_id: int) -> list:
+    def get_notes_by_location_id(self, location_id: int) -> List[Type[Note]]:
         """Get all notes associated with a location
 
         Parameters
         ----------
         location_id : int
             The id of the location
 
@@ -653,21 +720,25 @@
         -------
         list
             A list of note objects
         """
 
         with self._session as session:
             for location_note in session.query(LocationNote).filter(
-                LocationNote.location_id == location_id, LocationNote.user_id == self._owner.id
+                LocationNote.location_id == location_id,
+                LocationNote.user_id == self._owner.id
             ).all():
                 yield session.query(Note).filter(
-                    Note.id == location_note.note_id, Note.user_id == self._owner.id
+                    Note.id == location_note.note_id,
+                    Note.user_id == self._owner.id
                 ).first()
 
-    def get_notes_page_by_location_id(self, location_id: int, page: int, per_page: int) -> list:
+    def get_notes_page_by_location_id(
+        self, location_id: int, page: int, per_page: int
+    ) -> List[Type[Note]]:
         """Get a single page of notes associated with a location from the database
 
         Parameters
         ----------
         location_id : int
             The id of the location
         page : int
@@ -680,9 +751,10 @@
         list
             A list of note objects
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(LocationNote).filter(
-                LocationNote.location_id == location_id, LocationNote.user_id == self._owner.id
+                LocationNote.location_id == location_id,
+                LocationNote.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
```

### Comparing `noveler-0.1.0/noveler/controllers/NoteController.py` & `noveler-0.1.1/noveler/controllers/NoteController.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from datetime import datetime
-from typing import Type
+from typing import Type, List
 from sqlalchemy import or_
 from sqlalchemy.orm import Session
 from noveler.controllers.BaseController import BaseController
 from noveler.models import User, Note, Activity
 
 
 class NoteController(BaseController):
     """Note controller encapsulates note management functionality
 
     Attributes
     ----------
-    _self : NoteController
+    _instance : NoteController
         The instance of the note controller
     _owner : User
         The current user of the note controller
     _session : Session
         The database session
 
     Methods
@@ -31,15 +31,15 @@
     get_all_notes_page(page: int, per_page: int)
         Get a single page of notes associated with an owner from the database
     search_notes(search: str)
         Search for notes by title and content
     """
 
     def __init__(
-            self, path_to_config: str, session: Session, owner: Type[User]
+        self, path_to_config: str, session: Session, owner: Type[User]
     ):
         """Initialize the class"""
 
         super().__init__(path_to_config, session, owner)
 
     def create_note(self, title: str, content: str) -> Note:
         """Create a new note
@@ -112,17 +112,18 @@
                 if not note:
                     raise ValueError('Note not found.')
 
                 note.title = title
                 note.content = content
                 note.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Note {note.id} updated by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Note {note.id} updated \
+                    by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
@@ -143,23 +144,25 @@
         bool
             True on success
         """
 
         with self._session as session:
             try:
                 note = session.query(Note).filter(
-                    Note.id == note_id, Note.user_id == self._owner.id
+                    Note.id == note_id,
+                    Note.user_id == self._owner.id
                 ).first()
 
                 if not note:
                     raise ValueError('Note not found.')
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Note {note.id} deleted by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Note {note.id} deleted \
+                    by {self._owner.username}', created=datetime.now()
+                )
 
                 session.delete(note)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
@@ -180,30 +183,33 @@
         -------
         Note
             The note object
         """
 
         with self._session as session:
             return session.query(Note).filter(
-                Note.id == note_id, Note.user_id == self._owner.id
+                Note.id == note_id,
+                Note.user_id == self._owner.id
             ).first()
 
-    def get_all_notes(self) -> list:
+    def get_all_notes(self) -> List[Type[Note]]:
         """Get all notes associated with an owner
 
         Returns
         -------
         list
             A list of note objects
         """
 
         with self._session as session:
-            return session.query(Note).filter(Note.user_id == self._owner.id).all()
+            return session.query(Note).filter(
+                Note.user_id == self._owner.id
+            ).all()
 
-    def get_all_notes_page(self, page: int, per_page: int) -> list:
+    def get_all_notes_page(self, page: int, per_page: int) -> List[Type[Note]]:
         """Get a single page of notes associated with an owner from the database
 
         Parameters
         ----------
         page : int
             The page number
         per_page : int
@@ -217,15 +223,15 @@
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(Note).filter(
                 Note.owner_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def search_notes(self, search: str) -> list:
+    def search_notes(self, search: str) -> List[Type[Note]]:
         """Search for notes by title and content
 
         Parameters
         ----------
         search : str
             The search string
 
@@ -233,10 +239,13 @@
         -------
         list
             A list of note objects
         """
 
         with self._session as session:
             return session.query(Note).filter(
-                or_(Note.title.like(f'%{search}%'), Note.content.like(f'%{search}%')),
+                or_(
+                    Note.title.like(f'%{search}%'),
+                    Note.content.like(f'%{search}%')
+                ),
                 Note.user_id == self._owner.id
             ).all()
```

### Comparing `noveler-0.1.0/noveler/controllers/OllamaModelController.py` & `noveler-0.1.1/noveler/controllers/OllamaModelController.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from datetime import datetime
-from typing import Type
+from typing import Type, List
 from sqlalchemy.orm import Session
 from noveler.controllers import BaseController
 from noveler.models import User, OllamaModel, Activity
 
 
 class OllamaModelController(BaseController):
-    """Ollama model controller class
+    """The OllamaModelController class encapsulates the logic for managing
+    Ollama models in the database.
     """
 
     def __init__(
-            self, path_to_config: str, session: Session, owner: Type[User]
+        self, path_to_config: str, session: Session, owner: Type[User]
     ):
         """Initialize the class"""
 
         super().__init__(path_to_config, session, owner)
 
     def create_model(
         self, title: str, model: str, description: str = None,
@@ -90,20 +91,19 @@
 
             model = session.query(OllamaModel).filter(
                 OllamaModel.model == model
             ).first()
 
             return model if model else None
 
-    def get_models(self) -> list:
+    def get_models(self) -> List[Type[OllamaModel]]:
         """Get all models stored in the database
 
         Returns
         -------
         list
             A list of model objects
         """
 
         with self._session as session:
-
             return session.query(OllamaModel).all()
```

### Comparing `noveler-0.1.0/noveler/controllers/SceneController.py` & `noveler-0.1.1/noveler/controllers/SceneController.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 from configparser import ConfigParser
 from datetime import datetime
-from typing import Type
+from typing import Type, List
 from sqlalchemy import or_, func
 from sqlalchemy.orm import Session
 from noveler.controllers.BaseController import BaseController
 from noveler.models import User, Scene, Link, LinkScene, Note, NoteScene, Activity
 
 
 class SceneController(BaseController):
     """Scene controller encapsulates scene management functionality
 
     Attributes
     ----------
-    _self : SceneController
+    _instance : SceneController
         The instance of the scene controller
     _owner : User
         The current user of the scene controller
     _session : Session
         The database session
 
     Methods
@@ -55,22 +55,23 @@
     append_notes_to_scene(scene_id: int, note_ids: list)
         Append notes to a scene
     get_notes_by_scene_id(scene_id: int)
         Get all notes associated with a scene
     """
 
     def __init__(
-            self, path_to_config: str, session: Session, owner: Type[User]
+        self, path_to_config: str, session: Session, owner: Type[User]
     ):
         """Initialize the class"""
 
         super().__init__(path_to_config, session, owner)
 
     def create_scene(
-            self, story_id: int, chapter_id: int, title: str, description: str = None, content: str = None
+        self, story_id: int, chapter_id: int, title: str,
+        description: str = None, content: str = None
     ) -> Scene:
         """Create a new scene
 
         Parameters
         ----------
         story_id : int
             The id of the story
@@ -88,44 +89,56 @@
         Scene
             The new scene object
         """
 
         with self._session as session:
             try:
                 title_exists = session.query(Scene).filter(
-                    Scene.title == title, Scene.chapter_id == chapter_id, Scene.user_id == self._owner.id
+                    Scene.title == title,
+                    Scene.chapter_id == chapter_id,
+                    Scene.user_id == self._owner.id
                 ).first()
 
                 if title_exists:
                     raise Exception('This chapter already has a scene with the same title.')
 
-                position = session.query(func.max(Scene.position)).filter(Scene.chapter_id == chapter_id).scalar()
+                position = session.query(
+                    func.max(Scene.position)
+                ).filter(Scene.chapter_id == chapter_id).scalar()
                 position = int(position) + 1 if position else 1
                 created = datetime.now()
                 modified = created
 
-                scene = Scene(user_id=self._owner.id, story_id=story_id, chapter_id=chapter_id, position=position,
-                              title=title, description=description, content=content, created=created, modified=modified)
-
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Scene {scene.title[:50]} created by {self._owner.username}',
-                                    created=datetime.now())
+                scene = Scene(
+                    user_id=self._owner.id, story_id=story_id,
+                    chapter_id=chapter_id, position=position, title=title,
+                    description=description, content=content, created=created,
+                    modified=modified
+                )
+
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Scene {scene.title[:50]} \
+                    created by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(scene)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return scene
 
-    def update_scene(self, scene_id: int, title: str, description: str = None, content: str = None) -> Type[Scene]:
+    def update_scene(
+        self, scene_id: int, title: str, description: str = None,
+        content: str = None
+    ) -> Type[Scene]:
         """Update a scene
 
         Parameters
         ----------
         scene_id : int
             The id of the scene
         title : str
@@ -140,28 +153,30 @@
         bool
             True on success
         """
 
         with self._session as session:
             try:
                 scene = session.query(Scene).filter(
-                    Scene.id == scene_id, Scene.user_id == self._owner.id
+                    Scene.id == scene_id,
+                    Scene.user_id == self._owner.id
                 ).first()
 
                 if not scene:
                     raise ValueError('Scene not found.')
 
                 scene.title = title
                 scene.description = description
                 scene.content = content
                 scene.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Scene {scene.id} updated by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Scene {scene.id} updated \
+                    by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
@@ -237,17 +252,19 @@
                             config.get("formats", "datetime")
                         )
                         sibling.modified = datetime.now()
 
                 scene.position = position
                 scene.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Scene {scene.title[:50]} position changed by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Scene {scene.title[:50]} \
+                    position changed by {self._owner.username}',
+                    created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
@@ -293,17 +310,18 @@
                     sibling.position -= 1
                     sibling.created = datetime.strptime(
                         str(sibling.created),
                         config.get("formats", "datetime")
                     )
                     sibling.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Scene {scene.id} deleted by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Scene {scene.id} deleted \
+                    by {self._owner.username}', created=datetime.now()
+                )
 
                 session.delete(scene)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
@@ -329,15 +347,15 @@
         with self._session as session:
 
             return session.query(Scene).filter(
                 Scene.chapter_id == chapter_id,
                 Scene.user_id == self._owner.id
             ).count()
 
-    def get_scene_by_id(self, scene_id: int) -> Type[Scene]:
+    def get_scene_by_id(self, scene_id: int) -> Type[Scene] | None:
         """Get a scene by id
 
         Parameters
         ----------
         scene_id : int
             The id of the scene
 
@@ -350,31 +368,35 @@
         with self._session as session:
 
             return session.query(Scene).filter(
                 Scene.id == scene_id,
                 Scene.user_id == self._owner.id
             ).first()
 
-    def get_all_scenes(self) -> list:
+    def get_all_scenes(self) -> List[Type[Scene]]:
         """Get all scenes associated with an owner
 
         Scenes are sorted by story id, chapter id, and position in ascending order.
 
         Returns
         -------
         list
             A list of scene objects
         """
 
         with self._session as session:
-            return session.query(Scene).filter(Scene.user_id == self._owner.id).order_by(
+            return session.query(Scene).filter(
+                Scene.user_id == self._owner.id
+            ).order_by(
                 Scene.story_id, Scene.chapter_id, Scene.position
             ).all()
 
-    def get_all_scenes_page(self, page: int, per_page: int) -> list:
+    def get_all_scenes_page(
+        self, page: int, per_page: int
+    ) -> List[Type[Scene]]:
         """Get a single page of scenes associated with an owner from the database
 
         Scenes are sorted by story id, chapter id, and position in ascending order
 
         Parameters
         ----------
         page : int
@@ -388,17 +410,19 @@
             A list of scene objects
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(Scene).filter(
                 Scene.user_id == self._owner.id
-            ).order_by(Scene.story_id, Scene.chapter_id, Scene.position).offset(offset).limit(per_page).all()
+            ).order_by(
+                Scene.story_id, Scene.chapter_id, Scene.position
+            ).offset(offset).limit(per_page).all()
 
-    def get_scenes_by_story_id(self, story_id: int) -> list:
+    def get_scenes_by_story_id(self, story_id: int) -> List[Type[Scene]]:
         """Get all scenes associated with a story
 
         Scenes are sorted by chapter id and position in ascending order
 
         Parameters
         ----------
         story_id : int
@@ -408,20 +432,23 @@
         -------
         list
             A list of scene objects
         """
 
         with self._session as session:
             return session.query(Scene).filter(
-                Scene.story_id == story_id, Scene.user_id == self._owner.id
+                Scene.story_id == story_id,
+                Scene.user_id == self._owner.id
             ).order_by(
                 Scene.chapter_id, Scene.position
             ).all()
 
-    def get_scenes_page_by_story_id(self, story_id: int, page: int, per_page: int) -> list:
+    def get_scenes_page_by_story_id(
+        self, story_id: int, page: int, per_page: int
+    ) -> List[Type[Scene]]:
         """Get a single page of scenes associated with a story from the database
 
         Parameters
         ----------
         story_id : int
             The id of the story
         page : int
@@ -434,20 +461,21 @@
         list
             A list of scene objects
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(Scene).filter(
-                Scene.story_id == story_id, Scene.user_id == self._owner.id
+                Scene.story_id == story_id,
+                Scene.user_id == self._owner.id
             ).order_by(
                 Scene.chapter_id, Scene.position
             ).offset(offset).limit(per_page).all()
 
-    def get_scenes_by_chapter_id(self, chapter_id: int) -> list:
+    def get_scenes_by_chapter_id(self, chapter_id: int) -> List[Type[Scene]]:
         """Get all scenes associated with a chapter
 
         Scenes are sorted by position in ascending order
 
         Parameters
         ----------
         chapter_id : int
@@ -457,18 +485,21 @@
         -------
         list
             A list of scene objects
         """
 
         with self._session as session:
             return session.query(Scene).filter(
-                Scene.chapter_id == chapter_id, Scene.user_id == self._owner.id
+                Scene.chapter_id == chapter_id,
+                Scene.user_id == self._owner.id
             ).order_by(Scene.position).all()
 
-    def get_scenes_page_by_chapter_id(self, chapter_id: int, page: int, per_page: int) -> list:
+    def get_scenes_page_by_chapter_id(
+        self, chapter_id: int, page: int, per_page: int
+    ) -> List[Type[Scene]]:
         """Get a single page of scenes associated with a chapter from the database
 
         Scenes are sorted by position in ascending order
 
         Parameters
         ----------
         chapter_id : int
@@ -483,18 +514,19 @@
         list
             A list of scene objects
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(Scene).filter(
-                Scene.chapter_id == chapter_id, Scene.user_id == self._owner.id
+                Scene.chapter_id == chapter_id,
+                Scene.user_id == self._owner.id
             ).order_by(Scene.position).offset(offset).limit(per_page).all()
 
-    def search_scenes(self, search: str) -> list:
+    def search_scenes(self, search: str) -> List[Type[Scene]]:
         """Search for scenes by title, description, and content
 
         Parameters
         ----------
         search : str
             The search string
 
@@ -502,20 +534,25 @@
         -------
         list
             A list of scene objects
         """
 
         with self._session as session:
             return session.query(Scene).filter(
-                or_(Scene.title.like(f'%{search}%'), Scene.description.like(f'%{search}%'),
-                    Scene.content.like(f'%{search}%')),
+                or_(
+                    Scene.title.like(f'%{search}%'),
+                    Scene.description.like(f'%{search}%'),
+                    Scene.content.like(f'%{search}%')
+                ),
                 Scene.user_id == self._owner.id
             ).all()
 
-    def append_links_to_scene(self, scene_id: int, link_ids: list) -> Type[Scene]:
+    def append_links_to_scene(
+        self, scene_id: int, link_ids: list
+    ) -> Type[Scene]:
         """Append links to a scene
 
         Parameters
         ----------
         scene_id : int
             The id of the scene
         link_ids : list
@@ -526,46 +563,53 @@
         Scene
             The updated scene object
         """
 
         with self._session as session:
             try:
                 scene = session.query(Scene).filter(
-                    Scene.id == scene_id, Scene.user_id == self._owner.id
+                    Scene.id == scene_id,
+                    Scene.user_id == self._owner.id
                 ).first()
 
                 if not scene:
                     raise ValueError('Scene not found.')
 
                 for link_id in link_ids:
                     link = session.query(Link).filter(
-                        Link.id == link_id, Link.user_id == self._owner.id
+                        Link.id == link_id,
+                        Link.user_id == self._owner.id
                     ).first()
 
                     if not link:
                         raise ValueError('Link not found.')
 
-                    link_scene = LinkScene(user_id=self._owner.id, link_id=link_id, scene_id=scene_id,
-                                           created=datetime.now())
+                    link_scene = LinkScene(
+                        user_id=self._owner.id, link_id=link_id,
+                        scene_id=scene_id, created=datetime.now()
+                    )
 
-                    activity = Activity(user_id=self._owner.id, summary=f'Links appended to scene {scene.id} by \
-                                        {self._owner.username}', created=datetime.now())
+                    activity = Activity(
+                        user_id=self._owner.id, summary=f'Links appended to \
+                        scene {scene.id} by {self._owner.username}',
+                        created=datetime.now()
+                    )
 
                     session.add(link_scene)
                     session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return scene
 
-    def get_links_by_scene_id(self, scene_id: int) -> list:
+    def get_links_by_scene_id(self, scene_id: int) -> List[Type[Link]]:
         """Get all links associated with a scene
 
         Parameters
         ----------
         scene_id : int
             The id of the scene
 
@@ -573,18 +617,21 @@
         -------
         list
             A list of link objects
         """
 
         with self._session as session:
             return session.query(Link).join(LinkScene).filter(
-                LinkScene.scene_id == scene_id, LinkScene.user_id == self._owner.id
+                LinkScene.scene_id == scene_id,
+                LinkScene.user_id == self._owner.id
             ).all()
 
-    def append_notes_to_scene(self, scene_id: int, note_ids: list) -> Type[Scene]:
+    def append_notes_to_scene(
+        self, scene_id: int, note_ids: list
+    ) -> Type[Scene]:
         """Append notes to a scene
 
         Parameters
         ----------
         scene_id : int
             The id of the scene
         note_ids : list
@@ -595,46 +642,53 @@
         Scene
             The updated scene object
         """
 
         with self._session as session:
             try:
                 scene = session.query(Scene).filter(
-                    Scene.id == scene_id, Scene.user_id == self._owner.id
+                    Scene.id == scene_id,
+                    Scene.user_id == self._owner.id
                 ).first()
 
                 if not scene:
                     raise ValueError('Scene not found.')
 
                 for note_id in note_ids:
                     note = session.query(Note).filter(
-                        Note.id == note_id, Note.user_id == self._owner.id
+                        Note.id == note_id,
+                        Note.user_id == self._owner.id
                     ).first()
 
                     if not note:
                         raise ValueError('Note not found.')
 
-                    note_scene = NoteScene(user_id=self._owner.id, note_id=note_id, scene_id=scene_id,
-                                           created=datetime.now())
+                    note_scene = NoteScene(
+                        user_id=self._owner.id, note_id=note_id,
+                        scene_id=scene_id, created=datetime.now()
+                    )
 
-                    activity = Activity(user_id=self._owner.id, summary=f'Notes appended to scene {scene.id} by \
-                                        {self._owner.username}', created=datetime.now())
+                    activity = Activity(
+                        user_id=self._owner.id, summary=f'Notes appended to \
+                        scene {scene.id} by {self._owner.username}',
+                        created=datetime.now()
+                    )
 
                     session.add(note_scene)
                     session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return scene
 
-    def get_notes_by_scene_id(self, scene_id: int) -> list:
+    def get_notes_by_scene_id(self, scene_id: int) -> List[Type[Note]]:
         """Get all notes associated with a scene
 
         Parameters
         ----------
         scene_id : int
             The id of the scene
 
@@ -642,9 +696,10 @@
         -------
         list
             A list of note objects
         """
 
         with self._session as session:
             return session.query(Note).join(NoteScene).filter(
-                NoteScene.scene_id == scene_id, NoteScene.user_id == self._owner.id
+                NoteScene.scene_id == scene_id,
+                NoteScene.user_id == self._owner.id
             ).all()
```

### Comparing `noveler-0.1.0/noveler/controllers/StoryController.py` & `noveler-0.1.1/noveler/controllers/StoryController.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from datetime import datetime
-from typing import Type
+from typing import Type, List
 from sqlalchemy import or_
 from sqlalchemy.orm import Session
 from noveler.controllers.BaseController import BaseController
 from noveler.models import User, Story, Author, AuthorStory, Chapter, Activity, Character, CharacterStory, Link, \
     LinkStory, Note, NoteStory
 
 
 class StoryController(BaseController):
     """Story controller encapsulates story management functionality
 
     Attributes
     ----------
-    _self : StoryController
+    _instance : StoryController
         The instance of the story controller
     _owner : User
         The current user of the story controller
     _session : Session
         The database session
 
     Methods
@@ -70,15 +70,15 @@
     has_notes( story_id ) : bool
         Check if a story has notes
     get_notes_by_story_id(story_id: int)
         Get all notes associated with a story
     """
 
     def __init__(
-            self, path_to_config: str, session: Session, owner: Type[User]
+        self, path_to_config: str, session: Session, owner: Type[User]
     ):
         """Initialize the class"""
 
         super().__init__(path_to_config, session, owner)
 
     def create_story(self, title: str, description: str = None) -> Story:
         """Create a new story
@@ -97,33 +97,38 @@
         """
 
         with self._session as session:
             try:
                 created = datetime.now()
                 modified = created
 
-                story = Story(user_id=self._owner.id, title=title, description=description, created=created,
-                              modified=modified)
+                story = Story(
+                    user_id=self._owner.id, title=title, description=description,
+                    created=created, modified=modified
+                )
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Story {story.title[:50]} created by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Story {story.title[:50]} \
+                    created by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(story)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return story
 
-    def update_story(self, story_id: int, title: str, description: str = None) -> Type[Story]:
+    def update_story(
+        self, story_id: int, title: str, description: str = None
+    ) -> Type[Story]:
         """Update a story
 
         Parameters
         ----------
         story_id : int
             The id of the story
         title : str
@@ -136,27 +141,29 @@
         bool
             True on success
         """
 
         with self._session as session:
             try:
                 story = session.query(Story).filter(
-                    Story.id == story_id, Story.user_id == self._owner.id
+                    Story.id == story_id,
+                    Story.user_id == self._owner.id
                 ).first()
 
                 if not story:
                     raise ValueError('Story not found.')
 
                 story.title = title
                 story.description = description
                 story.modified = datetime.now()
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Story {story.id} updated by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Story {story.id} updated \
+                    by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
@@ -177,23 +184,25 @@
         bool
             True on success
         """
 
         with self._session as session:
             try:
                 story = session.query(Story).filter(
-                    Story.id == story_id, Story.user_id == self._owner.id
+                    Story.id == story_id,
+                    Story.user_id == self._owner.id
                 ).first()
 
                 if not story:
                     raise ValueError('Story not found.')
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'Story {story.id} deleted by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Story {story.id} deleted \
+                    by {self._owner.username}', created=datetime.now()
+                )
 
                 session.delete(story)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
@@ -244,31 +253,36 @@
         -------
         Story
             The story object
         """
 
         with self._session as session:
             story = session.query(Story).filter(
-                Story.id == story_id, Story.user_id == self._owner.id
+                Story.id == story_id,
+                Story.user_id == self._owner.id
             ).first()
             return story
 
-    def get_all_stories(self) -> list:
+    def get_all_stories(self) -> List[Type[Story]]:
         """Get all stories associated with an owner
 
         Returns
         -------
         list
             A list of story objects
         """
 
         with self._session as session:
-            return session.query(Story).filter(Story.user_id == self._owner.id).all()
+            return session.query(Story).filter(
+                Story.user_id == self._owner.id
+            ).all()
 
-    def get_all_stories_page(self, page: int, per_page: int) -> list:
+    def get_all_stories_page(
+        self, page: int, per_page: int
+    ) -> List[Type[Story]]:
         """Get a single page of stories associated with an owner from the database
 
         Parameters
         ----------
         page : int
             The page number
         per_page : int
@@ -282,15 +296,15 @@
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(Story).filter(
                 Story.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def search_stories(self, search: str) -> list:
+    def search_stories(self, search: str) -> List[Type[Story]]:
         """Search for stories by title and description
 
         Parameters
         ----------
         search : str
             The search string
 
@@ -298,19 +312,24 @@
         -------
         list
             A list of story objects
         """
 
         with self._session as session:
             return session.query(Story).filter(
-                or_(Story.title.like(f'%{search}%'), Story.description.like(f'%{search}%')),
+                or_(
+                    Story.title.like(f'%{search}%'),
+                    Story.description.like(f'%{search}%')
+                ),
                 Story.user_id == self._owner.id
             ).all()
 
-    def append_authors_to_story(self, story_id: int, author_ids: list) -> Type[Story]:
+    def append_authors_to_story(
+        self, story_id: int, author_ids: list
+    ) -> Type[Story]:
         """Append authors to a story
 
         Parameters
         ----------
         story_id : int
             The id of the story
         author_ids : list
@@ -321,34 +340,41 @@
         Story
             The updated story object
         """
 
         with self._session as session:
             try:
                 story = session.query(Story).filter(
-                    Story.id == story_id, Story.user_id == self._owner.id
+                    Story.id == story_id,
+                    Story.user_id == self._owner.id
                 ).first()
 
                 if not story:
                     raise ValueError('Story not found.')
 
                 for author_id in author_ids:
                     author = session.query(Author).filter(
-                        Author.id == author_id, Author.user_id == self._owner.id
+                        Author.id == author_id,
+                        Author.user_id == self._owner.id
                     ).first()
 
                     if not author:
                         raise ValueError('Author not found.')
 
-                    author_story = AuthorStory(user_id=self._owner.id, author_id=author_id, story_id=story_id,
-                                               created=datetime.now())
+                    author_story = AuthorStory(
+                        user_id=self._owner.id, author_id=author_id,
+                        story_id=story_id, created=datetime.now()
+                    )
                     story.authors.append(author_story)
 
-                activity = Activity(user_id=self._owner.id, summary=f'Authors appended to story {story.title[:50]} by \
-                                    {self._owner.username}', created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Authors appended to \
+                    story {story.title[:50]} by {self._owner.username}',
+                    created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
@@ -373,15 +399,15 @@
         with self._session as session:
 
             return session.query(Author).join(AuthorStory).filter(
                 AuthorStory.story_id == story_id,
                 AuthorStory.user_id == self._owner.id
             ).count() > 0
 
-    def get_authors_by_story_id(self, story_id: int) -> list:
+    def get_authors_by_story_id(self, story_id: int) -> List[Type[Author]]:
         """Get all authors associated with a story
 
         Parameters
         ----------
         story_id : int
             The id of the story
 
@@ -389,15 +415,16 @@
         -------
         list
             A list of author objects
         """
 
         with self._session as session:
             return session.query(Author).join(AuthorStory).filter(
-                AuthorStory.story_id == story_id, AuthorStory.user_id == self._owner.id
+                AuthorStory.story_id == story_id,
+                AuthorStory.user_id == self._owner.id
             ).all()
 
     def has_chapters(self, story_id: int) -> bool:
         """Check if a story has chapters
 
         Parameters
         ----------
@@ -413,15 +440,17 @@
         with self._session as session:
 
             return session.query(Chapter).filter(
                 Chapter.story_id == story_id,
                 Chapter.user_id == self._owner.id
             ).count() > 0
 
-    def get_chapter_by_position(self, story_id: int, position: int) -> Type[Chapter]:
+    def get_chapter_by_position(
+        self, story_id: int, position: int
+    ) -> Type[Chapter]:
         """Get a chapter by position
 
         Parameters
         ----------
         story_id : int
             The id of the story
         position : int
@@ -437,15 +466,17 @@
 
             return session.query(Chapter).filter(
                 Chapter.story_id == story_id,
                 Chapter.user_id == self._owner.id,
                 Chapter.position == position
             ).first()
 
-    def get_all_chapters_by_story_id(self, story_id: int) -> list:
+    def get_all_chapters_by_story_id(
+        self, story_id: int
+    ) -> List[Type[Chapter]]:
         """Get all chapters associated with a story
 
         Parameters
         ----------
         story_id : int
             The id of the story
 
@@ -458,15 +489,17 @@
         with self._session as session:
 
             return session.query(Chapter).filter(
                 Chapter.story_id == story_id,
                 Chapter.user_id == self._owner.id
             ).order_by(Chapter.position).all()
 
-    def append_characters_to_story(self, story_id: int, character_ids: list) -> Type[Story]:
+    def append_characters_to_story(
+        self, story_id: int, character_ids: list
+    ) -> Type[Story]:
         """Append characters to a story
 
         Parameters
         ----------
         story_id : int
             The id of the story
         character_ids : list
@@ -538,15 +571,17 @@
 
         with self._session as session:
 
             return session.query(Character).join(CharacterStory).filter(
                 CharacterStory.story_id == story_id, Character
             ).count() > 0
 
-    def get_characters_by_story_id(self, story_id: int) -> list:
+    def get_characters_by_story_id(
+        self, story_id: int
+    ) -> List[Type[Character]]:
         """Get all characters associated with a story
 
         Parameters
         ----------
         story_id : int
             The id of the story
 
@@ -558,15 +593,17 @@
 
         with self._session as session:
 
             return session.query(Character).join(CharacterStory).filter(
                 CharacterStory.story_id == story_id, Character
             ).all()
 
-    def get_characters_page_by_story_id(self, story_id: int, page: int, per_page: int) -> list:
+    def get_characters_page_by_story_id(
+        self, story_id: int, page: int, per_page: int
+    ) -> List[Type[Character]]:
         """Get a single page of characters associated with a story from the database
 
         Parameters
         ----------
         story_id : int
             The id of the story
         page : int
@@ -584,15 +621,17 @@
 
             offset = (page - 1) * per_page
 
             return session.query(Character).join(CharacterStory).filter(
                 CharacterStory.story_id == story_id, Character
             ).offset(offset).limit(per_page).all()
 
-    def append_links_to_story(self, story_id: int, link_ids: list) -> Type[Story]:
+    def append_links_to_story(
+        self, story_id: int, link_ids: list
+    ) -> Type[Story]:
         """Append links to a story
 
         Parameters
         ----------
         story_id : int
             The id of the story
         link_ids : list
@@ -603,34 +642,42 @@
         Story
             The updated story object
         """
 
         with self._session as session:
             try:
                 story = session.query(Story).filter(
-                    Story.id == story_id, Story.user_id == self._owner.id
+                    Story.id == story_id,
+                    Story.user_id == self._owner.id
                 ).first()
 
                 if not story:
                     raise ValueError('Story not found.')
 
                 for link_id in link_ids:
                     link = session.query(Link).filter(
-                        Link.id == link_id, Link.user_id == self._owner.id
+                        Link.id == link_id,
+                        Link.user_id == self._owner.id
                     ).first()
 
                     if not link:
                         raise ValueError('Link not found.')
 
-                    link_story = LinkStory(user_id=self._owner.id, story_id=story_id, link_id=link_id, created=datetime.now())
+                    link_story = LinkStory(
+                        user_id=self._owner.id, story_id=story_id,
+                        link_id=link_id, created=datetime.now()
+                    )
 
                     story.links.append(link_story)
 
-                activity = Activity(user_id=self._owner.id, summary=f'Links appended to story {story.title[:50]} by \
-                                    {self._owner.username}', created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Links appended to story \
+                    {story.title[:50]} by {self._owner.username}',
+                    created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
@@ -653,15 +700,15 @@
         """
 
         with self._session as session:
             return session.query(Link).join(LinkStory).filter(
                 LinkStory.story_id == story_id, LinkStory
             ).count() > 0
 
-    def get_links_by_story_id(self, story_id: int) -> list:
+    def get_links_by_story_id(self, story_id: int) -> List[Type[Link]]:
         """Get all links associated with a story
 
         Parameters
         ----------
         story_id : int
             The id of the story
 
@@ -669,18 +716,21 @@
         -------
         list
             A list of link objects
         """
 
         with self._session as session:
             return session.query(Link).join(LinkStory).filter(
-                LinkStory.story_id == story_id, LinkStory.user_id == self._owner.id
+                LinkStory.story_id == story_id,
+                LinkStory.user_id == self._owner.id
             ).all()
 
-    def append_notes_to_story(self, story_id: int, note_ids: list) -> Type[Story]:
+    def append_notes_to_story(
+        self, story_id: int, note_ids: list
+    ) -> Type[Story]:
         """Append notes to a story
 
         Parameters
         ----------
         story_id : int
             The id of the story
         note_ids : list
@@ -691,34 +741,42 @@
         Story
             The updated story object
         """
 
         with self._session as session:
             try:
                 story = session.query(Story).filter(
-                    Story.id == story_id, Story.user_id == self._owner.id
+                    Story.id == story_id,
+                    Story.user_id == self._owner.id
                 ).first()
 
                 if not story:
                     raise ValueError('Story not found.')
 
                 for note_id in note_ids:
                     note = session.query(Note).filter(
-                        Note.id == note_id, Note.user_id == self._owner.id
+                        Note.id == note_id,
+                        Note.user_id == self._owner.id
                     ).first()
 
                     if not note:
                         raise ValueError('Note not found.')
 
-                    note_story = NoteStory(user_id=self._owner.id, story_id=story_id, note_id=note_id, created=datetime.now())
+                    note_story = NoteStory(
+                        user_id=self._owner.id, story_id=story_id,
+                        note_id=note_id, created=datetime.now()
+                    )
 
                     story.notes.append(note_story)
 
-                activity = Activity(user_id=self._owner.id, summary=f'Notes appended to story {story.title[:50]} by \
-                                    {self._owner.username}', created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'Notes appended to story \
+                    {story.title[:50]} by {self._owner.username}',
+                    created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
@@ -742,15 +800,15 @@
 
         with self._session as session:
 
             return session.query(Note).join(NoteStory).filter(
                 NoteStory.story_id == story_id, NoteStory
             ).count() > 0
 
-    def get_notes_by_story_id(self, story_id: int) -> list:
+    def get_notes_by_story_id(self, story_id: int) -> List[Type[Note]]:
         """Get all notes associated with a story
 
         Parameters
         ----------
         story_id : int
             The id of the story
 
@@ -758,9 +816,10 @@
         -------
         list
             A list of note objects
         """
 
         with self._session as session:
             return session.query(Note).join(NoteStory).filter(
-                NoteStory.story_id == story_id, NoteStory.user_id == self._owner.id
+                NoteStory.story_id == story_id,
+                NoteStory.user_id == self._owner.id
             ).all()
```

### Comparing `noveler-0.1.0/noveler/controllers/SubmissionController.py` & `noveler-0.1.1/noveler/controllers/SubmissionController.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from configparser import ConfigParser
 from datetime import datetime, date
-from typing import Type
+from typing import Type, List
 from sqlalchemy.orm import Session
 from noveler.controllers.BaseController import BaseController
 from noveler.models import User, Submission, Activity
 
 
 class SubmissionController(BaseController):
     """Submission controller encapsulates submission management functionality
 
     Attributes
     ----------
-    _self : SubmissionController
+    _instance : SubmissionController
         The instance of the submission controller
     _owner : User
         The current user of the submission controller
     _session : Session
         The database session
 
     Methods
@@ -34,21 +34,23 @@
     get_submissions_by_story_id(story_id: int)
         Get all submissions associated with a story
     get_submissions_page_by_story_id(story_id: int, page
         Get a single page of submissions associated with a story from the database
     """
 
     def __init__(
-            self, path_to_config: str, session: Session, owner: Type[User]
+        self, path_to_config: str, session: Session, owner: Type[User]
     ):
         """Initialize the class"""
 
         super().__init__(path_to_config, session, owner)
 
-    def create_submission(self, story_id: int, submitted_to: str, date_sent: str = None) -> Submission:
+    def create_submission(
+        self, story_id: int, submitted_to: str, date_sent: str = None
+    ) -> Submission:
         """Create a new submission
 
         Parameters
         ----------
         story_id : int
             The id of the story
         submitted_to : str
@@ -99,16 +101,16 @@
 
             else:
                 session.commit()
                 return submission
 
     def update_submission(
         self, submission_id: int, submitted_to: str, date_sent: str,
-            date_reply_received: str, date_published: str, date_paid: str,
-            result: str, amount: float
+        date_reply_received: str, date_published: str, date_paid: str,
+        result: str, amount: float
     ) -> Type[Submission]:
         """Update a submission
 
         Parameters
         ----------
         submission_id : int
             The id of the submission
@@ -204,30 +206,32 @@
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return True
 
-    def get_all_submissions_by_owner_id(self) -> list:
+    def get_all_submissions(self) -> List[Type[Submission]]:
         """Get all submissions associated with an owner
 
         Returns
         -------
         list
             A list of submission objects
         """
 
         with self._session as session:
 
             return session.query(Submission).filter(
                 Submission.user_id == self._owner.id
             ).all()
 
-    def get_all_submissions_page(self, page: int, per_page: int) -> list:
+    def get_all_submissions_page(
+        self, page: int, per_page: int
+    ) -> List[Type[Submission]]:
         """Get a single page of submissions associated with an owner from the database
 
         Parameters
         ----------
         page : int
             The page number
         per_page : int
@@ -243,15 +247,17 @@
 
             offset = (page - 1) * per_page
 
             return session.query(Submission).filter(
                 Submission.user_id == self._owner.id
             ).offset(offset).limit(per_page).all()
 
-    def get_submissions_by_story_id(self, story_id: int) -> list:
+    def get_submissions_by_story_id(
+        self, story_id: int
+    ) -> List[Type[Submission]]:
         """Get all submissions associated with a story
 
         Parameters
         ----------
         story_id : int
             The id of the story
 
@@ -265,15 +271,15 @@
             return session.query(Submission).filter(
                 Submission.story_id == story_id,
                 Submission.user_id == self._owner.id
             ).all()
 
     def get_submissions_page_by_story_id(
         self, story_id: int, page: int, per_page: int
-    ) -> list:
+    ) -> List[Type[Submission]]:
         """Get a single page of submissions associated with a story from the database
 
         Parameters
         ----------
         story_id : int
             The id of the story
         page : int
```

### Comparing `noveler-0.1.0/noveler/controllers/UserController.py` & `noveler-0.1.1/noveler/controllers/UserController.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import uuid
 from datetime import datetime
-from typing import Type
+from typing import Type, List
 import bcrypt
 from sqlalchemy import func
 from sqlalchemy.orm import Session
-import noveler
 from noveler.controllers.BaseController import BaseController
 from noveler.models import User, Activity
 
 
 def hash_password(password: str) -> str:
     """Hash a password, return hashed password"""
 
@@ -35,15 +34,15 @@
 
 
 class UserController(BaseController):
     """User controller encapsulates user management functionality
 
     Attributes
     ----------
-    _self : UserController
+    _instance : UserController
         The instance of the user controller
     _owner : User
         The current user of the user controller
     _session : Session
         The database session
 
     Methods
@@ -77,15 +76,15 @@
     get_all_users_page(page: int, per_page: int)
         Get a single page of users from the database
     search_users(search: str)
         Search for users by username or email
     """
 
     def __init__(
-            self, path_to_config: str, session: Session, owner: Type[User]
+        self, path_to_config: str, session: Session, owner: Type[User]
     ):
         """Initialize the class"""
 
         super().__init__(path_to_config, session, owner)
 
     def create_user(self, username: str, password: str, email: str) -> User:
         """Create a new user
@@ -136,37 +135,44 @@
                 while uuid_exists:
 
                     uuid4 = str(uuid.uuid4())
                     uuid_exists = session.query(User).filter(
                         User.uuid == uuid4
                     ).first()
 
-                password = noveler.controllers.hash_password(password)
+                password = hash_password(password)
                 created = datetime.now()
                 modified = created
 
-                user = User(uuid=uuid4, username=username, password=password, email=email, created=created,
-                            modified=modified, is_active=True)
-
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'User {user.username} created by {self._owner.username}',
-                                    created=datetime.now())
+                user = User(
+                    uuid=uuid4, username=username, password=password,
+                    email=email, created=created, modified=modified,
+                    is_active=True
+                )
+
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'User {user.username} \
+                    created by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(user)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return user
 
-    def register_user(self, username: str, password: str, repassword: str, email: str, reemail: str) -> User:
+    def register_user(
+        self, username: str, password: str, repassword: str, email: str,
+        reemail: str
+    ) -> User:
         """Register a new user identity
 
         This method is for self-registration of new users. It is available to secondary users of the website and the
         desktop application. The method first checks if the username or email already exists. If either exists, an
         exception is raised. If neither exists, the method creates a new user and logs the activity. The method returns
         the new user's id on success and nothing on failure.
 
@@ -212,32 +218,36 @@
                 uuid4 = str(uuid.uuid4())
                 uuid_exists = session.query(User).filter(User.uuid == uuid4).first()
 
                 while uuid_exists:
                     uuid4 = str(uuid.uuid4())
                     uuid_exists = session.query(User).filter(User.uuid == uuid4).first()
 
-                password = noveler.controllers.hash_password(password)
+                password = hash_password(password)
                 created = datetime.now()
                 modified = created
-                user = User(uuid=uuid4, username=username, password=password, email=email, created=created,
-                            modified=modified, is_active=False)
+                user = User(
+                    uuid=uuid4, username=username, password=password,
+                    email=email, created=created, modified=modified,
+                    is_active=False
+                )
 
                 session.add(user)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
 
-                activity = Activity(user_id=user.id,
-                                    summary=f'User {user.username} registered by {user.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=user.id, summary=f'User {user.username} registered \
+                    by {user.username}', created=datetime.now()
+                )
 
                 try:
                     session.add(activity)
 
                 except Exception as e:
                     session.rollback()
                     raise e
@@ -266,17 +276,18 @@
 
             if not user:
                 raise ValueError('User not found.')
 
             try:
                 user.is_active = True
                 user.modified = datetime.now()
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'User {user.username} activated by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'User {user.username} \
+                    activated by {self._owner.username}', created=datetime.now()
+                )
 
                 session.add(user)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
@@ -305,17 +316,19 @@
 
             if not user:
                 raise ValueError('User not found.')
 
             try:
                 user.is_active = False
                 user.modified = datetime.now()
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'User {user.username} deactivated by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'User {user.username} \
+                    deactivated by {self._owner.username}',
+                    created=datetime.now()
+                )
 
                 session.add(user)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
@@ -344,32 +357,38 @@
 
             try:
                 candidate = session.query(User).filter(User.username == username).first()
 
                 if not candidate:
                     raise Exception('User not found.')
 
-                if not noveler.controllers.verify_password(password, candidate.password):
+                if not verify_password(password, candidate.password):
                     raise ValueError('Invalid password.')
 
-                activity = Activity(user_id=candidate.id,
-                                    summary=f'User {candidate.username} logged in',
-                                    created=datetime.now())
+                if not candidate.is_active:
+                    raise ValueError('User account is not activated.')
+
+                activity = Activity(
+                    user_id=candidate.id, summary=f'User {candidate.username} \
+                    logged in', created=datetime.now()
+                )
 
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
 
             else:
                 session.commit()
                 return candidate
 
-    def change_password(self, user_id: int, old_password: str, new_password, repassword: str) -> User:
+    def change_password(
+        self, user_id: int, old_password: str, new_password, repassword: str
+    ) -> User:
         """Change user password
 
         Parameters
         ----------
         user_id : int
             The id of the user
         old_password : str
@@ -386,30 +405,31 @@
         """
 
         user = self.get_user_by_id(user_id)
 
         if not user:
             raise ValueError('User not found.')
 
-        if not noveler.controllers.verify_password(old_password, user.password):
+        if not verify_password(old_password, user.password):
             raise ValueError('Invalid password.')
 
         if new_password != repassword:
             raise ValueError('The new passwords do not match.')
 
-        new_password = noveler.controllers.hash_password(new_password)
+        new_password = hash_password(new_password)
         user.password = new_password
         user.modified = str(datetime.now())
 
         with self._session as session:
 
             try:
-                activity = Activity(user_id=user.id,
-                                    summary=f'User {user.username} changed their password',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=user.id, summary=f'User {user.username} changed \
+                    their password', created=datetime.now()
+                )
 
                 session.add(user)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
@@ -436,17 +456,18 @@
 
             try:
                 user = session.query(User).filter(User.id == user_id).first()
 
                 if not user:
                     raise ValueError('User not found.')
 
-                activity = Activity(user_id=self._owner.id,
-                                    summary=f'User {user.username} deleted by {self._owner.username}',
-                                    created=datetime.now())
+                activity = Activity(
+                    user_id=self._owner.id, summary=f'User {user.username} \
+                    deleted by {self._owner.username}', created=datetime.now()
+                )
 
                 session.delete(user)
                 session.add(activity)
 
             except Exception as e:
                 session.rollback()
                 raise e
@@ -551,27 +572,27 @@
         int
             The number of users
         """
 
         with self._session as session:
             return session.query(func.count(User.id)).scalar()
 
-    def get_all_users(self) -> list:
+    def get_all_users(self) -> List[Type[User]]:
         """Get all users
 
         Returns
         -------
         list
             A list of users
         """
 
         with self._session as session:
             return session.query(User).all()
 
-    def get_all_users_page(self, page: int, per_page: int) -> list:
+    def get_all_users_page(self, page: int, per_page: int) -> List[Type[User]]:
         """Get a single page of users from the database
 
         Parameters
         ----------
         page : int
             The page number
         per_page : int
@@ -583,15 +604,15 @@
             A list of users
         """
 
         with self._session as session:
             offset = (page - 1) * per_page
             return session.query(User).offset(offset).limit(per_page).all()
 
-    def search_users(self, search: str) -> list:
+    def search_users(self, search: str) -> List[Type[User]]:
         """Search for users by username or email
 
         Parameters
         ----------
         search : str
             The search string
```

### Comparing `noveler-0.1.0/noveler/controllers/__init__.py` & `noveler-0.1.1/noveler/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/Activity.py` & `noveler-0.1.1/noveler/models/Activity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from datetime import datetime
 from sqlalchemy import Integer, String, DateTime, ForeignKey
 from sqlalchemy.orm import Mapped, mapped_column, relationship, validates
 from noveler.models import User, Base
 
 
 class Activity(Base):
-    """The Activity class represents an activity that a user has done.
+    """The Activity class documents any controller endpoint activities.
 
     Attributes
     ----------
         id: int
             The activity's id
         user_id: int
             The id of the owner of this entry
         summary: str
             The activity's summary
         created: str
             The activity's creation date in datetime form: yyy-mm-dd hh:mm:ss
         user: User
-            The user who owns this entry
+            The system user or user currently logged in
 
     Methods
     -------
         __repr__()
             Returns a string representation of the activity
         __str__()
             Returns a string representation of the activity
@@ -37,37 +37,39 @@
     __tablename__ = 'activities'
     id: Mapped[int] = mapped_column(
         Integer, primary_key=True, autoincrement=True
     )
     user_id: Mapped[int] = mapped_column(Integer, ForeignKey('users.id'))
     summary: Mapped[str] = mapped_column(String(250), nullable=True)
     created: Mapped[str] = mapped_column(DateTime, default=str(datetime.now()))
-    user: Mapped["User"] = relationship("User", back_populates="activities")
+    user: Mapped["User"] = relationship(
+        "User", back_populates="activities"
+    )
 
     def __repr__(self):
         """Returns a string representation of the activity.
 
         Returns
         -------
         str
             A string representation of the activity
         """
 
-        return f'<Activity {self.summary[:50]!r}>'
+        return f'<Activity {self.summary!r}>'
 
     def __str__(self):
         """Returns a string representation of the activity.
 
         Returns
         -------
         str
             A string representation of the activity
         """
 
-        return f'Activity: {self.summary[:50]}'
+        return f'{self.summary}'
 
     def serialize(self) -> dict:
         """Returns a dictionary representation of the activity.
 
         Returns
         -------
         dict
@@ -100,13 +102,17 @@
         self.summary = data.get('summary', self.summary)
         self.created = data.get('created', self.created)
 
         return self
 
     @validates("summary")
     def validate_summary(self, key, summary: str) -> str:
-        """Validates the summary's length."""
+        """Validates the summary's length.
+        """
 
         if len(summary) > 250:
-            raise ValueError("The activity summary must not have more than 250 characters.")
+            raise ValueError(
+                """The activity summary must be no more than 250 characters in length.
+                """
+            )
 
         return summary
```

### Comparing `noveler-0.1.0/noveler/models/Assistance.py` & `noveler-0.1.1/noveler/models/Assistance.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 
 class Assistance(Base):
     """The Assistance class represents an assistance request.
 
     Attributes
     ----------
     id: int
-        The assistance's id
+        The Assistance id
     user_id: int
         The id of the current user
     session_uuid: str
         The UUID of the session to be used when making the request. If other
-        messages in teh database have the same session_uuid value, they will be
+        messages in the database have the same session_uuid value, they will be
         loaded in order of their creation date, and the assistant will continue
         from the last message in the session.
     assistant: str
         The assistant to be used when making the request.
     model: str
-        The model to be used when making the request.
+        The language model to be used when making the request.
     priming: str
         The priming to be used when making the request.
     prompt: str
         The prompt to be used when making the request.
     temperature: float
         The temperature to be used when making the request.
     seed: int
         The seed to be used when making the request.
     content: str
-        The message to be used when making the request.
+        The language model's response to the prompt.
     done: bool
         Whether the assistance is done or not
     total_duration: int
         The total duration of the assistance (ns)
     load_duration: int
         The duration of the loading of the assistance (ns)
     prompt_eval_count: int
```

### Comparing `noveler-0.1.0/noveler/models/Author.py` & `noveler-0.1.1/noveler/models/Author.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/AuthorStory.py` & `noveler-0.1.1/noveler/models/AuthorStory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 from sqlalchemy import Integer, ForeignKey, DateTime
 from sqlalchemy.orm import Mapped, mapped_column, relationship
 from noveler.models import User, Author, Story, Base
 
 
 class AuthorStory(Base):
-    """The AuthorStory class represents the relationship between an author and a story.
+    """The AuthorStory class represents the relationship between an Author and a Story.
 
     Attributes
     ----------
         author_id: int
             The author's id
         story_id: int
             The story's id
```

### Comparing `noveler-0.1.0/noveler/models/Bibliography.py` & `noveler-0.1.1/noveler/models/Bibliography.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,35 +8,39 @@
 
 class Bibliography(Base):
     """The Bibliography class represents a reference to a story.
 
     Attributes
     ----------
         id: int
-            The reference's id
+            The Bibliography ID
         user_id: int
-            The id of the owner of this entry
+            The ID of the user who created this Bibliography entry
         story_id: int
-            The story's id
+            The Story ID that this Bibliography references
         title: str
-            The reference's title
+            The referenced work's title
         pages: str
-            The reference's pages
+            The pertinent pages of the referenced work
+        publisher: str
+            The referenced work's publisher
         publication_date: str
-            The reference's publication date in date form: yyy-mm-dd
+            The referenced work's publication date in date form: yyy-mm-dd
+        editor: str
+            The referenced work's editor
         created: str
-            The reference's creation date in datetime form: yyy-mm-dd hh:mm:ss
+            The referenced work's creation date in datetime form: yyy-mm-dd hh:mm:ss
         modified: str
-            The reference's last modification date in datetime form: yyy-mm-dd hh:mm:ss
+            The referenced work's last modification date in datetime form: yyy-mm-dd hh:mm:ss
         user: User
-            The user who owns this entry
+            The user who created this Bibliography entry
         story: Story
-            The story that the reference refers to
+            The Story to which this Bibliography entry belongs
         authors: List[BibliographyAuthor]
-            The authors of the reference
+            The author(s) of the referenced work
 
     Methods
     -------
         __repr__()
             Returns a string representation of the reference
         __str__()
             Returns a string representation of the reference
```

### Comparing `noveler-0.1.0/noveler/models/BibliographyAuthor.py` & `noveler-0.1.1/noveler/models/BibliographyAuthor.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,23 +38,27 @@
             Updates the author's attributes with the values from the dictionary
         validate_name(name: str)
             Validates the name's length
         validate_initials(initials: str)
             Validates the initials' length
     """
 
-    __tablename__ = 'bibliographies_authors'
+    __tablename__ = 'authors_bibliographies'
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
     user_id: Mapped[int] = mapped_column(Integer, ForeignKey('users.id'))
-    bibliography_id: Mapped[int] = mapped_column(Integer, ForeignKey('bibliographies.id'))
+    bibliography_id: Mapped[int] = mapped_column(
+        Integer, ForeignKey('bibliographies.id')
+    )
     name: Mapped[str] = mapped_column(String(150), nullable=False)
     initials: Mapped[str] = mapped_column(String(10), nullable=True)
     created: Mapped[str] = mapped_column(DateTime, default=str(datetime.now()))
     user: Mapped["User"] = relationship("User")
-    reference: Mapped["Bibliography"] = relationship("Bibliography", back_populates="authors")
+    reference: Mapped["Bibliography"] = relationship(
+        "Bibliography", back_populates="authors"
+    )
 
     def __repr__(self):
         """Returns a string representation of the author.
 
         Returns
         -------
         str
```

### Comparing `noveler-0.1.0/noveler/models/Chapter.py` & `noveler-0.1.1/noveler/models/Chapter.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/ChapterLink.py` & `noveler-0.1.1/noveler/models/ChapterLink.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/ChapterNote.py` & `noveler-0.1.1/noveler/models/ChapterNote.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/CharacterEvent.py` & `noveler-0.1.1/noveler/models/CharacterEvent.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/CharacterImage.py` & `noveler-0.1.1/noveler/models/CharacterImage.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/CharacterLink.py` & `noveler-0.1.1/noveler/models/CharacterLink.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/CharacterNote.py` & `noveler-0.1.1/noveler/models/CharacterNote.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/CharacterRelationship.py` & `noveler-0.1.1/noveler/models/CharacterRelationship.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/CharacterRelationshipTypes.py` & `noveler-0.1.1/noveler/models/CharacterRelationshipTypes.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/CharacterStory.py` & `noveler-0.1.1/noveler/models/CharacterStory.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/CharacterTrait.py` & `noveler-0.1.1/noveler/models/CharacterTrait.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/Event.py` & `noveler-0.1.1/noveler/models/Event.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional, List
 from sqlalchemy import Integer, ForeignKey, String, DateTime, Text
 from sqlalchemy.orm import Mapped, mapped_column, relationship, validates
 from noveler.models import User, EventLink, CharacterEvent, EventNote, EventLocation, Base
 
 
 class Event(Base):
-    """The Event class represents an event in a story.
+    """The Event class represents an event that is referenced by one or more stories.
 
     Attributes
     ----------
         id: int
             The event's id
         user_id: int
             The id of the owner of this entry
```

### Comparing `noveler-0.1.0/noveler/models/EventLink.py` & `noveler-0.1.1/noveler/models/EventLink.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/EventLocation.py` & `noveler-0.1.1/noveler/models/LocationNote.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,113 +1,100 @@
 from datetime import datetime
 from sqlalchemy import Integer, ForeignKey, DateTime
 from sqlalchemy.orm import Mapped, mapped_column, relationship
-from noveler.models import User, Event, Location, Base
+from noveler.models import User, Location, Note, Base
 
 
-class EventLocation(Base):
-    """The EventLocation class represents the relationship between an event and a location.
+class LocationNote(Base):
+    """The LocationNote class represents the relationship between a location and a note.
 
     Attributes
     ----------
         user_id: int
             The id of the owner of this entry
-        event_id: int
-            The event's id
         location_id: int
             The location's id
+        note_id: int
+            The note's id
         created: str
-            The creation datetime of the link between the Event and the Location
+            The creation datetime of the link between the Location and the Note
         user: User
             The user who owns this entry
-        event: Event
-            The event that the location belongs to
         location: Location
-            The location that the event has
+            The location that the note belongs to
+        note: Note
+            The note that the location has
 
     Methods
     -------
         __repr__()
             Returns a string representation of the relationship
         __str__()
             Returns a string representation of the relationship
         serialize()
             Returns a dictionary representation of the relationship
         unserialize(data: dict)
             Updates the relationship's attributes with the values from the dictionary
     """
 
-    __tablename__ = 'events_locations'
+    __tablename__ = 'locations_notes'
     user_id: Mapped[int] = mapped_column(Integer, ForeignKey('users.id'))
-    event_id: Mapped[int] = mapped_column(
-        Integer, ForeignKey('events.id'), primary_key=True
-    )
-    location_id: Mapped[int] = mapped_column(
-        Integer, ForeignKey('locations.id'), primary_key=True
-    )
+    location_id: Mapped[int] = mapped_column(Integer, ForeignKey('locations.id'), primary_key=True)
+    note_id: Mapped[int] = mapped_column(Integer, ForeignKey('notes.id'), primary_key=True)
     created: Mapped[str] = mapped_column(DateTime, default=str(datetime.now()))
     user: Mapped["User"] = relationship("User")
-    event: Mapped["Event"] = relationship(
-        "Event", back_populates="locations"
-    )
-    location: Mapped["Location"] = relationship(
-        "Location", back_populates="events"
-    )
+    location: Mapped["Location"] = relationship("Location", back_populates="notes")
+    note: Mapped["Note"] = relationship("Note", back_populates="locations")
 
     def __repr__(self):
         """Returns a string representation of the relationship.
 
         Returns
         -------
         str
             A string representation of the relationship
         """
 
-        return f'<EventLocation {self.event.title!r} - {self.location.title!r}>'
+        return f'<LocationNote {self.location.title!r} - {self.note.title!r}>'
 
     def __str__(self):
         """Returns a string representation of the relationship.
 
         Returns
         -------
         str
             A string representation of the relationship
         """
 
-        return f'{self.event.title} - {self.location.title}'
+        return f'{self.location.title} - {self.note.title}'
 
     def serialize(self) -> dict:
         """Returns a dictionary representation of the relationship.
 
         Returns
         -------
         dict
             A dictionary representation of the relationship
         """
 
         return {
             'user_id': self.user_id,
-            'event_id': self.event_id,
             'location_id': self.location_id,
+            'note_id': self.note_id,
             'created': str(self.created),
         }
 
-    def unserialize(self, data: dict) -> "EventLocation":
+    def unserialize(self, data: dict) -> "LocationNote":
         """Updates the relationship's attributes with the values from the dictionary.
 
         Parameters
         ----------
         data: dict
             The dictionary with the new values for the relationship
-
-        Returns
-        -------
-        EventLocation
-            The unserialized relationship
         """
 
         self.user_id = data.get('user_id', self.user_id)
-        self.event_id = data.get('event_id', self.event_id)
         self.location_id = data.get('location_id', self.location_id)
+        self.note_id = data.get('note_id', self.note_id)
         self.created = data.get('created', self.created)
 
         return self
```

### Comparing `noveler-0.1.0/noveler/models/EventNote.py` & `noveler-0.1.1/noveler/models/EventNote.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/Image.py` & `noveler-0.1.1/noveler/models/Image.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional, List
 from sqlalchemy import Integer, ForeignKey, String, DateTime
 from sqlalchemy.orm import Mapped, mapped_column, relationship, validates
 from noveler.models import ImageMimeTypes, User, CharacterImage, ImageLocation, Base
 
 
 class Image(Base):
-    """The Image class represents an image in the system.
+    """The Image class represents an image in the application.
 
     Attributes
     ----------
         id: int
             The image's id
         user_id: int
             The id of the owner of this entry
```

### Comparing `noveler-0.1.0/noveler/models/ImageLocation.py` & `noveler-0.1.1/noveler/models/ImageLocation.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/Link.py` & `noveler-0.1.1/noveler/models/Link.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from sqlalchemy import Integer, ForeignKey, String, DateTime
 from sqlalchemy.orm import Mapped, mapped_column, relationship, validates
 from noveler.models import User, LinkStory, ChapterLink, LinkScene, CharacterLink, EventLink, LinkLocation, Base
 from validators import url as url_validator
 
 
 class Link(Base):
-    """The Link class represents a link in the system.
+    """The Link class represents a web link in the application.
 
     Attributes
     ----------
         id: int
             The link's id
         user_id: int
             The id of the owner of this entry
```

### Comparing `noveler-0.1.0/noveler/models/LinkLocation.py` & `noveler-0.1.1/noveler/models/LinkLocation.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/LinkScene.py` & `noveler-0.1.1/noveler/models/LinkScene.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/LinkStory.py` & `noveler-0.1.1/noveler/models/LinkStory.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/noveler/models/Location.py` & `noveler-0.1.1/noveler/models/Location.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional, List
 from sqlalchemy import Integer, ForeignKey, String, Text, Float, DateTime
 from sqlalchemy.orm import Mapped, mapped_column, relationship, validates
 from noveler.models import User, ImageLocation, LinkLocation, EventLocation, LocationNote, Base
 
 
 class Location(Base):
-    """The Location class represents a location in the system.
+    """The Location class represents a location associated with one or more stories.
 
     Attributes
     ----------
         id: int
             The location's id
         user_id: int
             The id of the owner of this entry
```

### Comparing `noveler-0.1.0/noveler/models/LocationNote.py` & `noveler-0.1.1/noveler/models/NoteScene.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,100 +1,109 @@
 from datetime import datetime
 from sqlalchemy import Integer, ForeignKey, DateTime
 from sqlalchemy.orm import Mapped, mapped_column, relationship
-from noveler.models import User, Location, Note, Base
+from noveler.models import User, Note, Scene, Base
 
 
-class LocationNote(Base):
-    """The LocationNote class represents the relationship between a location and a note.
+class NoteScene(Base):
+    """The NoteScene class represents the relationship between a note and a scene.
 
     Attributes
     ----------
         user_id: int
             The id of the owner of this entry
-        location_id: int
-            The location's id
         note_id: int
             The note's id
+        scene_id: int
+            The scene's id
         created: str
-            The creation datetime of the link between the Location and the Note
+            The creation datetime of the link between the Note and the Scene
         user: User
             The user who owns this entry
-        location: Location
-            The location that the note belongs to
         note: Note
-            The note that the location has
+            The note that the scene belongs to
+        scene: Scene
+            The scene that the note has
 
     Methods
     -------
         __repr__()
             Returns a string representation of the relationship
         __str__()
             Returns a string representation of the relationship
         serialize()
             Returns a dictionary representation of the relationship
         unserialize(data: dict)
             Updates the relationship's attributes with the values from the dictionary
     """
 
-    __tablename__ = 'locations_notes'
+    __tablename__ = 'notes_scenes'
     user_id: Mapped[int] = mapped_column(Integer, ForeignKey('users.id'))
-    location_id: Mapped[int] = mapped_column(Integer, ForeignKey('locations.id'), primary_key=True)
     note_id: Mapped[int] = mapped_column(Integer, ForeignKey('notes.id'), primary_key=True)
+    scene_id: Mapped[int] = mapped_column(Integer, ForeignKey('scenes.id'), primary_key=True)
     created: Mapped[str] = mapped_column(DateTime, default=str(datetime.now()))
     user: Mapped["User"] = relationship("User")
-    location: Mapped["Location"] = relationship("Location", back_populates="notes")
-    note: Mapped["Note"] = relationship("Note", back_populates="locations")
+    note: Mapped["Note"] = relationship(
+        "Note", back_populates="scenes", lazy="joined"
+    )
+    scene: Mapped["Scene"] = relationship(
+        "Scene", back_populates="notes"
+    )
 
     def __repr__(self):
         """Returns a string representation of the relationship.
 
         Returns
         -------
         str
             A string representation of the relationship
         """
 
-        return f'<LocationNote {self.location.title!r} - {self.note.title!r}>'
+        return f'<NoteScene {self.note.title!r} - {self.scene.title!r}>'
 
     def __str__(self):
         """Returns a string representation of the relationship.
 
         Returns
         -------
         str
             A string representation of the relationship
         """
 
-        return f'{self.location.title} - {self.note.title}'
+        return f'{self.note.title} - {self.scene.title}'
 
     def serialize(self) -> dict:
         """Returns a dictionary representation of the relationship.
 
         Returns
         -------
         dict
             A dictionary representation of the relationship
         """
 
         return {
             'user_id': self.user_id,
-            'location_id': self.location_id,
             'note_id': self.note_id,
+            'scene_id': self.scene_id,
             'created': str(self.created),
         }
 
-    def unserialize(self, data: dict) -> "LocationNote":
+    def unserialize(self, data: dict) -> "NoteScene":
         """Updates the relationship's attributes with the values from the dictionary.
 
         Parameters
         ----------
         data: dict
             The dictionary with the new values for the relationship
+
+        Returns
+        -------
+        NoteScene
+            The unserialized relationship
         """
 
         self.user_id = data.get('user_id', self.user_id)
-        self.location_id = data.get('location_id', self.location_id)
         self.note_id = data.get('note_id', self.note_id)
+        self.scene_id = data.get('scene_id', self.scene_id)
         self.created = data.get('created', self.created)
 
         return self
```

### Comparing `noveler-0.1.0/noveler/models/Note.py` & `noveler-0.1.1/noveler/models/Note.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional, List
 from sqlalchemy import Integer, ForeignKey, String, Text, DateTime
 from sqlalchemy.orm import Mapped, mapped_column, relationship, validates
 from noveler.models import User, NoteStory, ChapterNote, NoteScene, CharacterNote, EventNote, LocationNote, Base
 
 
 class Note(Base):
-    """The Note class represents a note in the system.
+    """The Note class represents a note.
 
     Attributes
     ----------
         id: int
             The note's id
         user_id: int
             The id of the owner of this entry
```

### Comparing `noveler-0.1.0/noveler/models/NoteScene.py` & `noveler-0.1.1/noveler/models/NoteStory.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,109 +1,113 @@
 from datetime import datetime
 from sqlalchemy import Integer, ForeignKey, DateTime
 from sqlalchemy.orm import Mapped, mapped_column, relationship
-from noveler.models import User, Note, Scene, Base
+from noveler.models import User, Note, Story, Base
 
 
-class NoteScene(Base):
-    """The NoteScene class represents the relationship between a note and a scene.
+class NoteStory(Base):
+    """The NoteStory class represents the relationship between a note and a story.
 
     Attributes
     ----------
         user_id: int
             The id of the owner of this entry
         note_id: int
             The note's id
-        scene_id: int
-            The scene's id
+        story_id: int
+            The story's id
         created: str
-            The creation datetime of the link between the Note and the Scene
+            The creation datetime of the link between the Note and the Story
         user: User
             The user who owns this entry
         note: Note
-            The note that the scene belongs to
-        scene: Scene
-            The scene that the note has
+            The note that the story belongs to
+        story: Story
+            The story that the note has
 
     Methods
     -------
         __repr__()
             Returns a string representation of the relationship
         __str__()
             Returns a string representation of the relationship
         serialize()
             Returns a dictionary representation of the relationship
         unserialize(data: dict)
             Updates the relationship's attributes with the values from the dictionary
     """
 
-    __tablename__ = 'notes_scenes'
+    __tablename__ = 'notes_stories'
     user_id: Mapped[int] = mapped_column(Integer, ForeignKey('users.id'))
-    note_id: Mapped[int] = mapped_column(Integer, ForeignKey('notes.id'), primary_key=True)
-    scene_id: Mapped[int] = mapped_column(Integer, ForeignKey('scenes.id'), primary_key=True)
+    note_id: Mapped[int] = mapped_column(
+        Integer, ForeignKey('notes.id'), primary_key=True
+    )
+    story_id: Mapped[int] = mapped_column(
+        Integer, ForeignKey('stories.id'), primary_key=True
+    )
     created: Mapped[str] = mapped_column(DateTime, default=str(datetime.now()))
     user: Mapped["User"] = relationship("User")
     note: Mapped["Note"] = relationship(
-        "Note", back_populates="scenes", lazy="joined"
+        "Note", back_populates="stories", lazy="joined"
     )
-    scene: Mapped["Scene"] = relationship(
-        "Scene", back_populates="notes"
+    story: Mapped["Story"] = relationship(
+        "Story", back_populates="notes"
     )
 
     def __repr__(self):
         """Returns a string representation of the relationship.
 
         Returns
         -------
         str
             A string representation of the relationship
         """
 
-        return f'<NoteScene {self.note.title!r} - {self.scene.title!r}>'
+        return f'<NoteStory {self.note.title!r} - {self.story.title!r}>'
 
     def __str__(self):
         """Returns a string representation of the relationship.
 
         Returns
         -------
         str
             A string representation of the relationship
         """
 
-        return f'{self.note.title} - {self.scene.title}'
+        return f'{self.note.title} - {self.story.title}'
 
     def serialize(self) -> dict:
         """Returns a dictionary representation of the relationship.
 
         Returns
         -------
         dict
             A dictionary representation of the relationship
         """
 
         return {
             'user_id': self.user_id,
             'note_id': self.note_id,
-            'scene_id': self.scene_id,
+            'story_id': self.story_id,
             'created': str(self.created),
         }
 
-    def unserialize(self, data: dict) -> "NoteScene":
+    def unserialize(self, data: dict) -> "NoteStory":
         """Updates the relationship's attributes with the values from the dictionary.
 
         Parameters
         ----------
         data: dict
             The dictionary with the new values for the relationship
 
         Returns
         -------
-        NoteScene
+        NoteStory
             The unserialized relationship
         """
 
         self.user_id = data.get('user_id', self.user_id)
         self.note_id = data.get('note_id', self.note_id)
-        self.scene_id = data.get('scene_id', self.scene_id)
+        self.story_id = data.get('story_id', self.story_id)
         self.created = data.get('created', self.created)
 
         return self
```

### Comparing `noveler-0.1.0/noveler/models/OllamaModel.py` & `noveler-0.1.1/noveler/models/OllamaModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 from sqlalchemy import Integer, String, Text, DateTime
 from sqlalchemy.orm import Mapped, mapped_column, validates
 from noveler.models import Base
 
 
 class OllamaModel(Base):
-    """OllamaTemplate stores the name of the model, a description of the model, the template, and an example of the
+    """OllamaModel stores the name of the model, a description of the model, the template, and an example of the
     model's use.
     """
 
     __tablename__ = "ollama_models"
     id: Mapped[int] = mapped_column(Integer, primary_key=True)
     title: Mapped[str] = mapped_column(String(150), nullable=False)
     model: Mapped[str] = mapped_column(String(75), nullable=False)
```

### Comparing `noveler-0.1.0/noveler/models/Scene.py` & `noveler-0.1.1/noveler/models/Scene.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Optional, List
 from sqlalchemy import Integer, ForeignKey, String, DateTime, Text
 from sqlalchemy.orm import Mapped, mapped_column, relationship, validates
 from noveler.models import Chapter, User, LinkScene, NoteScene, Base
 
 
 class Scene(Base):
-    """The Scene class represents a scene in the system.
+    """The Scene class represents a scene in a chapter of a story.
 
     Attributes
     ----------
         id: int
             The scene's id
         user_id: int
             The id of the owner of this entry
```

### Comparing `noveler-0.1.0/noveler/models/Story.py` & `noveler-0.1.1/noveler/models/Story.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from sqlalchemy import Integer, ForeignKey, String, Text, DateTime
 from sqlalchemy.orm import Mapped, mapped_column, relationship, validates
 from noveler.models import User, Chapter, AuthorStory, Bibliography, Submission, LinkStory, NoteStory, CharacterStory, \
     Base
 
 
 class Story(Base):
-    """The Story class represents a story in the system.
+    """The Story class represents a story in the application.
 
     Attributes
     ----------
         id: int
             The story's id
         user_id: int
             The id of the owner of this entry
```

### Comparing `noveler-0.1.0/noveler/models/Submission.py` & `noveler-0.1.1/noveler/models/Submission.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime
 from sqlalchemy import Integer, ForeignKey, Text, Date, String, Float, DateTime
 from sqlalchemy.orm import Mapped, mapped_column, relationship, validates
 from noveler.models import SubmissionResultType, User, Story, Base
 
 
 class Submission(Base):
-    """The Submission class represents a submission in the system.
+    """The Submission class represents a submission of a story to some publisher or contest.
 
     Attributes
     ----------
         id: int
             The submission's id
         user_id: int
             The id of the owner of this entry
```

### Comparing `noveler-0.1.0/noveler/models/SubmissionResultType.py` & `noveler-0.1.1/noveler/models/SubmissionResultType.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from enum import Enum
 
 
 class SubmissionResultType(Enum):
-    """The SubmissionResultType class represents the possible results of a submission.
+    """The SubmissionResultType class represents the possible results or status of a story submission.
 
     Attributes
     ----------
         ACCEPTED: str
             The submission was accepted
         REJECTED: str
             The submission was rejected
```

### Comparing `noveler-0.1.0/noveler/models/User.py` & `noveler-0.1.1/noveler/models/User.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from noveler.models import Activity, Assistance, Author, Character, Event, Image, Link, Location, Note, Story, \
     Submission, Base
 from validators import email as email_validator
 from validators import uuid as uuid_validator
 
 
 class User(Base):
-    """The User class represents a user in the system.
+    """The User class represents a user in the application or the system user.
 
     Attributes
     ----------
         id: int
             The user's id
         uuid: str
             The user's UUID
```

### Comparing `noveler-0.1.0/noveler/models/__init__.py` & `noveler-0.1.1/noveler/models/__init__.py`

 * *Files identical despite different names*

### Comparing `noveler-0.1.0/pyproject.toml` & `noveler-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "noveler"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Richard Lucas <webmaster@applebiter.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project]
 name = "noveler"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Richard Lucas", email="webmaster@applebiter.com" },
 ]
 description = "Novel, short story, and serial authoring software"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `noveler-0.1.0/PKG-INFO` & `noveler-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noveler
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Richard Lucas
 Author-email: webmaster@applebiter.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -31,19 +31,19 @@
 needed.
 
 Using pip:
 From within your activated project, run `pip install noveler`.
 
 ### Usage
 Import the `Noveler` class from the `noveler` module and create a new 
-instance:
+instance. Pass in the path to the configuration file as the only argument.
 
     from noveler import Noveler
 
-    noveler = Noveler()
+    noveler = Noveler('path/to/noveler.cfg')
 
 To use a controller, pass a controller name to the noveler instance. For 
 example, to create a story do the following:
 
     story = noveler("story").create_story('title', 'description')
 
 You also create Chapter and Scene objects separately, and then append them to
@@ -67,8 +67,8 @@
 
 Noveler also exports Story and Character objects to plain text files, mainly to 
 use as input for the LLM tools. Noveler uses the Ollama ecosystem and supporting
 libraries to deliver a Retrieval-Augmented Generation session wherein the user 
 may talk to the LLM about a story and/or characters. The ability to export Events and
 Locations is not yet supported but will be in future releases.
 
-More documentation will be forthcoming.
+More documentation can be found in [this project's wiki](https://github.com/applebiter/noveler/wiki/Introduction-to-Noveler).
```

