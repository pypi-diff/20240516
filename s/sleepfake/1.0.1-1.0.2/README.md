# Comparing `tmp/sleepfake-1.0.1.tar.gz` & `tmp/sleepfake-1.0.2.tar.gz`

## Comparing `sleepfake-1.0.1.tar` & `sleepfake-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 sleepfake-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sleepfake-1.0.1/.python-version
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 sleepfake-1.0.1/requirements-dev.lock
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 sleepfake-1.0.1/requirements.lock
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 sleepfake-1.0.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sleepfake-1.0.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 sleepfake-1.0.1/src/sleepfake/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sleepfake-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 sleepfake-1.0.1/tests/test_async.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 sleepfake-1.0.1/tests/test_sync.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 sleepfake-1.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sleepfake-1.0.1/LICENSE
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 sleepfake-1.0.1/README.md
--rw-r--r--   0        0        0     3528 2020-02-02 00:00:00.000000 sleepfake-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     3199 2020-02-02 00:00:00.000000 sleepfake-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 sleepfake-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 sleepfake-1.0.2/.python-version
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 sleepfake-1.0.2/requirements-dev.lock
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 sleepfake-1.0.2/requirements.lock
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 sleepfake-1.0.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 sleepfake-1.0.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 sleepfake-1.0.2/src/sleepfake/__init__.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 sleepfake-1.0.2/src/sleepfake/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sleepfake-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 sleepfake-1.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 sleepfake-1.0.2/tests/test_async.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 sleepfake-1.0.2/tests/test_pytest_plugin.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 sleepfake-1.0.2/tests/test_sync.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 sleepfake-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 sleepfake-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 sleepfake-1.0.2/README.md
+-rw-r--r--   0        0        0     3591 2020-02-02 00:00:00.000000 sleepfake-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 sleepfake-1.0.2/PKG-INFO
```

### Comparing `sleepfake-1.0.1/.pre-commit-config.yaml` & `sleepfake-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sleepfake-1.0.1/requirements-dev.lock` & `sleepfake-1.0.2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `sleepfake-1.0.1/requirements.lock` & `sleepfake-1.0.2/requirements.lock`

 * *Files identical despite different names*

### Comparing `sleepfake-1.0.1/.github/workflows/release.yml` & `sleepfake-1.0.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `sleepfake-1.0.1/.github/workflows/test.yml` & `sleepfake-1.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `sleepfake-1.0.1/src/sleepfake/__init__.py` & `sleepfake-1.0.2/src/sleepfake/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,66 +7,98 @@
 import freezegun
 import pytz
 
 if TYPE_CHECKING:
     from unittest.mock import _patch_default_new
 
 
+class _NotInitializedError(Exception):
+    def __init__(self) -> None:
+        self.message = "sleep_queue is not initialized | should not happen"
+        super().__init__(self.message)
+
+    def __str__(self) -> str:
+        return self.message
+
+
 class SleepFake:
     """Fake the time.sleep/asyncio.sleep function during tests."""
 
     def __init__(self) -> None:
         self.sleep = time.sleep
         self.asleep = asyncio.sleep
         self.freeze_time = freezegun.freeze_time(datetime.datetime.now(tz=pytz.UTC))
         self.frozen_factory = self.freeze_time.start()
         self.time_patch: _patch_default_new
         self.asyncio_patch: _patch_default_new
+
         self.time_patch = patch("time.sleep", side_effect=self.mock_sleep)
         self.asyncio_patch = patch("asyncio.sleep", side_effect=self.amock_sleep)
