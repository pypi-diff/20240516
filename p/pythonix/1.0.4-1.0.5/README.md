# Comparing `tmp/pythonix-1.0.4.tar.gz` & `tmp/pythonix-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonix-1.0.4.tar", max compression
+gzip compressed data, was "pythonix-1.0.5.tar", max compression
```

## Comparing `pythonix-1.0.4.tar` & `pythonix-1.0.5.tar`

### file list

```diff
@@ -1,26 +1,30 @@
--rw-r--r--   0        0        0     3027 2024-05-08 15:21:18.899631 pythonix-1.0.4/README.md
--rw-r--r--   0        0        0      380 2024-05-12 03:55:29.569631 pythonix-1.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-13 01:39:00.350000 pythonix-1.0.4/pythonix/__init__.py
--rw-r--r--   0        0        0       85 2024-05-09 16:54:03.549631 pythonix-1.0.4/pythonix/curry.py
--rw-r--r--   0        0        0      141 2024-05-12 03:53:46.089631 pythonix-1.0.4/pythonix/dict_utils.py
--rw-r--r--   0        0        0     8262 2024-05-12 01:58:37.609631 pythonix-1.0.4/pythonix/internals/curry.py
--rw-r--r--   0        0        0     3777 2024-05-12 03:53:46.169631 pythonix-1.0.4/pythonix/internals/dict_utils.py
--rw-r--r--   0        0        0     3914 2024-05-09 16:54:03.669631 pythonix-1.0.4/pythonix/internals/mdeq.py
--rw-r--r--   0        0        0     4588 2024-05-12 03:53:46.229631 pythonix-1.0.4/pythonix/internals/op.py
--rw-r--r--   0        0        0     1381 2024-05-09 16:54:03.599631 pythonix-1.0.4/pythonix/internals/pair.py
--rw-r--r--   0        0        0     4510 2024-05-12 03:53:46.269631 pythonix-1.0.4/pythonix/internals/pipe.py
--rw-r--r--   0        0        0     7290 2024-05-11 22:43:50.979631 pythonix-1.0.4/pythonix/internals/req.py
--rw-r--r--   0        0        0    13960 2024-05-12 03:53:46.519631 pythonix-1.0.4/pythonix/internals/res.py
--rw-r--r--   0        0        0     2257 2024-05-12 03:54:55.059631 pythonix-1.0.4/pythonix/internals/trail.py
--rw-r--r--   0        0        0     2696 2024-05-09 20:50:48.239631 pythonix-1.0.4/pythonix/internals/tup.py
--rw-r--r--   0        0        0      178 2024-05-09 16:54:03.619631 pythonix-1.0.4/pythonix/internals/types.py
--rw-r--r--   0        0        0      207 2024-05-09 16:54:03.619631 pythonix-1.0.4/pythonix/mdeq.py
--rw-r--r--   0        0        0      154 2024-05-12 03:53:46.089631 pythonix-1.0.4/pythonix/op.py
--rw-r--r--   0        0        0      135 2024-05-09 16:54:03.619631 pythonix-1.0.4/pythonix/pair.py
--rw-r--r--   0        0        0      886 2024-04-18 16:47:23.234118 pythonix-1.0.4/pythonix/pipe.py
--rw-r--r--   0        0        0      349 2024-05-11 15:45:04.599631 pythonix-1.0.4/pythonix/prelude.py
--rw-r--r--   0        0        0      645 2024-05-09 16:54:03.639631 pythonix-1.0.4/pythonix/req.py
--rw-r--r--   0        0        0      467 2024-05-12 03:53:46.119631 pythonix-1.0.4/pythonix/res.py
--rw-r--r--   0        0        0      183 2024-04-25 18:08:10.144118 pythonix-1.0.4/pythonix/trail.py
--rw-r--r--   0        0        0      234 2024-05-12 03:53:46.109631 pythonix-1.0.4/pythonix/tup.py
--rw-r--r--   0        0        0     3498 1970-01-01 00:00:00.000000 pythonix-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3027 2024-05-08 15:21:18.899631 pythonix-1.0.5/README.md
+-rw-r--r--   0        0        0      409 2024-05-16 15:03:57.509631 pythonix-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-13 01:39:00.350000 pythonix-1.0.5/pythonix/__init__.py
+-rw-r--r--   0        0        0      465 2024-05-15 16:52:32.679631 pythonix-1.0.5/pythonix/curry.py
+-rw-r--r--   0        0        0      387 2024-05-15 18:24:17.999631 pythonix-1.0.5/pythonix/dict_utils.py
+-rw-r--r--   0        0        0      930 2024-05-15 19:41:41.229631 pythonix-1.0.5/pythonix/grammar.py
+-rw-r--r--   0        0        0     8262 2024-05-15 16:47:08.319631 pythonix-1.0.5/pythonix/internals/curry.py
+-rw-r--r--   0        0        0     3949 2024-05-15 03:15:10.619631 pythonix-1.0.5/pythonix/internals/dict_utils.py
+-rw-r--r--   0        0        0     3537 2024-05-15 19:41:41.979631 pythonix-1.0.5/pythonix/internals/grammar.py
+-rw-r--r--   0        0        0     3914 2024-05-15 15:58:00.019631 pythonix-1.0.5/pythonix/internals/mdeq.py
+-rw-r--r--   0        0        0     5233 2024-05-15 15:47:55.849631 pythonix-1.0.5/pythonix/internals/op.py
+-rw-r--r--   0        0        0     1381 2024-05-09 16:54:03.599631 pythonix-1.0.5/pythonix/internals/pair.py
+-rw-r--r--   0        0        0     4237 2024-05-15 18:26:22.289631 pythonix-1.0.5/pythonix/internals/pipe.py
+-rw-r--r--   0        0        0     1410 2024-05-15 16:49:20.859631 pythonix-1.0.5/pythonix/internals/prove.py
+-rw-r--r--   0        0        0     7268 2024-05-13 00:29:18.849631 pythonix-1.0.5/pythonix/internals/req.py
+-rw-r--r--   0        0        0    14088 2024-05-15 16:45:49.679631 pythonix-1.0.5/pythonix/internals/res.py
+-rw-r--r--   0        0        0     2253 2024-05-12 19:34:25.729631 pythonix-1.0.5/pythonix/internals/trail.py
+-rw-r--r--   0        0        0     2696 2024-05-09 20:50:48.239631 pythonix-1.0.5/pythonix/internals/tup.py
+-rw-r--r--   0        0        0      178 2024-05-09 16:54:03.619631 pythonix-1.0.5/pythonix/internals/types.py
+-rw-r--r--   0        0        0      420 2024-05-15 18:49:30.279631 pythonix-1.0.5/pythonix/mdeq.py
+-rw-r--r--   0        0        0      283 2024-05-15 18:51:21.519631 pythonix-1.0.5/pythonix/op.py
+-rw-r--r--   0        0        0      265 2024-05-15 18:52:34.069631 pythonix-1.0.5/pythonix/pair.py
+-rw-r--r--   0        0        0      886 2024-05-14 14:13:15.569631 pythonix-1.0.5/pythonix/pipe.py
+-rw-r--r--   0        0        0     2619 2024-05-16 15:03:06.689631 pythonix-1.0.5/pythonix/prelude.py
+-rw-r--r--   0        0        0      233 2024-05-15 19:53:17.099631 pythonix-1.0.5/pythonix/prove.py
+-rw-r--r--   0        0        0      645 2024-05-09 16:54:03.639631 pythonix-1.0.5/pythonix/req.py
+-rw-r--r--   0        0        0     6424 2024-05-15 21:16:57.849631 pythonix-1.0.5/pythonix/res.py
+-rw-r--r--   0        0        0      321 2024-05-16 14:59:03.309631 pythonix-1.0.5/pythonix/trail.py
+-rw-r--r--   0        0        0      358 2024-05-16 14:59:49.929631 pythonix-1.0.5/pythonix/tup.py
+-rw-r--r--   0        0        0     3649 1970-01-01 00:00:00.000000 pythonix-1.0.5/PKG-INFO
```

### Comparing `pythonix-1.0.4/README.md` & `pythonix-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.4/pythonix/internals/curry.py` & `pythonix-1.0.5/pythonix/internals/curry.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.4/pythonix/internals/dict_utils.py` & `pythonix-1.0.5/pythonix/internals/dict_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from typing import TypeVar, Dict, Callable
-from pythonix.res import Ok, Err, Nil
+from typing import TypeVar, Dict, Callable, Mapping
 from pythonix.op import item
 
 Val = TypeVar("Val")
 NewVal = TypeVar("NewVal")
 Key = TypeVar("Key", str, int, float, tuple)
 NewKey = TypeVar("NewKey", str, int, float, tuple)
 
