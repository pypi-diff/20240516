# Comparing `tmp/pythonix-1.0.5.tar.gz` & `tmp/pythonix-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonix-1.0.5.tar", max compression
+gzip compressed data, was "pythonix-1.0.6.tar", max compression
```

## Comparing `pythonix-1.0.5.tar` & `pythonix-1.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     3027 2024-05-08 15:21:18.899631 pythonix-1.0.5/README.md
--rw-r--r--   0        0        0      409 2024-05-16 15:03:57.509631 pythonix-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 01:39:00.350000 pythonix-1.0.5/pythonix/__init__.py
--rw-r--r--   0        0        0      465 2024-05-15 16:52:32.679631 pythonix-1.0.5/pythonix/curry.py
--rw-r--r--   0        0        0      387 2024-05-15 18:24:17.999631 pythonix-1.0.5/pythonix/dict_utils.py
--rw-r--r--   0        0        0      930 2024-05-15 19:41:41.229631 pythonix-1.0.5/pythonix/grammar.py
--rw-r--r--   0        0        0     8262 2024-05-15 16:47:08.319631 pythonix-1.0.5/pythonix/internals/curry.py
--rw-r--r--   0        0        0     3949 2024-05-15 03:15:10.619631 pythonix-1.0.5/pythonix/internals/dict_utils.py
--rw-r--r--   0        0        0     3537 2024-05-15 19:41:41.979631 pythonix-1.0.5/pythonix/internals/grammar.py
--rw-r--r--   0        0        0     3914 2024-05-15 15:58:00.019631 pythonix-1.0.5/pythonix/internals/mdeq.py
--rw-r--r--   0        0        0     5233 2024-05-15 15:47:55.849631 pythonix-1.0.5/pythonix/internals/op.py
--rw-r--r--   0        0        0     1381 2024-05-09 16:54:03.599631 pythonix-1.0.5/pythonix/internals/pair.py
--rw-r--r--   0        0        0     4237 2024-05-15 18:26:22.289631 pythonix-1.0.5/pythonix/internals/pipe.py
--rw-r--r--   0        0        0     1410 2024-05-15 16:49:20.859631 pythonix-1.0.5/pythonix/internals/prove.py
--rw-r--r--   0        0        0     7268 2024-05-13 00:29:18.849631 pythonix-1.0.5/pythonix/internals/req.py
--rw-r--r--   0        0        0    14088 2024-05-15 16:45:49.679631 pythonix-1.0.5/pythonix/internals/res.py
--rw-r--r--   0        0        0     2253 2024-05-12 19:34:25.729631 pythonix-1.0.5/pythonix/internals/trail.py
--rw-r--r--   0        0        0     2696 2024-05-09 20:50:48.239631 pythonix-1.0.5/pythonix/internals/tup.py
--rw-r--r--   0        0        0      178 2024-05-09 16:54:03.619631 pythonix-1.0.5/pythonix/internals/types.py
--rw-r--r--   0        0        0      420 2024-05-15 18:49:30.279631 pythonix-1.0.5/pythonix/mdeq.py
--rw-r--r--   0        0        0      283 2024-05-15 18:51:21.519631 pythonix-1.0.5/pythonix/op.py
--rw-r--r--   0        0        0      265 2024-05-15 18:52:34.069631 pythonix-1.0.5/pythonix/pair.py
--rw-r--r--   0        0        0      886 2024-05-14 14:13:15.569631 pythonix-1.0.5/pythonix/pipe.py
--rw-r--r--   0        0        0     2619 2024-05-16 15:03:06.689631 pythonix-1.0.5/pythonix/prelude.py
--rw-r--r--   0        0        0      233 2024-05-15 19:53:17.099631 pythonix-1.0.5/pythonix/prove.py
--rw-r--r--   0        0        0      645 2024-05-09 16:54:03.639631 pythonix-1.0.5/pythonix/req.py
--rw-r--r--   0        0        0     6424 2024-05-15 21:16:57.849631 pythonix-1.0.5/pythonix/res.py
--rw-r--r--   0        0        0      321 2024-05-16 14:59:03.309631 pythonix-1.0.5/pythonix/trail.py
--rw-r--r--   0        0        0      358 2024-05-16 14:59:49.929631 pythonix-1.0.5/pythonix/tup.py
--rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 pythonix-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3027 2024-05-08 15:21:18.899631 pythonix-1.0.6/README.md
+-rw-r--r--   0        0        0      409 2024-05-16 19:13:33.379631 pythonix-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-05-16 16:50:54.529631 pythonix-1.0.6/pythonix/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-16 16:50:54.539631 pythonix-1.0.6/pythonix/curry.py
+-rw-r--r--   0        0        0      387 2024-05-16 16:50:54.539631 pythonix-1.0.6/pythonix/dict_utils.py
+-rw-r--r--   0        0        0      953 2024-05-16 18:06:43.809631 pythonix-1.0.6/pythonix/grammar.py
+-rw-r--r--   0        0        0       28 2024-05-16 16:50:54.529631 pythonix-1.0.6/pythonix/internals/__init__.py
+-rw-r--r--   0        0        0     8835 2024-05-16 19:05:47.559631 pythonix-1.0.6/pythonix/internals/curry.py
+-rw-r--r--   0        0        0     3960 2024-05-16 16:50:54.709631 pythonix-1.0.6/pythonix/internals/dict_utils.py
+-rw-r--r--   0        0        0     3634 2024-05-16 18:14:38.709631 pythonix-1.0.6/pythonix/internals/grammar.py
+-rw-r--r--   0        0        0     4003 2024-05-16 19:12:13.159631 pythonix-1.0.6/pythonix/internals/mdeq.py
+-rw-r--r--   0        0        0     5374 2024-05-16 16:50:54.759631 pythonix-1.0.6/pythonix/internals/op.py
+-rw-r--r--   0        0        0     1349 2024-05-16 16:50:42.429631 pythonix-1.0.6/pythonix/internals/pair.py
+-rw-r--r--   0        0        0     2802 2024-05-16 16:50:54.619631 pythonix-1.0.6/pythonix/internals/pipe.py
+-rw-r--r--   0        0        0     1801 2024-05-16 19:06:43.679631 pythonix-1.0.6/pythonix/internals/prove.py
+-rw-r--r--   0        0        0     7203 2024-05-16 16:50:54.819631 pythonix-1.0.6/pythonix/internals/req.py
+-rw-r--r--   0        0        0    14294 2024-05-16 19:08:46.789631 pythonix-1.0.6/pythonix/internals/res.py
+-rw-r--r--   0        0        0     5041 2024-05-16 19:09:41.649631 pythonix-1.0.6/pythonix/internals/trail.py
+-rw-r--r--   0        0        0     2726 2024-05-16 16:26:19.349631 pythonix-1.0.6/pythonix/internals/tup.py
+-rw-r--r--   0        0        0      420 2024-05-16 16:50:54.629631 pythonix-1.0.6/pythonix/mdeq.py
+-rw-r--r--   0        0        0      251 2024-05-16 16:50:54.619631 pythonix-1.0.6/pythonix/op.py
+-rw-r--r--   0        0        0      265 2024-05-16 16:50:54.629631 pythonix-1.0.6/pythonix/pair.py
+-rw-r--r--   0        0        0      886 2024-05-16 16:18:58.339631 pythonix-1.0.6/pythonix/pipe.py
+-rw-r--r--   0        0        0     2565 2024-05-16 18:34:10.409631 pythonix-1.0.6/pythonix/prelude.py
+-rw-r--r--   0        0        0      210 2024-05-16 16:50:54.639631 pythonix-1.0.6/pythonix/prove.py
+-rw-r--r--   0        0        0      645 2024-05-16 16:24:04.869631 pythonix-1.0.6/pythonix/req.py
+-rw-r--r--   0        0        0     6424 2024-05-16 16:50:54.679631 pythonix-1.0.6/pythonix/res.py
+-rw-r--r--   0        0        0      290 2024-05-16 16:50:54.669631 pythonix-1.0.6/pythonix/trail.py
+-rw-r--r--   0        0        0      358 2024-05-16 16:50:54.679631 pythonix-1.0.6/pythonix/tup.py
+-rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 pythonix-1.0.6/PKG-INFO
```

### Comparing `pythonix-1.0.5/README.md` & `pythonix-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.5/pythonix/grammar.py` & `pythonix-1.0.6/pythonix/grammar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''
+"""
 Decorator classes that used to simulate prefix, infix, and suffix applications. Includes
 the special `p` object to pipe values from left to right into functions.
 #### Example
 ```python
 # Prefix Example
 @PipePrefix
 def absorb_right[T](val: T) -> T:
@@ -29,9 +29,15 @@
 
 # |p| Example
 add: Fn[Tuple[int, int], int] = lambda elems: sum(elems)
 
 assert (5, 5) |p| sum == 10
 assert p((5, 5))(sum) == 10
 ```
-'''
-from pythonix.internals.grammar import PipeApply, PipeSuffix, PipeInfix, PipePrefix, Pipe
+"""
+from pythonix.internals.grammar import (
+    PipeApply,
+    PipeSuffix,
+    PipeInfix,
+    PipePrefix,
+    P,
+)
```

### Comparing `pythonix-1.0.5/pythonix/internals/curry.py` & `pythonix-1.0.6/pythonix/internals/curry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 from typing import TypeVar, Callable
+from functools import wraps, update_wrapper, WRAPPER_ASSIGNMENTS
 
 T1 = TypeVar("T1")
 T2 = TypeVar("T2")
 T3 = TypeVar("T3")
 T4 = TypeVar("T4")
 T5 = TypeVar("T5")
 T6 = TypeVar("T6")
 T7 = TypeVar("T7")
 T8 = TypeVar("T8")
 T9 = TypeVar("T9")
 U = TypeVar("U")
 
