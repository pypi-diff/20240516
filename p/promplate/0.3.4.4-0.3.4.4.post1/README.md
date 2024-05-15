# Comparing `tmp/promplate-0.3.4.4.tar.gz` & `tmp/promplate-0.3.4.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promplate-0.3.4.4.tar", max compression
+gzip compressed data, was "promplate-0.3.4.4.post1.tar", max compression
```

## Comparing `promplate-0.3.4.4.tar` & `promplate-0.3.4.4.post1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0       45 2023-12-07 20:31:43.859313 promplate-0.3.4.4/promplate/__init__.py
--rw-r--r--   0        0        0      103 2024-02-05 14:52:39.251073 promplate-0.3.4.4/promplate/chain/__init__.py
--rw-r--r--   0        0        0     2309 2024-04-26 17:31:42.113544 promplate-0.3.4.4/promplate/chain/callback.py
--rw-r--r--   0        0        0    17376 2024-04-26 17:32:20.940322 promplate-0.3.4.4/promplate/chain/node.py
--rw-r--r--   0        0        0     1308 2024-04-18 10:26:42.315669 promplate-0.3.4.4/promplate/chain/utils.py
--rw-r--r--   0        0        0        0 2023-11-23 14:05:02.473815 promplate-0.3.4.4/promplate/llm/__init__.py
--rw-r--r--   0        0        0     1043 2024-04-18 10:26:42.319797 promplate-0.3.4.4/promplate/llm/base.py
--rw-r--r--   0        0        0      120 2023-12-17 20:48:44.211258 promplate-0.3.4.4/promplate/llm/openai/__init__.py
--rw-r--r--   0        0        0     4125 2024-04-18 10:26:42.326058 promplate-0.3.4.4/promplate/llm/openai/v0.py
--rw-r--r--   0        0        0     6002 2024-04-20 08:19:12.536648 promplate-0.3.4.4/promplate/llm/openai/v1.py
--rw-r--r--   0        0        0       87 2024-04-06 09:45:04.214579 promplate-0.3.4.4/promplate/prompt/__init__.py
--rw-r--r--   0        0        0     1633 2024-04-15 04:14:57.538290 promplate-0.3.4.4/promplate/prompt/builder.py
--rw-r--r--   0        0        0     3216 2024-04-26 17:31:42.143848 promplate-0.3.4.4/promplate/prompt/chat.py
--rw-r--r--   0        0        0     7362 2024-04-26 19:15:34.918440 promplate-0.3.4.4/promplate/prompt/template.py
--rw-r--r--   0        0        0     3285 2024-04-26 18:50:10.020121 promplate-0.3.4.4/promplate/prompt/utils.py
--rw-r--r--   0        0        0     1600 2024-04-26 19:15:52.361070 promplate-0.3.4.4/pyproject.toml
--rw-r--r--   0        0        0     1995 2024-04-15 04:14:57.536290 promplate-0.3.4.4/README.md
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 promplate-0.3.4.4/PKG-INFO
+-rw-r--r--   0        0        0       45 2023-12-07 20:31:43.859313 promplate-0.3.4.4.post1/promplate/__init__.py
+-rw-r--r--   0        0        0      103 2024-02-05 14:52:39.251073 promplate-0.3.4.4.post1/promplate/chain/__init__.py
+-rw-r--r--   0        0        0     2387 2024-05-15 23:14:27.617169 promplate-0.3.4.4.post1/promplate/chain/callback.py
+-rw-r--r--   0        0        0    17835 2024-05-15 23:14:27.623171 promplate-0.3.4.4.post1/promplate/chain/node.py
+-rw-r--r--   0        0        0     1333 2024-05-15 23:14:27.626165 promplate-0.3.4.4.post1/promplate/chain/utils.py
+-rw-r--r--   0        0        0        0 2023-11-23 14:05:02.473815 promplate-0.3.4.4.post1/promplate/llm/__init__.py
+-rw-r--r--   0        0        0     1074 2024-05-15 23:14:27.629166 promplate-0.3.4.4.post1/promplate/llm/base.py
+-rw-r--r--   0        0        0      120 2023-12-17 20:48:44.211258 promplate-0.3.4.4.post1/promplate/llm/openai/__init__.py
+-rw-r--r--   0        0        0     4368 2024-05-15 23:14:27.633169 promplate-0.3.4.4.post1/promplate/llm/openai/v0.py
+-rw-r--r--   0        0        0     6116 2024-05-15 23:14:27.636165 promplate-0.3.4.4.post1/promplate/llm/openai/v1.py
+-rw-r--r--   0        0        0       87 2024-04-06 09:45:04.214579 promplate-0.3.4.4.post1/promplate/prompt/__init__.py
+-rw-r--r--   0        0        0     1633 2024-04-15 04:14:57.538290 promplate-0.3.4.4.post1/promplate/prompt/builder.py
+-rw-r--r--   0        0        0     2976 2024-05-15 23:14:27.639934 promplate-0.3.4.4.post1/promplate/prompt/chat.py
+-rw-r--r--   0        0        0     7752 2024-05-15 23:15:03.640070 promplate-0.3.4.4.post1/promplate/prompt/template.py
+-rw-r--r--   0        0        0     3327 2024-05-15 23:16:35.334555 promplate-0.3.4.4.post1/promplate/prompt/utils.py
+-rw-r--r--   0        0        0      214 2024-05-15 23:14:27.650873 promplate-0.3.4.4.post1/promplate/typing.py
+-rw-r--r--   0        0        0     1671 2024-05-15 23:15:16.955718 promplate-0.3.4.4.post1/pyproject.toml
+-rw-r--r--   0        0        0     1995 2024-04-15 04:14:57.536290 promplate-0.3.4.4.post1/README.md
+-rw-r--r--   0        0        0     3376 1970-01-01 00:00:00.000000 promplate-0.3.4.4.post1/PKG-INFO
```

### Comparing `promplate-0.3.4.4/promplate/chain/node.py` & `promplate-0.3.4.4.post1/promplate/chain/node.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from inspect import isclass
 from itertools import accumulate
 from typing import Callable, Mapping, MutableMapping, overload
 
-from ..llm.base import *
+from ..llm.base import LLM, AsyncComplete, AsyncGenerate, Complete, Generate
 from ..prompt.template import Context, Loader, SafeChainMapContext, Template