@@ -122,7 +121,17 @@
     ) -> Callable[[Dict[Key, Val]], Dict[Key | NewKey, Val | NewVal]]:
         def get_dict(dict_obj: Dict[Key, Val]) -> Dict[Key | NewKey, Val | NewVal]:
             return merge(dict_obj)({key: val})
 
         return get_dict
 
     return get_val
+
+
+def get(key: Key):
+    '''
+    Retrieves a value from a mapping, returning `Nil` on error
+    '''
+    def get_data(mapping: Mapping[Key, Val]):
+        return item(key)(mapping)
+
+    return get_data
```

### Comparing `pythonix-1.0.4/pythonix/internals/mdeq.py` & `pythonix-1.0.5/pythonix/internals/mdeq.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.4/pythonix/internals/pair.py` & `pythonix-1.0.5/pythonix/internals/pair.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.4/pythonix/internals/pipe.py` & `pythonix-1.0.5/pythonix/internals/pipe.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,38 @@
 from __future__ import annotations
-from typing import Callable, Protocol, Tuple, overload, TypeVar, Generic
+from typing import Callable, Tuple, overload, TypeVar, Generic, NamedTuple
 from pythonix.internals import trail
 from pythonix.internals.trail import Trail, Log
 
 Val = TypeVar("Val")
 NewVal = TypeVar("NewVal")
 
