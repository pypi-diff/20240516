# Comparing `tmp/mentabotix-0.1.4.tar.gz` & `tmp/mentabotix-0.1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mentabotix-0.1.4.tar", last modified: Thu May 16 06:04:50 2024, max compression
+gzip compressed data, was "mentabotix-0.1.4.1.tar", last modified: Thu May 16 14:56:21 2024, max compression
```

## Comparing `mentabotix-0.1.4.tar` & `mentabotix-0.1.4.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1066 2024-05-16 06:04:25.185276 mentabotix-0.1.4/LICENSE
--rw-r--r--   0        0        0    23781 2024-05-16 06:04:25.185276 mentabotix-0.1.4/README.md
--rw-r--r--   0        0        0      678 2024-05-16 06:04:50.953431 mentabotix-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1158 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/__init__.py
--rw-r--r--   0        0        0    68552 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/modules/botix.py
--rw-r--r--   0        0        0      225 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/modules/exceptions.py
--rw-r--r--   0        0        0      580 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/modules/logger.py
--rw-r--r--   0        0        0    20144 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/modules/menta.py
--rw-r--r--   0        0        0     7841 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/tools/composers.py
--rw-r--r--   0        0        0     2292 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/tools/generators.py
--rw-r--r--   0        0        0     9429 2024-05-16 06:04:25.185276 mentabotix-0.1.4/src/mentabotix/vision/tagdetector.py
--rw-r--r--   0        0        0        0 2024-05-16 06:04:25.185276 mentabotix-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0    15471 2024-05-16 06:04:25.189276 mentabotix-0.1.4/tests/test_botix.py
--rw-r--r--   0        0        0     8534 2024-05-16 06:04:25.189276 mentabotix-0.1.4/tests/test_composer.py
--rw-r--r--   0        0        0     8998 2024-05-16 06:04:25.189276 mentabotix-0.1.4/tests/test_menta.py
--rw-r--r--   0        0        0     6488 2024-05-16 06:04:25.189276 mentabotix-0.1.4/tests/test_moving_state.py
--rw-r--r--   0        0        0     5578 2024-05-16 06:04:25.189276 mentabotix-0.1.4/tests/test_moving_transition.py
--rw-r--r--   0        0        0    24215 1970-01-01 00:00:00.000000 mentabotix-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/LICENSE
+-rw-r--r--   0        0        0    23799 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/README.md
+-rw-r--r--   0        0        0      680 2024-05-16 14:56:21.469197 mentabotix-0.1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1210 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/__init__.py
+-rw-r--r--   0        0        0    68524 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/modules/botix.py
+-rw-r--r--   0        0        0      225 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/modules/exceptions.py
+-rw-r--r--   0        0        0      580 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/modules/logger.py
+-rw-r--r--   0        0        0    20135 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/modules/menta.py
+-rw-r--r--   0        0        0     9471 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/tools/composers.py
+-rw-r--r--   0        0        0     2292 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/tools/generators.py
+-rw-r--r--   0        0        0     9429 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/src/mentabotix/vision/tagdetector.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/tests/__init__.py
+-rw-r--r--   0        0        0      682 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/tests/find_tests.py
+-rw-r--r--   0        0        0    15535 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/tests/test_botix.py
+-rw-r--r--   0        0        0    10196 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/tests/test_composer.py
+-rw-r--r--   0        0        0     8998 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/tests/test_menta.py
+-rw-r--r--   0        0        0     6488 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/tests/test_moving_state.py
+-rw-r--r--   0        0        0     5578 2024-05-16 14:55:57.161053 mentabotix-0.1.4.1/tests/test_moving_transition.py
+-rw-r--r--   0        0        0    24235 1970-01-01 00:00:00.000000 mentabotix-0.1.4.1/PKG-INFO
```

### Comparing `mentabotix-0.1.4/LICENSE` & `mentabotix-0.1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4/README.md` & `mentabotix-0.1.4.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -594,15 +594,15 @@
 # make the botix object
 botix = Botix(controller=CloseLoopController(motor_infos=[MotorInfo(i) for i in range(4)], port="COM3"))
 
 # add the transition
 botix.token_pool.extend([transition_a_bcd, transition_d_ef])
 
 # export the structure
-botix.export_structure("schema.puml")
+Botix.export_structure("schema.puml", botix.token_pool)
 ```
 
 The result will be written to `schema.puml` and below is the expected Puml source code.
 
 ```plantuml
 @startuml
 state "5-MovingState(600, 600, 600, 600)" as state_6