+from ..typing import AsyncIterable, Awaitable, Callable, Iterable, List, Mapping, MutableMapping, Optional, Protocol, Type, Union, cast, overload
 from .callback import BaseCallback, Callback
 from .utils import accumulate_any, resolve
 
 
 class ChainContext(SafeChainMapContext):
     @overload
     def __init__(self): ...
 
     @overload
-    def __init__(self, least: MutableMapping | None = None): ...
+    def __init__(self, least: Optional[MutableMapping] = None): ...
 
     @overload
-    def __init__(self, least: MutableMapping | None = None, *maps: Mapping): ...
+    def __init__(self, least: Optional[MutableMapping] = None, *maps: Mapping): ...
 
-    def __init__(self, least: MutableMapping | None = None, *maps: Mapping):
+    def __init__(self, least: Optional[MutableMapping] = None, *maps: Mapping):
         super().__init__({} if least is None else least, *maps)  # type: ignore
 
     @classmethod
     def ensure(cls, context):
         return context if isinstance(context, cls) else cls(context)
 
     @property
@@ -37,177 +38,177 @@
     def result(self):
         self.__delitem__("__result__")
 
     def __str__(self):
         return str({**self})
 
 
-Process = Callable[[ChainContext], Context | None]
+Process = Callable[[ChainContext], Optional[Context]]
 
-AsyncProcess = Callable[[ChainContext], Awaitable[Context | None]]
+AsyncProcess = Callable[[ChainContext], Awaitable[Optional[Context]]]
 
 
 class AbstractNode(Protocol):
     def invoke(
         self,
-        context: Context | None = None,
+        context: Optional[Context] = None,
         /,
-        complete: Complete | None = None,
+        complete: Optional[Complete] = None,
         **config,
     ) -> ChainContext: ...
 
     async def ainvoke(
         self,
-        context: Context | None = None,
+        context: Optional[Context] = None,
         /,
-        complete: Complete | AsyncComplete | None = None,
+        complete: Union[Complete, Optional[AsyncComplete]] = None,
         **config,
     ) -> ChainContext: ...
 
     def stream(
         self,
-        context: Context | None = None,
+        context: Optional[Context] = None,
         /,
-        generate: Generate | None = None,
+        generate: Optional[Generate] = None,
         **config,
     ) -> Iterable[ChainContext]: ...
 
     def astream(
         self,
-        context: Context | None = None,
+        context: Optional[Context] = None,
         /,
-        generate: Generate | AsyncGenerate | None = None,
+        generate: Union[Generate, Optional[AsyncGenerate]] = None,
         **config,
     ) -> AsyncIterable[ChainContext]: ...
 
     @classmethod
     def _get_chain_type(cls):
         return Chain
 
     def __add__(self, chain: "AbstractNode"):
         if isinstance(chain, Chain):
             return self._get_chain_type()(self, *chain)
         return self._get_chain_type()(self, chain)
 
 
-def ensure_callbacks(callbacks: list[BaseCallback | type[BaseCallback]]) -> list[BaseCallback]:
+def ensure_callbacks(callbacks: List[Union[BaseCallback, Type[BaseCallback]]]) -> List[BaseCallback]:
     return [i() if isclass(i) else i for i in callbacks]
 
 
 class Interruptable(AbstractNode, Protocol):
     def _invoke(
         self,
         context: ChainContext,
         /,
-        complete: Complete | None,
-        callbacks: list[BaseCallback],
+        complete: Optional[Complete],
+        callbacks: List[BaseCallback],
         **config,
     ): ...
 
     async def _ainvoke(
         self,
         context: ChainContext,
         /,
-        complete: Complete | AsyncComplete | None,
-        callbacks: list[BaseCallback],
+        complete: Union[Complete, Optional[AsyncComplete]],
+        callbacks: List[BaseCallback],
         **config,
     ): ...
 
     def _stream(
         self,
         context: ChainContext,
         /,
-        generate: Generate | None,
-        callbacks: list[BaseCallback],
+        generate: Optional[Generate],
+        callbacks: List[BaseCallback],
         **config,
     ) -> Iterable: ...
 
     def _astream(
         self,
         context: ChainContext,
         /,
-        generate: Generate | AsyncGenerate | None,
-        callbacks: list[BaseCallback],
+        generate: Union[Generate, Optional[AsyncGenerate]],
+        callbacks: List[BaseCallback],
         **config,
     ) -> AsyncIterable: ...
 
-    callbacks: list[BaseCallback | type[BaseCallback]]
+    callbacks: List[Union[BaseCallback, Type[BaseCallback]]]
 
-    def enter(self, context: Context | None, config: Context):
-        callbacks: list[BaseCallback] = ensure_callbacks(self.callbacks)
+    def enter(self, context: Optional[Context], config: Context):
+        callbacks: List[BaseCallback] = ensure_callbacks(self.callbacks)
         for callback in callbacks:
             context, config = callback.on_enter(self, context, config)
         return context, config, callbacks
 
-    def leave(self, context: ChainContext, config: Context, callbacks: list[BaseCallback]):
+    def leave(self, context: ChainContext, config: Context, callbacks: List[BaseCallback]):
         for callback in reversed(callbacks):
             context, config = callback.on_leave(self, context, config)
         return context, config
 
-    def add_pre_processes(self, *processes: Process | AsyncProcess):
+    def add_pre_processes(self, *processes: Union[Process, AsyncProcess]):
         self.callbacks.extend(Callback(pre_process=i) for i in processes)
         return self
 
-    def add_mid_processes(self, *processes: Process | AsyncProcess):
+    def add_mid_processes(self, *processes: Union[Process, AsyncProcess]):
         self.callbacks.extend(Callback(mid_process=i) for i in processes)
         return self
 
-    def add_end_processes(self, *processes: Process | AsyncProcess):
+    def add_end_processes(self, *processes: Union[Process, AsyncProcess]):
         self.callbacks.extend(Callback(end_process=i) for i in processes)
         return self
 
-    def add_callbacks(self, *callbacks: BaseCallback | type[BaseCallback]):
+    def add_callbacks(self, *callbacks: Union[BaseCallback, Type[BaseCallback]]):
         self.callbacks.extend(callbacks)
         return self
 
-    def pre_process(self, process: Process | AsyncProcess):
+    def pre_process(self, process: Union[Process, AsyncProcess]):
         self.add_pre_processes(process)
         return process
 
