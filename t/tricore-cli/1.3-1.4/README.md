# Comparing `tmp/tricore-cli-1.3.tar.gz` & `tmp/tricore_cli-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tricore-cli-1.3.tar", last modified: Thu Mar 21 12:05:57 2024, max compression
+gzip compressed data, was "tricore_cli-1.4.tar", last modified: Thu May 16 19:50:42 2024, max compression
```

## Comparing `tricore-cli-1.3.tar` & `tricore_cli-1.4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 francesco   (501) staff       (20)        0 2024-03-21 12:05:57.583800 tricore-cli-1.3/
--rw-r--r--   0 francesco   (501) staff       (20)     1068 2024-03-21 09:45:08.000000 tricore-cli-1.3/LICENSE
--rw-r--r--   0 francesco   (501) staff       (20)     1110 2024-03-21 12:05:57.583609 tricore-cli-1.3/PKG-INFO
--rw-r--r--   0 francesco   (501) staff       (20)      679 2024-03-21 12:05:30.000000 tricore-cli-1.3/README.md
--rw-r--r--   0 francesco   (501) staff       (20)      546 2024-03-21 12:05:46.000000 tricore-cli-1.3/pyproject.toml
--rw-r--r--   0 francesco   (501) staff       (20)       38 2024-03-21 12:05:57.583840 tricore-cli-1.3/setup.cfg
-drwxr-xr-x   0 francesco   (501) staff       (20)        0 2024-03-21 12:05:57.582364 tricore-cli-1.3/src/
-drwxr-xr-x   0 francesco   (501) staff       (20)        0 2024-03-21 12:05:57.583390 tricore-cli-1.3/src/tricore_cli.egg-info/
--rw-r--r--   0 francesco   (501) staff       (20)     1110 2024-03-21 12:05:57.000000 tricore-cli-1.3/src/tricore_cli.egg-info/PKG-INFO
--rw-r--r--   0 francesco   (501) staff       (20)      286 2024-03-21 12:05:57.000000 tricore-cli-1.3/src/tricore_cli.egg-info/SOURCES.txt
--rw-r--r--   0 francesco   (501) staff       (20)        1 2024-03-21 12:05:57.000000 tricore-cli-1.3/src/tricore_cli.egg-info/dependency_links.txt
--rw-r--r--   0 francesco   (501) staff       (20)       47 2024-03-21 12:05:57.000000 tricore-cli-1.3/src/tricore_cli.egg-info/entry_points.txt
--rw-r--r--   0 francesco   (501) staff       (20)       14 2024-03-21 12:05:57.000000 tricore-cli-1.3/src/tricore_cli.egg-info/requires.txt
--rw-r--r--   0 francesco   (501) staff       (20)       11 2024-03-21 12:05:57.000000 tricore-cli-1.3/src/tricore_cli.egg-info/top_level.txt
--rw-r--r--   0 francesco   (501) staff       (20)     2731 2024-03-21 11:43:54.000000 tricore-cli-1.3/src/tricorecli.py
+drwxr-xr-x   0 francesco   (501) staff       (20)        0 2024-05-16 19:50:42.538362 tricore_cli-1.4/
+-rw-r--r--   0 francesco   (501) staff       (20)     1068 2024-03-21 09:45:08.000000 tricore_cli-1.4/LICENSE
+-rw-r--r--   0 francesco   (501) staff       (20)     1110 2024-05-16 19:50:42.538138 tricore_cli-1.4/PKG-INFO
+-rw-r--r--   0 francesco   (501) staff       (20)      679 2024-03-21 12:05:30.000000 tricore_cli-1.4/README.md
+-rw-r--r--   0 francesco   (501) staff       (20)      560 2024-05-16 19:48:22.000000 tricore_cli-1.4/pyproject.toml
+-rw-r--r--   0 francesco   (501) staff       (20)       38 2024-05-16 19:50:42.538526 tricore_cli-1.4/setup.cfg
+drwxr-xr-x   0 francesco   (501) staff       (20)        0 2024-05-16 19:50:42.536552 tricore_cli-1.4/src/
+-rw-r--r--   0 francesco   (501) staff       (20)      178 2024-05-16 13:34:08.000000 tricore_cli-1.4/src/args.py
+-rw-r--r--   0 francesco   (501) staff       (20)     1764 2024-05-16 13:34:08.000000 tricore_cli-1.4/src/containers.py
+drwxr-xr-x   0 francesco   (501) staff       (20)        0 2024-05-16 19:50:42.537734 tricore_cli-1.4/src/tricore_cli.egg-info/
+-rw-r--r--   0 francesco   (501) staff       (20)     1110 2024-05-16 19:50:42.000000 tricore_cli-1.4/src/tricore_cli.egg-info/PKG-INFO
+-rw-r--r--   0 francesco   (501) staff       (20)      329 2024-05-16 19:50:42.000000 tricore_cli-1.4/src/tricore_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 francesco   (501) staff       (20)        1 2024-05-16 19:50:42.000000 tricore_cli-1.4/src/tricore_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 francesco   (501) staff       (20)       47 2024-05-16 19:50:42.000000 tricore_cli-1.4/src/tricore_cli.egg-info/entry_points.txt
+-rw-r--r--   0 francesco   (501) staff       (20)       14 2024-05-16 19:50:42.000000 tricore_cli-1.4/src/tricore_cli.egg-info/requires.txt
+-rw-r--r--   0 francesco   (501) staff       (20)       33 2024-05-16 19:50:42.000000 tricore_cli-1.4/src/tricore_cli.egg-info/top_level.txt
+-rw-r--r--   0 francesco   (501) staff       (20)     2513 2024-05-16 19:45:49.000000 tricore_cli-1.4/src/tricorecli.py
+-rw-r--r--   0 francesco   (501) staff       (20)     1605 2024-05-16 19:44:05.000000 tricore_cli-1.4/src/utils.py
```

### Comparing `tricore-cli-1.3/LICENSE` & `tricore_cli-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tricore-cli-1.3/PKG-INFO` & `tricore_cli-1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tricore-cli
-Version: 1.3
+Version: 1.4
 Summary: A utility script for interacting with containerized TriCore development environment
 Author: Francesco Mecatti
 Project-URL: Homepage, https://github.com/mc-cat-tty/tricore-dev-env
 Project-URL: Issues, https://github.com/mc-cat-tty/tricore-dev-env/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tricore-cli-1.3/README.md` & `tricore_cli-1.4/README.md`

 * *Files identical despite different names*