@@ -662,15 +662,15 @@
 
 # let's use botix to make the visualization!
 # first make the botix object
 con = CloseLoopController(motor_infos=[MotorInfo(i) for i in range(4)])
 botix = Botix(controller=con)
 
 # make the visualization
-botix.export_structure("composed.puml", transitions=transitions)
+Botix.export_structure("composed.puml", transitions=transitions)
 ```
 
 The exported structure will be written to `composed.puml`, and below is the expected Puml source code.
 
 ```plantuml
 @startuml
 state "3-MovingState(2000, 2000, 2000, 2000)" as state_3
```

### Comparing `mentabotix-0.1.4/pyproject.toml` & `mentabotix-0.1.4.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [project]
 name = "mentabotix"
-version = "0.1.4"
+version = "0.1.4.1"
 description = "A Bot control lib"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "coloredlogs>=15.0.1",
     "numpy>=1.26.4",
     "pyapriltags>=3.3.0.3",
     "terminaltables>=3.1.10",
-    "bdmc>=0.1.5.6",
+    "bdmc>=0.1.5.7",
     "opencv-python-headless>=4.9.0.80",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `mentabotix-0.1.4/src/mentabotix/__init__.py` & `mentabotix-0.1.4.1/src/mentabotix/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .modules.botix import MovingState, MovingTransition, Botix
 from .modules.exceptions import BadSignatureError, RequirementError, SamplerTypeError, TokenizeError, StructuralError
 from .modules.logger import set_log_level
 from .modules.menta import Menta, SequenceSampler, IndexedSampler, DirectSampler, SamplerUsage, SamplerType, Sampler
 
-from .tools.composers import MovingChainComposer, straight_chain, snaking_chain, scanning_chain
+from .tools.composers import MovingChainComposer, straight_chain, snaking_chain, scanning_chain, random_lr_turn_branch
 from .tools.generators import NameGenerator, Multipliers, make_multiplier_generator
 from .vision.tagdetector import TagDetector
 
 __all__ = [
     "set_log_level",
     # botix
     "MovingState",
@@ -30,11 +30,12 @@
     "TokenizeError",
     "StructuralError",
     # tools/composers
     "MovingChainComposer",
     "straight_chain",
     "snaking_chain",
     "scanning_chain",
+    "random_lr_turn_branch",
     # tools/generators
     "NameGenerator",
     "Multipliers",
 ]
```

### Comparing `mentabotix-0.1.4/src/mentabotix/modules/botix.py` & `mentabotix-0.1.4.1/src/mentabotix/modules/botix.py`

 * *Files 1% similar despite different names*

