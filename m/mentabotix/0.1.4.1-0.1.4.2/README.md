# Comparing `tmp/mentabotix-0.1.4.1.tar.gz` & `tmp/mentabotix-0.1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.4.1.tar", last modified: Thu May 16 14:56:21 2024, max compression
+gzip compressed data, was "mentabotix-0.1.4.2.tar", last modified: Thu May 16 15:29:17 2024, max compression
```

## Comparing `mentabotix-0.1.4.1.tar` & `mentabotix-0.1.4.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1066 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/LICENSE
--rw-r--r--   0        0        0    23799 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/README.md
--rw-r--r--   0        0        0      680 2024-05-16 14:56:21.469197 mentabotix-0.1.4.1/pyproject.toml
--rw-r--r--   0        0        0     1210 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    68524 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    20135 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0     9471 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0     9429 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/vision/tagdetector.py
--rw-r--r--   0        0        0        0 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/tests/__init__.py
--rw-r--r--   0        0        0      682 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/tests/find_tests.py
--rw-r--r--   0        0        0    15535 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/tests/test_botix.py
--rw-r--r--   0        0        0    10196 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/tests/test_composer.py
--rw-r--r--   0        0        0     8998 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/tests/test_menta.py
--rw-r--r--   0        0        0     6488 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/tests/test_moving_state.py
--rw-r--r--   0        0        0     5578 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24235 1970-01-01 00:00:00.000000 mentabotix-0.1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-16 15:28:53.013254 mentabotix-0.1.4.2/LICENSE
+-rw-r--r--   0        0        0    23799 2024-05-16 15:28:53.013254 mentabotix-0.1.4.2/README.md
+-rw-r--r--   0        0        0      680 2024-05-16 15:29:17.965503 mentabotix-0.1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     1210 2024-05-16 15:28:53.017254 mentabotix-0.1.4.2/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    67869 2024-05-16 15:28:53.017254 mentabotix-0.1.4.2/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-16 15:28:53.017254 mentabotix-0.1.4.2/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-16 15:28:53.017254 mentabotix-0.1.4.2/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    20135 2024-05-16 15:28:53.017254 mentabotix-0.1.4.2/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0     9471 2024-05-16 15:28:53.017254 mentabotix-0.1.4.2/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-16 15:28:53.017254 mentabotix-0.1.4.2/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0     9429 2024-05-16 15:28:53.017254 mentabotix-0.1.4.2/src/mentabotix/vision/tagdetector.py
+-rw-r--r--   0        0        0        0 2024-05-16 15:28:53.017254 mentabotix-0.1.4.2/tests/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-16 15:28:53.017254 mentabotix-0.1.4.2/tests/find_tests.py
+-rw-r--r--   0        0        0    15535 2024-05-16 15:28:53.017254 mentabotix-0.1.4.2/tests/test_botix.py
+-rw-r--r--   0        0        0    10196 2024-05-16 15:28:53.017254 mentabotix-0.1.4.2/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-16 15:28:53.017254 mentabotix-0.1.4.2/tests/test_menta.py
+-rw-r--r--   0        0        0     6488 2024-05-16 15:28:53.017254 mentabotix-0.1.4.2/tests/test_moving_state.py
+-rw-r--r--   0        0        0     5338 2024-05-16 15:28:53.017254 mentabotix-0.1.4.2/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24235 1970-01-01 00:00:00.000000 mentabotix-0.1.4.2/PKG-INFO
```

### Comparing `mentabotix-0.1.4.1/LICENSE` & `mentabotix-0.1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.1/README.md` & `mentabotix-0.1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.1/pyproject.toml` & `mentabotix-0.1.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mentabotix"
-version = "0.1.4.1"
+version = "0.1.4.2"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
```

### Comparing `mentabotix-0.1.4.1/src/mentabotix/__init__.py` & `mentabotix-0.1.4.2/src/mentabotix/__init__.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.1/src/mentabotix/modules/botix.py` & `mentabotix-0.1.4.2/src/mentabotix/modules/botix.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import inspect
 from collections import Counter
 from dataclasses import dataclass
 from enum import Enum