-    def mid_process(self, process: Process | AsyncProcess):
+    def mid_process(self, process: Union[Process, AsyncProcess]):
         self.add_mid_processes(process)
         return process
 
-    def end_process(self, process: Process | AsyncProcess):
+    def end_process(self, process: Union[Process, AsyncProcess]):
         self.add_end_processes(process)
         return process
 
-    def callback(self, callback: BaseCallback | type[BaseCallback]):
+    def callback(self, callback: Union[BaseCallback, Type[BaseCallback]]):
         self.add_callbacks(callback)
         return callback
 
     @staticmethod
-    def _apply_pre_processes(context: ChainContext, callbacks: list[BaseCallback]):
+    def _apply_pre_processes(context: ChainContext, callbacks: List[BaseCallback]):
         for callback in callbacks:
-            context |= cast(Context, callback.pre_process(context) or {})
+            context.update(cast(Context, callback.pre_process(context) or {}))
 
     @staticmethod
-    def _apply_mid_processes(context: ChainContext, callbacks: list[BaseCallback]):
+    def _apply_mid_processes(context: ChainContext, callbacks: List[BaseCallback]):
         for callback in callbacks:
-            context |= cast(Context, callback.mid_process(context) or {})
+            context.update(cast(Context, callback.mid_process(context) or {}))
 
     @staticmethod
-    def _apply_end_processes(context: ChainContext, callbacks: list[BaseCallback]):
+    def _apply_end_processes(context: ChainContext, callbacks: List[BaseCallback]):
         for callback in reversed(callbacks):
-            context |= cast(Context, callback.end_process(context) or {})
+            context.update(cast(Context, callback.end_process(context) or {}))
 
     @staticmethod
-    async def _apply_async_pre_processes(context: ChainContext, callbacks: list[BaseCallback]):
+    async def _apply_async_pre_processes(context: ChainContext, callbacks: List[BaseCallback]):
         for callback in callbacks:
-            context |= cast(Context, await resolve(callback.pre_process(context)) or {})
+            context.update(cast(Context, await resolve(callback.pre_process(context)) or {}))
 
     @staticmethod
-    async def _apply_async_mid_processes(context: ChainContext, callbacks: list[BaseCallback]):
+    async def _apply_async_mid_processes(context: ChainContext, callbacks: List[BaseCallback]):
         for callback in callbacks:
-            context |= cast(Context, await resolve(callback.mid_process(context)) or {})
+            context.update(cast(Context, await resolve(callback.mid_process(context)) or {}))
 
     @staticmethod
-    async def _apply_async_end_processes(context: ChainContext, callbacks: list[BaseCallback]):
+    async def _apply_async_end_processes(context: ChainContext, callbacks: List[BaseCallback]):
         for callback in reversed(callbacks):
-            context |= cast(Context, await resolve(callback.end_process(context)) or {})
+            context.update(cast(Context, await resolve(callback.end_process(context)) or {}))
 
     def invoke(self, context=None, /, complete=None, **config) -> ChainContext:
         context, config, callbacks = self.enter(context, config)
         context = ChainContext.ensure(context)
 
         try:
             self._invoke(ChainContext(context, self.context), complete, callbacks, **config)
@@ -268,118 +269,118 @@
                 raise jump from None
             if jump.into is not None:
                 async for i in jump.into.astream(context, generate, **config):
                     yield i
         else:
             context, config = self.leave(context, config, callbacks)
 
-    _context: Context | None
+    _context: Optional[Context]
 
     @property
     def context(self):
         if self._context is None:
             self._context = {}
         return self._context
 
     @context.setter
-    def context(self, context: Context | None):
+    def context(self, context: Optional[Context]):
         self._context = context
 
     @context.deleter
     def context(self):
         self._context = None
 
 
 class Node(Loader, Interruptable):
     def __init__(
         self,
-        template: Template | str,
-        partial_context: Context | None = None,
-        llm: LLM | None = None,
+        template: Union[Template, str],
+        partial_context: Optional[Context] = None,
+        llm: Optional[LLM] = None,
         **config,
     ):
         self.template = Template(template) if isinstance(template, str) else template
         self._context = partial_context
-        self.callbacks: list[BaseCallback | type[BaseCallback]] = []
+        self.callbacks: List[Union[BaseCallback, Type[BaseCallback]]] = []
         self.llm = llm
         self.run_config = config
 
     def _invoke(self, context, /, complete, callbacks, **config):
         complete = cast(Complete, self.llm.complete if self.llm else complete)
         assert complete is not None
 
         prompt = self.render(context, callbacks)
 
-        context.result = complete(prompt, **(self.run_config | config))
+        context.result = complete(prompt, **({**self.run_config, **config}))
 
         self._apply_mid_processes(context, callbacks)
 
         self._apply_end_processes(context, callbacks)
 
     def _stream(self, context, /, generate, callbacks, **config):
         generate = cast(Generate, self.llm.generate if self.llm else generate)
         assert generate is not None
 
         prompt = self.render(context, callbacks)
 
-        for result in accumulate(generate(prompt, **(self.run_config | config))):
+        for result in accumulate(generate(prompt, **({**self.run_config, **config}))):
             context.result = result
             self._apply_mid_processes(context, callbacks)
             yield
 
         self._apply_end_processes(context, callbacks)
 
     async def _ainvoke(self, context, /, complete, callbacks, **config):
-        complete = cast(Complete | AsyncComplete, self.llm.complete if self.llm else complete)
+        complete = cast(Union[Complete, AsyncComplete], self.llm.complete if self.llm else complete)
         assert complete is not None
 
         prompt = await self.arender(context, callbacks)
 
-        context.result = await resolve(complete(prompt, **(self.run_config | config)))
+        context.result = await resolve(complete(prompt, **({**self.run_config, **config})))
 
         await self._apply_async_mid_processes(context, callbacks)
 
         await self._apply_async_end_processes(context, callbacks)
 
     async def _astream(self, context, /, generate, callbacks, **config):
-        generate = cast(Generate | AsyncGenerate, self.llm.generate if self.llm else generate)
+        generate = cast(Union[Generate, AsyncGenerate], self.llm.generate if self.llm else generate)
         assert generate is not None
 
         prompt = await self.arender(context, callbacks)
 
