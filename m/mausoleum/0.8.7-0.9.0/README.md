# Comparing `tmp/mausoleum-0.8.7.tar.gz` & `tmp/mausoleum-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mausoleum-0.8.7.tar", last modified: Mon Oct  1 00:49:51 2018, max compression
+gzip compressed data, was "mausoleum-0.9.0.tar", last modified: Tue Oct 18 18:34:00 2022, max compression
```

## Comparing `mausoleum-0.8.7.tar` & `mausoleum-0.9.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-01 00:49:51.000000 mausoleum-0.8.7/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4877 2018-10-01 00:47:45.000000 mausoleum-0.8.7/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)      941 2018-10-01 00:47:45.000000 mausoleum-0.8.7/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-01 00:49:51.000000 mausoleum-0.8.7/mausoleum.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2018-10-01 00:49:50.000000 mausoleum-0.8.7/mausoleum.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2018-10-01 00:49:50.000000 mausoleum-0.8.7/mausoleum.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      536 2018-10-01 00:49:50.000000 mausoleum-0.8.7/mausoleum.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-10-01 00:49:50.000000 mausoleum-0.8.7/mausoleum.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       96 2018-10-01 00:49:50.000000 mausoleum-0.8.7/mausoleum.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      408 2018-10-01 00:49:50.000000 mausoleum-0.8.7/mausoleum.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2018-10-01 00:49:51.000000 mausoleum-0.8.7/setup.cfg
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-01 00:49:51.000000 mausoleum-0.8.7/mausoleum/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10794 2018-10-01 00:47:45.000000 mausoleum-0.8.7/mausoleum/wrapper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2018-10-01 00:47:45.000000 mausoleum-0.8.7/mausoleum/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-10-01 00:47:45.000000 mausoleum-0.8.7/mausoleum/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2018-10-01 00:47:45.000000 mausoleum-0.8.7/mausoleum/settings.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)    28513 2018-10-01 00:47:45.000000 mausoleum-0.8.7/mausoleum/application.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-01 00:49:51.000000 mausoleum-0.8.7/mausoleum/images/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2018-10-01 00:47:45.000000 mausoleum-0.8.7/mausoleum/images/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      342 2018-10-01 00:47:45.000000 mausoleum-0.8.7/mausoleum/images/ic_vpn_key_black_48dp_1x.png
--rw-rw-r--   0 travis    (2000) travis    (2000)      536 2018-10-01 00:49:51.000000 mausoleum-0.8.7/PKG-INFO
+drwxr-xr-x   0 mandeep   (1000) mandeep   (1001)        0 2022-10-18 18:34:00.355939 mausoleum-0.9.0/
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)    32886 2022-10-18 18:19:21.000000 mausoleum-0.9.0/LICENSE
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)      485 2022-10-18 18:34:00.355939 mausoleum-0.9.0/PKG-INFO
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)     4857 2022-10-18 18:19:21.000000 mausoleum-0.9.0/README.rst
+drwxr-xr-x   0 mandeep   (1000) mandeep   (1001)        0 2022-10-18 18:34:00.351939 mausoleum-0.9.0/mausoleum/
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)        0 2022-10-18 18:19:21.000000 mausoleum-0.9.0/mausoleum/__init__.py
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)       41 2022-10-18 18:19:21.000000 mausoleum-0.9.0/mausoleum/__main__.py
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)    27876 2022-10-18 18:19:21.000000 mausoleum-0.9.0/mausoleum/application.py
+drwxr-xr-x   0 mandeep   (1000) mandeep   (1001)        0 2022-10-18 18:34:00.355939 mausoleum-0.9.0/mausoleum/images/
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)        0 2022-10-18 18:19:21.000000 mausoleum-0.9.0/mausoleum/images/__init__.py
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)      342 2022-10-18 18:19:21.000000 mausoleum-0.9.0/mausoleum/images/ic_vpn_key_black_48dp_1x.png
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)       99 2022-10-18 18:19:21.000000 mausoleum-0.9.0/mausoleum/settings.toml
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)    11341 2022-10-18 18:19:21.000000 mausoleum-0.9.0/mausoleum/wrapper.py
+drwxr-xr-x   0 mandeep   (1000) mandeep   (1001)        0 2022-10-18 18:34:00.355939 mausoleum-0.9.0/mausoleum.egg-info/
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)      485 2022-10-18 18:34:00.000000 mausoleum-0.9.0/mausoleum.egg-info/PKG-INFO
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)      416 2022-10-18 18:34:00.000000 mausoleum-0.9.0/mausoleum.egg-info/SOURCES.txt
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)        1 2022-10-18 18:34:00.000000 mausoleum-0.9.0/mausoleum.egg-info/dependency_links.txt
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)       95 2022-10-18 18:34:00.000000 mausoleum-0.9.0/mausoleum.egg-info/entry_points.txt
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)       41 2022-10-18 18:34:00.000000 mausoleum-0.9.0/mausoleum.egg-info/requires.txt
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)       10 2022-10-18 18:34:00.000000 mausoleum-0.9.0/mausoleum.egg-info/top_level.txt
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)       38 2022-10-18 18:34:00.355939 mausoleum-0.9.0/setup.cfg
+-rw-r--r--   0 mandeep   (1000) mandeep   (1001)      941 2022-10-18 18:28:40.000000 mausoleum-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mausoleum-0.8.7/README.rst` & `mausoleum-0.9.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -115,16 +115,16 @@
 .. |travis| image:: https://img.shields.io/travis/mandeep/Mausoleum/master.svg
     :target: https://travis-ci.org/mandeep/Mausoleum/
 .. |coveralls| image:: https://img.shields.io/coveralls/mandeep/Mausoleum.svg 
     :target: https://coveralls.io/github/mandeep/Mausoleum
 .. |quality| image:: https://img.shields.io/scrutinizer/g/mandeep/Mausoleum.svg
     :target: https://scrutinizer-ci.com/g/mandeep/Mausoleum/
 .. |pypiversion| image:: https://img.shields.io/pypi/v/mausoleum.svg 
