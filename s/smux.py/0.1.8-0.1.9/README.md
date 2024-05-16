# Comparing `tmp/smux.py-0.1.8.tar.gz` & `tmp/smux.py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/smux.py-0.1.8.tar", last modified: Mon Dec 21 03:15:38 2020, max compression
+gzip compressed data, was "dist/smux.py-0.1.9.tar", last modified: Mon Dec 21 23:16:12 2020, max compression
```

## Comparing `smux.py-0.1.8.tar` & `smux.py-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 hq6       (1000) hq6       (1000)        0 2020-12-21 03:15:38.988671 smux.py-0.1.8/
--rw-rw-r--   0 hq6       (1000) hq6       (1000)     2490 2020-12-21 03:15:38.988671 smux.py-0.1.8/PKG-INFO
--rw-r--r--   0 hq6       (1000) hq6       (1000)     1519 2018-07-24 22:55:05.000000 smux.py-0.1.8/README.md
--rw-rw-r--   0 hq6       (1000) hq6       (1000)       38 2020-12-21 03:15:38.988671 smux.py-0.1.8/setup.cfg
--rw-rw-r--   0 hq6       (1000) hq6       (1000)     2147 2020-12-21 03:15:27.000000 smux.py-0.1.8/setup.py
--rwxrwxr-x   0 hq6       (1000) hq6       (1000)     8472 2020-12-21 03:15:27.000000 smux.py-0.1.8/smux.py
-drwxrwxr-x   0 hq6       (1000) hq6       (1000)        0 2020-12-21 03:15:38.988671 smux.py-0.1.8/smux.py.egg-info/
--rw-rw-r--   0 hq6       (1000) hq6       (1000)     2490 2020-12-21 03:15:38.000000 smux.py-0.1.8/smux.py.egg-info/PKG-INFO
--rw-rw-r--   0 hq6       (1000) hq6       (1000)      150 2020-12-21 03:15:38.000000 smux.py-0.1.8/smux.py.egg-info/SOURCES.txt
--rw-rw-r--   0 hq6       (1000) hq6       (1000)        1 2020-12-21 03:15:38.000000 smux.py-0.1.8/smux.py.egg-info/dependency_links.txt
--rw-rw-r--   0 hq6       (1000) hq6       (1000)        5 2020-12-21 03:15:38.000000 smux.py-0.1.8/smux.py.egg-info/top_level.txt
+drwxrwxr-x   0 hq6       (1000) hq6       (1000)        0 2020-12-21 23:16:12.633415 smux.py-0.1.9/
+-rw-rw-r--   0 hq6       (1000) hq6       (1000)     2496 2020-12-21 23:16:12.633415 smux.py-0.1.9/PKG-INFO
+-rw-r--r--   0 hq6       (1000) hq6       (1000)     1513 2020-12-21 10:26:53.000000 smux.py-0.1.9/README.md
+-rw-rw-r--   0 hq6       (1000) hq6       (1000)       38 2020-12-21 23:16:12.633415 smux.py-0.1.9/setup.cfg
+-rw-rw-r--   0 hq6       (1000) hq6       (1000)     2153 2020-12-21 23:16:09.000000 smux.py-0.1.9/setup.py
+-rwxrwxr-x   0 hq6       (1000) hq6       (1000)     9406 2020-12-21 23:11:07.000000 smux.py-0.1.9/smux.py
+drwxrwxr-x   0 hq6       (1000) hq6       (1000)        0 2020-12-21 23:16:12.633415 smux.py-0.1.9/smux.py.egg-info/
+-rw-rw-r--   0 hq6       (1000) hq6       (1000)     2496 2020-12-21 23:16:12.000000 smux.py-0.1.9/smux.py.egg-info/PKG-INFO
+-rw-rw-r--   0 hq6       (1000) hq6       (1000)      150 2020-12-21 23:16:12.000000 smux.py-0.1.9/smux.py.egg-info/SOURCES.txt
+-rw-rw-r--   0 hq6       (1000) hq6       (1000)        1 2020-12-21 23:16:12.000000 smux.py-0.1.9/smux.py.egg-info/dependency_links.txt
+-rw-rw-r--   0 hq6       (1000) hq6       (1000)        5 2020-12-21 23:16:12.000000 smux.py-0.1.9/smux.py.egg-info/top_level.txt
```

### Comparing `smux.py-0.1.8/PKG-INFO` & `smux.py-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: smux.py
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple tmux launcher that will take less than 2 minutes to learn and should work across all versions of tmux
 Home-page: https://github.com/hq6/smux
 Author: Henry Qin
 Author-email: root@hq6.me
 License: MIT
 Description: 
         smux
@@ -26,15 +26,15 @@
         * tmux (any version)
         
         Installation
         ========================================
         
         Run the following command::
         
-            sudo pip install smux.py
+            pip3 install --upgrade smux.py
         
         Usage (as a command line tool)
         ========================================
         
         0. Create a new file, either from scratch or by copying Sample.smux_.
         1. (Optional) Specify ``PANES_PER_WINDOW`` and ``LAYOUT`` and ``NO_CREATE`` as
            described in the usage message.
