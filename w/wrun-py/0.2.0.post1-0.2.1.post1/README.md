# Comparing `tmp/wrun_py-0.2.0.post1.tar.gz` & `tmp/wrun_py-0.2.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wrun_py-0.2.0.post1.tar", last modified: Sat Nov 18 21:14:45 2023, max compression
+gzip compressed data, was "wrun_py-0.2.1.post1.tar", last modified: Wed May 15 22:10:55 2024, max compression
```

## Comparing `wrun_py-0.2.0.post1.tar` & `wrun_py-0.2.1.post1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 21:14:45.368385 wrun_py-0.2.0.post1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-18 21:14:38.000000 wrun_py-0.2.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2023-11-18 21:14:45.368385 wrun_py-0.2.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2023-11-18 21:14:38.000000 wrun_py-0.2.0.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2023-11-18 21:14:45.368385 wrun_py-0.2.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2023-11-18 21:14:38.000000 wrun_py-0.2.0.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-18 21:14:45.368385 wrun_py-0.2.0.post1/wrun_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2023-11-18 21:14:45.000000 wrun_py-0.2.0.post1/wrun_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-11-18 21:14:45.000000 wrun_py-0.2.0.post1/wrun_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-18 21:14:45.000000 wrun_py-0.2.0.post1/wrun_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-18 21:14:45.000000 wrun_py-0.2.0.post1/wrun_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:10:55.087111 wrun_py-0.2.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 22:10:45.000000 wrun_py-0.2.1.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-15 22:10:55.087111 wrun_py-0.2.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-15 22:10:45.000000 wrun_py-0.2.1.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-15 22:10:55.087111 wrun_py-0.2.1.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-15 22:10:45.000000 wrun_py-0.2.1.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 22:10:55.087111 wrun_py-0.2.1.post1/wrun_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4535 2024-05-15 22:10:55.000000 wrun_py-0.2.1.post1/wrun_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-15 22:10:55.000000 wrun_py-0.2.1.post1/wrun_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 22:10:55.000000 wrun_py-0.2.1.post1/wrun_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 22:10:55.000000 wrun_py-0.2.1.post1/wrun_py.egg-info/top_level.txt
```

### Comparing `wrun_py-0.2.0.post1/LICENSE` & `wrun_py-0.2.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `wrun_py-0.2.0.post1/PKG-INFO` & `wrun_py-0.2.1.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: wrun_py
-Version: 0.2.0.post1
+Version: 0.2.1.post1
 Summary: Web executable launcher
 Home-page: https://github.com/scop/wrun
 Author: Ville Skyttä
 Author-email: ville.skytta@iki.fi
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Go
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wrun
@@ -50,15 +51,15 @@
 
 URL fragments, if present, are treated as hashAlgo-hexDigest strings, and downloads are checked against them.
 
 The first non-flag argument or -- terminates wrun arguments.
 Remaining ones are passed to the downloaded one.
 
 Environment variables:
-- WRUN_CACHE_HOME: cache location, defaults to wrun subdir in the user cache dir
+- WRUN_CACHE_HOME: cache location, defaults to wrun subdir in the user's cache dir
 - WRUN_OS_ARCH: override OS/arch for matching
 - WRUN_VERBOSE: output verbosity, false decreases, true increases
 ```
 
 ## Installation
 
 Prebuilt binaries are available in
@@ -100,22 +101,25 @@
 To verify downloads against known good digests, place a digest in the URL
 fragment.
 The fragment format to use is `digestAlgo-hexDigest`.
 
 For example:
 
 - `#sha256-2cf24dba5fb0a30e26e83b2ac5b9e29e1b161e5c1fa7425e73043362938b9842`
-- `#sha512-9b71d224bd62f3785d96d46ad3ea3d73319bfbc2890caadae2dff72519673ca72323c3d99ba5c11d7c7acc6e14b8c5da0c4663475c2e5c3adef46f73bcdec043`
-- `#md5-5d41402abc4b2a76b9719d911017c592`)
 
-## CI usage
+## Usage with pre-commit
 
