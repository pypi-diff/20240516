# Comparing `tmp/gpep517-8.tar.gz` & `tmp/gpep517-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpep517-8.tar", last modified: Wed Jul 20 05:10:40 2022, max compression
+gzip compressed data, was "gpep517-9.tar", last modified: Sun Jul 24 08:31:16 2022, max compression
```

## Comparing `gpep517-8.tar` & `gpep517-9.tar`

### file list

```diff
@@ -1,26 +1,28 @@
--rw-r--r--   0        0        0     1081 2022-05-03 19:57:48.470443 gpep517-8/LICENSE
--rw-r--r--   0        0        0     1249 2022-05-03 19:57:48.470443 gpep517-8/README.rst
--rw-r--r--   0        0        0       87 2022-07-20 05:09:59.364508 gpep517-8/gpep517/__init__.py
--rw-r--r--   0        0        0     7895 2022-07-20 04:33:34.675705 gpep517-8/gpep517/__main__.py
--rw-r--r--   0        0        0     3980 2022-07-20 04:59:04.131720 gpep517-8/gpep517/qa.py
--rw-r--r--   0        0        0      862 2022-05-05 07:51:14.986036 gpep517-8/pyproject.toml
--rw-r--r--   0        0        0        0 2022-05-03 19:57:48.470443 gpep517-8/test/__init__.py
--rw-r--r--   0        0        0     3472 2022-05-06 20:24:31.708825 gpep517-8/test/backend.py
--rw-r--r--   0        0        0      431 2022-05-03 19:57:48.470443 gpep517-8/test/integration/flit_core/pyproject.toml
--rw-r--r--   0        0        0      472 2022-05-03 19:57:48.470443 gpep517-8/test/integration/hatchling/pyproject.toml
--rw-r--r--   0        0        0       46 2022-07-17 09:07:16.944263 gpep517-8/test/integration/pdm.pep517/LICENSE
--rw-r--r--   0        0        0      512 2022-07-17 09:06:55.110457 gpep517-8/test/integration/pdm.pep517/pyproject.toml
--rw-r--r--   0        0        0      418 2022-05-03 19:57:48.470443 gpep517-8/test/integration/poetry.core/pyproject.toml
--rw-r--r--   0        0        0       81 2022-05-03 19:57:48.470443 gpep517-8/test/integration/setuptools/pyproject.toml
--rw-r--r--   0        0        0      494 2022-05-03 19:57:48.470443 gpep517-8/test/integration/setuptools/setup.cfg
--rw-r--r--   0        0        0      156 2022-05-03 19:57:48.470443 gpep517-8/test/sub-path/backend.py
--rw-r--r--   0        0        0     2147 2022-05-03 19:57:48.470443 gpep517-8/test/test-pkg/dist/test-1-py3-none-any.whl
--rw-r--r--   0        0        0       50 2022-05-03 19:57:48.470443 gpep517-8/test/test-pkg/oldscript
--rw-r--r--   0        0        0      463 2022-05-03 19:57:48.470443 gpep517-8/test/test-pkg/setup.py
--rw-r--r--   0        0        0       22 2022-05-03 19:57:48.470443 gpep517-8/test/test-pkg/test.h
--rw-r--r--   0        0        0       94 2022-05-03 19:57:48.470443 gpep517-8/test/test-pkg/testpkg/__init__.py
--rw-r--r--   0        0        0        5 2022-05-03 19:57:48.470443 gpep517-8/test/test-pkg/testpkg/datafile.txt
--rw-r--r--   0        0        0     9881 2022-05-10 07:44:40.607739 gpep517-8/test/test_main.py
--rw-r--r--   0        0        0     9141 2022-07-20 05:03:58.205719 gpep517-8/test/test_verify_pyc.py
--rw-r--r--   0        0        0      430 2022-05-10 07:49:52.614500 gpep517-8/tox.ini
--rw-r--r--   0        0        0     2040 1970-01-01 00:00:00.000000 gpep517-8/PKG-INFO
+-rw-r--r--   0        0        0     1081 2022-05-03 19:57:48.470443 gpep517-9/LICENSE
+-rw-r--r--   0        0        0     2838 2022-07-24 07:14:52.519954 gpep517-9/README.rst
+-rw-r--r--   0        0        0       88 2022-07-24 08:26:26.558319 gpep517-9/gpep517/__init__.py
+-rw-r--r--   0        0        0    11522 2022-07-24 06:54:02.750646 gpep517-9/gpep517/__main__.py
+-rw-r--r--   0        0        0     4114 2022-07-24 06:54:02.750646 gpep517-9/gpep517/qa.py
+-rw-r--r--   0        0        0      862 2022-07-23 05:47:42.407119 gpep517-9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-05-03 19:57:48.470443 gpep517-9/test/__init__.py
+-rw-r--r--   0        0        0     3472 2022-05-06 20:24:31.708825 gpep517-9/test/backend.py
+-rw-r--r--   0        0        0      431 2022-05-03 19:57:48.470443 gpep517-9/test/integration/flit_core/pyproject.toml
+-rw-r--r--   0        0        0      472 2022-05-03 19:57:48.470443 gpep517-9/test/integration/hatchling/pyproject.toml
+-rw-r--r--   0        0        0       46 2022-07-17 09:07:16.944263 gpep517-9/test/integration/pdm.pep517/LICENSE
+-rw-r--r--   0        0        0      512 2022-07-17 09:06:55.110457 gpep517-9/test/integration/pdm.pep517/pyproject.toml
+-rw-r--r--   0        0        0      418 2022-05-03 19:57:48.470443 gpep517-9/test/integration/poetry.core/pyproject.toml
+-rw-r--r--   0        0        0      494 2022-07-22 11:00:26.766865 gpep517-9/test/integration/setuptools-legacy/setup.cfg
+-rw-r--r--   0        0        0       39 2022-07-22 11:00:42.870555 gpep517-9/test/integration/setuptools-legacy/setup.py
+-rw-r--r--   0        0        0       81 2022-05-03 19:57:48.470443 gpep517-9/test/integration/setuptools/pyproject.toml
+-rw-r--r--   0        0        0      494 2022-05-03 19:57:48.470443 gpep517-9/test/integration/setuptools/setup.cfg
+-rw-r--r--   0        0        0      156 2022-05-03 19:57:48.470443 gpep517-9/test/sub-path/backend.py
+-rw-r--r--   0        0        0     2147 2022-05-03 19:57:48.470443 gpep517-9/test/test-pkg/dist/test-1-py3-none-any.whl
+-rw-r--r--   0        0        0       50 2022-05-03 19:57:48.470443 gpep517-9/test/test-pkg/oldscript
+-rw-r--r--   0        0        0      463 2022-05-03 19:57:48.470443 gpep517-9/test/test-pkg/setup.py
+-rw-r--r--   0        0        0       22 2022-05-03 19:57:48.470443 gpep517-9/test/test-pkg/test.h
+-rw-r--r--   0        0        0       94 2022-05-03 19:57:48.470443 gpep517-9/test/test-pkg/testpkg/__init__.py
+-rw-r--r--   0        0        0        5 2022-05-03 19:57:48.470443 gpep517-9/test/test-pkg/testpkg/datafile.txt
+-rw-r--r--   0        0        0    13542 2022-07-23 06:14:02.027079 gpep517-9/test/test_main.py
+-rw-r--r--   0        0        0     9141 2022-07-20 05:03:58.205719 gpep517-9/test/test_verify_pyc.py
+-rw-r--r--   0        0        0      449 2022-07-23 05:46:11.831843 gpep517-9/tox.ini
+-rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 gpep517-9/PKG-INFO
```

### Comparing `gpep517-8/LICENSE` & `gpep517-9/LICENSE`

 * *Files identical despite different names*

### Comparing `gpep517-8/gpep517/__main__.py` & `gpep517-9/gpep517/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,59 @@
 import argparse
 import functools
 import importlib
 import json
