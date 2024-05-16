# Comparing `tmp/motion2telegram-1.0.2.tar.gz` & `tmp/motion2telegram-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion2telegram-1.0.2.tar", last modified: Wed May 15 00:43:49 2024, max compression
+gzip compressed data, was "motion2telegram-1.1.0.tar", last modified: Thu May 16 10:40:55 2024, max compression
```

## Comparing `motion2telegram-1.0.2.tar` & `motion2telegram-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-15 00:43:48.999072 motion2telegram-1.0.2/
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)     1062 2024-05-12 22:06:34.000000 motion2telegram-1.0.2/LICENSE
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)      148 2024-05-14 10:52:39.000000 motion2telegram-1.0.2/MANIFEST.in
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)     3614 2024-05-15 00:43:48.989073 motion2telegram-1.0.2/PKG-INFO
--rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)     2484 2024-05-14 22:31:49.000000 motion2telegram-1.0.2/README.md
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)     1866 2024-05-15 00:39:02.000000 motion2telegram-1.0.2/pyproject.toml
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)       38 2024-05-15 00:43:48.999072 motion2telegram-1.0.2/setup.cfg
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)      529 2024-05-12 22:06:34.000000 motion2telegram-1.0.2/setup.py
-drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-15 00:43:48.559101 motion2telegram-1.0.2/src/
-drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-15 00:43:48.889079 motion2telegram-1.0.2/src/motion2telegram/
--rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)       84 2024-05-15 00:39:02.000000 motion2telegram-1.0.2/src/motion2telegram/__init__.py
--rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)     1261 2024-05-14 10:52:39.000000 motion2telegram-1.0.2/src/motion2telegram/cli.py
--rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)     2281 2024-05-14 23:54:04.000000 motion2telegram-1.0.2/src/motion2telegram/configure.py
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)      293 2024-05-14 10:52:39.000000 motion2telegram-1.0.2/src/motion2telegram/send.py
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)     5399 2024-05-14 10:52:39.000000 motion2telegram-1.0.2/src/motion2telegram/template.motion.conf
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)       37 2024-05-14 10:52:39.000000 motion2telegram-1.0.2/src/motion2telegram/template.motion.env
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)      256 2024-05-15 00:38:34.000000 motion2telegram-1.0.2/src/motion2telegram/template.motion.service
-drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-15 00:43:48.939076 motion2telegram-1.0.2/src/motion2telegram.egg-info/
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)     3614 2024-05-15 00:43:48.000000 motion2telegram-1.0.2/src/motion2telegram.egg-info/PKG-INFO
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)      558 2024-05-15 00:43:48.000000 motion2telegram-1.0.2/src/motion2telegram.egg-info/SOURCES.txt
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)        1 2024-05-15 00:43:48.000000 motion2telegram-1.0.2/src/motion2telegram.egg-info/dependency_links.txt
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)       60 2024-05-15 00:43:48.000000 motion2telegram-1.0.2/src/motion2telegram.egg-info/entry_points.txt
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)      172 2024-05-15 00:43:48.000000 motion2telegram-1.0.2/src/motion2telegram.egg-info/requires.txt
--rw-r--r--   0 p4irin    (1000) p4irin    (1000)       16 2024-05-15 00:43:48.000000 motion2telegram-1.0.2/src/motion2telegram.egg-info/top_level.txt
+drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-16 10:40:55.874286 motion2telegram-1.1.0/
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)     1062 2024-05-12 22:06:34.000000 motion2telegram-1.1.0/LICENSE
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)      148 2024-05-14 10:52:39.000000 motion2telegram-1.1.0/MANIFEST.in
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)     3740 2024-05-16 10:40:55.864286 motion2telegram-1.1.0/PKG-INFO
+-rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)     2610 2024-05-16 10:28:15.000000 motion2telegram-1.1.0/README.md
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)     1866 2024-05-16 10:12:17.000000 motion2telegram-1.1.0/pyproject.toml
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)       38 2024-05-16 10:40:55.874286 motion2telegram-1.1.0/setup.cfg
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)      529 2024-05-12 22:06:34.000000 motion2telegram-1.1.0/setup.py
+drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-16 10:40:55.674288 motion2telegram-1.1.0/src/
+drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-16 10:40:55.764287 motion2telegram-1.1.0/src/motion2telegram/
+-rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)       84 2024-05-16 10:12:17.000000 motion2telegram-1.1.0/src/motion2telegram/__init__.py
+-rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)     1261 2024-05-14 10:52:39.000000 motion2telegram-1.1.0/src/motion2telegram/cli.py
+-rwxr-xr-x   0 p4irin    (1000) p4irin    (1000)     2281 2024-05-14 23:54:04.000000 motion2telegram-1.1.0/src/motion2telegram/configure.py
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)      293 2024-05-14 10:52:39.000000 motion2telegram-1.1.0/src/motion2telegram/send.py
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)     5420 2024-05-16 10:28:15.000000 motion2telegram-1.1.0/src/motion2telegram/template.motion.conf
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)       37 2024-05-14 10:52:39.000000 motion2telegram-1.1.0/src/motion2telegram/template.motion.env
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)      256 2024-05-15 00:38:34.000000 motion2telegram-1.1.0/src/motion2telegram/template.motion.service
+drwxr-xr-x   0 p4irin    (1000) p4irin    (1000)        0 2024-05-16 10:40:55.814287 motion2telegram-1.1.0/src/motion2telegram.egg-info/
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)     3740 2024-05-16 10:40:55.000000 motion2telegram-1.1.0/src/motion2telegram.egg-info/PKG-INFO
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)      558 2024-05-16 10:40:55.000000 motion2telegram-1.1.0/src/motion2telegram.egg-info/SOURCES.txt
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)        1 2024-05-16 10:40:55.000000 motion2telegram-1.1.0/src/motion2telegram.egg-info/dependency_links.txt
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)       60 2024-05-16 10:40:55.000000 motion2telegram-1.1.0/src/motion2telegram.egg-info/entry_points.txt
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)      172 2024-05-16 10:40:55.000000 motion2telegram-1.1.0/src/motion2telegram.egg-info/requires.txt
+-rw-r--r--   0 p4irin    (1000) p4irin    (1000)       16 2024-05-16 10:40:55.000000 motion2telegram-1.1.0/src/motion2telegram.egg-info/top_level.txt
```

### Comparing `motion2telegram-1.0.2/LICENSE` & `motion2telegram-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `motion2telegram-1.0.2/PKG-INFO` & `motion2telegram-1.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion2telegram
-Version: 1.0.2
+Version: 1.1.0
 Summary: Notify a Telegram user when the motion service detects motion
 Author-email: p4irin <p4irin.github.io@gmail.com>
 Project-URL: Homepage, https://github.com/p4irin/motion2telegram
 Project-URL: Bug Tracker, https://github.com/p4irin/motion2telegram/issues
 Keywords: motion,python,telegram,motion-detection,webcam,raspberry-pi
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -61,34 +61,39 @@
 (venv) $ motion2telegram -V
 x.y.z
 (venv) $
 ```
 
 ## Configuration
 