-
-class HasInner(Generic[Val], Protocol):
-    inner: Val
-
-
-class Bind(Generic[Val]):
+class Bind(Generic[Val], NamedTuple):
     """
     Container that allows sequential functions calls to change its inner value and type.
     Transformations can be done with with either the `run` or `__call__` methods.
     #### Example
     ```python
     y: bool = (
         Bind(5)
         (lambda x: x + 6)   # -> 5 + 6 = 11
         (lambda x: x == 11) # -> 11 == 11 == True
     )
     assert y == True
     ```
-    #### Methods
-    - `run(Fn(T) -> U) -> Bind<U>`: Runs the provided function and returns a new `Bind` object containing
-    its result
-    - `__call__(Fn(T) -> U) -> Bind<U>`: Identical to the `run` function.
     """
 
     inner: Val
 
-    def __init__(self, inner: Val) -> None:
-        self.inner = inner
-
     @property
     def do(self) -> Do[Val]:
         """
-        Converts the `Bind` pipe to a `Do` pipe
+        Converts the `Bind` pipe to a `Do` pipe, which changes the call to run the function but not change the
+        inner value of the container. Call `bind` to revert back to a `Bind` container, whose call will
+        change the inner value.
         """
         return Do(self.inner)
 
     def run(self, using: Callable[[Val], NewVal]) -> Bind[NewVal]:
         """
         Performs a transformation on the contained value using the function provided.
         Returns a new `Bind` object containing the new value. Works only with single arity
@@ -52,54 +42,49 @@
 
     def __call__(self, using: Callable[[Val], NewVal]) -> Bind[NewVal]:
         """
         Performs a transformation on the contained value using the function provided.
         Returns a new `Bind` object containing the new value. Works only with single arity
         functions.
         """
-        return Bind(using(self.inner))
+        return self.run(using)
+    
 
-
-class Do(Generic[Val]):
+class Do(Generic[Val], NamedTuple):
     """
     Container used to run arbitrary functions on an `inner` value without changing its
     state. Useful for logging, printing, or other inconsequential side effects.
     #### Example
     ```python
     do: Do[int] = Do(5)
     (
         do
         (print)             # Prints 5
         (lambda x: x * 2)   # -> 10
         (lambda x: x - 3)   # -> 2
     )
     assert do.inner == 5
     ```
-    #### Methods
-    - `run(Fn(T) -> U) -> Do[T]`: Runs the provided function on the contained value and returns itself.
-    - `__call__(Fn(T) -> U) -> Do[T]`: Identical to the `run` function.
     """
 
     inner: Val
 
-    def __init__(self, inner: Val) -> None:
-        self.inner = inner
-
     def run(self, using: Callable[[Val], NewVal]) -> Do[Val]:
         """
         Performs the provided function on the `inner` value, but does not return its result.
         Returns itself instead.
         """
         using(self.inner)
         return self
 
     @property
     def bind(self) -> Bind[Val]:
         """
