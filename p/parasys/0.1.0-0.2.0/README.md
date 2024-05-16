# Comparing `tmp/parasys-0.1.0.tar.gz` & `tmp/parasys-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parasys-0.1.0.tar", last modified: Wed May 15 05:43:12 2024, max compression
+gzip compressed data, was "parasys-0.2.0.tar", last modified: Thu May 16 15:50:16 2024, max compression
```

## Comparing `parasys-0.1.0.tar` & `parasys-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 avramscore   (501) staff       (20)        0 2024-05-15 05:43:12.829275 parasys-0.1.0/
--rw-r--r--   0 avramscore   (501) staff       (20)     1087 2024-05-15 03:16:32.000000 parasys-0.1.0/LICENSE
--rw-r--r--   0 avramscore   (501) staff       (20)     1368 2024-05-15 05:43:12.829078 parasys-0.1.0/PKG-INFO
--rw-r--r--   0 avramscore   (501) staff       (20)      651 2024-05-15 03:20:38.000000 parasys-0.1.0/README.md
-drwxr-xr-x   0 avramscore   (501) staff       (20)        0 2024-05-15 05:43:12.827988 parasys-0.1.0/parasys/
--rw-r--r--   0 avramscore   (501) staff       (20)        0 2024-05-15 02:09:37.000000 parasys-0.1.0/parasys/__init__.py
--rw-r--r--   0 avramscore   (501) staff       (20)     4332 2024-05-15 03:02:36.000000 parasys-0.1.0/parasys/monitor.py
-drwxr-xr-x   0 avramscore   (501) staff       (20)        0 2024-05-15 05:43:12.828814 parasys-0.1.0/parasys.egg-info/
--rw-r--r--   0 avramscore   (501) staff       (20)     1368 2024-05-15 05:43:12.000000 parasys-0.1.0/parasys.egg-info/PKG-INFO
--rw-r--r--   0 avramscore   (501) staff       (20)      253 2024-05-15 05:43:12.000000 parasys-0.1.0/parasys.egg-info/SOURCES.txt
--rw-r--r--   0 avramscore   (501) staff       (20)        1 2024-05-15 05:43:12.000000 parasys-0.1.0/parasys.egg-info/dependency_links.txt
--rw-r--r--   0 avramscore   (501) staff       (20)       49 2024-05-15 05:43:12.000000 parasys-0.1.0/parasys.egg-info/entry_points.txt
--rw-r--r--   0 avramscore   (501) staff       (20)       33 2024-05-15 05:43:12.000000 parasys-0.1.0/parasys.egg-info/requires.txt
--rw-r--r--   0 avramscore   (501) staff       (20)        8 2024-05-15 05:43:12.000000 parasys-0.1.0/parasys.egg-info/top_level.txt
--rw-r--r--   0 avramscore   (501) staff       (20)       38 2024-05-15 05:43:12.829309 parasys-0.1.0/setup.cfg
--rw-r--r--   0 avramscore   (501) staff       (20)     1099 2024-05-15 03:17:26.000000 parasys-0.1.0/setup.py
+drwxr-xr-x   0 avramscore   (501) staff       (20)        0 2024-05-16 15:50:16.268435 parasys-0.2.0/
+-rw-r--r--   0 avramscore   (501) staff       (20)     1087 2024-05-15 03:16:32.000000 parasys-0.2.0/LICENSE
+-rw-r--r--   0 avramscore   (501) staff       (20)     1395 2024-05-16 15:50:16.268215 parasys-0.2.0/PKG-INFO
+-rw-r--r--   0 avramscore   (501) staff       (20)      651 2024-05-15 03:20:38.000000 parasys-0.2.0/README.md
+drwxr-xr-x   0 avramscore   (501) staff       (20)        0 2024-05-16 15:50:16.266832 parasys-0.2.0/parasys/
+-rw-r--r--   0 avramscore   (501) staff       (20)        0 2024-05-15 02:09:37.000000 parasys-0.2.0/parasys/__init__.py
+-rw-r--r--   0 avramscore   (501) staff       (20)     5082 2024-05-16 13:37:31.000000 parasys-0.2.0/parasys/monitor.py
+drwxr-xr-x   0 avramscore   (501) staff       (20)        0 2024-05-16 15:50:16.267900 parasys-0.2.0/parasys.egg-info/
+-rw-r--r--   0 avramscore   (501) staff       (20)     1395 2024-05-16 15:50:16.000000 parasys-0.2.0/parasys.egg-info/PKG-INFO
+-rw-r--r--   0 avramscore   (501) staff       (20)      253 2024-05-16 15:50:16.000000 parasys-0.2.0/parasys.egg-info/SOURCES.txt
+-rw-r--r--   0 avramscore   (501) staff       (20)        1 2024-05-16 15:50:16.000000 parasys-0.2.0/parasys.egg-info/dependency_links.txt
+-rw-r--r--   0 avramscore   (501) staff       (20)       49 2024-05-16 15:50:16.000000 parasys-0.2.0/parasys.egg-info/entry_points.txt
+-rw-r--r--   0 avramscore   (501) staff       (20)       45 2024-05-16 15:50:16.000000 parasys-0.2.0/parasys.egg-info/requires.txt
+-rw-r--r--   0 avramscore   (501) staff       (20)        8 2024-05-16 15:50:16.000000 parasys-0.2.0/parasys.egg-info/top_level.txt
+-rw-r--r--   0 avramscore   (501) staff       (20)       38 2024-05-16 15:50:16.268471 parasys-0.2.0/setup.cfg
+-rw-r--r--   0 avramscore   (501) staff       (20)     1072 2024-05-16 14:09:43.000000 parasys-0.2.0/setup.py
```

### Comparing `parasys-0.1.0/LICENSE` & `parasys-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parasys-0.1.0/PKG-INFO` & `parasys-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parasys
-Version: 0.1.0
+Version: 0.2.0
 Summary: A platform-agnostic command-line tool for system monitoring.
 Home-page: https://github.com/avigold/parasys
 Author: Avram Score
 Author-email: ascore@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Monitoring
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil
+Requires-Dist: asciimatics
 Provides-Extra: windows
 Requires-Dist: windows-curses; extra == "windows"
 
 # Parasys
 
 `parasys` is a command-line tool designed to monitor and display system performance metrics such as CPU usage and memory consumption in realtime. It offers a lightweight, efficient solution for system administrators, developers, or any user who needs to monitor his or her system's resources.