```diff
@@ -654,16 +654,16 @@
             ValueError: If from_states is not None, a MovingState object, or an iterable of MovingState objects.
             ValueError: If to_states is not None, a MovingState object, a dictionary mapping keys to MovingState objects,
                 or None.
 
         Returns:
             None
         """
-        if duration <= 0:
-            raise ValueError(f"Duration must be positive, got {duration}")
+        if duration < 0:
+            raise ValueError(f"Duration can't be negative, got {duration}")
         if breaker is not None and signature(breaker).return_annotation == Signature.empty:
             raise ValueError(f"Breaker {breaker} must have annotated return type!")
 
         self.duration: float = duration
         self.breaker: Optional[Callable[[], Any]] = breaker
         self.check_interval: float = check_interval
         match from_states:
@@ -783,27 +783,28 @@
         *token_pool* : A `TokenPool` object that represents the bot's token pool.
     """
 
     def __init__(self, controller: CloseLoopController, token_pool: Optional[TokenPool] = None):
         self.controller: CloseLoopController = controller
         self.token_pool: TokenPool = token_pool or []
 
-    def acquire_unique_start(self, token_pool: TokenPool, none_check: bool = True) -> MovingState | None:
+    @staticmethod
+    def acquire_unique_start(token_pool: TokenPool, none_check: bool = True) -> MovingState | None:
         """
         Retrieves a unique starting state from the given token pool.
 
         Parameters:
         - token_pool: An instance of TokenPool, representing a collection of tokens.
         - none_check: A boolean, defaulting to True. If True, raises a ValueError when no unique starting state is found; otherwise, returns None.
 
         Returns:
         - Either a MovingState or None. Returns the starting state (with indegree 0) if uniquely identified; based on none_check's value, either returns None or raises an exception.
         """
         # Identifies states with an indegree of zero
-        zero_indegree_states = list(states_indegree := self.acquire_start_states(token_pool))
+        zero_indegree_states = list(states_indegree := Botix.acquire_start_states(token_pool))
 
         # Validates that there is exactly one state with an indegree of zero
         if len(zero_indegree_states) == 1:
             return zero_indegree_states[0]
         else:
             if none_check:
                 # Raises an error if none_check is enabled and no unique starting state is present
@@ -1336,26 +1337,26 @@
                 lines = self._assembly_match_cases(match_expression=match_expr, cases=match_branch)
                 return lines
             case _:
                 compiled_lines.append(line)
                 # If no forward transition is present, return the compiled lines
                 return compiled_lines
 
-    def export_structure(self, save_path: str, transitions: Optional[List[MovingTransition]] = None) -> Self:
+    @classmethod
+    def export_structure(cls, save_path: str, transitions: TokenPool) -> Self:
         """
         Export the structure to a UML file based on the provided transitions.
 
         Args:
             save_path (str): The path to save the UML file.
             transitions (Optional[List[MovingTransition]]): The list of transitions to represent in the UML.
 
         Returns:
             Self: The current instance.
         """
-        transitions: TokenPool = transitions or self.token_pool
         start_string = "@startuml\n"
         end_string = "@enduml\n"
 
         used_state: Dict[MovingState, str] = {}
 
         lines: List[str] = []
         name_gen: NameGenerator = NameGenerator(basename="state_")
@@ -1393,24 +1394,24 @@
                             used_state[to_state] = to_state_alias
                             lines.insert(0, f'state "{to_state}" as {to_state_alias}\n')
                         else:
                             to_state_alias = used_state.get(to_state)
 
                         lines.append(f"{break_node_name} --> {to_state_alias}: {case_name}\n")
 
-        start_states = self.acquire_start_states(token_pool=transitions)
-        end_states = self.acquire_end_states(token_pool=transitions)
+        start_states: Set[MovingState] = Botix.acquire_start_states(token_pool=transitions)
+        end_states: Set[MovingState] = Botix.acquire_end_states(token_pool=transitions)
 
         start_heads: List[str] = [f"[*] --> {used_state.get(sta)}\n" for sta in start_states]
         end_heads: List[str] = [f"{used_state.get(sta)} --> [*]\n" for sta in end_states]
 
         with open(save_path, "w") as f:
 
             f.writelines([start_string, *lines, "\n", *start_heads, "\n", *end_heads, "\n", end_string])
-        return self
+        return cls
 
     def compile(self, return_median: bool = False) -> Callable[[], None] | Tuple[List[str], Context]:
         """
         Compiles the bot's code and returns a callable function or a tuple of compiled lines and context.
 
         Args:
             return_median (bool, optional): Whether to return the compiled lines and context instead of a callable function. Defaults to False.
```

### Comparing `mentabotix-0.1.4/src/mentabotix/modules/logger.py` & `mentabotix-0.1.4.1/src/mentabotix/modules/logger.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4/src/mentabotix/modules/menta.py` & `mentabotix-0.1.4.1/src/mentabotix/modules/menta.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 
         参数:
         - usages: 一个SamplerUsage对象的列表，描述了每个采样器是如何被使用的。
         - judging_source: 判断源，可以是字符串或字符串列表。定义了判断逻辑的代码。
         - extra_context: 可选的字典，提供了额外的上下文信息，这些信息在执行判断函数时会包含在执行环境中。
 
         返回值:
-        - 一个无参数的布尔型函数，执行时根据判断逻辑返回Any类型的结果。
+        - 一个无参数的函数，执行时根据判断逻辑返回Any类型的结果。
 
         Args:
             return_raw:
         """
 
         # 将judging_source统一处理为字符串格式
         judging_source: str = judging_source if isinstance(judging_source, str) else "\n ".join(judging_source)
```

### Comparing `mentabotix-0.1.4/src/mentabotix/tools/composers.py` & `mentabotix-0.1.4.1/src/mentabotix/tools/composers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List, Tuple, Callable, Optional, Self, Type, TypeVar, Dict
 
 from numpy import arange
+from numpy.random import random
 
 from ..modules.botix import MovingState, MovingTransition, __PLACE_HOLDER__
 
 StateTransitionPack = Tuple[List[MovingState], List[MovingTransition]]
 
 UnitType = TypeVar("UnitType", Type[MovingState], Type[MovingTransition])
 
@@ -195,7 +196,52 @@
 def snaking_chain():
     """
     A function that calculates the states and transitions for a snaking chain.
     Returns:
 
     """
     raise NotImplementedError
+
+
+def random_lr_turn_branch(
+    start_state: MovingState,
+    end_state: MovingState,
+    start_state_duration: float,
+    turn_speed: int,
+    turn_duration: float,
+    turn_left_prob: 0.5,
+) -> Tuple[MovingTransition, MovingTransition]:
+    """
+    A function that generates random left and right turn states based on probabilities.
+    It creates two transition states, a start transition, and a turn transition.
+
+    Parameters:
+        start_state (MovingState): The initial state.
+        end_state (MovingState): The final state.
+        start_state_duration (float): The duration of the start state.
+        turn_speed (int): The speed of the turn.
+        turn_duration (float): The duration of the turn.
+        turn_left_prob (float): The probability of turning left.
+
+    Returns:
+        tuple: A tuple containing the start transition and the turn transition.
+    """
+    if not 0 < turn_left_prob < 1:
+        raise ValueError("turn_speed must be between 0 and 1")
+
+    def _die() -> bool:
+        return random() > turn_left_prob
+
+    left_turn_state = MovingState.turn("l", turn_speed)
+    right_turn_state = MovingState.turn("r", turn_speed)
+    start_transition = MovingTransition(
+        from_states=start_state,
+        to_states={False: right_turn_state, True: left_turn_state},
+        duration=start_state_duration,
+        breaker=_die,
+    )
+    turn_transition = MovingTransition(
+        from_states=[left_turn_state, right_turn_state],
+        to_states={__PLACE_HOLDER__: end_state},
+        duration=turn_duration,
+    )
+    return start_transition, turn_transition
```

### Comparing `mentabotix-0.1.4/src/mentabotix/tools/generators.py` & `mentabotix-0.1.4.1/src/mentabotix/tools/generators.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4/src/mentabotix/vision/tagdetector.py` & `mentabotix-0.1.4.1/src/mentabotix/vision/tagdetector.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4/tests/test_botix.py` & `mentabotix-0.1.4.1/tests/test_botix.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
                 "                    con.set_motors_speed((600, 600, 600, 600))",
             ],
             compiled[0],
         )
 
         obj = self.botix_instance.compile()
         obj()
-        self.botix_instance.export_structure("test.puml")
+        self.botix_instance.export_structure("test.puml", self.botix_instance.token_pool)
 
     def test_export_structure(self):
         MovingState.__state_id_counter__ = 0
         MovingTransition.__state_id_counter__ = 0
         state_a = MovingState(100)
         state_b = MovingState(200)
         state_c = MovingState(300)
@@ -323,15 +323,15 @@
         transition_d_ef = MovingTransition(
             duration=1,
             from_states=state_d,
             to_states={1: state_e, 2: state_f},
             breaker=transition_breaker_fac([1, 2]),
         )
         self.botix_instance.token_pool = [transition_a_bcd, transition_d_ef]
-        self.botix_instance.export_structure("test.puml")
+        self.botix_instance.export_structure("test.puml", self.botix_instance.token_pool)
 
     def test_compile_expressions(self):
         MovingState.__state_id_counter__ = 0
         MovingTransition.__state_id_counter__ = 0
 
         state_a = MovingState(speed_expressions="var1", used_context_variables=["var1"])
         state_b = MovingState(speed_expressions=("var1", "var2"), used_context_variables=["var1", "var2"])
```

### Comparing `mentabotix-0.1.4/tests/test_composer.py` & `mentabotix-0.1.4.1/tests/test_composer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import random
 import unittest
 
 from bdmc import CloseLoopController, MotorInfo
 
-from mentabotix import MovingChainComposer, MovingState, MovingTransition, straight_chain, Botix
+from mentabotix import MovingChainComposer, MovingState, MovingTransition, straight_chain, Botix, random_lr_turn_branch
+from mentabotix.tools.composers import __PLACE_HOLDER__
 
 
 # Assuming MovingState, MovingTransition, UnitType, StateTransitionPack are defined elsewhere
 # You'll need to replace these with the actual classes and types
 
 
 class TestComposer(unittest.TestCase):
@@ -187,15 +188,15 @@
             duration=duration,
             power_exponent=power_exponent,
             interval=interval,
             breaker=break_function,
         )
 
         botix = Botix(controller=CloseLoopController([MotorInfo(i) for i in range(4)]), token_pool=transitions)
-        botix.export_structure("long_chain.puml")
+        botix.export_structure("long_chain.puml", botix.token_pool)
 
     # 测试breaker不是None且不是callable的情况
     def test_straight_chain_with_invalid_breaker(self):
         start_speed = 50
         end_speed = 100
         duration = 5.0
         power_exponent = 1.0
@@ -232,12 +233,48 @@
 
         # let's use botix to make the visualization!
         # first make the botix object
         con = CloseLoopController(motor_infos=[MotorInfo(i) for i in range(4)])
         botix = Botix(controller=con, token_pool=transitions)
 
         # make the visualization
-        botix.export_structure("composed.puml")
+        botix.export_structure("composed.puml", botix.token_pool)
+
+    def test_valid_input(self):
+
+        # 定义测试用的变量
+        start_state = MovingState(100)
+        end_state = MovingState(500)
+        start_state_duration = 2.0
+        turn_speed = 5000
+        turn_duration = 1.5
+        turn_left_prob = 0.5
+
+        # 正常输入的测试
+        start_transition, turn_transition = random_lr_turn_branch(
+            start_state, end_state, start_state_duration, turn_speed, turn_duration, turn_left_prob
+        )
+
+        Botix.export_structure("random_lr_turn_branch.puml", [start_transition, turn_transition])
+        # 检查 start_transition 是否正确
+        self.assertIsInstance(start_transition, MovingTransition)
+        self.assertEqual(start_transition.from_states[0], start_state)
+        self.assertIn(False, start_transition.to_states)
+        self.assertIn(True, start_transition.to_states)
+
+        # 检查 turn_transition 是否正确
+        self.assertIsInstance(turn_transition, MovingTransition)
+        for a, b in zip(
+            turn_transition.from_states, [MovingState.turn("l", turn_speed), MovingState.turn("r", turn_speed)]
+        ):
+            self.assertEqual(a, b)
+        self.assertEqual(turn_transition.to_states[__PLACE_HOLDER__], end_state)
+        self.assertEqual(turn_transition.duration, turn_duration)
+
+    def test_invalid_turn_speed(self):
+        # 测试无效的 turn_speed 输入
+        with self.assertRaises(ValueError):
+            random_lr_turn_branch(MovingState(0), MovingState(20), 2.0, -1, 1.5, 1.5)  # Invalid turn_speed
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `mentabotix-0.1.4/tests/test_menta.py` & `mentabotix-0.1.4.1/tests/test_menta.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4/tests/test_moving_state.py` & `mentabotix-0.1.4.1/tests/test_moving_state.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4/tests/test_moving_transition.py` & `mentabotix-0.1.4.1/tests/test_moving_transition.py`

 * *Files identical despite different names*

### Comparing `mentabotix-0.1.4/PKG-INFO` & `mentabotix-0.1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mentabotix
-Version: 0.1.4
+Version: 0.1.4.1
 Summary: A Bot control lib
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: coloredlogs>=15.0.1
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pyapriltags>=3.3.0.3
 Requires-Dist: terminaltables>=3.1.10
-Requires-Dist: bdmc>=0.1.5.6
+Requires-Dist: bdmc>=0.1.5.7
 Requires-Dist: opencv-python-headless>=4.9.0.80
 Description-Content-Type: text/markdown
 
 # mentabotix
 
 > A dedicated lib to control 4-fixed-wheels robot
 ---
@@ -609,15 +609,15 @@
 # make the botix object
 botix = Botix(controller=CloseLoopController(motor_infos=[MotorInfo(i) for i in range(4)], port="COM3"))
 
 # add the transition
 botix.token_pool.extend([transition_a_bcd, transition_d_ef])
 
 # export the structure
-botix.export_structure("schema.puml")
+Botix.export_structure("schema.puml", botix.token_pool)
 ```
 
 The result will be written to `schema.puml` and below is the expected Puml source code.
 
 ```plantuml
 @startuml
 state "5-MovingState(600, 600, 600, 600)" as state_6
@@ -677,15 +677,15 @@
 
 # let's use botix to make the visualization!
 # first make the botix object
 con = CloseLoopController(motor_infos=[MotorInfo(i) for i in range(4)])
 botix = Botix(controller=con)
 
 # make the visualization
-botix.export_structure("composed.puml", transitions=transitions)
+Botix.export_structure("composed.puml", transitions=transitions)
 ```
 
 The exported structure will be written to `composed.puml`, and below is the expected Puml source code.
 
 ```plantuml
 @startuml
 state "3-MovingState(2000, 2000, 2000, 2000)" as state_3
```