-        Converts the `Do` pipe to a `Bind` pipe
+        Converts the `Do` pipe to a `Bind` pipe, whose call will change the inner value of the container.
+        Call `do` afterwards to revert to a `Do` pipe.
         """
         return Bind(self.inner)
 
     def __call__(self, using: Callable[[Val], NewVal]) -> Do[Val]:
         """
         Performs the provided function on the `inner` value, but does not return its result.
         Returns itself instead.
```

### Comparing `pythonix-1.0.4/pythonix/internals/req.py` & `pythonix-1.0.5/pythonix/internals/req.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 class Delete(Request):
     """
     An HTTP request set as a `DELETE`
     """
 
     method: Callable[P, Response] = _delete
 
+R = TypeVar('R', bound='Request')
 
 @singledispatch
 def to_bytes(value: int) -> bytes:
     return bytes(value)
 
 
 @to_bytes.register(str)
@@ -240,48 +241,48 @@
 
 
 def set_url(url: str):
     """
     Recreates the given request type with a new URL
     """
 
-    def get_content[R: (Request)](content: R) -> R:
+    def get_content(content: R) -> R:
         return content.__class__(url, content.headers, content.params, content.data)
 
     return get_content
 
 
 def set_headers(*headers: Pair[str | int]):
     """
     Recreates the given request types with a new set of headers
     """
 
-    def get_content[R: (Request)](content: R) -> R:
+    def get_content(content: R) -> R:
         return content.__class__(content.url, headers, content.params, content.data)
 
     return get_content
 
 
 def set_params(*params: Pair[str | int]):
     """
     Recreates the given request type with a new set of headers
     """
 
-    def get_content[R: (Request)](content: R) -> R:
+    def get_content(content: R) -> R:
         return content.__class__(content.url, content.headers, params, content.data)
 
     return get_content
 
 
 def set_data(*data: Pair[str | int]):
     """
     Recreates the given request type with a new set of data
     """
 
-    def get_content[R: (Request)](content: R) -> R:
+    def get_content(content: R) -> R:
         return content.__class__(content.url, content.headers, content.params, data)
 
     return get_content
 
 
 def body(content: RequestType) -> Tuple[Pair[bytes], ...]:
     """
```

### Comparing `pythonix-1.0.4/pythonix/internals/res.py` & `pythonix-1.0.5/pythonix/internals/res.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 from collections.abc import Iterator
-from typing import TypeVar, Generic, NamedTuple, cast, ParamSpec, Callable
+from typing import TypeVar, Generic, NamedTuple, cast, ParamSpec, Callable, TypeAlias
 from pythonix.internals.types import Fn
 
 P = ParamSpec("P")
 
 UnwrapErr = ValueError("Attempted to retrieve an Err from an Ok")
 Val = TypeVar("Val")
 NewVal = TypeVar("NewVal")
@@ -23,28 +23,28 @@
 
 class Ok(Generic[Val], NamedTuple):
     """
     Represents a successful outcome of a function that could have failed.
     Useful for pattern matching on a function that returns `Ok[T] | Err[E]`
     ### Example
     ```python
-    success: Res[int, ValueError] = ok(5)(ValueError)
+    success: Res[int, ValueError] = ok(ValueError)(5)
     match success:
         case Ok(t):
             assert t == 5
         case Err(e):
             raise e
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
@@ -59,15 +59,15 @@
 
     inner: ErrVal
 
     def __iter__(self) -> Iterator[ErrVal | None]:
         return iter((None, self.inner))
 
 
-type Res[T, E] = Ok[T] | Err[E]
+Res: TypeAlias = Ok[Val] | Err[ErrVal]
 
 
 def err(ok_type: type[Val]) -> Callable[[ErrVal], Res[Val, ErrVal]]:
     """
     Sets the `Ok` type of the `Res`
     #### Example
     ```python