```

### Comparing `parasys-0.1.0/README.md` & `parasys-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `parasys-0.1.0/parasys/monitor.py` & `parasys-0.2.0/parasys/monitor.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,104 +1,128 @@
 import sys
 import psutil
-import time
+from collections import deque
+
 try:
     import curses
 except ImportError:
     if sys.platform.startswith('win'):
         try:
-            import windows_curses as curses # might as well support windows
+            import windows_curses as curses
         except ImportError:
             print("The curses module is required to run parasys. Please install with 'pip install windows-curses'.")
             sys.exit(1)
     else:
         raise ImportError("Failed to import the curses module.")
 
 def draw_bar(stdscr, y, x, max_width, percentage, label):
     max_label_width = max_width - 20  # reserve some space for the bar itself
     label = label[:max_label_width]  # ensure label does not exceed the space
     bar_length = max_width - len(label) - 10 
     filled_length = int(bar_length * percentage / 100)
     bar_graph = f"{label} [{'#' * filled_length}{'.' * (bar_length - filled_length)}]"
     stdscr.addstr(y, x, bar_graph)
 
-def draw_process_list(stdscr, start_y, start_x, processes, title, max_x):
-    stdscr.addstr(start_y, start_x, title[:max_x])  # ensure the title fits within the screen width
-    for i, proc in enumerate(processes):
-        try:
-            cpu_percent = 0.0 if proc.info['cpu_percent'] is None else proc.info['cpu_percent']
-            memory_percent = 0.0 if proc.info['memory_percent'] is None else proc.info['memory_percent']
-            proc_info = f"{proc.pid:>5} {proc.info['name'][:15]:<15} {cpu_percent:>5.1f}% {memory_percent:>5.1f}%"
-            stdscr.addstr(start_y + i + 1, start_x, proc_info[:max_x])
-        except (psutil.NoSuchProcess, psutil.AccessDenied, curses.error) as e:
-            print("Error displaying process:", e)
+def draw_line_graph(stdscr, y, x, data, label, width):
+    stdscr.addstr(y, x, label)
+    max_data = max(data) if data else 1
+    graph_height = 10
+    data_points = list(data)[-width:]
+    for i, value in enumerate(data_points):
+        bar_height = int((value / max_data) * graph_height)
+        for j in range(graph_height):
+            char = '#' if j < bar_height else ' '
+            stdscr.addstr(y + graph_height - j, x + i + len(label) + 1, char)
+
+def draw_process_list(stdscr, start_y, start_x, processes, title, max_x, max_y, display_type):
+    stdscr.addstr(start_y, start_x, title[:max_x])
+
+    if display_type == 'cpu':
+        headers = "  PID Name               CPU%"
+    elif display_type == 'memory':
+        headers = "  PID Name               MEM%"
 
+    stdscr.addstr(start_y + 1, start_x, headers[:max_x])
+    max_processes = max_y - start_y - 3
+
+    for i, proc in enumerate(processes[:max_processes]):
+        try:
+            if display_type == 'cpu':
+                num_cores = psutil.cpu_count
+                cpu_percent = proc['cpu_percent']
+                proc_info = f"{proc['pid']:>5} {proc['name'][:15]:<15} {cpu_percent / num_cores():>6.1f}%"
+            elif display_type == 'memory':
+                memory_percent = proc['memory_percent']
+                proc_info = f"{proc['pid']:>5} {proc['name'][:15]:<15} {memory_percent:>6.1f}%"
+            stdscr.addstr(start_y + i + 2, start_x, proc_info[:max_x])
+        except curses.error:
+            continue
 
 def get_top_processes_by_cpu():
-    processes = psutil.process_iter(['name', 'cpu_percent', 'memory_percent'])
+    processes = list(psutil.process_iter(['pid', 'name', 'cpu_percent']))
     valid_processes = []
     for p in processes:
         try:
-            p.info['cpu_percent'] = 0.0 if p.info['cpu_percent'] is None else p.info['cpu_percent']
-            p.info['memory_percent'] = 0.0 if p.info['memory_percent'] is None else p.info['memory_percent']
-            valid_processes.append(p)
+            cpu_percent = p.cpu_percent(interval=None)
+            valid_processes.append({'pid': p.pid, 'name': p.info['name'], 'cpu_percent': cpu_percent})
         except (psutil.NoSuchProcess, psutil.AccessDenied):
             continue
-    return sorted(valid_processes, key=lambda p: p.info['cpu_percent'], reverse=True)[:20]
+    return sorted(valid_processes, key=lambda p: p['cpu_percent'], reverse=True)[:20]
 
 def get_top_processes_by_memory():
-    processes = psutil.process_iter(['name', 'cpu_percent', 'memory_percent'])
+    processes = psutil.process_iter(['pid', 'name', 'memory_percent'])
     valid_processes = []
     for p in processes:
         try:
-            p.info['memory_percent'] = 0.0 if p.info['memory_percent'] is None else p.info['memory_percent']
-            valid_processes.append(p)
+            memory_percent = p.memory_percent()
+            valid_processes.append({'pid': p.pid, 'name': p.info['name'], 'memory_percent': memory_percent})
         except (psutil.NoSuchProcess, psutil.AccessDenied):
             continue
-    return sorted(valid_processes, key=lambda p: p.info['memory_percent'], reverse=True)[:20]
-
+    return sorted(valid_processes, key=lambda p: p['memory_percent'], reverse=True)[:20]
 
 def main(stdscr):
-    curses.curs_set(0)  # hide the cursor
+    curses.curs_set(0) # hide cursor
     curses.noecho()
-    stdscr.nodelay(True)  # do not wait for input when calling getch
+    stdscr.nodelay(True)
+
+    cpu_data = deque(maxlen=50)
+    memory_data = deque(maxlen=50)
     
     try:
         while True:
             stdscr.erase()
-            max_y, max_x = stdscr.getmaxyx()  # get the size of the window
+            max_y, max_x = stdscr.getmaxyx()
 
-            cpu_percent = psutil.cpu_percent(interval=0.1)
+            cpu_percent = psutil.cpu_percent(interval=1)
             memory = psutil.virtual_memory()
             mem_amount = memory.used
             mem_percent = memory.percent
 
-            display_text = [
-                f"CPU Usage: {cpu_percent}%",
-                f"Memory Usage: {round(mem_amount / (1024 ** 3), 2)}GB ({mem_percent}%) of {round(memory.total / (1024 ** 3), 2)}GB",
-            ]
+            cpu_data.append(cpu_percent)
+            memory_data.append(mem_percent)
+
+            draw_line_graph(stdscr, 1, 0, list(cpu_data), "CPU Usage Over Time: ", max_x - 1)
+            draw_line_graph(stdscr, 15, 0, list(memory_data), "Memory Usage Over Time: ", max_x - 1)
 
-            draw_bar(stdscr, 1, 0, max_x, cpu_percent, display_text[0])
-            draw_bar(stdscr, 3, 0, max_x, mem_percent, display_text[1])
+            draw_bar(stdscr, 13, 0, max_x, cpu_percent, f"Current CPU Usage: {cpu_percent}%")
+            draw_bar(stdscr, 27, 0, max_x, mem_percent, f"CurrentMemory Usage: {round(mem_amount / (1024 ** 3), 2)}GB ({mem_percent}%) of {round(memory.total / (1024 ** 3), 2)}GB")
 
             top_cpu = get_top_processes_by_cpu()
             top_memory = get_top_processes_by_memory()
             half_width = max_x // 2
-            draw_process_list(stdscr, 5, 0, top_cpu, "Top CPU Processes", max_x // 2)
-            draw_process_list(stdscr, 5, half_width, top_memory, "Top Memory Processes", max_x // 2)
+            draw_process_list(stdscr, 30, 0, top_cpu, "Top CPU Processes", half_width, max_y, 'cpu')
+            draw_process_list(stdscr, 30, half_width, top_memory, "Top Memory Processes", half_width, max_y, 'memory')
 
             stdscr.refresh()
-            time.sleep(1)  # update interval
 
-            # check for the 'q' key to quit
+            # pressing q can quit
             k = stdscr.getch()
             if k == ord('q'):
                 break
     except KeyboardInterrupt:
-        # handle ctrl + c gracefully
         pass
     finally:
         # cleanup
         curses.nocbreak()
         stdscr.keypad(False)
         curses.echo()
         curses.endwin()
```