-        async for result in accumulate_any(generate(prompt, **(self.run_config | config))):
+        async for result in accumulate_any(generate(prompt, **({**self.run_config, **config}))):
             context.result = result
             await self._apply_async_mid_processes(context, callbacks)
             yield
 
         await self._apply_async_end_processes(context, callbacks)
 
-    def render(self, context: Context | None = None, callbacks: list[BaseCallback] | None = None):
+    def render(self, context: Optional[Context] = None, callbacks: Optional[List[BaseCallback]] = None):
         if callbacks is None:
             callbacks = ensure_callbacks(self.callbacks)
         context = ChainContext(context, self.context)
         self._apply_pre_processes(context, callbacks)
         return self.template.render(context)
 
-    async def arender(self, context: Context | None = None, callbacks: list[BaseCallback] | None = None):
+    async def arender(self, context: Optional[Context] = None, callbacks: Optional[List[BaseCallback]] = None):
         if callbacks is None:
             callbacks = ensure_callbacks(self.callbacks)
         context = ChainContext(context, self.context)
         await self._apply_async_pre_processes(context, callbacks)
         return await self.template.arender(context)
 
     def __str__(self):
         return f"</{self.name}/>"
 
 
 class Loop(Interruptable):
-    def __init__(self, chain: AbstractNode, partial_context: Context | None = None):
+    def __init__(self, chain: AbstractNode, partial_context: Optional[Context] = None):
         self.chain = chain
         self._context = partial_context
-        self.callbacks: list[BaseCallback | type[BaseCallback]] = []
+        self.callbacks: List[Union[BaseCallback, Type[BaseCallback]]] = []
 
     def _invoke(self, context, /, complete, callbacks, **config):
         while True:
             self._apply_pre_processes(context, callbacks)
             self.chain.invoke(context, complete, **config)
             self._apply_mid_processes(context, callbacks)
             self._apply_end_processes(context, callbacks)
@@ -405,64 +406,64 @@
             async for _ in self.chain.astream(context, generate, **config):
                 await self._apply_async_mid_processes(context, callbacks)
                 yield
             await self._apply_async_end_processes(context, callbacks)
 
 
 class Chain(Interruptable):
-    def __init__(self, *nodes: AbstractNode, partial_context: Context | None = None):
+    def __init__(self, *nodes: AbstractNode, partial_context: Optional[Context] = None):
         self.nodes = list(nodes)
         self._context = partial_context
-        self.callbacks: list[BaseCallback | type[BaseCallback]] = []
+        self.callbacks: List[Union[BaseCallback, Type[BaseCallback]]] = []
 
     @classmethod
     def _get_chain_type(cls):
         return cls
 
     def __iadd__(self, chain: AbstractNode):
         self.nodes.append(chain)
         return self
 
     def __iter__(self):
         return iter(self.nodes)
 
-    def _invoke(self, context, /, complete, callbacks: list[BaseCallback], **config):
+    def _invoke(self, context, /, complete, callbacks: List[BaseCallback], **config):
         self._apply_pre_processes(context, callbacks)
         for node in self.nodes:
             node.invoke(context, complete, **config)
             self._apply_mid_processes(context, callbacks)
         self._apply_end_processes(context, callbacks)
 
-    async def _ainvoke(self, context, /, complete, callbacks: list[BaseCallback], **config):
+    async def _ainvoke(self, context, /, complete, callbacks: List[BaseCallback], **config):
         await self._apply_async_pre_processes(context, callbacks)
         for node in self.nodes:
             await node.ainvoke(context, complete, **config)
             await self._apply_async_mid_processes(context, callbacks)
         await self._apply_async_end_processes(context, callbacks)
 
-    def _stream(self, context, /, generate, callbacks: list[BaseCallback], **config):
+    def _stream(self, context, /, generate, callbacks: List[BaseCallback], **config):
         self._apply_pre_processes(context, callbacks)
         for node in self.nodes:
             for _ in node.stream(context, generate, **config):
                 self._apply_mid_processes(context, callbacks)
                 yield
         self._apply_end_processes(context, callbacks)
 
-    async def _astream(self, context, /, generate, callbacks: list[BaseCallback], **config):
+    async def _astream(self, context, /, generate, callbacks: List[BaseCallback], **config):
         await self._apply_async_pre_processes(context, callbacks)
         for node in self.nodes:
             async for _ in node.astream(context, generate, **config):
                 await self._apply_async_mid_processes(context, callbacks)
                 yield
         await self._apply_async_end_processes(context, callbacks)
 
     def __repr__(self):
         return " + ".join(map(str, self.nodes))
 
 
 class Jump(Exception):
-    def __init__(self, into: Interruptable | None = None, out_of: Interruptable | None = None):
+    def __init__(self, into: Optional[Interruptable] = None, out_of: Optional[Interruptable] = None):
         self.into = into
         self.out_of = out_of
 
     def __str__(self):
         return f"{self.out_of} does not exist in the chain hierarchy"
```

### Comparing `promplate-0.3.4.4/promplate/chain/utils.py` & `promplate-0.3.4.4.post1/promplate/chain/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from inspect import Parameter, isasyncgen, isawaitable, signature
 from itertools import accumulate
-from typing import AsyncIterable, Awaitable, Callable, Iterable, TypeVar, cast
+from typing import AsyncIterable, Awaitable, Callable, Iterable, List, TypeVar, Union, cast
 
 T = TypeVar("T")
 
 
-def appender(to_append: list[T]) -> Callable[[T], T]:
+def appender(to_append: List[T]) -> Callable[[T], T]:
     def append_processer(func: T) -> T:
         to_append.append(func)
 
         return func
 
     return append_processer
 
@@ -18,29 +18,29 @@
     return p.kind is Parameter.POSITIONAL_OR_KEYWORD or p.kind is Parameter.KEYWORD_ONLY
 
 
 def count_position_parameters(func):
     return sum(map(is_positional_parameter, signature(func).parameters.values()))
 
 
-async def resolve(maybe_awaitable: T | Awaitable[T], /) -> T:
+async def resolve(maybe_awaitable: Union[T, Awaitable[T]], /) -> T:
     while isawaitable(maybe_awaitable):
         maybe_awaitable = await maybe_awaitable
 
     return maybe_awaitable  # type: ignore
 
 
 async def async_accumulate(async_iterable: AsyncIterable[str]):
     result = ""
     async for delta in async_iterable:
         result += delta
         yield result
 
 