-    :target: https://pypi.python.org/pypi/mausoleum/
+    :target: https://pypi.org/project/mausoleum/
 .. |pypistatus| image:: https://img.shields.io/pypi/status/mausoleum.svg 
-    :target: https://pypi.python.org/pypi/mausoleum/
+    :target: https://pypi.org/project/mausoleum/
 .. |pythonversion| image:: https://img.shields.io/pypi/pyversions/mausoleum.svg 
-    :target: https://pypi.python.org/pypi/mausoleum/
+    :target: https://pypi.org/project/mausoleum/
 .. |pypiformat| image:: https://img.shields.io/pypi/format/mausoleum.svg
-    :target: https://pypi.python.org/pypi/mausoleum/
+    :target: https://pypi.org/project/mausoleum/
 .. |license| image:: https://img.shields.io/pypi/l/mausoleum.svg
-    :target: https://pypi.python.org/pypi/mausoleum/
+    :target: https://pypi.org/project/mausoleum/
```

### Comparing `mausoleum-0.8.7/setup.py` & `mausoleum-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='mausoleum',
-    version='0.8.7',
+    version='0.9.0',
     description='A Python GUI, CLI, and wrapper for Tomb',
     author='Mandeep',
     author_email='info@mandeep.xyz',
     license='GPLv3+',
     url='https://github.com/mandeep/Mausoleum',
     packages=['mausoleum', 'mausoleum.images'],
     package_data={'mausoleum.images': ['*.png'], 'mausoleum': ['*.toml']},
@@ -22,11 +22,11 @@
         'click==7.0',
         'pytoml==0.1.13',
     ],
     keywords='Mausoleum',
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Development Status :: 4 - Beta',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ]
 )
```

### Comparing `mausoleum-0.8.7/mausoleum/wrapper.py` & `mausoleum-0.9.0/mausoleum/wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,29 +94,32 @@
         else:
             fabrication = forge_tomb(key, password)
 
         if fabrication == 0:
             lock_tomb(name, key, password)
 
 