-        self.sleep_queue: "asyncio.Queue[tuple[datetime.datetime, asyncio.Future[None]]]" = (
-            asyncio.Queue()
+        self.sleep_queue: "asyncio.Queue[tuple[datetime.datetime, asyncio.Future[None]]] | None" = (
+            None
         )
+        self.sleep_processor: "asyncio.Task[None] | None" = None
+
+    async def _init_async_patch(self) -> None:
+        if not self.sleep_processor and asyncio.get_event_loop().is_running():
+            self.sleep_processor = asyncio.create_task(self.process_sleeps())
+            self.sleep_queue = asyncio.Queue()
 
     def __enter__(self) -> "SleepFake":
         """Replace the time.sleep/asyncio.sleep function with the mock function when entering the context."""
         self.time_patch.start()
         self.asyncio_patch.start()
+        self.sleep_processor = None
 
-        if asyncio.get_event_loop().is_running():
-            self.sleep_processor = asyncio.create_task(self.process_sleeps())
         return self
 
     async def __aenter__(self) -> "SleepFake":
         return self.__enter__()
 
     async def __aexit__(self, exc_type: object, exc_val: object, exc_tb: object) -> None:
         self.__exit__(exc_type, exc_val, exc_tb)
 
     def __exit__(self, exc_type: object, exc_val: object, exc_tb: object) -> None:
         """Restore the original time.sleep/asyncio.sleep function when exiting the context."""
         self.time_patch.stop()
         self.asyncio_patch.stop()
         self.freeze_time.stop()
-        if asyncio.get_event_loop().is_running():
+        if (
+            self.sleep_processor
+            and asyncio.get_event_loop().is_running()
+            and not self.sleep_processor.done()
+        ):
             self.sleep_processor.cancel()
 
     def mock_sleep(self, seconds: float) -> None:
         """A mock sleep function that advances the frozen time instead of actually sleeping."""
         self.frozen_factory.move_to(datetime.timedelta(seconds=seconds))
 
     async def amock_sleep(self, seconds: float) -> None:
         """A mock sleep function that advances the frozen time instead of actually sleeping."""
+        # lazy initialize the sleep queue and processor (useful for async tests fixture)
+        if self.sleep_processor is None:
+            await self._init_async_patch()
+
+        if self.sleep_queue is None:
+            raise _NotInitializedError
+
         future: asyncio.Future[None] = asyncio.Future()
         await self.sleep_queue.put(
             (datetime.datetime.now() + datetime.timedelta(seconds=seconds), future)  # noqa: DTZ005
         )
         await future
 
     async def process_sleeps(self) -> None:
         """Process the sleep queue, advancing the time when necessary."""
-        while True:
-            sleep_time, future = await self.sleep_queue.get()
+        if self.sleep_queue is None:
+            raise _NotInitializedError
 
-            if self.frozen_factory.time_to_freeze < sleep_time:
-                self.frozen_factory.move_to(sleep_time)
-            future.set_result(None)
+        while True:
+            try:
+                sleep_time, future = await self.sleep_queue.get()
+            except RuntimeError:
+                return  # the queue is closed, when fixture pytest and pytest-asyncio
+            else:
+                if self.frozen_factory.time_to_freeze < sleep_time:
+                    self.frozen_factory.move_to(sleep_time)
+                future.set_result(None)
```

### Comparing `sleepfake-1.0.1/tests/test_async.py` & `sleepfake-1.0.2/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `sleepfake-1.0.1/tests/test_sync.py` & `sleepfake-1.0.2/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `sleepfake-1.0.1/LICENSE` & `sleepfake-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepfake-1.0.1/README.md` & `sleepfake-1.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 
 ```bash
 pip install sleepfake
 ```
 
 ## 🚀 Usage
 
+### Context Manager
+
 ```python
 import asyncio
 import time
 
 from sleepfake import SleepFake
 
 
@@ -27,27 +29,50 @@
         start = time.time()
         time.sleep(10)
         end = time.time()
         assert end - start == 10
     real_end = time.time()
     assert real_end - real_start < 1
 
-
+@pytest.mark.asyncio
 async def test_async_example():
     real_start = asyncio.get_event_loop().time()
     with SleepFake():
         start = asyncio.get_event_loop().time()
         await asyncio.gather(asyncio.sleep(5), asyncio.sleep(5), asyncio.sleep(5))
         end = asyncio.get_event_loop().time()
         assert end - start <= 5.5  # almost 5 seconds  # noqa: PLR2004
         assert end - start >= 5  # almost 5 seconds  # noqa: PLR2004
     real_end = asyncio.get_event_loop().time()
     assert real_end - real_start < 1  # almost 0 seconds
 ```
 
+### With Fixture (Beta)
+
+```python
+import asyncio
+import time
+
+from sleepfake import SleepFake
+
+def test_example(sleepfake: SleepFake):
+    start = time.time()
+    time.sleep(10)
+    end = time.time()
+    assert end - start == 10
+
+@pytest.mark.asyncio
+async def test_async_example(sleepfake: SleepFake):
+    start = asyncio.get_event_loop().time()
+    await asyncio.gather(asyncio.sleep(5), asyncio.sleep(5), asyncio.sleep(5))
+    end = asyncio.get_event_loop().time()
+    assert end - start <= 5.5  # almost 5 seconds  # noqa: PLR2004
+    assert end - start >= 5  # almost 5 seconds  # noqa: PLR2004
+```
+
 ## Local Development
 
 ### Prerequisites
 
 Install [rye](https://rye-up.com/)
 
 ```bash
```

### Comparing `sleepfake-1.0.1/pyproject.toml` & `sleepfake-1.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sleepfake"
-version = "1.0.1"
+version = "1.0.2"
 description = "Fake the time.sleep/asyncio.sleep function during tests."
 authors = [
     { name = "Guillaume Pouyat", email = "guillaume.pouyat@protonmail.com" },
 ]
 dependencies = [
     "freezegun>=1.4.0",
     "pytest>=8.0.2",
@@ -172,7 +172,10 @@
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.ruff.lint.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
+
+[project.entry-points.pytest11]
+pytest11 = "sleepfake.plugin"
```

### Comparing `sleepfake-1.0.1/PKG-INFO` & `sleepfake-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepfake
-Version: 1.0.1
+Version: 1.0.2
 Summary: Fake the time.sleep/asyncio.sleep function during tests.
 Author-email: Guillaume Pouyat <guillaume.pouyat@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -38,14 +38,16 @@
 
 ```bash
 pip install sleepfake
 ```
 
 ## 🚀 Usage
 
+### Context Manager
+
 ```python
 import asyncio
 import time
 
 from sleepfake import SleepFake
 
 
@@ -55,27 +57,50 @@
         start = time.time()
         time.sleep(10)
         end = time.time()
         assert end - start == 10
     real_end = time.time()
     assert real_end - real_start < 1
 
-
+@pytest.mark.asyncio
 async def test_async_example():
     real_start = asyncio.get_event_loop().time()
     with SleepFake():
         start = asyncio.get_event_loop().time()
         await asyncio.gather(asyncio.sleep(5), asyncio.sleep(5), asyncio.sleep(5))
         end = asyncio.get_event_loop().time()
         assert end - start <= 5.5  # almost 5 seconds  # noqa: PLR2004
         assert end - start >= 5  # almost 5 seconds  # noqa: PLR2004
     real_end = asyncio.get_event_loop().time()
     assert real_end - real_start < 1  # almost 0 seconds
 ```
 
+### With Fixture (Beta)
+
+```python
+import asyncio
+import time
+
+from sleepfake import SleepFake
+
+def test_example(sleepfake: SleepFake):
+    start = time.time()
+    time.sleep(10)
+    end = time.time()
+    assert end - start == 10
+
+@pytest.mark.asyncio
+async def test_async_example(sleepfake: SleepFake):
+    start = asyncio.get_event_loop().time()
+    await asyncio.gather(asyncio.sleep(5), asyncio.sleep(5), asyncio.sleep(5))
+    end = asyncio.get_event_loop().time()
+    assert end - start <= 5.5  # almost 5 seconds  # noqa: PLR2004
+    assert end - start >= 5  # almost 5 seconds  # noqa: PLR2004
+```
+
 ## Local Development
 
 ### Prerequisites
 
 Install [rye](https://rye-up.com/)
 
 ```bash
```