@@ -80,40 +80,40 @@
         Sets the value of the `Err` inner value of the `Res`
         """
         return Err(exception_object)
 
     return get_err
 
 
-def ok(ok_obj: Val) -> Callable[[type[ErrVal]], Res[Val, ErrVal]]:
+def ok(err_type: type[ErrVal]) -> Callable[[Val], Res[Val, ErrVal]]:
     """
     Sets the `Ok` inner value of the `Res`
     #### Example
     ```python
     success: Res[int, ValueError] = ok(5)(ValueError)
     ```
     """
 
-    def get_err(err_type: type[ErrVal]) -> Res[Val, ErrVal]:
+    def get_err(ok_obj: Val) -> Res[Val, ErrVal]:
         """
         Sets the `Err` type of the `Res`
         """
-        return Ok(ok_obj)
+        return cast(Res[Val, ErrVal], Ok(ok_obj))
 
     return get_err
 
 
-def some(inner: Val | None) -> Res[Val, Nil]:
+def some(inner: Val | None) -> Ok[Val] | Err[Nil]:
     """
     Converts the passed in value `T | None` to `Err[Nil]` if None,
     else `Ok[T]`. Useful for checking for null values before they
     cause unexpected defects.
     """
     if inner is not None:
-        return ok(inner)(Nil)
+        return ok(Nil)(inner)
     return err(Val)(Nil())
 
 
 def is_ok(res: Res[Val, ErrVal]) -> bool:
     """
     Return `True` if the `Res` is `Ok`.
     """
@@ -167,15 +167,15 @@
 
 def unwrap(result: Res[Val, ErrVal]) -> Val:
     """
     Return the `Ok` value or panic if `Err`
     """
     match result:
         case Ok(value):
-            return value
+            return cast(Val, value)
         case Err(e):
             raise e
 
 
 def unwrap_or(default: Val) -> Fn[Res[Val, ErrVal], Val]:
     """
     Return the `Ok` value if `Ok`, else return the default
@@ -221,15 +221,15 @@
     """
     Run the function on the `Ok` if `Ok`, else return the current `Err`
     """
 
     def inner(res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal]:
         match res:
             case Ok(t):
-                return ok(using(t))(ErrVal)
+                return ok(ErrVal)(using(t))
             case _:
                 return cast(Res[NewVal, ErrVal], res)
 
     return inner
 
 
 def map_or(
@@ -241,17 +241,17 @@
 
     def get_default(
         default: NewVal,
     ) -> Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]:
         def inner(res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal]:
             match res:
                 case Ok(t):
-                    return ok(using(t))(ErrVal)
+                    return ok(ErrVal)(using(t))
                 case _:
-                    return ok(default)(ErrVal)
+                    return ok(ErrVal)(default)
 
         return inner
 
     return get_default
 
 
 def map_err(
@@ -281,15 +281,15 @@
     def get_catch(
         catch: type[ErrVal],
     ) -> Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]:
         def inner(res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal]:
             match res:
                 case Ok(t):
                     try:
-                        return ok(using(t))(ErrVal)
+                        return ok(ErrVal)(using(t))
                     except catch as e:
                         return err(NewVal)(e)
                 case Err(e):
                     return cast(Res[NewVal, ErrVal], res)
 
         return inner
 
@@ -307,17 +307,17 @@
 
     def get_default(
         default: Callable[[], NewVal]
     ) -> Callable[[Res[Val, ErrVal]], Res[NewVal, ErrVal]]:
         def inner(res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal]:
             match res:
                 case Ok(t):
-                    return ok(using(t))(ErrVal)
+                    return ok(ErrVal)(using(t))
                 case _:
-                    return ok(default())(ErrVal)
+                    return ok(ErrVal)(default())
 
         return inner
 
     return get_default
 
 
 def and_then(
@@ -364,15 +364,15 @@
         catch: type[NewErrVal],
     ) -> Fn[Res[Val, ErrVal], Res[NewVal, ErrVal | NewErrVal]]:
         def inner(res: Res[Val, ErrVal]) -> Res[NewVal, ErrVal | NewErrVal]:
             match res:
                 case Ok(t):
                     try:
                         return cast(
-                            Res[NewVal, ErrVal | NewErrVal], ok(using(t))(ErrVal)
+                            Res[NewVal, ErrVal | NewErrVal], ok(ErrVal)(using(t))
                         )
                     except catch as f:
                         return cast(Res[NewVal, ErrVal | NewErrVal], err(NewVal)(f))
                 case Err(f):
                     return cast(Res[NewVal, ErrVal | NewErrVal], err(NewVal)(f))
 
         return inner
@@ -409,23 +409,23 @@
                 return new_res
             case Err():
                 return cast(Res[NewVal, ErrVal], old_res)
 
     return inner
 
 