### Comparing `parasys-0.1.0/parasys.egg-info/PKG-INFO` & `parasys-0.2.0/parasys.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parasys
-Version: 0.1.0
+Version: 0.2.0
 Summary: A platform-agnostic command-line tool for system monitoring.
 Home-page: https://github.com/avigold/parasys
 Author: Avram Score
 Author-email: ascore@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Monitoring
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psutil
+Requires-Dist: asciimatics
 Provides-Extra: windows
 Requires-Dist: windows-curses; extra == "windows"
 
 # Parasys
 
 `parasys` is a command-line tool designed to monitor and display system performance metrics such as CPU usage and memory consumption in realtime. It offers a lightweight, efficient solution for system administrators, developers, or any user who needs to monitor his or her system's resources.
```

### Comparing `parasys-0.1.0/setup.py` & `parasys-0.2.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup, find_packages
 
-# Conditionally add windows-specific dependencies
+
 extras = {
-    'windows': ['windows-curses']  # Required for curses support on Windows
+    'windows': ['windows-curses']  # required for curses support on Windows
 }
 
 setup(
     name='parasys',
-    version='0.1.0',
+    version='0.2.0',
     author='Avram Score',
     author_email='ascore@gmail.com',
     description='A platform-agnostic command-line tool for system monitoring.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/avigold/parasys',
     packages=find_packages(),
     install_requires=[
         'psutil',
+        'asciimatics'
     ],
     extras_require=extras,
     entry_points={
         'console_scripts': [
             'parasys=parasys.monitor:main',
         ],
     },
```