-def accumulate_any(any_iterable: Iterable[str] | AsyncIterable[str]):
+def accumulate_any(any_iterable: Union[Iterable[str], AsyncIterable[str]]):
     if isasyncgen(any_iterable):
         return async_accumulate(any_iterable)
 
     async def _():
         for i in accumulate(cast(Iterable[str], any_iterable)):
             yield i
```

### Comparing `promplate-0.3.4.4/promplate/llm/base.py` & `promplate-0.3.4.4.post1/promplate/llm/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import partial
-from typing import AsyncIterable, Awaitable, Iterable, Protocol, cast
+from typing import AsyncIterable, Awaitable, Iterable, Protocol, Union, cast
 
 
 class Configurable:
     def __init__(self, **config):
         for key, val in config.items():
             setattr(self, key, val)
 
@@ -25,12 +25,12 @@
 
 
 class AsyncGenerate(Protocol):
     def __call__(self, prompt, /, **config) -> AsyncIterable[str]: ...
 
 
 class LLM(Protocol):
-    @partial(cast, Complete | AsyncComplete)
-    def complete(self, prompt, /, **config) -> str | Awaitable[str]: ...
+    @partial(cast, Union[Complete, AsyncComplete])
+    def complete(self, prompt, /, **config) -> Union[str, Awaitable[str]]: ...
 
-    @partial(cast, Generate | AsyncGenerate)
-    def generate(self, prompt, /, **config) -> Iterable[str] | AsyncIterable[str]: ...
+    @partial(cast, Union[Generate, AsyncGenerate])
+    def generate(self, prompt, /, **config) -> Union[Iterable[str], AsyncIterable[str]]: ...
```

### Comparing `promplate-0.3.4.4/promplate/llm/openai/v0.py` & `promplate-0.3.4.4.post1/promplate/llm/openai/v0.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 from importlib.metadata import metadata
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 import openai
 from openai import ChatCompletion, Completion  # type: ignore
 
 from ...prompt.chat import Message, ensure
-from ..base import *
+from ..base import AsyncComplete, AsyncGenerate, Complete, Configurable, Generate
 
 meta = metadata("promplate")
 
 if openai.api_key is None:
     openai.api_key = ""
 