+import logging
 import os
 import pathlib
 import sys
 import sysconfig
+import tempfile
 
+from pathlib import Path
 
-def get_toml(path):
+
+ALL_OPT_LEVELS = [0, 1, 2]
+DEFAULT_PREFIX = Path("/usr")
+DEFAULT_FALLBACK_BACKEND = "setuptools.build_meta:__legacy__"
+
+logger = logging.getLogger("gpep517")
+
+
+def get_toml(path: Path):
     if sys.version_info >= (3, 11):
         import tomllib
     else:
         import tomli as tomllib
 
     try:
-        with open(path, "rb") as f:
+        with path.open("rb") as f:
             return tomllib.load(f)
     except FileNotFoundError:
         return {}
 
 
 def get_backend(args):
     with os.fdopen(args.output_fd, "w") as out:
         print(get_toml(args.pyproject_toml)
               .get("build-system", {})
               .get("build-backend", ""),
               file=out)
     return 0
 
 
-def build_wheel(args):
+def build_wheel_impl(args, wheel_dir: Path):
     build_sys = get_toml(args.pyproject_toml).get("build-system", {})
-    backend_s = args.backend or build_sys["build-backend"]
+    backend_s = args.backend
+    if backend_s is None:
+        backend_s = build_sys.get("build-backend", args.fallback_backend)
+        if backend_s is None:
+            raise RuntimeError(
+                "pyproject.toml is missing or does not specify build-backend "
+                "and --no-fallback-backend specified")
     package, _, obj = backend_s.partition(":")
 
     if not args.allow_compressed:
         import zipfile
         orig_open = zipfile.ZipFile.open
         orig_write = zipfile.ZipFile.write
         orig_writestr = zipfile.ZipFile.writestr
