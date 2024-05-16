# Comparing `tmp/wandarr-1.0.9.tar.gz` & `tmp/wandarr-1.1.0.tar.gz`

## Comparing `wandarr-1.0.9.tar` & `wandarr-1.1.0.tar`

### file list

```diff
@@ -1,56 +1,57 @@
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 wandarr-1.0.9/CHANGES.md
--rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 wandarr-1.0.9/FAQ.md
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 wandarr-1.0.9/agent.md
--rwxr-xr-x   0        0        0       54 2020-02-02 00:00:00.000000 wandarr-1.0.9/build.sh
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 wandarr-1.0.9/examples.md
--rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 wandarr-1.0.9/host-types.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wandarr-1.0.9/main.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 wandarr-1.0.9/play.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 wandarr-1.0.9/setup.py
--rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 wandarr-1.0.9/upload.sh
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 wandarr-1.0.9/.github/workflows/pypi.yml
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 wandarr-1.0.9/config-samples/quickstart.yml
--rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 wandarr-1.0.9/config-samples/wandarr.yml
--rw-r--r--   0        0        0    24498 2020-02-02 00:00:00.000000 wandarr-1.0.9/diagrams/agent-unshared.jpg
--rw-r--r--   0        0        0   107956 2020-02-02 00:00:00.000000 wandarr-1.0.9/diagrams/host-types.png
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 wandarr-1.0.9/docs/agent.md
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 wandarr-1.0.9/docs/examples.md
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 wandarr-1.0.9/docs/host-types.md
--rw-r--r--   0        0        0    24498 2020-02-02 00:00:00.000000 wandarr-1.0.9/docs/diagrams/agent-unshared.jpg
--rw-r--r--   0        0        0   231883 2020-02-02 00:00:00.000000 wandarr-1.0.9/docs/diagrams/cluster-1.jpg
--rw-r--r--   0        0        0   107956 2020-02-02 00:00:00.000000 wandarr-1.0.9/docs/diagrams/host-types.png
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 wandarr-1.0.9/tests/__init__.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 wandarr-1.0.9/tests/basic_config.yml
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 wandarr-1.0.9/tests/ffmpeg.txt
--rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 wandarr-1.0.9/tests/ffprobe.json
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 wandarr-1.0.9/tests/fixtures.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 wandarr-1.0.9/tests/test_cluster.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 wandarr-1.0.9/tests/test_config.py
--rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 wandarr-1.0.9/tests/test_hosts.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wandarr-1.0.9/tests/test_parsers.py
--rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr/__init__.py
--rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr/__main__.py
--rwxr-xr-x   0        0        0     9397 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr/agent.py
--rwxr-xr-x   0        0        0     9769 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr/agenthost.py
--rwxr-xr-x   0        0        0     8844 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr/base.py
--rwxr-xr-x   0        0        0    12195 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr/cluster.py
--rwxr-xr-x   0        0        0     2506 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr/config.py
--rwxr-xr-x   0        0        0     8804 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr/ffmpeg.py
--rwxr-xr-x   0        0        0     4477 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr/localhost.py
--rwxr-xr-x   0        0        0    11536 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr/media.py
--rwxr-xr-x   0        0        0     5162 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr/mountedhost.py
--rwxr-xr-x   0        0        0     6965 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr/streaminghost.py
--rwxr-xr-x   0        0        0     3542 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr/template.py
--rwxr-xr-x   0        0        0     5471 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr/transcode.py
--rwxr-xr-x   0        0        0     4209 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr/utils.py
--rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr.egg-info/PKG-INFO
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr.egg-info/entry_points.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr.egg-info/requires.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 wandarr-1.0.9/wandarr.egg-info/top_level.txt
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 wandarr-1.0.9/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wandarr-1.0.9/LICENSE
--rw-r--r--   0        0        0    14984 2020-02-02 00:00:00.000000 wandarr-1.0.9/README.md
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 wandarr-1.0.9/pyproject.toml
--rw-r--r--   0        0        0    15871 2020-02-02 00:00:00.000000 wandarr-1.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 wandarr-1.1.0/CHANGES.md
+-rw-r--r--   0        0        0     3444 2020-02-02 00:00:00.000000 wandarr-1.1.0/FAQ.md
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 wandarr-1.1.0/agent.md
+-rwxr-xr-x   0        0        0       54 2020-02-02 00:00:00.000000 wandarr-1.1.0/build.sh
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 wandarr-1.1.0/examples.md
+-rw-r--r--   0        0        0     3192 2020-02-02 00:00:00.000000 wandarr-1.1.0/host-types.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wandarr-1.1.0/main.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 wandarr-1.1.0/play.py
+-rw-r--r--   0        0        0    21757 2020-02-02 00:00:00.000000 wandarr-1.1.0/pylintrc
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 wandarr-1.1.0/setup.py
+-rwxr-xr-x   0        0        0       30 2020-02-02 00:00:00.000000 wandarr-1.1.0/upload.sh
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 wandarr-1.1.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 wandarr-1.1.0/config-samples/quickstart.yml
+-rw-r--r--   0        0        0     7468 2020-02-02 00:00:00.000000 wandarr-1.1.0/config-samples/wandarr.yml
+-rw-r--r--   0        0        0    24498 2020-02-02 00:00:00.000000 wandarr-1.1.0/diagrams/agent-unshared.jpg
+-rw-r--r--   0        0        0   107956 2020-02-02 00:00:00.000000 wandarr-1.1.0/diagrams/host-types.png
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 wandarr-1.1.0/docs/agent.md
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 wandarr-1.1.0/docs/examples.md
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 wandarr-1.1.0/docs/host-types.md
+-rw-r--r--   0        0        0    24498 2020-02-02 00:00:00.000000 wandarr-1.1.0/docs/diagrams/agent-unshared.jpg
+-rw-r--r--   0        0        0   231883 2020-02-02 00:00:00.000000 wandarr-1.1.0/docs/diagrams/cluster-1.jpg
+-rw-r--r--   0        0        0   107956 2020-02-02 00:00:00.000000 wandarr-1.1.0/docs/diagrams/host-types.png
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 wandarr-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 wandarr-1.1.0/tests/basic_config.yml
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 wandarr-1.1.0/tests/ffmpeg.txt
+-rw-r--r--   0        0        0     7156 2020-02-02 00:00:00.000000 wandarr-1.1.0/tests/ffprobe.json
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 wandarr-1.1.0/tests/fixtures.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 wandarr-1.1.0/tests/test_cluster.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 wandarr-1.1.0/tests/test_config.py
+-rw-r--r--   0        0        0     5161 2020-02-02 00:00:00.000000 wandarr-1.1.0/tests/test_hosts.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wandarr-1.1.0/tests/test_parsers.py
+-rwxr-xr-x   0        0        0      300 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr/__init__.py
+-rwxr-xr-x   0        0        0       59 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr/__main__.py
+-rwxr-xr-x   0        0        0     9355 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr/agent.py
+-rwxr-xr-x   0        0        0     9841 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr/agenthost.py
+-rwxr-xr-x   0        0        0     8855 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr/base.py
+-rwxr-xr-x   0        0        0    12083 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr/cluster.py
+-rwxr-xr-x   0        0        0     2505 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr/config.py
+-rwxr-xr-x   0        0        0     8829 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr/ffmpeg.py
+-rwxr-xr-x   0        0        0     4477 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr/localhost.py
+-rwxr-xr-x   0        0        0    11513 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr/media.py
+-rwxr-xr-x   0        0        0     5162 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr/mountedhost.py
+-rwxr-xr-x   0        0        0     6965 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr/streaminghost.py
+-rwxr-xr-x   0        0        0     3542 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr/template.py
+-rwxr-xr-x   0        0        0     5471 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr/transcode.py
+-rwxr-xr-x   0        0        0     3586 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr/utils.py
+-rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr.egg-info/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr.egg-info/entry_points.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr.egg-info/requires.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 wandarr-1.1.0/wandarr.egg-info/top_level.txt
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 wandarr-1.1.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 wandarr-1.1.0/LICENSE
+-rw-r--r--   0        0        0    14984 2020-02-02 00:00:00.000000 wandarr-1.1.0/README.md
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 wandarr-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    15871 2020-02-02 00:00:00.000000 wandarr-1.1.0/PKG-INFO
```