-def open_tomb(name, key, password, path='tomb', read_only=False, sudo=None):
+def open_tomb(name, key, password, path='tomb', read_only=False, sudo=None, mountpoint=None):
     """Open a tomb container with the given key.
 
     Positional arguments:
     name -- the name of the container, e.g. secret.tomb
     key -- the name of the container's key, e.g. secret.tomb.key
     password -- the password of the container's key
 
     Keyword arguments:
+    mountpoint -- where to mount the tomb
     path -- the path to the tomb executable
     read_only -- mount the tomb as read only
     sudo -- the sudo password of the current admin, default is None
     """
     arguments = ['sudo', '--stdin', path, 'open', '--unsafe',
-                 '--tomb-pwd', password, name, '-k', key]
+                 '--tomb-pwd', password, '-k', key, name]
+    if mountpoint:
+        arguments.append(mountpoint)
     if read_only:
         arguments.extend(['-o', 'ro'])
 
     if sudo is not None:
         open_command = subprocess.Popen(arguments, stdin=subprocess.PIPE,
                                         stdout=subprocess.PIPE, universal_newlines=True)
         return open_command.communicate(sudo + '\n')
@@ -274,24 +277,32 @@
         open_tomb(name, key, password)
 
 
 @cli.command()
 @click.argument('name')
 @click.argument('key', required=False, default=None)
 @click.option('--password', prompt=True, hide_input=True, confirmation_prompt=False)
-def enter(name, key, password):
+@click.option('--mountpoint', default=None)
+def enter(name, key, password, mountpoint):
     """Open an existing tomb container.
 
     The default key name is the name of the tomb with .key as the suffix. If the
     key uses a different naming convention, it must be passed as an argument.
     """
     if key is None:
         key = '{}.key' .format(name)
 
-    open_tomb(name, key, password)
+    open_tomb(name, key, password, mountpoint=mountpoint)
+
+
+@cli.command()
+@click.argument('name')
+def leave(name):
+    """Close a currently open tomb."""
+    close_tomb(name=name)
 
 
 @cli.command()
 @click.argument('name')
 @click.argument('size')
 @click.argument('key', required=False, default=None)
 @click.option('--password', prompt=True, hide_input=True, confirmation_prompt=False)
@@ -337,7 +348,21 @@
 
 @cli.command()
 @click.argument('image')
 @click.option('--password', prompt=True, hide_input=True, confirmation_prompt=False)
 def resurrect(image, password):
     """Print to stdout a tomb key that's embedded in a JPEG image."""
     exhume_tomb(image, password)
+
+
+@cli.command(name='list')
+def list_cmd():
+    """Lists all known tombs."""
+    tombs = list_tombs()
+    for tomb in tombs:
+        print(tomb)
+
+
+@cli.command()
+def escape():
+    """Slams shut all open tombs."""
+    slam_tombs()
```

### Comparing `mausoleum-0.8.7/mausoleum/application.py` & `mausoleum-0.9.0/mausoleum/application.py`

 * *Files 8% similar despite different names*

```diff
@@ -58,45 +58,37 @@
 
         size_box_layout = QHBoxLayout()
         size_box_label = QLabel('Size (MB):')
         self.size_box = QSpinBox()
         self.size_box.setMaximum(999999)
         self.size_box.setMinimum(10)
         self.size_box.setFixedWidth(100)
+        size_box_label.setBuddy(self.size_box)
         size_box_layout.addWidget(size_box_label)
         size_box_layout.addWidget(self.size_box)
         size_box_layout.setSpacing(0)
 
         kdf_box_layout = QHBoxLayout()
         kdf_box_label = QLabel('KDF Iterations:')
         self.kdf_box = QSpinBox()
         self.kdf_box.setFixedWidth(100)
+        kdf_box_label.setBuddy(self.kdf_box)
         kdf_box_layout.addWidget(kdf_box_label)
         kdf_box_layout.addWidget(self.kdf_box)
 
         spinbox_layout = QVBoxLayout()
         spinbox_layout.addLayout(size_box_layout)
         spinbox_layout.addLayout(kdf_box_layout)
         spinbox_layout.setAlignment(Qt.AlignLeft)
 