+assignments = list(WRAPPER_ASSIGNMENTS)
+assignments.remove('__annotations__')
+updated_assignments = WRAPPER_ASSIGNMENTS
+# updated_assignments = tuple(assignments)
 
 def two(func: Callable[[T1, T2], U]) -> Callable[[T1], Callable[[T2], U]]:
+    @wraps(func, assigned=updated_assignments)
     def in1(t1: T1) -> Callable[[T2], U]:
         def in2(t2: T2) -> U:
             return func(t1, t2)
 
         return in2
-
     return in1
 
 
 def three(
     func: Callable[[T1, T2, T3], U]
 ) -> Callable[[T1], Callable[[T2], Callable[[T3], U]]]:
+    @wraps(func, assigned=updated_assignments)
     def in1(t1: T1) -> Callable[[T2], Callable[[T3], U]]:
         def in2(t2: T2) -> Callable[[T3], U]:
             def in3(t3: T3) -> U:
                 return func(t1, t2, t3)
 
             return in3
 
@@ -36,14 +42,15 @@
 
     return in1
 
 
 def four(
     func: Callable[[T1, T2, T3, T4], U]
 ) -> Callable[[T1], Callable[[T2], Callable[[T3], Callable[[T4], U]]]]:
+    @wraps(four)
     def in1(t1: T1) -> Callable[[T2], Callable[[T3], Callable[[T4], U]]]:
         def in2(t2: T2) -> Callable[[T3], Callable[[T4], U]]:
             def in3(t3: T3) -> Callable[[T4], U]:
                 def in4(t4: T4) -> U:
                     func(t1, t2, t3, t4)
 
                 return in4
@@ -54,14 +61,15 @@
 
     return in1
 
 
 def five(
     func: Callable[[T1, T2, T3, T4, T5], U]
 ) -> Callable[[T1], Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], U]]]]]:
+    @wraps(func, assigned=updated_assignments)
     def in1(
         t1: T1,
     ) -> Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], U]]]]:
         def in2(t2: T2) -> Callable[[T3], Callable[[T4], Callable[[T5], U]]]:
             def in3(t3: T3) -> Callable[[T4], Callable[[T5], U]]:
                 def in4(t4: T4) -> Callable[[T5], U]:
                     def in5(t5: T5) -> U:
@@ -80,14 +88,15 @@
 
 def six(
     func: Callable[[T1, T2, T3, T4, T5, T6], U]
 ) -> Callable[
     [T1],
     Callable[[T2], Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], U]]]]],
 ]:
+    @wraps(func, assigned=updated_assignments)
     def in1(
         t1: T1,
     ) -> Callable[
         [T2], Callable[[T3], Callable[[T4], Callable[[T5], Callable[[T6], U]]]]
     ]:
         def in2(
             t2: T2,
@@ -118,14 +127,15 @@
     Callable[
         [T2],
         Callable[
             [T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], U]]]]
         ],
     ],
 ]:
+    @wraps(func, assigned=updated_assignments)
     def in1(
         t1: T1,
     ) -> Callable[
         [T2],
         Callable[
             [T3], Callable[[T4], Callable[[T5], Callable[[T6], Callable[[T7], U]]]]
         ],
@@ -169,14 +179,15 @@
             [T3],
             Callable[
                 [T4], Callable[[T5], Callable[[T6], Callable[[T7], Callable[[T8], U]]]]
             ],
         ],
     ],
 ]:
+    @wraps(func, assigned=updated_assignments)
     def in1(
         t1: T1,
     ) -> Callable[
         [T2],
         Callable[
             [T3],
             Callable[
@@ -239,14 +250,15 @@
                     [T5],
                     Callable[[T6], Callable[[T7], Callable[[T8], Callable[[T9], U]]]],
                 ],
             ],
         ],
     ],
 ]:
+    @wraps(func, assigned=updated_assignments)
     def in1(
         t1: T1,
     ) -> Callable[
         [T2],
         Callable[
             [T3],
             Callable[
```

### Comparing `pythonix-1.0.5/pythonix/internals/dict_utils.py` & `pythonix-1.0.6/pythonix/internals/dict_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import TypeVar, Dict, Callable, Mapping
-from pythonix.op import item
+from pythonix.internals.op import item
 
 Val = TypeVar("Val")
 NewVal = TypeVar("NewVal")
 Key = TypeVar("Key", str, int, float, tuple)
 NewKey = TypeVar("NewKey", str, int, float, tuple)
 
 
@@ -124,14 +124,15 @@
 
         return get_dict
 
     return get_val
 
 
 def get(key: Key):
-    '''
+    """
     Retrieves a value from a mapping, returning `Nil` on error
-    '''
+    """
+
     def get_data(mapping: Mapping[Key, Val]):
         return item(key)(mapping)
 
     return get_data
```

### Comparing `pythonix-1.0.5/pythonix/internals/grammar.py` & `pythonix-1.0.6/pythonix/internals/grammar.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,121 +1,131 @@
 from __future__ import annotations
 from typing import TypeVar, Callable, Generic
-from pythonix.curry import two
+from pythonix.internals.curry import two
 
 Val = TypeVar("Val")
 Val2 = TypeVar("Val2")
 RetVal = TypeVar("RetVal")
-ErrVal = TypeVar('ErrVal', bound='Exception')
+ErrVal = TypeVar("ErrVal", bound="Exception")
 
 
 class PipeSuffix(Generic[Val, RetVal], object):
     """
     Class decorator used to create custom behavior that uses the `|` symbol.
     Wrap functions whose parameters you want to receive from the left of a `|` in the class.
     You can still call the function normally. Type information is not preserved for nested classes like
     `Ok`, `Err`, `Bind`, or `Do`
     ```python
     @PipeSuffix
     def add_one(x: int) -> int:
         return x + 1
-    
+
     assert 1 | add_one == 2
     assert add_one(1) == 2
     ```
     """
-    _op: Callable[[Val], RetVal]
+
+    op: Callable[[Val], RetVal]
 
     def __init__(self, op: Callable[[Val], RetVal]) -> None:
-        self._op = op
-    
+        self.op = op
+
     def __ror__(self, left: Val) -> RetVal:
-        return self._op(left)
-    
-    def __call__(self, left: Val) -> RetVal:
-        return self._op(left)
+        return self.op(left)
 
+    def __call__(self, left: Val) -> RetVal:
+        return self.op(left)
 
 
 class PipePrefix(Generic[Val, RetVal], object):
     """
     Class decorator used to create custom behavior that uses the `|` symbol.
     Wrap functions whose parameters you want to receive from the right of a `|` in the class.
     You can still call the function normally.
     ```python
     @PipePrefix
     def add_one(x: int) -> int:
         return x + 1
-    
+
     assert add_one | 1 == 2
     assert add_one(1) == 2
     ```
     """
-    _op: Callable[[Val], RetVal]
+
+    op: Callable[[Val], RetVal]
 
     def __init__(self, op: Callable[[Val], RetVal]) -> None:
-        self._op = op
-    
+        self.op = op
+
     def __or__(self, right: Val) -> RetVal:
-        return self._op(right)
-    
+        return self.op(right)
+
     def __call__(self, right: Val) -> RetVal:
-        return self._op(right)
-    
+        return self.op(right)
+
 
 class PipeInfix(Generic[Val, Val2, RetVal], object):
     """
     Class decorator used to create custom behavior that uses the `|` symbol.
     Wrap functions whose parameters you want to receive from the left and right of a `|` in the class.
     You can still call the function normally
     ```python
     @PipeInfix
     def add(x: int, y: int) -> int:
         return x + y
-    
+
     assert 1 | add | 1 == 2
     assert add(1, 1) == 2
     ```
     """
-    _op: Callable[[Val], Callable[[Val2], RetVal]]
+
+    op: Callable[[Val], Callable[[Val2], RetVal]]
 
     def __init__(self, op: Callable[[Val, Val2], RetVal]) -> None:
-        self._op = two(op)
-    
+        self.op = two(op)
+
     def __ror__(self, left: Val) -> PipePrefix[Val2, RetVal]:
-        return PipePrefix(self._op(left))
-    
+        return PipePrefix(self.op(left))
+
     def __call__(self, left: Val, right: Val2) -> RetVal:
-        return self._op(left)(right)
+        return self.op(left)(right)
 
 
 class PipeApply(Generic[Val], object):
-    '''
+    """
     Special infix operator that takes a value from the left and a function from the right. It calls
     the right function with the value from the left, which allows you to chain function calls together.
     Note though, that this can lose type hint support when using complex objects with nested types like
     the `res` functions.
     ### Example
     ```python
     p = PipeApply()
     add_three = lambda x: x + 3
     x: int = 0 |p| add_three |p| add_three
     y: int = p(x, add_three)
     assert y == 9
     ```
-    '''
+    """
+
     inner: Val
 
     def __init__(self, inner: Val) -> None:
         self.inner = inner
-    
+
     def __ror__(self, inner: RetVal) -> PipeApply[RetVal]:
         return PipeApply(inner)
-    
+
     def __or__(self, op: Callable[[Val], RetVal]) -> RetVal:
         return op(self.inner)
 
     def __call__(self, op: Callable[[Val], RetVal]) -> RetVal:
         return op(self.inner)
 
 
-Pipe: PipeApply[None] = PipeApply(None)
+P: PipeApply[None] = PipeApply(None)
+'''Special infix operator that pushes the value from the left into the right
+
+Example:
+    ```python
+    foo = 'foo' |P| bytes |P| str
+    ```
+'''
```

### Comparing `pythonix-1.0.5/pythonix/internals/mdeq.py` & `pythonix-1.0.6/pythonix/internals/mdeq.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 """
-### MDeq
-
 Functions used to create and perform operations safely on a singly typed mutable linked list.
-
 """
 from collections import deque
-from __future__ import annotations
 from typing import Iterable, Generic, TypeVar
-from pythonix.res import null_and_error_safe, safe, Ok
-from pythonix.curry import two, three
+from pythonix.internals.res import null_and_error_safe, safe, Ok
+from pythonix.internals.curry import two, three
 
 Val = TypeVar("Val")
 NewVal = TypeVar("NewVal")
 
 
 class MDeq(Generic[Val], object):
     """
@@ -51,14 +47,18 @@
     return MDeq(*vals)
 
 
 @two
 def push(element: Val, deq: MDeq[Val]) -> Ok[None]:
     """
     Pushes a new element `T` to the end of an `MDeq`.
+
+    Note:
+        This function is curried automatically. Apply function arguments
+        separated by brackets.
     """
     deq.inner.append(element)
     return Ok(None)
 
 
 @two
 def pushleft(element: Val, deq: MDeq[Val]) -> Ok[None]:
```

### Comparing `pythonix-1.0.5/pythonix/internals/op.py` & `pythonix-1.0.6/pythonix/internals/op.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Any,
     SupportsIndex,
     TypeVar,
     overload,
     MutableSequence,
     Sequence,
     MutableMapping,
-    Mapping
+    Mapping,
 )
 from functools import reduce
 from copy import deepcopy
 from pythonix.internals.res import null_and_error_safe, safe, Res
 from operator import setitem
 
 
@@ -105,23 +105,26 @@
     assert x.inner = 5
     assert z.inner is Nil
     ```
     """
 
     @null_and_error_safe(IndexError, KeyError)
     @overload
-    def inner(mapping: Mapping[Key, Val]) -> Val: ...
+    def inner(mapping: Mapping[Key, Val]) -> Val:
+        ...
 
     @null_and_error_safe(IndexError)
     @overload
-    def inner(sequence: Sequence[Val]) -> Val: ...
+    def inner(sequence: Sequence[Val]) -> Val:
+        ...
 
     @null_and_error_safe(IndexError)
     @overload
-    def inner(iterable: Iterable[Val]) -> Val: ...
+    def inner(iterable: Iterable[Val]) -> Val:
+        ...
 
     @null_and_error_safe(IndexError, KeyError)
     def inner(iterable: Mapping[Key, Val] | Sequence[Val] | Iterable[Val]) -> Val:
         return iterable[index]
 
     return inner
 
@@ -135,51 +138,62 @@
     def get_op(op: Callable[[Val], NewVal]) -> NewVal:
         return op(val)
 
     return get_op
 
 
 def assign(key: Key):
-    '''
+    """
     Assign a value to a given index or name on any mutable sequence (i.e. `list`), mutable mapping (i.e. `dict`)
     or any mutable object. Returns a copy of the updated object wrapped in a `Res` that reflects potential errors.
     Has full type support for each of the three different types.
     ```python
     # Assign to a dictionary
     start_d: dict[str, int] = {'foo': 1}
     end_d: dict[str, int | str] = assign('bar')('hello')(start_d)
     assert end_d['bar'] == 'hello'
 
     # Assign to a list
     start_l: list[int] = [1, 2, 3]
-    end_l: list[int | str] = assign(0)('first')(start_l) 
+    end_l: list[int | str] = assign(0)('first')(start_l)
     assert end_l[0] == 'first'
 
     # Assign to an object
     start_obj: object = object.__new__(object)
     end_obj: object = assign('foo')('bar')(start_obj)
     assert end_obj == 'bar'
     ```
-    '''
-    def get_val(val: NewVal):
+    """
 
+    def get_val(val: NewVal):
         @overload
-        def get_obj(sequence: MutableSequence[Val]) -> Res[MutableSequence[Val | NewVal], IndexError]: ...
+        def get_obj(
+            sequence: MutableSequence[Val],
+        ) -> Res[MutableSequence[Val | NewVal], IndexError]:
+            ...
 
         @overload
-        def get_obj(mapping: MutableMapping[Key, Val]) -> Res[MutableMapping[Key, Val | NewVal], IndexError | KeyError]: ...
+        def get_obj(
+            mapping: MutableMapping[Key, Val]
+        ) -> Res[MutableMapping[Key, Val | NewVal], IndexError | KeyError]:
+            ...
 
         @overload
-        def get_obj(obj: ObjT) -> Res[ObjT, AttributeError]: ...
+        def get_obj(obj: ObjT) -> Res[ObjT, AttributeError]:
+            ...
 
         @safe(IndexError, KeyError, AttributeError)
-        def get_obj(obj: MutableSequence[Val] | MutableMapping[Key, Val] | ObjT) -> MutableSequence[Val | NewVal] | MutableMapping[Key, Val | NewVal] | ObjT:
+        def get_obj(
+            obj: MutableSequence[Val] | MutableMapping[Key, Val] | ObjT
+        ) -> MutableSequence[Val | NewVal] | MutableMapping[Key, Val | NewVal] | ObjT:
             copy = deepcopy(obj)
-            if not isinstance(obj, MutableMapping) and not isinstance(obj, MutableSequence):
+            if not isinstance(obj, MutableMapping) and not isinstance(
+                obj, MutableSequence
+            ):
                 setattr(copy, key, val)
                 return copy
             setitem(copy, key, val)
             return copy
-            
+
         return get_obj
-    
+
     return get_val
```

### Comparing `pythonix-1.0.5/pythonix/internals/pair.py` & `pythonix-1.0.6/pythonix/internals/pair.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Module for handling key value pairs.
 """
 
-from typing import NamedTuple, Tuple, TypeVar, Generic, TypeAlias
-from pythonix.internals.types import Fn
-from pythonix.internals.curry import two
+from typing import NamedTuple, Tuple, TypeVar, Generic, TypeAlias, Callable
+from pythonix.curry import two
 
 
 Val = TypeVar("Val")
 NewVal = TypeVar("NewVal")
 KeyStr: TypeAlias = str
 
 
@@ -59,12 +58,12 @@
     """
     Retrieves the `key` of a provided `Pair`
     """
     return pair.key
 
 
 @two
-def map(using: Fn[Val, NewVal], pair: Pair[Val]) -> Pair[NewVal]:
+def map(using: Callable[[Val], NewVal], pair: Pair[Val]) -> Pair[NewVal]:
     """
     Change the inner value of a `Pair` with a function
     """
     return set_value(using(pair.value))(pair)
```

### Comparing `pythonix-1.0.5/pythonix/internals/pipe.py` & `pythonix-1.0.6/pythonix/internals/trail.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,132 +1,195 @@
 from __future__ import annotations
-from typing import Callable, Tuple, overload, TypeVar, Generic, NamedTuple
-from pythonix.internals import trail
-from pythonix.internals.trail import Trail, Log
+from functools import wraps
+from typing import NamedTuple, Tuple, Callable, ParamSpec, TypeVar, Generic, overload
+from datetime import datetime, timezone
 
+P = ParamSpec("P")
+LogType = TypeVar("LogType", bound="Log")
 Val = TypeVar("Val")
 NewVal = TypeVar("NewVal")
 
-class Bind(Generic[Val], NamedTuple):
+
+class Log(NamedTuple):
+    '''Immutable container for log messages.
+
+    Note:
+        Avoid creating this directly and use the `info`, `debug`, `warning`, `error`,
+        or `critical` functions instead.
+    '''
+    created_dt: datetime
+    '''datetime object for when the object was created'''
+    message: str
+    '''The log message'''
+
+    def __str__(self) -> str:
+        return f'{type(self).__name__}("{self.created_dt.strftime('%Y-%m-%dT%H:%M:%SZ')}", "{self.message}")'
+
+
+class Info(Log):
+    '''Log object at the INFO severity'''
+    ...
+
+
+class Debug(Log):
+    '''Log object at the DEBUG severity'''
+    ...
+
+
+class Warning(Log):
+    '''Log object at the WARNING severity'''
+    ...
+
+
+class Error(Log):
+    '''Log object at the ERROR severity'''
+    ...
+
+
+class Critical(Log):
+    '''Log object at the CRITICAL severity'''
+    ...
+
+
+def log(log_type: type[LogType]):
     """
-    Container that allows sequential functions calls to change its inner value and type.
-    Transformations can be done with with either the `run` or `__call__` methods.
-    #### Example
-    ```python
-    y: bool = (
-        Bind(5)
-        (lambda x: x + 6)   # -> 5 + 6 = 11
-        (lambda x: x == 11) # -> 11 == 11 == True
-    )
-    assert y == True
-    ```
+    Creates a function to create a Log
     """
 
+    def inner(message: str) -> LogType:
+        '''Create a Log with the message and type'''
+        return log_type(datetime.now(timezone.utc), message)
+
+    return inner
+
+
+debug = log(Debug)
+'''Severity: DEBUG'''
+info = log(Info)
+'''Severity: INFO'''
+warning = log(Warning)
+'''Severity: WARNING'''
+error = log(Error)
+'''Severity: ERROR'''
+critical = log(Critical)
+'''Severity: CRITICAL'''
+
+
+class Trail(Generic[Val], NamedTuple):
+    """Container type used to wrap a value with a series of Log type records
+    """
+
+    logs: Tuple[Log, ...]
     inner: Val
 
-    @property
-    def do(self) -> Do[Val]:
-        """
-        Converts the `Bind` pipe to a `Do` pipe, which changes the call to run the function but not change the
-        inner value of the container. Call `bind` to revert back to a `Bind` container, whose call will
-        change the inner value.
-        """
-        return Do(self.inner)
 
-    def run(self, using: Callable[[Val], NewVal]) -> Bind[NewVal]:
-        """
-        Performs a transformation on the contained value using the function provided.
-        Returns a new `Bind` object containing the new value. Works only with single arity
-        functions.
-        """
-        return Bind(using(self.inner))
+def new(*logs: LogType):
+    """
+    Create a new `Trail` object with the desired logs attached.
+    """
 
-    def __call__(self, using: Callable[[Val], NewVal]) -> Bind[NewVal]:
+    def get_inner(inner: Val) -> Trail[Val]:
         """
-        Performs a transformation on the contained value using the function provided.
-        Returns a new `Bind` object containing the new value. Works only with single arity
-        functions.
+        Attach the wrapped value to the `Trail`
         """
-        return self.run(using)
-    
+        return Trail(logs, inner)
+
+    return get_inner
 
-class Do(Generic[Val], NamedTuple):
+
+def append(*logs: LogType):
     """
-    Container used to run arbitrary functions on an `inner` value without changing its
-    state. Useful for logging, printing, or other inconsequential side effects.
-    #### Example
-    ```python
-    do: Do[int] = Do(5)
-    (
-        do
-        (print)             # Prints 5
-        (lambda x: x * 2)   # -> 10
-        (lambda x: x - 3)   # -> 2
-    )
-    assert do.inner == 5
-    ```
+    Append a new series of logs to a `Trail`
     """
 
-    inner: Val
+    def inner(trail: Trail[Val]) -> Trail[Val]:
+        return new(*(trail.logs + logs))(trail.inner)
 
-    def run(self, using: Callable[[Val], NewVal]) -> Do[Val]:
-        """
-        Performs the provided function on the `inner` value, but does not return its result.
-        Returns itself instead.
-        """
-        using(self.inner)
-        return self
+    return inner
 
-    @property
-    def bind(self) -> Bind[Val]:
-        """
-        Converts the `Do` pipe to a `Bind` pipe, whose call will change the inner value of the container.
-        Call `do` afterwards to revert to a `Do` pipe.
-        """
-        return Bind(self.inner)
 
-    def __call__(self, using: Callable[[Val], NewVal]) -> Do[Val]:
-        """
-        Performs the provided function on the `inner` value, but does not return its result.
-        Returns itself instead.
-        """
-        return self.run(using)
+def logs(trail: Trail[Val]) -> Tuple[LogType, ...]:
+    """
+    Convenience function to return the logs of a `Trail`
+    """
+    return trail.logs
 
 
-class Blaze(Generic[Val]):
+def trail(*logs: LogType):
     """
-    `Bind` container used to accumulate log messages during runtime without
-    side effects to the functions being ran. Runs functions with an optional
-    log message attached. If the function being called returns a `Trail` log container,
-    then it will attach its logs to the currently accumulated logs.
+    Decorator function used to wrap the output of a function with a default set of logs.
+    This also changes the output of the function to return a `Trail` of the type returned
+    by the function.
+    """
+
+    def inner(func: Callable[P, NewVal]):
+        @wraps(func)
+        def wrapper(*args: P.args, **kwargs: P.kwargs) -> Trail[NewVal]:
+            return new(*logs)(func(*args, **kwargs))
+
+        return wrapper
+
+    return inner
+
+
+class Blaze(Generic[Val]):
+    """Bind container used to accumulate log messages.
+    
+    Example:
+        ```python
+        blaze: Blaze[int] = Blaze(5, info('Starting'))
+        logs: tuple[Log, ...] = (
+            blaze
+            (lambda x: x + 1, info('Added one'))
+            (lambda x: x / 2, info('Divided by two'), debug('Val is now float'))
+            (lambda x: x,     info('Finished'))
+        ).logs
+        ```   
     """
 
     logs: Tuple[Log, ...] = tuple()
-    inner: trail.Trail[Val]
+    '''The sequence of accumulated logs'''
+    inner: Trail[Val]
+    '''The wrapped `Trail` value'''
 
     def __init__(self, inner: Val | Trail[Val], *logs: Log):
+        '''Initializes the Blaze object.
+        
+        Args:
+            inner (Val | Trail[Val]): The wrapped value. Can be anything or a `Trail` of anything.
+            *logs (Log): Optional series of logs to be accumulated to the Blaze 
+
+        '''
         match inner:
             case Trail():
                 self.inner = inner
                 self.logs = logs + inner.logs
             case _:
-                self.inner = trail.new()(inner)
+                self.inner = new()(inner)
                 self.logs = logs
 
     @overload
     def __call__(
         self, using: Callable[[Val], trail.Trail[NewVal]], *logs: Log
     ) -> Blaze[NewVal]:
         ...
 
     @overload
     def __call__(self, using: Callable[[Val], NewVal], *logs: Log) -> Blaze[NewVal]:
         ...
 
     def __call__(
-        self, using: Callable[[Val], trail.Trail[NewVal] | NewVal], *logs: Log
+        self, using: Callable[[Val], Trail[NewVal] | NewVal], *logs: Log
     ) -> Blaze[NewVal]:
-        """
-        Call the function and attach the logs from the function `Trail` and the optional logs
-        to the new instance of `Blaze` containing the result.
+        """Calls the provided function on the contained value while appending any attached logs
+
+        Args:
+            using ((Val) -> Trail[NewVal] | Newval): Function that takes the contained value
+            and returns a new one wrapped in `Trail` or not.
+            *logs (Log): A series of any Log subclassed objects to be attached with the function call
+        
+        Returns:
+            _ (Blaze[NewVal]): A new instance of a `Blaze` with the updated logs from the `using` function
+            and the `*logs` arguments appended.
+        
         """
         return Blaze(using(self.inner.inner), *(self.logs + logs))
```

### Comparing `pythonix-1.0.5/pythonix/internals/req.py` & `pythonix-1.0.6/pythonix/internals/req.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from typing import NamedTuple, ParamSpec, Callable, Tuple, TypeVar
-from pythonix.op import mapx
-from pythonix.pipe import Bind
-from pythonix.res import Res
-import pythonix.pair as pair
+from pythonix.internals.op import mapx
+from pythonix.internals.pipe import Bind
+from pythonix.internals.res import Res, safe, map as rmap
+from pythonix.internals.pair import Pair, Pairs, map
 from functools import singledispatch
 from requests import (
     get as _get,
     post as _post,
     put as _put,
     delete as _delete,
     Response as OGResponse,
     HTTPError,
 )
-from pythonix.internals.pair import Pair, Pairs
-from pythonix.internals.pipe import Bind
-from pythonix import res
 
 P = ParamSpec("P")
 
 
 class Response(NamedTuple):
     """
     Parsed response from an HTTP request.
@@ -32,15 +29,15 @@
 def parse_response(response: OGResponse) -> Response:
     """
     Converts a response from a `requests` library HTTP request to a `pythonix` response
     """
     return Response(response.url, response.content, response.status_code)
 
 
-@res.safe(HTTPError)
+@safe(HTTPError)
 def check_status(response: OGResponse) -> OGResponse:
     """
     Captures an `HTTPError` from a `requests` HTTP response in `Result`
     """
     response.raise_for_status()
     return response
 
@@ -86,28 +83,30 @@
 class Delete(Request):
     """
     An HTTP request set as a `DELETE`
     """
 
     method: Callable[P, Response] = _delete
 
-R = TypeVar('R', bound='Request')
+
+R = TypeVar("R", bound="Request")
+
 
 @singledispatch
 def to_bytes(value: int) -> bytes:
     return bytes(value)
 
 
 @to_bytes.register(str)
 def _(value: str) -> bytes:
     return bytes(value, "utf-8")
 
 
 def set_value_to_bytes(keyvalue: Pair[str | int]) -> Pair[bytes]:
-    Bind(keyvalue)(pair.map(to_bytes)).inner
+    Bind(keyvalue)(map(to_bytes)).inner
 
 
 def get(url: str):
     """
     Set the URL for the request type
     """
 
@@ -293,10 +292,8 @@
 
 def send(request: RequestType) -> Res[Response, HTTPError]:
     """
     Sends the provided `Request` and then parses its response, capturing any errors that occur.
     """
     return Bind(request)(body)(
         lambda body: {"url": request.url} | {k: v for k, v in body}
-    )(lambda kwargs: request.method(**kwargs))(check_status)(
-        res.map(parse_response)
-    ).inner
+    )(lambda kwargs: request.method(**kwargs))(check_status)(rmap(parse_response)).inner
```

### Comparing `pythonix-1.0.5/pythonix/internals/res.py` & `pythonix-1.0.6/pythonix/internals/res.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 from __future__ import annotations
-from collections.abc import Iterator
-from typing import TypeVar, Generic, NamedTuple, cast, ParamSpec, Callable, TypeAlias
-from pythonix.internals.types import Fn
+from functools import wraps
+from typing import (
+    TypeVar,
+    Generic,
+    NamedTuple,
+    cast,
+    ParamSpec,
+    Callable,
+    TypeAlias,
+    Iterator,
+)
 
 P = ParamSpec("P")
 
 UnwrapErr = ValueError("Attempted to retrieve an Err from an Ok")
 Val = TypeVar("Val")
 NewVal = TypeVar("NewVal")
 ErrVal = TypeVar("ErrVal", bound="Exception")
@@ -36,15 +44,15 @@
     ```
     """
 
     inner: Val
 
     def __iter__(self) -> Iterator[Val | None]:
         return iter((self.inner, None))
-    
+
 
 class Err(Generic[ErrVal], NamedTuple):
     """
     Represents a successful outcome of a function that could have failed.
     Useful for pattern matching on a function that returns `Ok[T] | Err[E]`
     ### Example
     ```python
@@ -131,30 +139,32 @@
     match res:
         case Ok():
             return False
         case Err():
             return True
 
 
-def is_ok_and(predicate: Fn[Val, bool]) -> Callable[[Res[Val, ErrVal]], bool]:
+def is_ok_and(predicate: Callable[[Val], bool]) -> Callable[[Res[Val, ErrVal]], bool]:
     """
     Return `True` if the `Res` is `Ok` and the `predicate` evaluates to `True`.
     """
 
     def inner(res: Res[Val, ErrVal]) -> bool:
         match res:
             case Ok(t):
                 return predicate(t)
             case _:
                 return False
 
     return inner
 
 
-def is_err_and(predicate: Fn[ErrVal, bool]) -> Callable[[Res[Val, ErrVal]], bool]:
+def is_err_and(
+    predicate: Callable[[ErrVal], bool]
+) -> Callable[[Res[Val, ErrVal]], bool]:
     """
     Return `True` if the `Res` is `Err` and the `predicate` evaluates to `True`
     """
 
     def inner(res: Res[Val, ErrVal]) -> bool:
         match res:
             case Err(e):
@@ -172,30 +182,30 @@
     match result:
         case Ok(value):
             return cast(Val, value)
         case Err(e):
             raise e
 
 
-def unwrap_or(default: Val) -> Fn[Res[Val, ErrVal], Val]:
+def unwrap_or(default: Val) -> Callable[[Res[Val, ErrVal]], Val]:
     """
     Return the `Ok` value if `Ok`, else return the default
     """
 
     def inner(res: Res[Val, ErrVal]) -> Val:
         match res:
             case Ok(val):
                 return val
             case _:
                 return default
 
     return inner
 
 
-def unwrap_or_else(on_err: Callable[[], Val]) -> Fn[Res[Val, ErrVal], Val]:
+def unwrap_or_else(on_err: Callable[[], Val]) -> Callable[[Res[Val, ErrVal]], Val]:
     """
     Return the `Ok` value if `Ok`, else run the `on_err` function that returns the same type.
     """
 
     def inner(res: Res[Val, ErrVal]) -> Val:
         match res:
             case Ok(val):
@@ -213,15 +223,17 @@
     match result:
         case Ok():
             raise UnwrapErr
         case Err(e):
             return e
 
 
-def map(using: Fn[Val, NewVal]) -> Fn[Res[Val, ErrVal], Res[NewVal, ErrVal]]:
+def map(
+    using: Callable[[Val], NewVal]
+) -> Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]:
     """
     Run the function on the `Ok` if `Ok`, else return the current `Err`
     """
 
     def inner(res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal]:
         match res:
             case Ok(t):
@@ -229,15 +241,15 @@
             case _:
                 return cast(Res[NewVal, ErrVal], res)
 
     return inner
 
 
 def map_or(
-    using: Fn[Val, NewVal]
+    using: Callable[[Val], NewVal]
 ) -> Callable[[NewVal], Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]]:
     """
     Runs the function on the `Ok` or return the `default` if `Err`
     """
 
     def get_default(
         default: NewVal,
@@ -251,15 +263,15 @@
 
         return inner
 
     return get_default
 
 
 def map_err(
-    using: Fn[ErrVal, NewErrVal]
+    using: Callable[[ErrVal], NewErrVal]
 ) -> Callable[[Res[Val, ErrVal]], Res[Val, NewErrVal]]:
     """
     Runs the function on the `ErrVal` if in `Err` or returns the current `Ok`
     """
 
     def inner(res: Res[Val, ErrVal]) -> Res[Val, ErrVal]:
         match res:
@@ -293,15 +305,15 @@
 
         return inner
 
     return get_catch
 
 
 def map_or_else(
-    using: Fn[Val, NewVal]
+    using: Callable[[Val], NewVal]
 ) -> Callable[
     [Callable[[], NewVal]], Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]
 ]:
     """
     Runs the provided function if `Ok`, or runs the default function if `Err`
     """
 
@@ -317,16 +329,16 @@
 
         return inner
 
     return get_default
 
 
 def and_then(
-    using: Fn[Val, Res[NewVal, ErrVal]]
-) -> Fn[Res[Val, ErrVal], Res[NewVal, ErrVal]]:
+    using: Callable[[Val], Res[NewVal, ErrVal]]
+) -> Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]:
     """
     Runs the function that returns a new `Res` if `Ok`, else return the current `Err`
     """
 
     def inner(res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal]:
         match res:
             case Ok(t):
@@ -334,39 +346,39 @@
             case _:
                 return cast(Res[NewVal, ErrVal], res)
 
     return inner
 
 
 def or_else(
-    using: Fn[ErrVal, Res[NewVal, NewErrVal]]
-) -> Fn[Res[Val, ErrVal], Res[Val, NewErrVal]]:
+    using: Callable[[ErrVal], Res[NewVal, NewErrVal]]
+) -> Callable[[Res[Val, ErrVal]], Res[Val, NewErrVal]]:
     """
     Runs the function that returns a new `Res` if in `Err`, else it will return the current `Ok`
     """
 
     def inner(res: Res[Val, ErrVal]) -> Res[Val, NewErrVal]:
         match res:
             case Err(e):
                 return cast(Res[Val, NewErrVal], using(e))
             case _:
                 return cast(Res[Val, NewErrVal], res)
 
     return inner
 
 
-def and_then_catch(using: Fn[Val, NewVal]):
+def and_then_catch(using: Callable[[Val], NewVal]):
     """
     Runs the function that could fail, catching the specified error and returning a new `Res`.
     Will only be ran if `Ok`, else it will return its current `Err`
     """
 
     def get_catch(
         catch: type[NewErrVal],
-    ) -> Fn[Res[Val, ErrVal], Res[NewVal, ErrVal | NewErrVal]]:
+    ) -> Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal | NewErrVal]]:
         def inner(res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal | NewErrVal]:
             match res:
                 case Ok(t):
                     try:
                         return cast(
                             Res[NewVal, ErrVal | NewErrVal], ok(ErrVal)(using(t))
                         )
@@ -376,15 +388,15 @@
                     return cast(Res[NewVal, ErrVal | NewErrVal], err(NewVal)(f))
 
         return inner
 
     return get_catch
 
 
-def map_err(using: Fn[ErrVal, NewErrVal]):
+def map_err(using: Callable[[ErrVal], NewErrVal]):
     """
     Changes the internal `Err` using the function if in an `Err` state. Otherwise it returns
     the `Ok`
     """
 
     def inner(res: Res[Val, ErrVal]) -> Res[Val, NewErrVal]:
         match res:
@@ -409,15 +421,17 @@
                 return new_res
             case Err():
                 return cast(Res[NewVal, ErrVal], old_res)
 
     return inner
 
 
-def or_res(new_res: Res[Val, NewErrVal]) -> Callable[[Res[Val, ErrVal]], Res[Val, NewErrVal]]:
+def or_res(
+    new_res: Res[Val, NewErrVal]
+) -> Callable[[Res[Val, ErrVal]], Res[Val, NewErrVal]]:
     """
     Returns the provided result if the current one is an `Err`
     """
 
     def inner(old_res: Res[Val, ErrVal]) -> Res[Val, NewErrVal]:
         match old_res:
             case Ok():
@@ -446,86 +460,89 @@
     type hints for the `Res`.
     #### Example
     ```python
     # The two functions are equivalent
     @safe(ValueError, TypeError)
     def func_1():
         return 'success'
-    
+
     def func_2():
         try:
             return ok('success')(ValueError | TypeError)
         except (ValueError, TypeError) as e:
             return err(str)(e)
     ```
     """
-    def inner(using: Callable[P, NewVal]) -> Callable[P, Res[NewVal, ErrVal]]:
 
+    def inner(using: Callable[P, NewVal]) -> Callable[P, Res[NewVal, ErrVal]]:
+        @wraps(using)
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> Res[NewVal, ErrVal]:
             try:
-                return cast(Res[NewVal, ErrVal],ok(ErrVal)(using(*args, **kwargs)))
+                return cast(Res[NewVal, ErrVal], ok(ErrVal)(using(*args, **kwargs)))
             except err_type as e:
                 return cast(Res[NewVal, ErrVal], err(NewVal)(e))
-            
+
         return wrapper
-    
+
     return inner
 
 
 def null_safe(using: Callable[P, NewVal | None]):
     """
     Wraps the output of the function in a `Res[T, Nil]` object.
     """
 
+    @wraps(using)
     def inner(*args: P.args, **kwargs: P.kwargs) -> Res[NewVal, Nil]:
         return some(using(*args, **kwargs))
 
     return inner
 
 
 def null_and_error_safe(*err_types: type[ErrVal]):
     """
     Wraps the output in the `some` function and consumes the error if it is thrown, replacing it with `Nil`
     """
 
     def inner(using: Callable[P, Val]):
+        @wraps(using)
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> Res[Val, Nil]:
             try:
                 return some(using(*args, **kwargs))
             except err_types as e:
                 return map_err(lambda f: Nil(str(f)))(err(Val)(e))
 
         return wrapper
 
     return inner
 
 
 def combine_errors(to: NewErrVal, inherit_message: bool = False):
-    '''
+    """
     Decorator function used to convert function that return a `Res[Val, ErrVal]` to `Res[Val, NewErrVal]`, consuming
     the references to the original captured errors. Useful for when a function could throw a lot of errors and you
     need to convert them into one error instead.
     #### Example
     ```python
     @combine_errors(CustomError)
     @safe(TypeError, ValueError)
     def do_thing(s: str) -> str:
         if not isinstance(s, str):
             raise TypeError('Must be str')
         return s
     done: Res[str, CustomError] = do_thing('ok')
-    ``` 
-    '''
-    
+    ```
+    """
     def inner(using: Callable[P, Ok[Val] | Err[ErrVal]]):
-
+        @wraps(using)
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> Res[Val, NewErrVal]:
-            
-            return map_err(lambda e: to.__class__(str(e)) if inherit_message else to)(using(*args, **kwargs)) 
-        
+            return map_err(lambda e: to.__class__(str(e)) if inherit_message else to)(
+                using(*args, **kwargs)
+            )
+
         return wrapper
 
     return inner
 
 
 q = unwrap
 qe = unwrap_err
```

### Comparing `pythonix-1.0.5/pythonix/internals/trail.py` & `pythonix-1.0.6/pythonix/internals/tup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,113 +1,114 @@
-from typing import NamedTuple, Tuple, Callable, ParamSpec, TypeVar, Generic
-from datetime import datetime, timezone
+"""
+Module for handling tuples without risk of panics
+"""
+from typing import Tuple, TypeVar
+from pythonix.internals.op import item
+from pythonix.internals.res import safe, null_and_error_safe
+from pythonix.internals.curry import two, three
+from enum import Enum
 
-P = ParamSpec("P")
-LogType = TypeVar("LogType", bound="Log")
 Val = TypeVar("Val")
 NewVal = TypeVar("NewVal")
+type IndexInt = int
 
 
-class Log(NamedTuple):
-    datetime: datetime
-    message: str
+class Side(Enum):
+    LEFT: str = "LEFT"
+    RIGHT: str = "RIGHT"
 
-    def __str__(self) -> str:
-        return f'{type(self).__name__}("{self.datetime.strftime('%Y-%m-%dT%H:%M:%SZ')}", "{self.message}")'
 
-
-class Info(Log):
-    ...
-
-
-class Debug(Log):
-    ...
-
-
-class Warning(Log):
-    ...
-
-
-class Error(Log):
-    ...
-
-
-class Critical(Log):
-    ...
+def new(*elements: Val) -> Tuple[Val, ...]:
+    """
+    Convenience function to create a new series of data of a given type
+    """
+    return elements
 
 
-def log(log_type: type[LogType]):
+def push(side: Side = Side.RIGHT):
     """
-    Creates a new `Log` instance with the specified message attached
+    Push an element to either side of a `Tuple`
     """
 
-    def inner(message: str) -> LogType:
-        """
-        Attach a message to the log
-        """
-        return log_type(datetime.now(timezone.utc), message)
+    def get_element(element: NewVal):
+        def inner(tuples: Tuple[Val, ...]) -> Tuple[Val | NewVal, ...]:
+            match side:
+                case Side.LEFT:
+                    return (element,) + tuples
+                case Side.RIGHT:
+                    return tuples + (element,)
 
-    return inner
+        return inner
 
+    return get_element
 
-debug = log(Debug)
-info = log(Info)
-warning = log(Warning)
-error = log(Error)
-critical = log(Critical)
 
-
-class Trail(Generic[Val], NamedTuple):
+@two
+def get(index: IndexInt, tuples: Tuple[Val, ...]):
     """
-    Container type used to wrap a value with a series of `Log` type records
+    Retrieve an element from a `Tuple` at the provided index
     """
-
-    logs: Tuple[Log, ...]
-    inner: Val
+    return item(index)(tuples)
 
 
-def new(*logs: LogType):
+def extend(side: Side = Side.RIGHT):
     """
-    Create a new `Trail` object with the desired logs attached.
+    Combine two tuple series together
     """
 
-    def get_inner(inner: Val) -> Trail[Val]:
-        """
-        Attach the wrapped value to the `Trail`
-        """
-        return Trail(logs, inner)
+    def get_left(new: Tuple[Val, ...]):
+        def get_right(old: Tuple[NewVal, ...]) -> Tuple[Val | NewVal, ...]:
+            match side:
+                case Side.LEFT:
+                    return new + old
+                case Side.RIGHT:
+                    return old + new
 
-    return get_inner
+        return get_right
 
+    return get_left
 
-def append(*logs: LogType):
+
+@two
+@null_and_error_safe(ValueError)
+def index(element: Val, tuples: Tuple[Val, ...]) -> int:
     """
-    Append a new series of logs to a `Trail`
+    Find the index of an element in `Tuple` if it exists
     """
+    return tuples.index(element)
 
-    def inner(trail: Trail[Val]) -> Trail[Val]:
-        return new(*(trail.logs + logs))(trail.inner)
 
-    return inner
+@two
+def count_occurrences(value: Val, tuples: Tuple[Val, ...]) -> int:
+    """
+    Count the occurrences of the provided value in a `Tuple`
+    """
+    return tuples.count(value)
 
 
-def logs(trail: Trail[Val]) -> Tuple[LogType, ...]:
+@three
+def insert(
+    index: IndexInt, insert: NewVal, tuples: Tuple[Val, ...]
+) -> Tuple[Val | NewVal, ...]:
     """
-    Convenience function to return the logs of a `Trail`
+    Recreate the `Tuple` with the provided element at the index
     """
-    return trail.logs
+    return tuples[:index] + (insert,) + tuples[index:]
 
 
-def trail(*logs: LogType):
+@two
+@safe(IndexError)
+def remove(index: IndexInt, tuples: Tuple[Val, ...]) -> Tuple[Val, ...]:
     """
-    Decorator function used to wrap the output of a function with a default set of logs.
-    This also changes the output of the function to return a `Trail` of the type returned
-    by the function.
+    Recreate the `Tuple` without the element at the provided index
     """
+    if index > (length := len(tuples)):
+        raise IndexError(f"Incompatible index {index} is greater than length {length}")
+    return tuples[:index] + tuples[index + 1 :]
 
-    def inner(func: Callable[P, NewVal]):
-        def wrapper(*args: P.args, **kwargs: P.kwargs) -> Trail[NewVal]:
-            return new(*logs)(func(*args, **kwargs))
-
-        return wrapper
 
-    return inner
+push_left = push(Side.LEFT)
+push_right = push(Side.RIGHT)
+extend_left = extend(Side.LEFT)
+extend_right = extend(Side.RIGHT)
+last = get(-1)
+first = get(0)
```

### Comparing `pythonix-1.0.5/pythonix/pipe.py` & `pythonix-1.0.6/pythonix/pipe.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.5/pythonix/prelude.py` & `pythonix-1.0.6/pythonix/prelude.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''
+"""
 ## Submodules
 A mass import of all the pythonix submodules including
 - `pipe`: Wrapper types for piping and transforming sequentially
 - `res`: Wrapper types and functions for handling errors
 - `trail`: Wrapper types for managing and concatenating logs to objects
 - `op`: Functions for mapping over and transforming data structures and objects safely
 - `req`: Functions and wrapper types for creating, sending, and handling HTTP requests
@@ -28,25 +28,25 @@
 - `Fn[T, U]`: Shorthand for `Callable[[T], U]`. Denotes a function that takes a single argument and returns an output
 - `FnOnce[U]`: Shorthand for `Callable[[], U]`, meaning a function that takes no input but provides a single output.
 
 ## Included Functions
 And the following utility functions
 - `q`: Unwraps the value of an `Ok` or panics if `Err`. Shorthand for `res.unwrap`
 - `qe`: Unwraps the err value of an `Err` or panics if `Ok`. Shorthand for `res.unwrap_err`
-'''
+"""
 import pythonix.pipe as pipe
 import pythonix.res as res
 import pythonix.trail as trail
 import pythonix.op as op
-from pythonix.internals.types import Fn, FnOnce
 import pythonix.req as req
 import pythonix.curry as curry
 import pythonix.tup as tup
 import pythonix.dict_utils as dict_utils
 import pythonix.grammar as grammar
 import pythonix.prove as prove
-from pythonix.grammar import Pipe
-from pythonix.grammar import Pipe as P
+from pythonix.grammar import P
 
 from pythonix.res import Ok, Err, Nil, q, Res, qe
 from pythonix.pipe import Bind, Do
 from pythonix.pipe import Bind as B, Do as D
+
+from pythonix.mdeq import pushleft
```

### Comparing `pythonix-1.0.5/pythonix/req.py` & `pythonix-1.0.6/pythonix/req.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.5/pythonix/res.py` & `pythonix-1.0.6/pythonix/res.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-'''
+"""
 Functions and types for handling expected and unexpected outcomes, like Exceptions and errors.
 Works well with `Bind` and `Do` to capture, handle, and unwrap the results of operations as values.
 
 The basic flow is as follows:
 1. Capture Errors
 2. Handle Errors
 3. Retrieve Desired Values
@@ -187,16 +187,15 @@
                 case _:
                     error('Unidentified error')
                     raise _
         case _:
             error(f'Unexpected value was found {_}')
             raise Exception('An unidentified value was returned')
 ```
-
-'''
+"""
 from pythonix.internals.res import (
     and_res,
     and_then,
     and_then_catch,
     err,
     flatten,
     is_err,
@@ -221,9 +220,9 @@
     unwrap_err,
     unwrap_or,
     unwrap_or_else,
     Ok,
     Err,
     null_and_error_safe,
     q,
-    qe
+    qe,
 )
```

### Comparing `pythonix-1.0.5/PKG-INFO` & `pythonix-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythonix
-Version: 1.0.5
+Version: 1.0.6
 Summary: Rust and Gleam like functional programming in Python, complete with Results, pipes, and currying
 Author: jhok2013
 Author-email: jhok2013@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