@@ -80,145 +97,230 @@
     sys.path[:0] = build_sys.get("backend-path", [])
     backend = importlib.import_module(package)
 
     if obj:
         for name in obj.split("."):
             backend = getattr(backend, name)
 
-    wheel_name = backend.build_wheel(args.wheel_dir, args.config_json)
+    logger.info(f"Building wheel via backend {backend_s}")
+    wheel_name = backend.build_wheel(str(wheel_dir), args.config_json)
+    logger.info(f"The backend produced {wheel_dir / wheel_name}")
 
     for mod in frozenset(sys.modules).difference(orig_modules):
         del sys.modules[mod]
     sys.path = orig_path
 
     if not args.allow_compressed:
         zipfile.ZipFile.open = orig_open
         zipfile.ZipFile.write = orig_write
         zipfile.ZipFile.writestr = orig_writestr
 
+    return wheel_name
+
+
+def build_wheel(args):
     with os.fdopen(args.output_fd, "w") as out:
-        print(wheel_name, file=out)
+        print(build_wheel_impl(args, args.wheel_dir), file=out)
     return 0
 
 
-def install_scheme_dict(prefix, dist_name):
-    ret = sysconfig.get_paths(vars={"base": prefix,
-                                    "platbase": prefix})
+def install_scheme_dict(prefix: Path, dist_name: str):
+    ret = sysconfig.get_paths(vars={"base": str(prefix),
+                                    "platbase": str(prefix)})
     # header path hack copied from installer's __main__.py
     ret["headers"] = os.path.join(
-        sysconfig.get_path("include", vars={"installed_base": prefix}),
+        sysconfig.get_path("include", vars={"installed_base": str(prefix)}),
         dist_name)
     # end of copy-paste
     return ret
 
 
-def install_wheel(args):
+def parse_optimize_arg(val):
+    spl = val.split(",")
+    if "all" in spl:
+        return ALL_OPT_LEVELS
+    return [int(x) for x in spl]
+
+
+def install_wheel_impl(args, wheel: Path):
     from installer import install
     from installer.destinations import SchemeDictionaryDestination
     from installer.sources import WheelFile
     from installer.utils import get_launcher_kind
 
-    with WheelFile.open(args.wheel) as source:
+    with WheelFile.open(wheel) as source:
         dest = SchemeDictionaryDestination(
-            install_scheme_dict(args.prefix or "/usr", source.distribution),
-            args.interpreter,
+            install_scheme_dict(args.prefix, source.distribution),
+            str(args.interpreter),
             get_launcher_kind(),
-            bytecode_optimization_levels=[],
-            destdir=args.destdir,
+            bytecode_optimization_levels=args.optimize,
+            destdir=str(args.destdir),
         )
+        logger.info(f"Installing {wheel} into {args.destdir}")
         install(source, dest, {})
+        logger.info("Installation complete")
+
+
+def install_wheel(args):
+    install_wheel_impl(args, args.wheel)
+
+    return 0
+
+
+def install_from_source(args):
+    with tempfile.TemporaryDirectory() as temp_dir:
+        temp_path = Path(temp_dir)
+        wheel = build_wheel_impl(args, temp_path)
+        install_wheel_impl(args, temp_path / wheel)
 
     return 0
 
 
 def verify_pyc(args):
     from gpep517.qa import qa_verify_pyc
 
-    install_dict = install_scheme_dict(args.prefix or "/usr", "")
-    sitedirs = frozenset(install_dict[x] for x in ("purelib", "platlib"))
+    install_dict = install_scheme_dict(args.prefix, "")
+    sitedirs = frozenset(Path(install_dict[x]) for x in ("purelib", "platlib"))
     result = qa_verify_pyc(args.destdir, sitedirs)
 
     def fpath(p):
-        if p.startswith("/"):
-            return "/" + os.path.relpath(p, args.destdir)
+        if isinstance(p, Path):
+            return str(p.root / p.relative_to(args.destdir))
         return p
 
     for kind, entries in result.items():
         for e in sorted(entries):
             print(f"{kind}:{':'.join(fpath(x) for x in e)}")
     return 1 if any(v for v in result.values()) else 0
 
 