### Comparing `wandarr-1.0.9/CHANGES.md` & `wandarr-1.1.0/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 ## Changes
 
+#### 05/16/2024 v1.1.0
+* Fixed bug in progress calculation for agent mode.
+
 #### 05/10/2024 v1.0.9
 * More updates to compensate for ffmpeg 7.0 occasional missing or erroneous time calculations.
 
 #### 05/2/2024 v1.0.8
 * Added compatibility with new ffmpeg (7.0) changes that prevented progress updates.
 
 #### 02/27/2024 v1.0.7
```

### Comparing `wandarr-1.0.9/FAQ.md` & `wandarr-1.1.0/FAQ.md`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/agent.md` & `wandarr-1.1.0/agent.md`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/examples.md` & `wandarr-1.1.0/examples.md`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/host-types.md` & `wandarr-1.1.0/host-types.md`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/setup.py` & `wandarr-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/.github/workflows/pypi.yml` & `wandarr-1.1.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/config-samples/quickstart.yml` & `wandarr-1.1.0/config-samples/quickstart.yml`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/config-samples/wandarr.yml` & `wandarr-1.1.0/config-samples/wandarr.yml`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/diagrams/agent-unshared.jpg` & `wandarr-1.1.0/diagrams/agent-unshared.jpg`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/diagrams/host-types.png` & `wandarr-1.1.0/diagrams/host-types.png`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/docs/agent.md` & `wandarr-1.1.0/docs/agent.md`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/docs/examples.md` & `wandarr-1.1.0/docs/examples.md`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/docs/host-types.md` & `wandarr-1.1.0/docs/host-types.md`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/docs/diagrams/agent-unshared.jpg` & `wandarr-1.1.0/docs/diagrams/agent-unshared.jpg`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/docs/diagrams/cluster-1.jpg` & `wandarr-1.1.0/docs/diagrams/cluster-1.jpg`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/docs/diagrams/host-types.png` & `wandarr-1.1.0/docs/diagrams/host-types.png`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/tests/basic_config.yml` & `wandarr-1.1.0/tests/basic_config.yml`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/tests/ffmpeg.txt` & `wandarr-1.1.0/tests/ffmpeg.txt`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/tests/ffprobe.json` & `wandarr-1.1.0/tests/ffprobe.json`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/tests/fixtures.py` & `wandarr-1.1.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/tests/test_cluster.py` & `wandarr-1.1.0/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/tests/test_config.py` & `wandarr-1.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/tests/test_hosts.py` & `wandarr-1.1.0/tests/test_hosts.py`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/tests/test_parsers.py` & `wandarr-1.1.0/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/wandarr/agent.py` & `wandarr-1.1.0/wandarr/agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import socket
 import os
 import subprocess
 import sys
