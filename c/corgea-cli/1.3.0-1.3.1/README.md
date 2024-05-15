# Comparing `tmp/corgea_cli-1.3.0.tar.gz` & `tmp/corgea_cli-1.3.1.tar.gz`

## Comparing `corgea_cli-1.3.0.tar` & `corgea_cli-1.3.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 corgea_cli-1.3.0/Cargo.toml
--rw-r--r--   0     1001      127     3285 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/.github/workflows/release.yml
--rw-r--r--   0     1001      127       39 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/.gitignore
--rw-r--r--   0     1001      127    37633 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/Cargo.lock
--rw-r--r--   0     1001      127    26530 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/LICENSE
--rw-r--r--   0     1001      127      490 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/README.md
--rwxr-xr-x   0     1001      127      844 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/build_release.sh
--rw-r--r--   0     1001      127      698 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/src/cicd.rs
--rw-r--r--   0     1001      127     2102 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/src/config.rs
--rw-r--r--   0     1001      127      627 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/src/login.rs
--rw-r--r--   0     1001      127     3213 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/src/main.rs
--rw-r--r--   0     1001      127    12146 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/src/scan.rs
--rw-r--r--   0     1001      127     1109 2024-04-29 01:14:02.000000 corgea_cli-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1612 1970-01-01 00:00:00.000000 corgea_cli-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 corgea_cli-1.3.1/Cargo.toml
+-rw-r--r--   0     1001      127     3285 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/.github/workflows/release.yml
+-rw-r--r--   0     1001      127       39 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/.gitignore
+-rw-r--r--   0     1001      127    37633 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/Cargo.lock
+-rw-r--r--   0     1001      127    26530 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/LICENSE
+-rw-r--r--   0     1001      127      780 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/README.md
+-rwxr-xr-x   0     1001      127      844 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/build_release.sh
+-rw-r--r--   0     1001      127      698 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/src/cicd.rs
+-rw-r--r--   0     1001      127     2102 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/src/config.rs
+-rw-r--r--   0     1001      127      123 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/src/log.rs
+-rw-r--r--   0     1001      127      687 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/src/login.rs
+-rw-r--r--   0     1001      127     3222 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/src/main.rs
+-rw-r--r--   0     1001      127    14889 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/src/scan.rs
+-rw-r--r--   0     1001      127     1109 2024-05-15 22:36:03.000000 corgea_cli-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1902 1970-01-01 00:00:00.000000 corgea_cli-1.3.1/PKG-INFO
```

### Comparing `corgea_cli-1.3.0/Cargo.toml` & `corgea_cli-1.3.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "corgea"
-version = "1.3.0"
+version = "1.3.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
 clap = {  version = "4.4.13", features = ["derive"] }
 dirs = "5.0.1"
```

### Comparing `corgea_cli-1.3.0/.github/workflows/release.yml` & `corgea_cli-1.3.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.3.0/Cargo.lock` & `corgea_cli-1.3.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "corgea"
-version = "1.3.0"
+version = "1.3.1"
 dependencies = [
  "clap",
  "dirs",
  "reqwest",
  "serde",
  "serde_derive",
  "serde_json",
```

### Comparing `corgea_cli-1.3.0/LICENSE` & `corgea_cli-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.3.0/build_release.sh` & `corgea_cli-1.3.1/build_release.sh`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.3.0/src/cicd.rs` & `corgea_cli-1.3.1/src/cicd.rs`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.3.0/src/config.rs` & `corgea_cli-1.3.1/src/config.rs`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.3.0/src/main.rs` & `corgea_cli-1.3.1/src/main.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 mod login;
 mod config;
 mod scan;
 mod cicd;
+mod log;
 
 use std::str::FromStr;
 use clap::{Parser, Subcommand};
 use config::Config;
 
 #[derive(Parser)]
 #[command(author, version, about, long_about = None, arg_required_else_help = true)]
```

### Comparing `corgea_cli-1.3.0/pyproject.toml` & `corgea_cli-1.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `corgea_cli-1.3.0/PKG-INFO` & `corgea_cli-1.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: corgea-cli
-Version: 1.3.0
+Version: 1.3.1
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -32,7 +32,23 @@
 
 [Watch video](https://www.loom.com/share/0d3ed94d1f01401a86906fc9713ee709?sid=b11c1f5a-66ff-4dbf-a83a-c9bea15a5d7b)
 
 [![](https://cdn.loom.com/sessions/thumbnails/0d3ed94d1f01401a86906fc9713ee709-with-play.gif)](https://www.loom.com/share/0d3ed94d1f01401a86906fc9713ee709?sid=b11c1f5a-66ff-4dbf-a83a-c9bea15a5d7b)
 
 </Card>
 
+## Installation
+
+### Using pip
+```
+pip install corgea-cli
+```
+
+### Manual Installation
+You can get the latest binaries for your OS from https://github.com/Corgea/cli/releases.
+
+### Setup
+Once the binary is installed, login with your token from the Corgea app.
+```
+corgea login <token>
+```
+
```