+def add_install_path_args(parser):
+    group = parser.add_argument_group("install paths")
+    group.add_argument("--destdir",
+                       type=Path,
+                       help="Staging directory for the install (it will "
+                       "be prepended to all paths)",
+                       required=True)
+    group.add_argument("--prefix",
+                       type=Path,
+                       default=DEFAULT_PREFIX,
+                       help="Prefix to install to "
+                       f"(default: {DEFAULT_PREFIX})")
+
+
+def add_build_args(parser):
+    group = parser.add_argument_group("backend selection")
+    group.add_argument("--backend",
+                       help="Backend to use (defaults to reading "
+                            "from pyproject.toml)")
+    group.add_argument("--fallback-backend",
+                       default=DEFAULT_FALLBACK_BACKEND,
+                       help="Backend to use if pyproject.toml does not exist "
+                       "or does not specify one "
+                       f"(default: {DEFAULT_FALLBACK_BACKEND!r})")
+    group.add_argument("--no-fallback-backend",
+                       action="store_const",
+                       dest="fallback_backend",
+                       const=None,
+                       help="Disable backend fallback (i.e. require backend "
+                       "declaration in pyproject.toml")
+    group.add_argument("--pyproject-toml",
+                       type=Path,
+                       default="pyproject.toml",
+                       help="Path to pyproject.toml file (used only if "
+                       "--backend is not specified)")
+
+    group = parser.add_argument_group("build options")
+    group.add_argument("--allow-compressed",
+                       help="Allow creating compressed zipfiles (gpep517 "
+                       "will attempt to patch compression out by default)",
+                       action="store_true")
+    group.add_argument("--config-json",
+                       help="JSON-encoded dictionary of config_settings "
+                            "to pass to the build backend",
+                       type=json.loads)
+
+
+def add_install_args(parser):
+    add_install_path_args(parser)
+
+    group = parser.add_argument_group("install options")
+    group.add_argument("--interpreter",
+                       type=Path,
+                       default=sys.executable,
+                       help="The interpreter to put in script shebangs "
+                       f"(default: {sys.executable})")
+    group.add_argument("--optimize",
+                       type=parse_optimize_arg,
+                       default=[],
+                       help="Comma-separated list of optimization levels "
+                       "to compile bytecode for (default: none), pass 'all' "
+                       "to enable all known optimization levels (currently: "
+                       f"{', '.join(str(x) for x in ALL_OPT_LEVELS)})")
+
+
 def main(argv=sys.argv):
     argp = argparse.ArgumentParser(prog=argv[0])
+    argp.add_argument("-q", "--quiet",
+                      action="store_const",
+                      dest="loglevel",
+                      const=logging.WARNING,
+                      default=logging.INFO,
+                      help="Disable verbose progress reporting")
 
     subp = argp.add_subparsers(dest="command",
                                required=True)
 
     parser = subp.add_parser("get-backend",
                              help="Print build-backend from pyproject.toml")
     parser.add_argument("--output-fd",
                         default=1,
                         help="FD to use for output (default: 1)",
                         type=int)
     parser.add_argument("--pyproject-toml",
+                        type=Path,
                         default="pyproject.toml",
                         help="Path to pyproject.toml file")
 
     parser = subp.add_parser("build-wheel",
-                             help="Build wheel using specified backend")
-    parser.add_argument("--backend",
-                        help="Backend to use (defaults to reading "
-                             "from pyproject.toml")
-    parser.add_argument("--config-json",
-                        help="JSON-encoded dictionary of config_settings "
-                             "to pass to the build backend",
-                        type=json.loads)
-    parser.add_argument("--allow-compressed",
-                        help="Allow creating compressed zipfiles (gpep517 "
-                        "will attempt to patch compression out by default)",
-                        action="store_true")
-    parser.add_argument("--output-fd",
-                        help="FD to output the wheel name to",
-                        required=True,
-                        type=int)
-    parser.add_argument("--pyproject-toml",
-                        default="pyproject.toml",
-                        help="Path to pyproject.toml file")
-    parser.add_argument("--wheel-dir",
-                        help="Directory to output the wheel into",
-                        required=True)
+                             help="Build wheel from sources")
+    group = parser.add_argument_group("required arguments")
+    group.add_argument("--output-fd",
+                       help="FD to output the wheel name to",
+                       required=True,
+                       type=int)
+    group.add_argument("--wheel-dir",
+                       type=Path,
+                       help="Directory to write the wheel into",
+                       required=True)
+    add_build_args(parser)
+
+    parser = subp.add_parser("install-from-source",
+                             help="Build and install wheel from sources "
+                             "(without preserving the wheel)")
+    add_build_args(parser)
+    add_install_args(parser)
 
     parser = subp.add_parser("install-wheel",
-                             help="Install wheel")
-    parser.add_argument("--destdir",
-                        help="Directory to install to",
-                        required=True)
-    parser.add_argument("--interpreter",
-                        default=sys.executable,
-                        help="The interpreter to put in script shebangs "
-                        f"(default: {sys.executable})")
-    parser.add_argument("--prefix",
-                        default="/usr",
-                        help="Prefix to install to (default: /usr)")
+                             help="Install the specified wheel")
+    add_install_args(parser)
     parser.add_argument("wheel",
+                        type=Path,
                         help="Wheel to install")
 
     parser = subp.add_parser("verify-pyc",
                              help="Verify that all installed modules were "
                                   "byte-compiled and there are no stray .pyc "
                                   "files")
-    parser.add_argument("--destdir",
-                        help="Offset directory where modules were installed",
-                        required=True)
-    parser.add_argument("--prefix",
-                        default="/usr",
-                        help="Prefix used for install (default: /usr)")
+    add_install_path_args(parser)
 
     args = argp.parse_args(argv[1:])