-import time
 from threading import Thread
-from typing import List
 
 import wandarr
 
 
 class Runner(Thread):
     def __init__(self, c, addr, thread_id: int):
         super().__init__(name=f"Runner {thread_id}", daemon=True)
@@ -123,25 +121,25 @@
                             # transcode complete
                             break
 
                         confirmation = response.decode()
                         if confirmation == "PING":
                             # ping received out of context, ignore
                             continue
-                        elif confirmation == "STOP":
+                        if confirmation == "STOP":
                             proc.kill()
                             print(f"[{self.thread_id}] Client stopped the transcode, cleaning up")
                             vetoed = True
                             break
-                        elif confirmation == "VETO":
+                        if confirmation == "VETO":
                             proc.kill()
                             print(f"[{self.thread_id}] Client vetoed the transcode, cleaning up")
                             vetoed = True
                             break
-                        elif confirmation != "ACK!":
+                        if confirmation != "ACK!":
                             proc.kill()
                             print(f"[{self.thread_id}] Protocol error - expected ACK from client, got {confirmation}")
                             print("Cleaning up")
                             vetoed = True
                             break
 
                     # wait for process to end
```

### Comparing `wandarr-1.0.9/wandarr/agenthost.py` & `wandarr-1.1.0/wandarr/agenthost.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 class AgentManagedHost(ManagedHost):
     """Implementation of an agent host worker thread"""
 
     def __init__(self, hostname, props: RemoteHostProperties, queue: Queue):
         super().__init__(hostname, props, queue)
 