-openai.app_info = (openai.app_info or {}) | {  # type: ignore
-    "name": "Promplate",
-    "version": meta["version"],
-    "url": meta["home-page"],
+openai.app_info = {  # type: ignore
+    **(openai.app_info or {}),  # type: ignore
+    **{
+        "name": "Promplate",
+        "version": meta["version"],
+        "url": meta["home-page"],
+    },
 }
 
 
 if TYPE_CHECKING:
 
     class Config(Configurable):
         def __init__(
             self,
             model: str,
-            temperature: float | int | None = None,
-            top_p: float | int | None = None,
-            stop: str | list[str] | None = None,
-            max_tokens: int | None = None,
-            api_key: str | None = None,
-            api_base: str | None = None,
+            temperature: Optional[Union[float, int]] = None,
+            top_p: Optional[Union[float, int]] = None,
+            stop: Optional[Union[str, List[str]]] = None,
+            max_tokens: Optional[int] = None,
+            api_key: Optional[str] = None,
+            api_base: Optional[str] = None,
             **other_config,
         ):
             self.model = model
             self.temperature = temperature
             self.top_p = top_p
             self.stop = stop
             self.max_tokens = max_tokens
@@ -50,69 +53,69 @@
 
 else:
     Config = Configurable
 
 
 class TextComplete(Config, Complete):
     def __call__(self, text: str, /, **config):
-        config = self._config | config | {"stream": False, "prompt": text}
+        config = {**self._config, **config, **{"stream": False, "prompt": text}}
         result: Any = Completion.create(**config)
         return result["choices"][0]["text"]
 
 
 class AsyncTextComplete(Config, AsyncComplete):
     async def __call__(self, text: str, /, **config):
-        config = self._config | config | {"stream": False, "prompt": text}
+        config = {**self._config, **config, **{"stream": False, "prompt": text}}
         result: Any = await Completion.acreate(**config)
         return result["choices"][0]["text"]
 
 
 class TextGenerate(Config, Generate):
     def __call__(self, text: str, /, **config):
-        config = self._config | config | {"stream": True, "prompt": text}
+        config = {**self._config, **config, **{"stream": True, "prompt": text}}
         stream: Any = Completion.create(**config)
         for event in stream:
             yield event["choices"][0]["text"]
 
 
 class AsyncTextGenerate(Config, AsyncGenerate):
     async def __call__(self, text: str, /, **config):
-        config = self._config | config | {"stream": True, "prompt": text}
+        config = {**self._config, **config, **{"stream": True, "prompt": text}}
         stream: Any = await Completion.acreate(**config)
         async for event in stream:
             yield event["choices"][0]["text"]
 
 
 class ChatComplete(Config, Complete):
-    def __call__(self, messages: list[Message] | str, /, **config):
+    def __call__(self, messages: Union[List[Message], str], /, **config):
         messages = ensure(messages)
-        config = self._config | config | {"stream": False, "messages": messages}
+        config = {**self._config, **config, **{"stream": False, "messages": messages}}
         result: Any = ChatCompletion.create(**config)
         return result["choices"][0]["message"]["content"]
 
 
 class AsyncChatComplete(Config, AsyncComplete):
-    async def __call__(self, messages: list[Message] | str, /, **config):
+    async def __call__(self, messages: Union[List[Message], str], /, **config):
         messages = ensure(messages)
-        config = self._config | config | {"stream": False, "messages": messages}
+        config = {**self._config, **config, **{"stream": False, "messages": messages}}
         result: Any = await ChatCompletion.acreate(**config)
         return result["choices"][0]["message"]["content"]
 
 
 class ChatGenerate(Config, Generate):
-    def __call__(self, messages: list[Message] | str, /, **config):
+    def __call__(self, messages: Union[List[Message], str], /, **config):
         messages = ensure(messages)
-        config = self._config | config | {"stream": True, "messages": messages}
+        config = {**self._config, **config, **{"stream": True, "messages": messages}}
         stream: Any = ChatCompletion.create(**config)
         for event in stream:
             delta: dict = event["choices"][0]["delta"]
             yield delta.get("content", "")
 
 
 class AsyncChatGenerate(Config, AsyncGenerate):
-    async def __call__(self, messages: list[Message] | str, /, **config):
+    async def __call__(self, messages: Union[List[Message], str], /, **config):
         messages = ensure(messages)
-        config = self._config | config | {"stream": True, "messages": messages}
+        config = {**self._config, **config, **{"stream": True, "messages": messages}}
         stream: Any = await ChatCompletion.acreate(**config)
         async for event in stream:
             delta: dict = event["choices"][0]["delta"]
             yield delta.get("content", "")
```

### Comparing `promplate-0.3.4.4/promplate/llm/openai/v1.py` & `promplate-0.3.4.4.post1/promplate/llm/openai/v1.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from copy import copy
 from functools import cached_property
 from types import MappingProxyType
-from typing import TYPE_CHECKING, Any, Callable, ParamSpec, TypeVar
 
 from openai import AsyncClient, Client  # type: ignore
 
 from ...prompt.chat import Message, ensure
 from ...prompt.utils import _get_aclient, _get_client, get_user_agent
-from ..base import *
+from ...typing import TYPE_CHECKING, Any, Callable, List, ParamSpec, TypeVar, Union
+from ..base import LLM, Configurable
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
 def same_params_as(_: Callable[P, Any]):
     def func(__init__: Callable[..., None]) -> Callable[P, None]:
@@ -23,28 +23,28 @@
 class Config(Configurable):
     def __init__(self, **config):
         super().__init__(**config)
         self._run_config = {}
 
     def bind(self, **run_config):
         obj = copy(self)
-        obj._run_config = self._run_config | run_config
+        obj._run_config = {**self._run_config, **run_config}
         return obj
 
     @cached_property
     def _user_agent(self):
         from openai.version import VERSION
 
         return get_user_agent(self, ("OpenAI", VERSION))
 
     @property
     def _config(self):  # type: ignore
         ua_header = {"User-Agent": self._user_agent}
         config = dict(super()._config)
-        config["default_headers"] = config.get("default_headers", {}) | ua_header
+        config["default_headers"] = {**config.get("default_headers", {}), **ua_header}
         return MappingProxyType(config)
 
     @cached_property
     def _client(self):
         if "http_client" in self._config:
             return Client(**self._config)
         else:
@@ -70,80 +70,80 @@
 
 else:
     ClientConfig = AsyncClientConfig = Config
 
 
 class TextComplete(ClientConfig):
     def __call__(self, text: str, /, **config):
-        config = self._run_config | config | {"stream": False, "prompt": text}
+        config = {**self._run_config, **config, **{"stream": False, "prompt": text}}
         result = self._client.completions.create(**config)
         return result.choices[0].text
 
 
 class AsyncTextComplete(AsyncClientConfig):
     async def __call__(self, text: str, /, **config):
-        config = self._run_config | config | {"stream": False, "prompt": text}
+        config = {**self._run_config, **config, **{"stream": False, "prompt": text}}
         result = await self._aclient.completions.create(**config)
         return result.choices[0].text
 
 
 class TextGenerate(ClientConfig):
     def __call__(self, text: str, /, **config):
-        config = self._run_config | config | {"stream": True, "prompt": text}
+        config = {**self._run_config, **config, **{"stream": True, "prompt": text}}
         stream = self._client.completions.create(**config)
         for event in stream:
             try:
                 yield event.choices[0].text
             except AttributeError:
                 pass
 
 
 class AsyncTextGenerate(AsyncClientConfig):
     async def __call__(self, text: str, /, **config):
-        config = self._run_config | config | {"stream": True, "prompt": text}
+        config = {**self._run_config, **config, **{"stream": True, "prompt": text}}
         stream = await self._aclient.completions.create(**config)
         async for event in stream:
             try:
                 yield event.choices[0].text
             except AttributeError:
                 pass
 
 
 class ChatComplete(ClientConfig):
-    def __call__(self, messages: list[Message] | str, /, **config):
+    def __call__(self, messages: Union[List[Message], str], /, **config):
         messages = ensure(messages)
-        config = self._run_config | config | {"stream": False, "messages": messages}
+        config = {**self._run_config, **config, **{"stream": False, "messages": messages}}
         result = self._client.chat.completions.create(**config)
         return result.choices[0].message.content
 
 
 class AsyncChatComplete(AsyncClientConfig):
-    async def __call__(self, messages: list[Message] | str, /, **config):
+    async def __call__(self, messages: Union[List[Message], str], /, **config):
         messages = ensure(messages)
-        config = self._run_config | config | {"stream": False, "messages": messages}
+        config = {**self._run_config, **config, **{"stream": False, "messages": messages}}
         result = await self._aclient.chat.completions.create(**config)
         return result.choices[0].message.content
 
 
 class ChatGenerate(ClientConfig):
-    def __call__(self, messages: list[Message] | str, /, **config):
+    def __call__(self, messages: Union[List[Message], str], /, **config):
         messages = ensure(messages)
-        config = self._run_config | config | {"stream": True, "messages": messages}
+        config = {**self._run_config, **config, **{"stream": True, "messages": messages}}
         stream = self._client.chat.completions.create(**config)
         for event in stream:
             try:
                 yield event.choices[0].delta.content or ""
             except AttributeError:
                 pass
 
 
 class AsyncChatGenerate(AsyncClientConfig):
-    async def __call__(self, messages: list[Message] | str, /, **config):
+    async def __call__(self, messages: Union[List[Message], str], /, **config):
         messages = ensure(messages)
-        config = self._run_config | config | {"stream": True, "messages": messages}
+        config = {**self._run_config, **config, **{"stream": True, "messages": messages}}
         stream = await self._aclient.chat.completions.create(**config)
         async for event in stream:
             try:
                 yield event.choices[0].delta.content or ""
             except AttributeError:
                 pass
```

### Comparing `promplate-0.3.4.4/promplate/prompt/builder.py` & `promplate-0.3.4.4.post1/promplate/prompt/builder.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.4/promplate/prompt/chat.py` & `promplate-0.3.4.4.post1/promplate/prompt/chat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,24 @@
-from sys import version_info
-from typing import Literal
-
+from ..typing import List, Literal, NotRequired, Optional, TypedDict, Union
 from .utils import is_message_start
 
 Role = Literal["user", "assistant", "system"]
 
-if version_info >= (3, 12):
-    from typing import NotRequired, TypedDict
 
-    class Message(TypedDict):  # type: ignore
-        role: Role
-        content: str
-        name: NotRequired[str]
-
-else:
-    from typing_extensions import NotRequired, TypedDict
-
-    class Message(TypedDict):
-        role: Role
-        content: str
-        name: NotRequired[str]
+class Message(TypedDict):
+    role: Role
+    content: str
+    name: NotRequired[str]
 
 
 class MessageBuilder:
     _initializing = True
     __slots__ = ("role", "content", "name")
 
-    def __init__(self, role: Role, /, content: str = "", name: str | None = None):
+    def __init__(self, role: Role, /, content: str = "", name: Optional[str] = None):
         self.role: Role = role
         self.content = content
         self.name = name
 
     def __repr__(self):
         if self.name is not None:
             return f"<| {self.role} {self.name} |>"
@@ -66,19 +54,19 @@
 
 U = user = MessageBuilder("user")
 A = assistant = MessageBuilder("assistant")
 S = system = MessageBuilder("system")
 MessageBuilder._initializing = False
 
 
-def ensure(text_or_list: list[Message] | str) -> list[Message]:
+def ensure(text_or_list: Union[List[Message], str]) -> List[Message]:
     return parse_chat_markup(text_or_list) if isinstance(text_or_list, str) else text_or_list
 
 
-def parse_chat_markup(text: str) -> list[Message]:
+def parse_chat_markup(text: str) -> List[Message]:
     messages = []
     current_message = None
     buffer = []
 
     for line in text.splitlines():
         match = is_message_start.match(line)
         if match:
@@ -100,9 +88,9 @@
     if current_message:
         current_message["content"] = "\n".join(buffer)
         messages.append(current_message)
 
     if messages:
         return messages
     elif text and text != "\n":
-        return [{"role": "user", "content": text.removesuffix("\n")}]
+        return [{"role": "user", "content": text[:-1] if text[-1] == "\n" else text}]
     return []
```

### Comparing `promplate-0.3.4.4/promplate/prompt/template.py` & `promplate-0.3.4.4.post1/promplate/prompt/template.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from ast import Expr, parse, unparse
+from ast import Expr, parse
 from collections import ChainMap
 from functools import cached_property
 from pathlib import Path
+from sys import version_info
 from textwrap import dedent
-from typing import TYPE_CHECKING, Any, Protocol
 
-from .builder import *
-from .utils import *
+from ..typing import TYPE_CHECKING, Any, Callable, Dict, Optional, Protocol, Self, Union
+from .builder import get_base_builder
+from .utils import AutoNaming, get_user_agent, split_template_tokens
 
-Context = dict[str, Any]  # globals must be a real dict
+Context = Dict[str, Any]  # globals must be a real dict
 
 
 class Component(Protocol):
     def render(self, context: Context) -> str: ...
 
     async def arender(self, context: Context) -> str: ...
 
@@ -39,29 +40,35 @@
 
     def _on_eval_token(self, token):
         token = self._unwrap_token(token)
         if "\n" in token:
             mod = parse(token)
             [*rest, last] = mod.body
             assert isinstance(last, Expr), "{{ }} block must end with an expression, or you should use {# #} block"
-            self._buffer.extend(unparse(rest).splitlines())  # type: ignore
+            if version_info >= (3, 9):
+                from ast import unparse
+            else:
+                from astor import to_source as unparse  # type: ignore
+
+            for line in rest:
+                self._buffer.extend(unparse(line).splitlines())
             exp = unparse(last)
         else:
             exp = token
         self._buffer.append(f"__append__({exp})")
 
     def _on_exec_token(self, token):
         self._buffer.extend(self._unwrap_token(token).splitlines())
 
     def _on_special_token(self, token, sync: bool):
         inner = self._unwrap_token(token)
 
         if inner.startswith("end"):
             last = self._ops_stack.pop()
-            assert last == inner.removeprefix("end")
+            assert last == inner[3:]
             self._flush()
             self._builder.dedent()
 
         else:
             op = inner.split(" ", 1)[0]
 
             if op == "if" or op == "for" or op == "while":
@@ -82,16 +89,17 @@
                     self._buffer.append(f"__append__({op}.render({params}))")
                 else:
                     self._buffer.append(f"__append__(await {op}.arender({params}))")
 
     @staticmethod
     def _make_context(text: str):
         """generate context parameter if specified otherwise use locals() by default"""
-
-        return f"locals() | dict({text[text.index(' ') + 1:]})" if " " in text else "locals()"
+        if version_info >= (3, 10):
+            return f"(__l__:=locals().copy(), __l__.update(dict({text[text.index(' ') + 1:]})))[0]" if " " in text else "locals()"
+        return f"(__l__:=globals().copy(), __l__.update(dict({text[text.index(' ') + 1:]})))[0]" if " " in text else "globals()"
 
     def compile(self, sync=True, indent_str="\t"):
         self._buffer = []
         self._ops_stack = []
         self._builder = get_base_builder(sync, indent_str)
 
         for token in split_template_tokens(self.text):
@@ -134,35 +142,35 @@
         """compile template string into python script"""
         self.compile(sync, indent_str)
         return str(self._builder)
 
 
 class Loader(AutoNaming):
     @classmethod
-    def read(cls, path: str | Path, encoding="utf-8"):
+    def read(cls, path: Union[str, Path], encoding="utf-8"):
         path = Path(path)
         obj = cls(path.read_text(encoding))
         obj.name = path.stem
         return obj
 
     @classmethod
-    async def aread(cls, path: str | Path, encoding="utf-8"):
+    async def aread(cls, path: Union[str, Path], encoding="utf-8"):
         from aiofiles import open
 
         async with open(path, encoding=encoding) as f:
             content = await f.read()
 
         path = Path(path)
         obj = cls(content)
         obj.name = path.stem
         return obj
 
     @classmethod
     def _patch_kwargs(cls, kwargs: dict) -> dict:
-        return {"headers": {"User-Agent": get_user_agent(cls)}} | kwargs
+        return {**{"headers": {"User-Agent": get_user_agent(cls)}}, **kwargs}
 
     @staticmethod
     def _join_url(url: str):
         if url.startswith("http"):
             return url
 
         from urllib.parse import urljoin
@@ -188,35 +196,30 @@
         return obj
 
 
 class SafeChainMapContext(ChainMap, dict):
     if TYPE_CHECKING:  # fix type from `collections.ChainMap`
         from sys import version_info
 
-        if version_info >= (3, 11):
-            from typing_extensions import Self
-        else:
-            from typing import Self
-
         copy: Callable[[Self], Self]
 
 
 class Template(TemplateCore, Loader):
-    def __init__(self, text: str, /, context: Context | None = None):
+    def __init__(self, text: str, /, context: Optional[Context] = None):
         super().__init__(text)
         self.context = {} if context is None else context
 
-    def render(self, context: Context | None = None):
+    def render(self, context: Optional[Context] = None):
         if context is None:
             context = SafeChainMapContext({}, self.context)
         else:
             context = SafeChainMapContext({}, context, self.context)
 
         return super().render(context)
 
-    async def arender(self, context: Context | None = None):
+    async def arender(self, context: Optional[Context] = None):
         if context is None:
             context = SafeChainMapContext({}, self.context)
         else:
             context = SafeChainMapContext({}, context, self.context)
 
         return await super().arender(context)
```

### Comparing `promplate-0.3.4.4/promplate/prompt/utils.py` & `promplate-0.3.4.4.post1/promplate/prompt/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from functools import cache, cached_property, wraps
+from functools import cached_property, lru_cache, wraps
 from inspect import currentframe, isclass
 from re import compile
-from typing import Any, Callable, ParamSpec, TypeVar
+from typing import Dict, Tuple
 
-split_template_tokens = compile(
-    r"((?:\s{%-|{%).*?(?:%}|-%}\s))|((?:\s{{-|{{)[\s\S]*?(?:}}|-}}\s))|((?:\s{#-|{#)[\s\S]*?(?:#}|-#}\s))"
-).split
+from ..typing import Any, Callable, ParamSpec, TypeVar
+
+split_template_tokens = compile(r"((?:\s{%-|{%).*?(?:%}|-%}\s))|((?:\s{{-|{{)[\s\S]*?(?:}}|-}}\s))|((?:\s{#-|{#)[\s\S]*?(?:#}|-#}\s))").split
 
 
 var_name_checker = compile(r"[_a-zA-Z]\w*$")
 
 is_message_start = compile(r"<\|\s?(user|system|assistant)\s?(\w{1,64})?\s?\|>")
 
 
@@ -82,30 +82,30 @@
             result = func(*args, **kwargs)
         return result
 
     return wrapper
 
 
 @cache_once
-def get_builtins() -> dict[str, Any]:
+def get_builtins() -> Dict[str, Any]:
     return __builtins__ if isinstance(__builtins__, dict) else __builtins__.__dict__
 
 
-@cache
+@lru_cache(None)
 def version(package: str):
     from importlib.metadata import PackageNotFoundError, version
 
     try:
         return version(package)
     except PackageNotFoundError:
         return None
 
 
 @cache_once
-def get_user_agent(self, *additional_packages: tuple[str, str]):
+def get_user_agent(self, *additional_packages: Tuple[str, str]):
     from sys import version as py_version
 
     return " ".join(
         (
             f"Promplate/{version('promplate')} ({self.__name__ if isclass(self) else self.__class__.__name__})",
             *(f"{name}/{v}" for name, v in additional_packages),
             f"HTTPX/{version('httpx') or '-'}",
```

### Comparing `promplate-0.3.4.4/pyproject.toml` & `promplate-0.3.4.4.post1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promplate"
-version = "0.3.4.4"
+version = "0.3.4.4.post1"
 description = "Prompt engineering framework for humans"
 homepage = "https://promplate.dev/"
 documentation = "https://docs.py.promplate.dev/"
 repository = "https://github.com/promplate/core"
 authors = ["Muspi Merol <me@promplate.dev>"]
 license = "MIT"
 readme = "README.md"
@@ -13,15 +13,16 @@
     "Development Status :: 5 - Production/Stable",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Text Processing :: Markup",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
+astor = { version = "^0.8", python = "<3.9" }
 typing-extensions = { version = "^4", python = "<3.12" }
 aiofiles = { version = "^23.2", optional = true }
 httpx = { version = ">=0.24, <1.0", optional = true }
 openai = { version = ">=0.27, <2.0", optional = true }
 
 [tool.poetry.extras]
 aiofiles = ["aiofiles"]
@@ -39,17 +40,18 @@
 [tool.pdm.scripts]
 format = { composite = ["isort ./{args}", "black ./{args}"] }
 test = "pytest"
 cov = { composite = ["coverage run -m pytest", "coverage report"] }
 
 [tool.isort]
 profile = "black"
+line_length = 150
 
 [tool.black]
-line-length = 130
+line-length = 150
 
 [tool.coverage.run]
 source = ["promplate"]
 branch = true
 
 [tool.coverage.report]
 fail_under = 45
```

### Comparing `promplate-0.3.4.4/README.md` & `promplate-0.3.4.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.4/PKG-INFO` & `promplate-0.3.4.4.post1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 Metadata-Version: 2.1
 Name: promplate
-Version: 0.3.4.4
+Version: 0.3.4.4.post1
 Summary: Prompt engineering framework for humans
 Home-page: https://promplate.dev/
 License: MIT
 Keywords: prompt,template,nlp,llm
 Author: Muspi Merol
 Author-email: me@promplate.dev
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Typing :: Typed
 Provides-Extra: aiofiles
 Provides-Extra: all
 Provides-Extra: httpx
 Provides-Extra: openai
 Requires-Dist: aiofiles (>=23.2,<24.0) ; extra == "aiofiles" or extra == "all"
+Requires-Dist: astor (>=0.8,<0.9) ; python_version < "3.9"
 Requires-Dist: httpx (>=0.24,<1.0) ; extra == "httpx" or extra == "all"
 Requires-Dist: openai (>=0.27,<2.0) ; extra == "openai" or extra == "all"
 Requires-Dist: typing-extensions (>=4,<5) ; python_version < "3.12"
 Project-URL: Documentation, https://docs.py.promplate.dev/
 Project-URL: Repository, https://github.com/promplate/core
 Description-Content-Type: text/markdown
```