-from inspect import signature, Signature
 from itertools import zip_longest
 from queue import Queue
 from typing import (
     Tuple,
     TypeAlias,
     Self,
     Unpack,
     Literal,
     Any,
     Callable,
-    Iterable,
     Hashable,
     TypeVar,
     Dict,
     Optional,
     List,
     ClassVar,
     Set,
@@ -631,65 +629,59 @@
         duration: float,
         breaker: Optional[Callable[[], KT] | Callable[[], bool] | Callable[[], Any]] = None,
         check_interval: Optional[float] = 0.01,
         from_states: Optional[Sequence[MovingState] | MovingState] = None,
         to_states: Optional[Dict[KT, MovingState] | MovingState] = None,
     ):
         """
-        Initialize a new instance of the MovingTransition class.
+        Initialize a MovingTransition object.
 
         Args:
-            duration (float): The duration of the transition in seconds. Must be positive.
-            breaker (Optional[Callable[[], KT] | Callable[[], bool] | Callable[[], Any]]): A function that determines
-                whether the transition should be broken. If None, no breaker function is used. Must have an annotated
-                return type.
-            check_interval (Optional[float]): The interval in seconds at which the breaker function should be checked.
-                Defaults to 0.01 seconds.
-            from_states (Optional[Iterable[MovingState] | MovingState]): The states that the transition originates from.
-                Can be a single state or an iterable of states. Defaults to None.
-            to_states (Optional[Dict[KT, MovingState] | MovingState]): The states that the transition leads to. Can be a
-                single state or a dictionary mapping keys to states. Defaults to None.
+            duration: The transition duration, must be a non-negative float.
+            breaker: An optional callback function that can return a key (of type KT), a boolean, or any other value, used to interrupt the current state transition.
+            check_interval: The frequency at which to check for state transition, i.e., how often in seconds to check.
+            from_states: The starting states for the transition, can be a MovingState instance or a sequence of them.
+            to_states: The destination states mapped to corresponding MovingState instances, or directly a MovingState instance.
 
         Raises:
-            ValueError: If duration is not positive or if breaker has an empty return type annotation.
-            ValueError: If from_states is not None, a MovingState object, or an iterable of MovingState objects.
-            ValueError: If to_states is not None, a MovingState object, a dictionary mapping keys to MovingState objects,
-                or None.
-
-        Returns:
-            None
+            ValueError: If duration is negative, or from_states, to_states parameters are incorrectly formatted.
         """
+
+        # Validate the duration
         if duration < 0:
             raise ValueError(f"Duration can't be negative, got {duration}")
-        if breaker is not None and signature(breaker).return_annotation == Signature.empty:
-            raise ValueError(f"Breaker {breaker} must have annotated return type!")
 
+        # Initialize attributes
         self.duration: float = duration
         self.breaker: Optional[Callable[[], Any]] = breaker
         self.check_interval: float = check_interval
+
+        # Process the initial states parameter
         match from_states:
             case None:
                 self.from_states: List[MovingState] = []
             case state if isinstance(state, MovingState):
                 self.from_states: List[MovingState] = [from_states]
             case state if isinstance(state, Sequence) and all(isinstance(s, MovingState) for s in state):
                 self.from_states: List[MovingState] = list(from_states)
             case _:
                 raise ValueError(f"Invalid from_states, got {from_states}")
 
+        # Process the target states parameter
         match to_states:
             case None:
                 self.to_states: Dict[KT, MovingState] = {}
             case state if isinstance(state, MovingState):
                 self.to_states: Dict[KT, MovingState] = {__PLACE_HOLDER__: state}
             case state if isinstance(state, Dict):
                 self.to_states: Dict[KT, MovingState] = to_states
             case _:
                 raise ValueError(f"Invalid to_states, got {to_states}")
 
+        # Assign a unique transition ID
         self._transition_id: int = MovingTransition.__state_id_counter__
         MovingTransition.__state_id_counter__ += 1
 
     def add_from_state(self, state: MovingState) -> Self:
         """
         Adds a `MovingState` object to the `from_state` list.
```

### Comparing `mentabotix-0.1.4.1/src/mentabotix/modules/logger.py` & `mentabotix-0.1.4.2/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.1/src/mentabotix/modules/menta.py` & `mentabotix-0.1.4.2/src/mentabotix/modules/menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.1/src/mentabotix/tools/composers.py` & `mentabotix-0.1.4.2/src/mentabotix/tools/composers.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.1/src/mentabotix/tools/generators.py` & `mentabotix-0.1.4.2/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.1/src/mentabotix/vision/tagdetector.py` & `mentabotix-0.1.4.2/src/mentabotix/vision/tagdetector.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.1/tests/find_tests.py` & `mentabotix-0.1.4.2/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.1/tests/test_botix.py` & `mentabotix-0.1.4.2/tests/test_botix.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.1/tests/test_composer.py` & `mentabotix-0.1.4.2/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.1/tests/test_menta.py` & `mentabotix-0.1.4.2/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.1/tests/test_moving_state.py` & `mentabotix-0.1.4.2/tests/test_moving_state.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4.1/tests/test_moving_transition.py` & `mentabotix-0.1.4.2/tests/test_moving_transition.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,21 +38,14 @@
         self.assertIsInstance(transition.from_states, list)
         self.assertIsInstance(transition.to_states, dict)
 
     def test_init_duration_not_positive(self):
         with self.assertRaises(ValueError):
             MovingTransition(-1, None, None, None, None)
 
-    def test_init_breaker_no_return_type_annotation(self):
-        def invalid_breaker():
-            pass
-
-        with self.assertRaises(ValueError):
-            MovingTransition(self.default_duration, invalid_breaker, None, None, None)
-
     def test_init_from_states_valid_types(self):
         # Test valid from_states types
         transition = MovingTransition(self.default_duration, None, None, self.default_from_state, None)
         self.assertEqual(len(transition.from_states), 1)
         self.assertEqual(transition.from_states[0], self.default_from_state)
 
         from_states_iterable = [MovingState(0), MovingState(0)]
```

### Comparing `mentabotix-0.1.4.1/PKG-INFO` & `mentabotix-0.1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.4.1
+Version: 0.1.4.2
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pyapriltags>=3.3.0.3
```