+    logging.basicConfig(format="{asctime} {name} {levelname} {message}",
+                        style="{",
+                        level=args.loglevel)
 
     func = globals()[args.command.replace("-", "_")]
     return func(args)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `gpep517-8/gpep517/qa.py` & `gpep517-9/gpep517/qa.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import importlib.util
 import os
 import os.path
 import struct
+import typing
+
+from pathlib import Path
 
 
 class PEP552Header:
     def __init__(self, pyc_f):
         # per PEP 552, the header consists of:
         # 4-byte magic (16-bit uint + b"\r\n")
         # 4-byte flags
@@ -39,61 +42,62 @@
             assert len(self.py_hash) == 8
         else:
             # timestamp-based invalidation
             self.py_timestamp, self.py_size = (
                 struct.unpack_from("<LL", self.header, 8))
 
 
-def qa_verify_pyc(destdir, sitedirs):
+def qa_verify_pyc(destdir: Path, sitedirs: typing.Iterable[Path]):
     missing_pyc = []
     invalid_pyc = []
     mismatched_pyc = []
     stray_pyc = []
 
     for sitedir in sitedirs:
-        top_path = destdir + sitedir
-        if not os.path.isdir(top_path):
+        top_path = destdir / sitedir.relative_to(sitedir.root)
+        if not top_path.is_dir():
             continue
 
-        py_files = set()
-        pyc_files = set()
+        py_files: typing.Set[Path] = set()
+        pyc_files: typing.Set[Path] = set()
 
         for path, dirs, files in os.walk(top_path):
             for fn in files:
                 if fn.endswith(".py"):
-                    py_files.add(os.path.join(path, fn))
+                    py_files.add(Path(path) / fn)
                 elif fn.endswith((".pyc", ".pyo")):
-                    pyc_files.add(os.path.join(path, fn))
+                    pyc_files.add(Path(path) / fn)
 
         for py in py_files:
-            py_stat = os.stat(py)
+            py_stat = py.stat()
 
             for opt in ("", 1, 2):
-                pyc = importlib.util.cache_from_source(py, optimization=opt)
+                pyc = Path(
+                    importlib.util.cache_from_source(py, optimization=opt))
                 # 1. check for missing .pyc files
                 if pyc not in pyc_files:
                     missing_pyc.append((pyc, py))
                     continue
 
                 pyc_files.remove(pyc)
                 # 2. check the header
-                with open(pyc, "rb") as f:
+                with pyc.open("rb") as f:
                     try:
                         header = PEP552Header(f)
                     except ValueError:
                         invalid_pyc.append((pyc, py))
                         continue
 
                 # 3. check whether .pyc matches the .py file
                 if header.invalidate_hash:
                     # NB: even though !checked_source implies that Python
                     # does not verify the .pyc validity, we do because
                     # per that mode we're actually responsible for ensuring
                     # that the file is valid
-                    with open(py, "rb") as f:
+                    with py.open("rb") as f:
                         py_hash = importlib.util.source_hash(f.read())
                     if py_hash != header.py_hash:
                         mismatched_pyc.append((pyc, py, "hash"))
                 else:
                     if int(py_stat.st_mtime) != header.py_timestamp:
                         mismatched_pyc.append((pyc, py, "timestamp"))
                     if py_stat.st_size != header.py_size:
```

### Comparing `gpep517-8/pyproject.toml` & `gpep517-9/pyproject.toml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 dependencies = [
     "installer >= 0.5",
     "tomli >= 1.2.3; python_version < '3.11'",
 ]
 
 [project.optional-dependencies]
 test = [
-    "flit_core",
     "pytest",
 ]
 test-full = [
+    "flit_core",
     "hatchling",
     "pdm-pep517",
     "poetry-core",
     "setuptools",
     "wheel",
 ]