-Create a motion.env file and change it's access permissions. This file is used by the motion service to retrieve the Telegram bot token and the recipient's chat id.
+Create a motion.env file with the following command.
 
 ```bash
 (venv) $ motion2telegram --init
 ```
+
+This file is used by the motion service to retrieve the Telegram bot token and the recipient's chat id.
+
 Specify your Telegram chat id and bot token in the file motion.env
 
 ```bash
 # motion.env
 TELEGRAM_BOT_TOKEN=
 TELEGRAM_CHAT_ID=
 ```
 
-Configure motion and install /etc/motion/motion.conf and /lib/systemd/system/motion.service.
+Configure motion with
 
 ```bash
 (venv) $ motion2telegram --configure
 ```
 
-motion is configured to write logs into log/motion.log and media files into media/ relative to the current directory.
+This will install /etc/motion/motion.conf and /lib/systemd/system/motion.service.
+
+Motion is configured to write logs into log/motion.log and media files into media/YYYYMMDD relative to the current directory. Media captured on the same date are grouped together in a YYYYMMDD directory.
 
-The motion systemd service will reference the motion.env file in the current directory. The command will stop, configure and bring the motion service back up.
+The motion systemd service will reference the motion.env file in the current directory for the chat id and the bot token. The command will stop, configure and bring the motion service back up.
 
 ## Reference
 
 - [Motion](https://motion-project.github.io/)
 - [Telegram](https://telegram.org/)
```

### Comparing `motion2telegram-1.0.2/README.md` & `motion2telegram-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -34,34 +34,39 @@
 (venv) $ motion2telegram -V
 x.y.z
 (venv) $
 ```
 
 ## Configuration
 
-Create a motion.env file and change it's access permissions. This file is used by the motion service to retrieve the Telegram bot token and the recipient's chat id.
+Create a motion.env file with the following command.
 
 ```bash
 (venv) $ motion2telegram --init
 ```
+
+This file is used by the motion service to retrieve the Telegram bot token and the recipient's chat id.
+
 Specify your Telegram chat id and bot token in the file motion.env
 
 ```bash
 # motion.env
 TELEGRAM_BOT_TOKEN=
 TELEGRAM_CHAT_ID=
 ```
 
-Configure motion and install /etc/motion/motion.conf and /lib/systemd/system/motion.service.
+Configure motion with
 
 ```bash
 (venv) $ motion2telegram --configure
 ```
 
-motion is configured to write logs into log/motion.log and media files into media/ relative to the current directory.
+This will install /etc/motion/motion.conf and /lib/systemd/system/motion.service.
+
+Motion is configured to write logs into log/motion.log and media files into media/YYYYMMDD relative to the current directory. Media captured on the same date are grouped together in a YYYYMMDD directory.
 
-The motion systemd service will reference the motion.env file in the current directory. The command will stop, configure and bring the motion service back up.
+The motion systemd service will reference the motion.env file in the current directory for the chat id and the bot token. The command will stop, configure and bring the motion service back up.
 
 ## Reference
 
 - [Motion](https://motion-project.github.io/)
 - [Telegram](https://telegram.org/)
```

### Comparing `motion2telegram-1.0.2/pyproject.toml` & `motion2telegram-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "motion2telegram"
-version = "1.0.2"
+version = "1.1.0"
 authors = [
   { name="p4irin", email="p4irin.github.io@gmail.com" },
 ]
 description = "Notify a Telegram user when the motion service detects motion"
 readme = "README.md"
 requires-python = ">=3.8.10"
 keywords = [
@@ -56,15 +56,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 
 [tool.bumpver]
-current_version = "1.0.2"
+current_version = "1.1.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "Bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 commit = true
 tag = true
 push = false
```

### Comparing `motion2telegram-1.0.2/setup.py` & `motion2telegram-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `motion2telegram-1.0.2/src/motion2telegram/cli.py` & `motion2telegram-1.1.0/src/motion2telegram/cli.py`

 * *Files identical despite different names*

### Comparing `motion2telegram-1.0.2/src/motion2telegram/configure.py` & `motion2telegram-1.1.0/src/motion2telegram/configure.py`

 * *Files identical despite different names*

### Comparing `motion2telegram-1.0.2/src/motion2telegram/template.motion.conf` & `motion2telegram-1.1.0/src/motion2telegram/template.motion.conf`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 ############################################################
 # Script execution configuration parameters
 ############################################################
 
 # Command to be executed when an event starts.
 ; on_event_start value
-on_event_start {% motion2telegram %} -p {% pwd %}/media/%Y%m%d%H%M%S-%q.jpg
+on_event_start {% motion2telegram %} -p {% pwd %}/media/%Y%m%d/%Y%m%d%H%M%S-%q.jpg
 
 # Command to be executed when an event ends.
 ; on_event_end value
 
 # Command to be executed when a movie file is closed.
 ; on_movie_end value
 
@@ -115,15 +115,15 @@
 # Picture output configuration parameters
 ############################################################
 
 # Output pictures when motion is detected
 picture_output on
 
 # File name(without extension) for pictures relative to target directory
-picture_filename %Y%m%d%H%M%S-%q
+picture_filename %Y%m%d/%Y%m%d%H%M%S-%q
 
 ############################################################
 # Movie output configuration parameters
 ############################################################
 
 # Create movies of motion events.
 movie_output off
@@ -134,15 +134,15 @@
 # The encoding quality of the movie. (0=use bitrate. 1=worst quality, 100=best)
 movie_quality 45
 
 # Container/Codec to used for the movie. See motion_guide.html
 movie_codec mkv
 
 # File name(without extension) for movies relative to target directory
-movie_filename %t-%v-%Y%m%d%H%M%S
+movie_filename %Y%m%d/%t-%v-%Y%m%d%H%M%S
 
 ############################################################
 # Webcontrol configuration parameters
 ############################################################
 
 # Port number used for the webcontrol.
 ;webcontrol_port 8080
```

### Comparing `motion2telegram-1.0.2/src/motion2telegram.egg-info/PKG-INFO` & `motion2telegram-1.1.0/src/motion2telegram.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion2telegram
-Version: 1.0.2
+Version: 1.1.0
 Summary: Notify a Telegram user when the motion service detects motion
 Author-email: p4irin <p4irin.github.io@gmail.com>
 Project-URL: Homepage, https://github.com/p4irin/motion2telegram
 Project-URL: Bug Tracker, https://github.com/p4irin/motion2telegram/issues
 Keywords: motion,python,telegram,motion-detection,webcam,raspberry-pi
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -61,34 +61,39 @@
 (venv) $ motion2telegram -V
 x.y.z
 (venv) $
 ```
 
 ## Configuration
 
-Create a motion.env file and change it's access permissions. This file is used by the motion service to retrieve the Telegram bot token and the recipient's chat id.
+Create a motion.env file with the following command.
 
 ```bash
 (venv) $ motion2telegram --init
 ```
+
+This file is used by the motion service to retrieve the Telegram bot token and the recipient's chat id.
+
 Specify your Telegram chat id and bot token in the file motion.env
 
 ```bash
 # motion.env
 TELEGRAM_BOT_TOKEN=
 TELEGRAM_CHAT_ID=
 ```
 
-Configure motion and install /etc/motion/motion.conf and /lib/systemd/system/motion.service.
+Configure motion with
 
 ```bash
 (venv) $ motion2telegram --configure
 ```
 
-motion is configured to write logs into log/motion.log and media files into media/ relative to the current directory.
+This will install /etc/motion/motion.conf and /lib/systemd/system/motion.service.
+
+Motion is configured to write logs into log/motion.log and media files into media/YYYYMMDD relative to the current directory. Media captured on the same date are grouped together in a YYYYMMDD directory.
 
-The motion systemd service will reference the motion.env file in the current directory. The command will stop, configure and bring the motion service back up.
+The motion systemd service will reference the motion.env file in the current directory for the chat id and the bot token. The command will stop, configure and bring the motion service back up.
 
 ## Reference
 
 - [Motion](https://motion-project.github.io/)
 - [Telegram](https://telegram.org/)
```

### Comparing `motion2telegram-1.0.2/src/motion2telegram.egg-info/SOURCES.txt` & `motion2telegram-1.1.0/src/motion2telegram.egg-info/SOURCES.txt`

 * *Files identical despite different names*