```

### Comparing `smux.py-0.1.8/README.md` & `smux.py-0.1.9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 debug) distributed systems bugs that required sshing into a lot of servers and
 starting processes, smux is a general purpose tmux launcher whose input
 resembles in all respects a concatenation of bash scripts to be run on each
 terminal.
 
 ## Dependencies
 
- - Python 2 or 3
+ - Python 3.8+
  - tmux (any version)
 
 ## Installation
 
 Manual Method:
 
     git clone https://github.com/hq6/smux.git
     # Add the directory to your PATH
 
 Automatic Method:
 
-    sudo pip install smux.py
+    pip3 install smux.py
 
 ## Usage (as a command line tool)
    
    0. Create a new file, either from scratch or by copying Sample.smux.
    1. (Optional) Specify PANES_PER_WINDOW and LAYOUT as described in the usage message.
    2. For every pane you want to launch, write an entry of the following form.
          ```
```

### Comparing `smux.py-0.1.8/setup.py` & `smux.py-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 * tmux (any version)
 
 Installation
 ========================================
 
 Run the following command::
 
-    sudo pip install smux.py
+    pip3 install --upgrade smux.py
 
 Usage (as a command line tool)
 ========================================
 
 0. Create a new file, either from scratch or by copying Sample.smux_.
 1. (Optional) Specify ``PANES_PER_WINDOW`` and ``LAYOUT`` and ``NO_CREATE`` as
    described in the usage message.
@@ -62,15 +62,15 @@
              ])
 
 .. _Sample.smux: https://github.com/hq6/smux/blob/master/Sample.smux
 """
 
 setup(
   name="smux.py",
-  version='0.1.8',
+  version='0.1.9',
   author="Henry Qin",
   author_email="root@hq6.me",
   description="Simple tmux launcher that will take less than 2 minutes to learn and should work across all versions of tmux",
   long_description=long_description,
   platforms=["All platforms that tmux runs on."],
   license="MIT",
   url="https://github.com/hq6/smux",
```

### Comparing `smux.py-0.1.8/smux.py` & `smux.py-0.1.9/smux.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,14 +81,24 @@
    if not window: window = getCurrentWindow()
    # If the command is a directive to smux itself, then do not pass it through.
    if cmd.startswith("#smux "):
        # Skip the initial command
        args = shlex.split(cmd)[1:]
        if args[0] == 'paste-buffer':
            tcmd(f"paste-buffer -t ':{window}.{pane}' " + shlex.join(args[1:]))
+       elif args[0] == 'send-keys':
+           # This option is useful for sending something like "Enter" with
+           # semantic meaning, rather than literally. This is needed rather
+           # than just allowing the script to directly invoke `tmux send-keys`
+           # because the target pane may be runnig a completely different
+           # process which we want to feed special input to (e.g. it is waiting
+           # for the user to type a special key such as Enter).
+           tcmd(f"send-keys -t ':{window}.{pane}' " + shlex.join(args[1:]))
+       elif args[0] == 'sleep':
+           time.sleep(float(args[1]))
        return
    # We must send commands one character to avoid weird quote treatment by the
    # sell when invoking send-keys.
    if ex:
        tcmd(f"send-keys -t {window}.{pane} -l " + prepareCommand(cmd))
        tcmd(f"send-keys -t {window}.{pane} Enter")
    else:
@@ -125,14 +135,20 @@
        return
    tmux = os.environ.get('TMUX')
    if noCreate and (not tmux or len(commands) != 1):
        print("noCreate parameter ignored because we are not in a tmux session or len(commands) != 1")
    if not tmux:
        tcmd("new-session -d")
    elif noCreate and len(commands) == 1:
+       # Run ourselves in a subshell, so that Python does not consume the input
+       # intended for the new foreground processes started by the script.
+       if not os.environ.get('SMUX_SUBSHELL'):
+           os.system(f'SMUX_SUBSHELL=1 {shlex.join(sys.argv)}  & > /dev/null 2>&1')
+           return
+
        # Target the current window that invoked this command.
        currentWindow = getCurrentWindow()
        currentPane = getCurrentPane()
        for x in commands[0]:
           sendCommand(x, currentPane, currentWindow)
        return
    else:
```

### Comparing `smux.py-0.1.8/smux.py.egg-info/PKG-INFO` & `smux.py-0.1.9/smux.py.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: smux.py
-Version: 0.1.8
+Version: 0.1.9
 Summary: Simple tmux launcher that will take less than 2 minutes to learn and should work across all versions of tmux
 Home-page: https://github.com/hq6/smux
 Author: Henry Qin
 Author-email: root@hq6.me
 License: MIT
 Description: 
         smux
@@ -26,15 +26,15 @@
         * tmux (any version)
         
         Installation
         ========================================
         
         Run the following command::
         
-            sudo pip install smux.py
+            pip3 install --upgrade smux.py
         
         Usage (as a command line tool)
         ========================================
         
         0. Create a new file, either from scratch or by copying Sample.smux_.
         1. (Optional) Specify ``PANES_PER_WINDOW`` and ``LAYOUT`` and ``NO_CREATE`` as
            described in the usage message.
```