```

### Comparing `gpep517-8/test/backend.py` & `gpep517-9/test/backend.py`

 * *Files identical despite different names*

### Comparing `gpep517-8/test/integration/pdm.pep517/pyproject.toml` & `gpep517-9/test/integration/pdm.pep517/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpep517-8/test/test-pkg/dist/test-1-py3-none-any.whl` & `gpep517-9/test/test-pkg/dist/test-1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `gpep517-8/test/test_main.py` & `gpep517-9/test/test_main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import contextlib
+import importlib.machinery
+import importlib.util
 import io
 import os
 import pathlib
 import shutil
 import sys
 import sysconfig
 import zipfile
 
 import pytest
 
 from gpep517 import __version__
-from gpep517.__main__ import main
+from gpep517.__main__ import main, ALL_OPT_LEVELS
 
 
 FLIT_TOML = """
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 """
@@ -103,14 +105,32 @@
     assert 0 == main(["", "build-wheel",
                       "--backend", backend,
                       "--output-fd", "1",
                       "--wheel-dir", "."])
     assert f"{expected}\n" == capfd.readouterr().out
 
 
+def test_build_wheel_fallback(capfd, verify_mod_cleanup):
+    assert 0 == main(["", "build-wheel",
+                      "--fallback-backend", "test.backend",
+                      "--output-fd", "1",
+                      "--pyproject-toml", "enoent.toml",
+                      "--wheel-dir", "."])
+    assert "frobnicate-1-py3-none-any.whl\n" == capfd.readouterr().out
+
+
+def test_build_wheel_no_fallback():
+    with pytest.raises(RuntimeError):
+        main(["", "build-wheel",
+                  "--no-fallback-backend",
+                  "--output-fd", "1",
+                  "--pyproject-toml", "enoent.toml",
+                  "--wheel-dir", "."])
+
+
 @pytest.mark.parametrize(
     ("path", "expected"),
     [("test/sub-path", "frobnicate-4-py3-none-any.whl"),
      ("test", "frobnicate-1-py3-none-any.whl"),
      ])
 def test_build_wheel_backend_path(tmp_path, capfd, path, expected,
                                   verify_mod_cleanup):
@@ -142,86 +162,135 @@
 def all_files(top_path):
     for cur_dir, sub_dirs, sub_files in os.walk(top_path):
         if cur_dir.endswith(".dist-info"):
             yield (str(pathlib.Path(cur_dir).relative_to(top_path)), None)
             continue
         for f in sub_files:
             file_path = pathlib.Path(cur_dir) / f
+            if f.endswith(".pyc"):
+                # for .pyc files, we're interested in whether the correct
+                # source path was embedded inside it
+                loader = importlib.machinery.SourcelessFileLoader(
+                    "testpkg", file_path)
+                data = loader.get_code("testpkg").co_filename
+            else:
+                data = file_path.read_text().splitlines()[0]
             yield (str(file_path.relative_to(top_path)),
-                   (os.access(file_path, os.X_OK),
-                    file_path.read_text().splitlines()[0]))
+                   (os.access(file_path, os.X_OK), data))
 
 
+@pytest.mark.parametrize(["optimize"], [(None,), ("0",), ("1,2",), ("all",)])
 @pytest.mark.parametrize(["prefix"], [("/usr",), ("/eprefix/usr",)])
-def test_install_wheel(tmp_path, prefix):
+def test_install_wheel(tmp_path, optimize, prefix):
     assert 0 == main(["", "install-wheel",
                       "--destdir", str(tmp_path),
                       "--interpreter", "/usr/bin/pythontest",
                       "test/test-pkg/dist/test-1-py3-none-any.whl"] +
-                     (["--prefix", prefix] if prefix != "/usr" else []))
+                     (["--prefix", prefix] if prefix != "/usr" else []) +
+                     (["--optimize", optimize]
+                      if optimize is not None else []))
 
     expected_shebang = "#!/usr/bin/pythontest"
     prefix = prefix.lstrip("/")
     incdir = sysconfig.get_path("include", vars={"installed_base": ""})
     sitedir = sysconfig.get_path("purelib", vars={"base": ""})
 
-    assert {
+    expected = {
         f"{prefix}/bin/newscript": (True, expected_shebang),
         f"{prefix}/bin/oldscript": (True, expected_shebang),
         f"{prefix}{incdir}/test/test.h":
         (False, "#define TEST_HEADER 1"),
         f"{prefix}{sitedir}/test-1.dist-info": None,
         f"{prefix}{sitedir}/testpkg/__init__.py":
         (False, '"""A test package"""'),
         f"{prefix}{sitedir}/testpkg/datafile.txt":
         (False, "data"),
         f"{prefix}/share/test/datafile.txt": (False, "data"),
-    } == dict(all_files(tmp_path))
+    }
 
+    opt_levels = []
+    if optimize == "all":
+        opt_levels = ALL_OPT_LEVELS
+    elif optimize is not None:
+        opt_levels = [int(x) for x in optimize.split(",")]
+    init_mod = f"{prefix}{sitedir}/testpkg/__init__.py"
+    for opt in opt_levels:
+        pyc = importlib.util.cache_from_source(
+            init_mod, optimization=opt if opt != 0 else "")
+        expected[pyc] = (False, "/" + init_mod)
 
-def test_build_self(tmp_path, capfd, verify_mod_cleanup):
+    assert expected == dict(all_files(tmp_path))
+
+
+def test_build_self(tmp_path, capfd):
+    pytest.importorskip("flit_core")
     assert 0 == main(["", "build-wheel",
                       "--allow-compressed",
                       "--output-fd", "1",
                       "--wheel-dir", str(tmp_path)])
     pkg = f"gpep517-{__version__}"
     wheel_name = f"{pkg}-py3-none-any.whl"
     assert f"{wheel_name}\n" == capfd.readouterr().out
 
     with zipfile.ZipFile(tmp_path / wheel_name, "r") as zipf:
-        assert all(x in zipf.namelist() for x in [
-            f"{pkg}.dist-info/METADATA",
-            f"{pkg}.dist-info/entry_points.txt",
-            "gpep517/__init__.py",
-            "gpep517/__main__.py",
-        ])
+        assert all(dict((x, x in zipf.namelist()) for x in
+                        [f"{pkg}.dist-info/METADATA",
+                         f"{pkg}.dist-info/entry_points.txt",
+                         "gpep517/__init__.py",
+                         "gpep517/__main__.py",
+                         ]).values())
+
+
+def test_install_self(tmp_path):
+    pytest.importorskip("flit_core")
+    assert 0 == main(["", "install-from-source",
+                      "--allow-compressed",
+                      "--destdir", str(tmp_path),
+                      "--prefix", "/usr"])
+
+    pkg = f"gpep517-{__version__}"
+    sitedir = tmp_path / (sysconfig.get_path("purelib", vars={"base": "/usr"})
+                          .lstrip(os.path.sep))
+    assert all(dict((x, os.path.exists(x)) for x in
+                    [f"{sitedir}/{pkg}.dist-info/METADATA",
+                     f"{sitedir}/{pkg}.dist-info/entry_points.txt",
+                     f"{sitedir}/gpep517/__init__.py",
+                     f"{sitedir}/gpep517/__main__.py",
+                     ]).values())
 
 
 @contextlib.contextmanager
 def pushd(path):
     orig_dir = pathlib.Path.cwd()
     os.chdir(path)
     try:
         yield
     finally:
         os.chdir(orig_dir)
 
 
-@pytest.mark.parametrize(
-    ["buildsys", "extra_deps"],
-    [("flit_core", []),
-     ("hatchling", []),
-     ("pdm.pep517", []),
-     ("poetry.core", []),
-     ("setuptools", ["wheel"]),
-     ])
-def test_integration(tmp_path, capfd, buildsys, extra_deps,
-                     verify_zipfile_cleanup):
-    pytest.importorskip(buildsys)
-    for dep in extra_deps:
+INTEGRATION_TESTS = [
+    "flit_core",
+    "hatchling",
+    "pdm.pep517",
+    "poetry.core",
+    "setuptools",
+    "setuptools-legacy",
+]
+
+INTEGRATION_TEST_EXTRA_DEPS = {
+    "setuptools": ["wheel"],
+    "setuptools-legacy": ["wheel"],
+}
+
+
+@pytest.mark.parametrize("buildsys", INTEGRATION_TESTS)
+def test_integration(tmp_path, capfd, buildsys, verify_zipfile_cleanup):
+    pytest.importorskip(buildsys.split("-", 1)[0])
+    for dep in INTEGRATION_TEST_EXTRA_DEPS.get(buildsys, []):
         pytest.importorskip(dep)
 
     shutil.copytree(pathlib.Path("test/integration") / buildsys, tmp_path,
                     dirs_exist_ok=True)
 
     with pushd(tmp_path):
         assert 0 == main(["", "build-wheel",
@@ -240,14 +309,38 @@
         assert (b"[console_scripts]\nnewscript=testpkg:entry_point" ==
                 zipf.read(f"{pkg}.dist-info/entry_points.txt")
                 .strip().replace(b" ", b""))
         assert ({zipfile.ZIP_STORED}
                 == {x.compress_type for x in zipf.infolist()})
 
 
+@pytest.mark.parametrize("buildsys", INTEGRATION_TESTS)
+def test_integration_install(tmp_path, buildsys, verify_zipfile_cleanup):
+    pytest.importorskip(buildsys.split("-", 1)[0])
+    for dep in INTEGRATION_TEST_EXTRA_DEPS.get(buildsys, []):
+        pytest.importorskip(dep)
+
+    shutil.copytree(pathlib.Path("test/integration") / buildsys, tmp_path,
+                    dirs_exist_ok=True)
+
+    destdir = tmp_path / "install"
+    with pushd(tmp_path):
+        assert 0 == main(["", "install-from-source",
+                          "--destdir", str(destdir),
+                          "--prefix", "/usr"])
+
+    sitedir = destdir / (sysconfig.get_path("purelib", vars={"base": "/usr"})
+                         .lstrip(os.path.sep))
+    assert all(dict((x, os.path.exists(x)) for x in
+                    [f"{destdir}/usr/bin/newscript",
+                     f"{sitedir}/testpkg/__init__.py",
+                     f"{sitedir}/testpkg/datafile.txt",
+                     ]).values())
+
+
 def test_backend_opening_zipfile_compressed(tmp_path, capfd,
                                             verify_mod_cleanup):
     with open(tmp_path / "pyproject.toml", "w") as f:
         f.write(ZIP_BACKEND_TOML.format(backend="zip_writestr_backend"))
 
     wheel_name = "frobnicate-7-py3-none-any.whl"
     with zipfile.ZipFile(tmp_path / "test.zip", "w") as zipf:
```