-Cache resides by default in the
-[`$XDG_CACHE_HOME`](https://github.com/adrg/xdg#xdg-base-directory)`/wrun`
-directory. `$WRUN_CACHE_HOME` overrides it.
+See `.pre-commit-config.yaml` examples in
+[`.pre-commit-hooks.yaml`](.pre-commit-hooks.yaml).
+
+## Usage in CI
+
+Cache resides by default in the `wrun` subdirectory of
+the [user's cache directory](https://pkg.go.dev/os#UserCacheDir).
+`$WRUN_CACHE_HOME` overrides it.
 
 If the `-use-pre-commit-cache` flag is given, a subdirectory in
 [pre-commit's cache dir](https://pre-commit.com/#managing-ci-caches) is used instead.
 
 [pre-commit.ci](https://pre-commit.ci) is not supported, because it
 [disallows network access at runtime](https://github.com/pre-commit-ci/issues/issues/196#issuecomment-1810937079).
```

### Comparing `wrun_py-0.2.0.post1/README.md` & `wrun_py-0.2.1.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 URL fragments, if present, are treated as hashAlgo-hexDigest strings, and downloads are checked against them.
 
 The first non-flag argument or -- terminates wrun arguments.
 Remaining ones are passed to the downloaded one.
 
 Environment variables:
-- WRUN_CACHE_HOME: cache location, defaults to wrun subdir in the user cache dir
+- WRUN_CACHE_HOME: cache location, defaults to wrun subdir in the user's cache dir
 - WRUN_OS_ARCH: override OS/arch for matching
 - WRUN_VERBOSE: output verbosity, false decreases, true increases
 ```
 
 ## Installation
 
 Prebuilt binaries are available in
@@ -80,22 +80,25 @@
 To verify downloads against known good digests, place a digest in the URL
 fragment.
 The fragment format to use is `digestAlgo-hexDigest`.
 
 For example:
 
 - `#sha256-2cf24dba5fb0a30e26e83b2ac5b9e29e1b161e5c1fa7425e73043362938b9842`
-- `#sha512-9b71d224bd62f3785d96d46ad3ea3d73319bfbc2890caadae2dff72519673ca72323c3d99ba5c11d7c7acc6e14b8c5da0c4663475c2e5c3adef46f73bcdec043`
-- `#md5-5d41402abc4b2a76b9719d911017c592`)
 
-## CI usage
+## Usage with pre-commit
 
-Cache resides by default in the
-[`$XDG_CACHE_HOME`](https://github.com/adrg/xdg#xdg-base-directory)`/wrun`
-directory. `$WRUN_CACHE_HOME` overrides it.
+See `.pre-commit-config.yaml` examples in
+[`.pre-commit-hooks.yaml`](.pre-commit-hooks.yaml).
+
+## Usage in CI
+
+Cache resides by default in the `wrun` subdirectory of
+the [user's cache directory](https://pkg.go.dev/os#UserCacheDir).
+`$WRUN_CACHE_HOME` overrides it.
 
 If the `-use-pre-commit-cache` flag is given, a subdirectory in
 [pre-commit's cache dir](https://pre-commit.com/#managing-ci-caches) is used instead.
 
 [pre-commit.ci](https://pre-commit.ci) is not supported, because it
 [disallows network access at runtime](https://github.com/pre-commit-ci/issues/issues/196#issuecomment-1810937079).
```

### Comparing `wrun_py-0.2.0.post1/setup.cfg` & `wrun_py-0.2.1.post1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wrun_py
-version = 0.2.0-1
+version = 0.2.1-1
 description = Web executable launcher
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/scop/wrun
 author = Ville Skyttä
 author_email = ville.skytta@iki.fi
 license = Apache License 2.0
@@ -12,67 +12,68 @@
 classifiers = 
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: Apache Software License
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
 	Operating System :: POSIX :: Linux
+	Programming Language :: Go
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Utilities
 
 [options]
 packages = 
 python_requires = >=3.8
 setup_requires = 
 	setuptools-download
 
 [setuptools_download]
 download_scripts = 
 	[wrun]
 	group = wrun-binary
 	marker = sys_platform == "darwin" and platform_machine == "x86_64"
-	url = https://github.com/scop/wrun/releases/download/v0.2.0/wrun_0.2.0_darwin_amd64
-	sha256 = 81024935283d76ed47694cc792009a7c4e3e9f77b2eaf0f6ace1f4716fbb313c
+	url = https://github.com/scop/wrun/releases/download/v0.2.1/wrun_0.2.1_darwin_amd64
+	sha256 = a0f38144ea8696837393e790a96807140e0392e5a2bfef71532f4726602082e9
 	[wrun]
 	group = wrun-binary
 	marker = sys_platform == "darwin" and platform_machine == "arm64"
-	url = https://github.com/scop/wrun/releases/download/v0.2.0/wrun_0.2.0_darwin_arm64
-	sha256 = d19dba337876b24643344eccc9760e05df196e8eba79912b65ec5f47450efd09
+	url = https://github.com/scop/wrun/releases/download/v0.2.1/wrun_0.2.1_darwin_arm64
+	sha256 = fc628331d9a382ca00c7474434688bbb5250e90c4750ffb8b66d32bae71a19e1
 	[wrun]
 	group = wrun-binary
 	marker = sys_platform == "linux" and platform_machine == "i386"
 	marker = sys_platform == "linux" and platform_machine == "i686"
-	url = https://github.com/scop/wrun/releases/download/v0.2.0/wrun_0.2.0_linux_386
-	sha256 = 8fdd51b3fec1d1b2f1392a07ba1288c48f24921deb7a63650786b6b972bc9255
+	url = https://github.com/scop/wrun/releases/download/v0.2.1/wrun_0.2.1_linux_386
+	sha256 = 70e592d87348afae322aedc18e36e121de55f352f163ef44b62037d4c6f8e72a
 	[wrun]
 	group = wrun-binary
 	marker = sys_platform == "linux" and platform_machine == "x86_64"
-	url = https://github.com/scop/wrun/releases/download/v0.2.0/wrun_0.2.0_linux_amd64
-	sha256 = adca47b79ff70f49eca71bef6a134348c53b96183dd79a499e5b946825e22f93
+	url = https://github.com/scop/wrun/releases/download/v0.2.1/wrun_0.2.1_linux_amd64
+	sha256 = 8fa6a96ebfd3ae46769c29b3b5b194fcdca98ae6349e54a466f190484355e582
 	[wrun]
 	group = wrun-binary
 	marker = sys_platform == "linux" and platform_machine == "aarch64"
-	url = https://github.com/scop/wrun/releases/download/v0.2.0/wrun_0.2.0_linux_arm64
-	sha256 = d95c627f10fc0e3175b2606622631e4b1f65d7a425e5126cfe1c9f95035754e5
+	url = https://github.com/scop/wrun/releases/download/v0.2.1/wrun_0.2.1_linux_arm64
+	sha256 = ac5baa72d5cfc488aaddde840a35f37ce308b724d5acc96782a557260569fcbb
 	[wrun]
 	group = wrun-binary
 	marker = sys_platform == "linux" and platform_machine == "armv6hf"
 	marker = sys_platform == "linux" and platform_machine == "armv7l"
-	url = https://github.com/scop/wrun/releases/download/v0.2.0/wrun_0.2.0_linux_armv6
-	sha256 = b50b4dafc235b268c10381d1fbe4512028396d0a98c3de7a691064617454b6a6
+	url = https://github.com/scop/wrun/releases/download/v0.2.1/wrun_0.2.1_linux_armv6
+	sha256 = d6f70092736fcf25e3bb5634a822be479a12eeffbb1a2092c22ce14fed7336dc
 	[wrun.exe]
 	group = wrun-binary
 	marker = sys_platform == "win32" and platform_machine == "x86"
 	marker = sys_platform == "cygwin" and platform_machine == "i386"
-	url = https://github.com/scop/wrun/releases/download/v0.2.0/wrun_0.2.0_windows_386.exe
-	sha256 = 480d3012a005b285eb5350db183637049ef5cda698ad36b4cb2eaa7efbc2ea36
+	url = https://github.com/scop/wrun/releases/download/v0.2.1/wrun_0.2.1_windows_386.exe
+	sha256 = 5109ad7157598b00ba86d609ac3bf7cc009575d12ef07fa9b9947fed4ece8bbc
 	[wrun.exe]
 	group = wrun-binary
 	marker = sys_platform == "win32" and platform_machine == "AMD64"
 	marker = sys_platform == "cygwin" and platform_machine == "x86_64"
-	url = https://github.com/scop/wrun/releases/download/v0.2.0/wrun_0.2.0_windows_amd64.exe
-	sha256 = cffcbcf3e297380022b65a499eff0b3838d9be509babdb939324befae00b8240
+	url = https://github.com/scop/wrun/releases/download/v0.2.1/wrun_0.2.1_windows_amd64.exe
+	sha256 = d960ddd763c978790b5fdb1bd9c95de70e5b02df7fcd242b737f2d08eda8eafe
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `wrun_py-0.2.0.post1/setup.py` & `wrun_py-0.2.1.post1/setup.py`

 * *Files identical despite different names*

### Comparing `wrun_py-0.2.0.post1/wrun_py.egg-info/PKG-INFO` & `wrun_py-0.2.1.post1/wrun_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
-Name: wrun-py
-Version: 0.2.0.post1
+Name: wrun_py
+Version: 0.2.1.post1
 Summary: Web executable launcher
 Home-page: https://github.com/scop/wrun
 Author: Ville Skyttä
 Author-email: ville.skytta@iki.fi
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Go
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # wrun
@@ -50,15 +51,15 @@
 
 URL fragments, if present, are treated as hashAlgo-hexDigest strings, and downloads are checked against them.
 
 The first non-flag argument or -- terminates wrun arguments.
 Remaining ones are passed to the downloaded one.
 
 Environment variables:
-- WRUN_CACHE_HOME: cache location, defaults to wrun subdir in the user cache dir
+- WRUN_CACHE_HOME: cache location, defaults to wrun subdir in the user's cache dir
 - WRUN_OS_ARCH: override OS/arch for matching
 - WRUN_VERBOSE: output verbosity, false decreases, true increases
 ```
 
 ## Installation
 
 Prebuilt binaries are available in
@@ -100,22 +101,25 @@
 To verify downloads against known good digests, place a digest in the URL
 fragment.
 The fragment format to use is `digestAlgo-hexDigest`.
 
 For example:
 
 - `#sha256-2cf24dba5fb0a30e26e83b2ac5b9e29e1b161e5c1fa7425e73043362938b9842`
-- `#sha512-9b71d224bd62f3785d96d46ad3ea3d73319bfbc2890caadae2dff72519673ca72323c3d99ba5c11d7c7acc6e14b8c5da0c4663475c2e5c3adef46f73bcdec043`
-- `#md5-5d41402abc4b2a76b9719d911017c592`)
 
-## CI usage
+## Usage with pre-commit
 
-Cache resides by default in the
-[`$XDG_CACHE_HOME`](https://github.com/adrg/xdg#xdg-base-directory)`/wrun`
-directory. `$WRUN_CACHE_HOME` overrides it.
+See `.pre-commit-config.yaml` examples in
+[`.pre-commit-hooks.yaml`](.pre-commit-hooks.yaml).
+
+## Usage in CI
+
+Cache resides by default in the `wrun` subdirectory of
+the [user's cache directory](https://pkg.go.dev/os#UserCacheDir).
+`$WRUN_CACHE_HOME` overrides it.
 
 If the `-use-pre-commit-cache` flag is given, a subdirectory in
 [pre-commit's cache dir](https://pre-commit.com/#managing-ci-caches) is used instead.
 
 [pre-commit.ci](https://pre-commit.ci) is not supported, because it
 [disallows network access at runtime](https://github.com/pre-commit-ci/issues/issues/196#issuecomment-1810937079).
```