+        self.remote_in_path = None
+        self.remote_out_path = None
+
     #
     # override the standard ssh-based host_ok for agent verification
     #
     def host_ok(self):
         if not super().ping_test_ok():
             return False
```

### Comparing `wandarr-1.0.9/wandarr/base.py` & `wandarr-1.1.0/wandarr/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,15 +170,15 @@
     def testrun(self):
         pass
 
     def converted_path(self, path):
         if " " in path:
             path = '"' + path + '"'
         if self.props.is_windows():
-            path = path.replace(' ', '\ ')
+            path = path.replace(' ', '\\')
             return str(PureWindowsPath(path))
         return str(PosixPath(path))
 
     def ssh_cmd(self):
         return [wandarr.SSH, self.props.user + '@' + self.props.ip]
 
     def ping_test_ok(self):
@@ -186,15 +186,15 @@
         if os.name == "nt":
             ping = [r'C:\WINDOWS\system32\ping.exe', '-n', '1', '-w', '5', addr]
         else:
             ping = ['ping', '-c', '1', '-W', '5', addr]
         with subprocess.Popen(ping, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=False) as p:
             p.communicate()
             if p.returncode != 0:
-                self.log(f"Host at address {addr} cannot be reached - skipped", style="magenta")
+                self.log(f"ping test: Host at address {addr} cannot be reached - skipped", style="magenta")
                 return False
             return True
 
     def ssh_test_ok(self):
         try:
             remote_cmd = 'dir' if self.props.is_windows() else 'ls'
             # remote_cmd = 'ls'
```

### Comparing `wandarr-1.0.9/wandarr/cluster.py` & `wandarr-1.1.0/wandarr/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,34 +74,31 @@
 
                         case "mounted":
                             if wandarr.VERBOSE:
                                 print(f"{host=} {qname=} {host_engine_name=} {cli=}")
                             if not self._init_host_mounted(host, host_props, qname, host_engine_name, cli, host not in up_hosts):
                                 down_hosts.append(host)
                                 continue
-                            else:
-                                up_hosts.append(host)
+                            up_hosts.append(host)
 
                         case "streaming":
                             if wandarr.VERBOSE:
                                 print(f"{host=} {qname=} {host_engine_name=} {cli=}")
                             if not self._init_host_streaming(host, host_props, qname, host_engine_name, cli, host not in up_hosts):
                                 down_hosts.append(host)
                                 continue
-                            else:
-                                up_hosts.append(host)
+                            up_hosts.append(host)
 
                         case "agent":
                             if wandarr.VERBOSE:
                                 print(f"{host=} {qname=} {host_engine_name=} {cli=}")
                             if not self._init_host_agent(host, host_props, qname, host_engine_name, cli, host not in up_hosts):
-                               down_hosts.append(host)
-                               continue
-                            else:
-                                up_hosts.append(host)
+                                down_hosts.append(host)
+                                continue
+                            up_hosts.append(host)
 
                         case _:
                             print(f'Unknown cluster host type "{host_type}" - skipping')
 
     def _init_host_local(self, host: str, host_props: RemoteHostProperties, qname: str, engine_name: str, cli: str):
         _h = LocalHost(host, host_props, self.queues[qname])
         if not _h.validate_settings():
```

### Comparing `wandarr-1.0.9/wandarr/config.py` & `wandarr-1.1.0/wandarr/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,8 +81,7 @@
     @property
     def ffmpeg_path(self):
         return self.settings['ffmpeg']
 
     @property
     def ssh_path(self):
         return self.settings.get('ssh', '/usr/bin/ssh')
-
```

### Comparing `wandarr-1.0.9/wandarr/ffmpeg.py` & `wandarr-1.1.0/wandarr/ffmpeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,16 +186,15 @@
                 if c.startswith("DONE|") or c.startswith("ERR|"):
 #                    print("Transcode complete")
                     # found end of processing marker
                     try:
                         if c.startswith("ERR|"):
                             print(f"See error log at {self.log_path}")
                             break
-                        else:
-                            os.remove(str(self.log_path))
+                        os.remove(str(self.log_path))
                         self.log_path = None
                     except Exception as ex:
                         print(str(ex))
 
                     yield c
 
                 sock.send(bytes("ACK!".encode()))