-def or_res[T, F](new_res: Res[T, F]) -> Callable[[Res[T, ErrVal]], Res[T, F]]:
+def or_res(new_res: Res[Val, NewErrVal]) -> Callable[[Res[Val, ErrVal]], Res[Val, NewErrVal]]:
     """
     Returns the provided result if the current one is an `Err`
     """
 
-    def inner(old_res: Res[T, ErrVal]) -> Res[T, F]:
+    def inner(old_res: Res[Val, ErrVal]) -> Res[Val, NewErrVal]:
         match old_res:
             case Ok():
-                return cast(Res[T, F], old_res)
+                return cast(Res[Val, NewErrVal], old_res)
             case Err():
                 return new_res
 
     return inner
 
 
 def flatten(res: Res[Res[Val, ErrVal], NewErrVal]) -> Res[Val, ErrVal | NewErrVal]:
@@ -446,32 +446,32 @@
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
-
     def inner(using: Callable[P, NewVal]) -> Callable[P, Res[NewVal, ErrVal]]:
+
         def wrapper(*args: P.args, **kwargs: P.kwargs) -> Res[NewVal, ErrVal]:
             try:
-                return cast(Res[NewVal, ErrVal], ok(using(*args, **kwargs))(ErrVal))
+                return cast(Res[NewVal, ErrVal],ok(ErrVal)(using(*args, **kwargs)))
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
@@ -496,36 +496,36 @@
 
         return wrapper
 
     return inner
 
 
 def combine_errors(to: NewErrVal, inherit_message: bool = False):
-    """
+    '''
     Decorator function used to convert function that return a `Res[Val, ErrVal]` to `Res[Val, NewErrVal]`, consuming
     the references to the original captured errors. Useful for when a function could throw a lot of errors and you
     need to convert them into one error instead.
     #### Example
+    ```python
     @combine_errors(CustomError)
     @safe(TypeError, ValueError)
     def do_thing(s: str) -> str:
         if not isinstance(s, str):
             raise TypeError('Must be str')
         return s
-
     done: Res[str, CustomError] = do_thing('ok')
-
-    """
-
+    ``` 
+    '''
+    
     def inner(using: Callable[P, Ok[Val] | Err[ErrVal]]):
-        def wrapper(*args: P.args, **kwargs: P.kwargs) -> Res[Val, NewErrVal]:
-            return map_err(lambda e: to.__class__(str(e)) if inherit_message else to)(
-                using(*args, **kwargs)
-            )
 
+        def wrapper(*args: P.args, **kwargs: P.kwargs) -> Res[Val, NewErrVal]:
+            
+            return map_err(lambda e: to.__class__(str(e)) if inherit_message else to)(using(*args, **kwargs)) 
+        
         return wrapper
 
     return inner
 
 
 q = unwrap
 qe = unwrap_err
```

### Comparing `pythonix-1.0.4/pythonix/internals/trail.py` & `pythonix-1.0.5/pythonix/internals/trail.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class Log(NamedTuple):
     datetime: datetime
     message: str
 
     def __str__(self) -> str:
-        return f'{self.__class__.__name__}("{self.datetime.strftime('%Y-%m-%dT%H:%M:%SZ')}", "{self.message}")'
+        return f'{type(self).__name__}("{self.datetime.strftime('%Y-%m-%dT%H:%M:%SZ')}", "{self.message}")'
 
 
 class Info(Log):
     ...
 
 
 class Debug(Log):
```

### Comparing `pythonix-1.0.4/pythonix/internals/tup.py` & `pythonix-1.0.5/pythonix/internals/tup.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.4/pythonix/pipe.py` & `pythonix-1.0.5/pythonix/pipe.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.4/pythonix/req.py` & `pythonix-1.0.5/pythonix/req.py`

 * *Files identical despite different names*

### Comparing `pythonix-1.0.4/PKG-INFO` & `pythonix-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: pythonix
-Version: 1.0.4
+Version: 1.0.5
 Summary: Rust and Gleam like functional programming in Python, complete with Results, pipes, and currying
 Author: jhok2013
 Author-email: jhok2013@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # PYTHONIX
 
 A collection of functional modules in Python 11 inspired by Gleam and Rust.
 If you have like functional programming, but have to program in Python, then check this out.
```