### Comparing `gpep517-8/test/test_verify_pyc.py` & `gpep517-9/test/test_verify_pyc.py`

 * *Files identical despite different names*

### Comparing `gpep517-8/PKG-INFO` & `gpep517-9/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,91 @@
-Metadata-Version: 2.1
-Name: gpep517
-Version: 8
-Summary: A backend script to aid installing Python packages in Gentoo.
-Author-email: Michał Górny <mgorny@gentoo.org>
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Classifier: License :: OSI Approved :: MIT License
-Requires-Dist: installer >= 0.5
-Requires-Dist: tomli >= 1.2.3; python_version < '3.11'
-Requires-Dist: flit_core ; extra == "test"
-Requires-Dist: pytest ; extra == "test"
-Requires-Dist: hatchling ; extra == "test-full"
-Requires-Dist: pdm-pep517 ; extra == "test-full"
-Requires-Dist: poetry-core ; extra == "test-full"
-Requires-Dist: setuptools ; extra == "test-full"
-Requires-Dist: wheel ; extra == "test-full"
-Project-URL: Home, https://github.com/mgorny/gpep517/
-Provides-Extra: test
-Provides-Extra: test-full
-
 =======
 gpep517
 =======
 
-gpep517 is a minimal backend script to aid installing Python packages
-through `PEP 517`_-compliant build systems.  Its main purpose is
-to supplement Gentoo eclasses with the necessary Python code.
+gpep517 is a minimal tool to aid building wheels for Python packages
+through `PEP 517`_-compliant build systems and installing them.
+The tool originated from Gentoo with its primary goals being absolutely
+minimal dependency footprint to ease clean bootstrap without bundling
+dependencies, and clean separation of functions to aid external package
+managers.  It is the tool of choice for a world that does not revolve
+around pip and venvs.
 
 
 Commands
 ========