@@ -203,14 +202,15 @@
 
                 match = status_re.match(line)
                 if match is not None and len(match.groups()) >= 5:
                     if datetime.datetime.now() > event:
                         event = datetime.datetime.now() + diff
                         info: Dict[str, Any] = match.groupdict()
 
+                        info['frame'] = int(info['frame'])
                         info['size'] = int(info['size'].strip()) * 1024
                         hh, mm, ss = info['time'].split(':')
                         ss = ss.split('.')[0]
                         info['time'] = (int(hh) * 3600) + (int(mm) * 60) + int(ss)
                         yield info
 
     def run(self, params, event_callback) -> Optional[int]:
```

### Comparing `wandarr-1.0.9/wandarr/localhost.py` & `wandarr-1.1.0/wandarr/localhost.py`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/wandarr/media.py` & `wandarr-1.1.0/wandarr/media.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         self.fps = info['fps']
         self.colorspace = info['colorspace']
         self.audio: List[StreamInfoWrapper] = info['audio']
         self.subtitle: List[StreamInfoWrapper] = info['subtitle']
 
     def __str__(self):
         runtime = "{:0>8}".format(str(timedelta(seconds=self.runtime)))
-        print("DEBUG")
         for a in self.audio:
             print(a)
 
         audios = []
         for a in self.audio:
             dind = '*' if a.default == "1" else ''
             lang = a.lang
```

### Comparing `wandarr-1.0.9/wandarr/mountedhost.py` & `wandarr-1.1.0/wandarr/mountedhost.py`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/wandarr/streaminghost.py` & `wandarr-1.1.0/wandarr/streaminghost.py`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/wandarr/template.py` & `wandarr-1.1.0/wandarr/template.py`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/wandarr/transcode.py` & `wandarr-1.1.0/wandarr/transcode.py`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/wandarr/utils.py` & `wandarr-1.1.0/wandarr/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,32 +22,18 @@
         try:
             with urllib.request.urlopen(
                     "https://raw.githubusercontent.com/mlsmithjr/wandarr/master/wandarr/__init__.py") as response:
                 page = response.read().decode("utf-8")
                 match = re.search(r'^__version__.=.[\'\"](\w\.\w\.\w)[\'\"]', page)
                 if match:
                     self.version = match.group(1)
-
         except Exception as ex:
             # nothing we can do about this anyhow
             pass
 
-# def pypi_latest_version() -> Optional[str]:
-#     try:
-#         with urllib.request.urlopen("https://github.com/mlsmithjr/wandarr/blob/master/wandarr/__init__.py") as response:
-# #        with urllib.request.urlopen('https://pypi.org/project/wandarr/') as response:
-#             page = response.read()
-# #            match = re.search(r'.*<h1>.*wan (\w\.\w\.\w).*</h1>', page)
-#             match = re.search(r'^__version__.=.[\'\"](\w\.\w\.\w)[\'\"]', page)
-#             if match:
-#                 return match.group(0)
-#     except:
-#         # nothing we can do about this anyhow
-#         pass
-#     return None
 
 def filter_threshold(template: Template, in_path: str, out_path: str):
     if template.threshold() > 0:
         orig_size = os.path.getsize(in_path)
         new_size = os.path.getsize(out_path)
         return is_exceeded_threshold(template.threshold(), orig_size, new_size)
     return True
```

### Comparing `wandarr-1.0.9/wandarr.egg-info/PKG-INFO` & `wandarr-1.1.0/wandarr.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/LICENSE` & `wandarr-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/README.md` & `wandarr-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `wandarr-1.0.9/pyproject.toml` & `wandarr-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "wandarr"
-version = "1.0.9"
+version = "1.1.0"
 authors = [
   { name="Marshall L Smith Jr", email="marshallsmithjr@gmail.com" }
 ]
 description = "A ffmpeg transcoding workflow engine with clustered host support"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `wandarr-1.0.9/PKG-INFO` & `wandarr-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: wandarr
-Version: 1.0.9
+Version: 1.1.0
 Summary: A ffmpeg transcoding workflow engine with clustered host support
 Project-URL: Homepage, https://github.com/mlsmithjr/wandarr
 Author-email: Marshall L Smith Jr <marshallsmithjr@gmail.com>
 License-File: LICENSE
 Keywords: cuda,encode,ffmpeg,qsv,transcode
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