-        open_checkbox_layout = QHBoxLayout()
-        open_checkbox_label = QLabel('Open Upon Creation:')
-        self.open_checkbox = QCheckBox()
-        open_checkbox_layout.addWidget(open_checkbox_label)
-        open_checkbox_layout.addWidget(self.open_checkbox)
-
-        random_checkbox_layout = QHBoxLayout()
-        random_checkbox_label = QLabel('Random Integer Key:')
-        self.random_checkbox = QCheckBox()
-        random_checkbox_layout.addWidget(random_checkbox_label)
-        random_checkbox_layout.addWidget(self.random_checkbox)
-
         checkbox_layout = QVBoxLayout()
-        checkbox_layout.addLayout(open_checkbox_layout)
-        checkbox_layout.addLayout(random_checkbox_layout)
+        self.open_checkbox = QCheckBox('Open Upon Creation')
+        self.random_checkbox = QCheckBox('Random Integer Key')
+        checkbox_layout.addWidget(self.open_checkbox)
+        checkbox_layout.addWidget(self.random_checkbox)
         checkbox_layout.setAlignment(Qt.AlignLeft)
 
         parameters_layout = QHBoxLayout()
         parameters_layout.addLayout(spinbox_layout)
         parameters_layout.addLayout(checkbox_layout)
 
         parameters_group.setLayout(parameters_layout)
@@ -213,22 +205,17 @@
         button_layout.addWidget(self.open_button, alignment=Qt.AlignCenter)
         button_layout.setContentsMargins(25, 25, 25, 25)
 
         self.message = QLabel()
 
         parameters_group = QGroupBox('Mount Options')
 
-        read_only_layout = QHBoxLayout()
-        read_only_label = QLabel('Read Only:')
-        self.read_only_checkbox = QCheckBox()
-        read_only_layout.addWidget(read_only_label)
-        read_only_layout.addWidget(self.read_only_checkbox)
-
         checkbox_layout = QVBoxLayout()
-        checkbox_layout.addLayout(read_only_layout)
+        self.read_only_checkbox = QCheckBox('Read Only')
+        checkbox_layout.addWidget(self.read_only_checkbox)
         checkbox_layout.setAlignment(Qt.AlignLeft)
 
         parameters_layout = QHBoxLayout()
 
         parameters_layout.addLayout(checkbox_layout)
 
         parameters_group.setLayout(parameters_layout)
@@ -371,30 +358,26 @@
 
         size_box_layout = QHBoxLayout()
         size_box_label = QLabel('Size (MB):')
         self.size_box = QSpinBox()
         self.size_box.setMaximum(999999)
         self.size_box.setMinimum(10)
         self.size_box.setFixedWidth(100)
+        size_box_label.setBuddy(self.size_box)
         size_box_layout.addWidget(size_box_label)
         size_box_layout.addWidget(self.size_box)
         size_box_layout.setSpacing(0)
 
         spinbox_layout = QVBoxLayout()
         spinbox_layout.addLayout(size_box_layout)
         spinbox_layout.setAlignment(Qt.AlignLeft)
 
-        open_checkbox_layout = QHBoxLayout()
-        open_checkbox_label = QLabel('Open Upon Resize:')
-        self.open_checkbox = QCheckBox()
-        open_checkbox_layout.addWidget(open_checkbox_label)
-        open_checkbox_layout.addWidget(self.open_checkbox)
-
         checkbox_layout = QVBoxLayout()
-        checkbox_layout.addLayout(open_checkbox_layout)
+        self.open_checkbox = QCheckBox('Open Upon Resize')
+        checkbox_layout.addWidget(self.open_checkbox)
         checkbox_layout.setAlignment(Qt.AlignLeft)
 
         parameters_layout = QHBoxLayout()
         parameters_layout.addLayout(spinbox_layout)
         parameters_layout.addLayout(checkbox_layout)
 
         parameters_group.setLayout(parameters_layout)
@@ -732,7 +715,11 @@
     window = Mausoleum()
     desktop = QDesktopWidget().availableGeometry()
     width = (desktop.width() - window.width()) / 2
     height = (desktop.height() - window.height()) / 2
     window.show()
     window.move(width, height)
     sys.exit(application.exec_())
+
+
+if __name__ == "__main__":
+    main()
```