-gpep517 implements three commands:
+gpep517 implements the following commands:
 
-1. ``get-backend`` to read ``build-backend`` from ``pyproject.toml``.
+1. ``get-backend`` to read ``build-backend`` from ``pyproject.toml``
+   (auxiliary command).
 
 2. ``build-wheel`` to call the respeective PEP 517 backend in order
    to produce a wheel.
 
-3. ``install-wheel`` to install the wheel into specified directory.
+3. ``install-wheel`` to install a wheel into the specified directory,
+
+4. ``install-from-source`` that combines building a wheel and installing
+   it (without leaving the artifacts),
+
+5. ``verify-pyc`` to verify that the ``.pyc`` files in the specified
+   install tree are correct and up-to-date.
 
 
 Dependencies
 ============
-gpep517 aims to minimize the dependency footprint to ease boostrap.
+gpep517 aims to minimize the dependency footprint to ease bootstrap.
 At the moment, it depends on two packages:
 
 1. tomli_ for TOML parsing in Python < 3.11
 
 2. installer_ for wheel installation
 
+Additionally, PEP 517 build requires flit_core_.  However, the package
+can be used from the source tree or manually installed without that
+dependency.
 
-Example
-=======
-Example use (without error handling):
+Running the test suite requires pytest_ and flit_core_ (as provided
+by the ``test`` extra).  Additional build systems can be installed
+to extend integration testing (``test-full`` extra).  A tox_ file
+is also provided to ease running tests.
+
+
+Examples
+========
+The simplest way to install a package from the current directory
+is to use the ``install-from-source`` command, e.g.:
+
+.. code-block:: bash
+
+    gpep517 install-from-source --destdir install --optimize all
+
+gpep517 can also be used as a thin wrapper over the installer_ package,
+to install a prebuilt wheel:
+
+.. code-block:: bash
+
+    gpep517 install-wheel --destdir install --optimize all \
+        gpep517-8-py3-none-any.whl
+
+Alternatively, the wheel can be built and installed separately.
+Notably, this leaves the built wheel in the specified directory
+for reuse:
 
 .. code-block:: bash
 
-    backend=$(gpep517 get-backend)
-    mkdir -p build
+    set -e
+    mkdir -p dist
     wheel_name=$(
+        # the output forwarding trick guarantees that the underlying
+        # backend will not output into ${wheel_name}
         gpep517 build-wheel --output-fd 3 --wheel-dir dist \
-            --backend "${backend:-setuptools.build_meta:__legacy__}" \
             3>&1 >&2
     )
     gpep517 install-wheel --destdir install "dist/${wheel_name}"
 
 
 .. _PEP 517: https://peps.python.org/pep-0517/
 .. _tomli: https://pypi.org/project/tomli/
 .. _installer: https://pypi.org/project/installer/
-
+.. _flit_core: https://pypi.org/project/flit_core/
+.. _pytest: https://pypi.org/project/pytest/
+.. _tox: https://pypi.org/project/tox/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