### Comparing `tricore-cli-1.3/pyproject.toml` & `tricore_cli-1.4/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "tricore-cli"
-version = "1.3"
+version = "1.4"
 authors = [{ name = "Francesco Mecatti" }]
 description = "A utility script for interacting with containerized TriCore development environment"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = ["docker>=7.0.0"]
 
 [project.urls]
 Homepage = "https://github.com/mc-cat-tty/tricore-dev-env"
 Issues = "https://github.com/mc-cat-tty/tricore-dev-env/issues"
 
 [project.scripts]
 tricorecli = "tricorecli:main"
 
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = ["setuptools>=61.0", "rich>=13.7"]
 build-backend = "setuptools.build_meta"
```

### Comparing `tricore-cli-1.3/src/tricore_cli.egg-info/PKG-INFO` & `tricore_cli-1.4/src/tricore_cli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tricore-cli
-Version: 1.3
+Version: 1.4
 Summary: A utility script for interacting with containerized TriCore development environment
 Author: Francesco Mecatti
 Project-URL: Homepage, https://github.com/mc-cat-tty/tricore-dev-env
 Project-URL: Issues, https://github.com/mc-cat-tty/tricore-dev-env/issues
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `tricore-cli-1.3/src/tricorecli.py` & `tricore_cli-1.4/src/tricorecli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,94 @@
-import docker, argparse, os, time
-from docker.errors import DockerException
-from docker import DockerClient
-from docker.types import Mount
-from operator import attrgetter
-from itertools import chain
-from typing import Any, Callable
-
-IMAGE: str = 'francescomecatti/tricore-dev-env:1.0'
-
-def container_startup(f) -> Callable:
-  def inner(*args, **kwargs):
-    try:
-      client = docker.from_env()
-    except DockerException:
-      print('Docker engine not found. Make sure to have a running Docker engine!')
-      exit(1)
-
-    installed_images = chain.from_iterable(
-      map(
-        attrgetter('tags'),
-        client.images.list()
-      )
-    )
-
-    if IMAGE not in installed_images:
-      print(f'Downloading container {IMAGE}...')
-      client.images.pull(IMAGE)
-      print('Done!')
-    
-    f(client, *args, **kwargs)
-  
-  return inner
+import argparse, os
+from args import *
+from containers import *
+from utils import *
+
 
+def build(args: BuildHanderArgs) -> None:
+  GlobalConfiguration().verbosity_level = args.verbosity_level
 
-@container_startup
-def build(client: DockerClient, args: Any) -> None:
-  abs_path = os.path.join(os.getcwd(), args.folder)
-  if not os.path.isfile(os.path.join(abs_path, "CMakeLists.txt")):
-    raise FileNotFoundError("Missing CMake file.")
+  abs_path = os.path.abspath(args.folder)
+  
+  check_file_or_exit(
+    os.path.join(abs_path, 'CMakeLists.txt'),
+    f'Missing CMakeLists.txt in {abs_path}',
+    ExitCode.CMAKE_LISTS_NOT_FOUND
+  )
 
-  build_path = os.path.join(abs_path, "build")
+  check_file_or_exit(
+    os.path.join(abs_path, 'tricore_toolchain.cmake'),
+    f'Missing tricore_toolchain.cmake in {abs_path}',
+    ExitCode.CMAKE_TOOLCHAIN_NOT_FOUND
+  )
+  
+  build_path = os.path.join(abs_path, 'build')
   if not os.path.isdir(build_path):
     os.makedirs(build_path)
 
-  src_folder = Mount("/home/src", abs_path, type='bind')
+  CPUS: int = int(os.cpu_count()*1.5) if os.cpu_count() else 2
 
-  print(f"Building source from {args.folder} ...")
-  out = client.containers.run(
-    IMAGE,
-    remove=True,
-    mounts=[src_folder],
-    entrypoint = '/bin/bash -c',
-    command='"cd /home/src/build && cmake --toolchain tricore_toolchain.cmake .. && make -j$(nproc)"'
-  )
-  print(out)
-  print("Done!")
-
-
-@container_startup
-def flash(client: DockerClient, args: Any) -> None:
-  raise NotImplementedError("Feature not implemented yet")
+  with BuildDisposableContainer(abs_path) as build_container:
+    print(f'Building source with {CPUS} jobs from {abs_path}')
+
+    res = build_container.exec_run('cmake -B build --toolchain tricore_toolchain.cmake', stream=True)
+    print_stream(res)
+    
+    res = build_container.exec_run(f'cmake --build build --parallel {CPUS}', stream=True)
+    print_stream(res)
+  
+  print(f"Successfully built artifacts in {build_path}")
+    
+
+def flash(args: FlashHandlerArgs) -> None:
+  raise NotImplementedError('Feature not implemented yet')
 
 
 def main() -> None:
-  parser = argparse.ArgumentParser(description='Utility script for managing the build of TriCore applications with ease.')
+  parser = argparse.ArgumentParser(
+    description='Utility script for managing the build of TriCore applications with ease.'
+  )
   subparsers = parser.add_subparsers(title='action', required=True)
 
-  build_subparser = subparsers.add_parser('build', help='Build a project for TriCore architecture. A CMake file is required.')
-  build_subparser.add_argument('folder', metavar='SRCDIR', type=str)
-  build_subparser.add_argument('-v', '--verbose', help='Enable container log on the terminal.', action='count', default=0, required=False)
+  build_subparser = subparsers.add_parser(
+    'build',
+    help='Build projectes for TriCore architecture. A CMake file is required inside SRCDIR directory.'
+  )
+  build_subparser.add_argument(
+    'folder',
+    metavar='SRCDIR',
+    type=str
+  )
+  build_subparser.add_argument(
+    '-v', '--verbose',
+    dest='verbosity_level',
+    help='Enable container log on the terminal.',
+    action='count',
+    default=0,
+    required=False
+  )
   build_subparser.set_defaults(handler=build)
 
-  flash_subparser = subparsers.add_parser('flash', help='Flash a .hex binary file to a board.')
-  flash_subparser.add_argument('filename', metavar='FILENAME', type=str)
-  flash_subparser.add_argument('-v', '--verbose', help='Enable container log on the terminal.', action='count', default=0, required=False)
+  flash_subparser = subparsers.add_parser(
+    'flash',
+    help='Flash Intel-hex binaries on Aurix boards.'
+  )
+  flash_subparser.add_argument(
+    'filename',
+    metavar='FILENAME',
+    type=str
+  )
+  flash_subparser.add_argument(
+    '-v', '--verbose',
+    dest='verbosity_level',
+    help='Enable container log on the terminal.',
+    action='count',
+    default=0,
+    required=False
+  )
   flash_subparser.set_defaults(handler=flash)
 
   args = parser.parse_args()
   args.handler(args)
 
 if __name__ == '__main__':
   main()
```

