# Comparing `tmp/abses-0.6.3.post0.tar.gz` & `tmp/abses-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abses-0.6.3.post0.tar", max compression
+gzip compressed data, was "abses-0.6.4.tar", max compression
```

## Comparing `abses-0.6.3.post0.tar` & `abses-0.6.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.6.3.post0/LICENSE
-drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.6.3.post0/LICENSES/
--rw-r--r--   0        0        0     6273 2024-04-10 23:24:41.142521 abses-0.6.3.post0/README.md
--rw-r--r--   0        0        0     1081 2024-05-12 13:09:44.792287 abses-0.6.3.post0/abses/__init__.py
--rw-r--r--   0        0        0     2651 2024-05-11 09:28:11.068165 abses-0.6.3.post0/abses/_bases/bases.py
--rw-r--r--   0        0        0     3124 2024-05-11 09:28:11.068264 abses-0.6.3.post0/abses/_bases/components.py
--rw-r--r--   0        0        0     3128 2024-05-11 09:28:11.068727 abses-0.6.3.post0/abses/_bases/dynamic.py
--rw-r--r--   0        0        0      298 2024-05-11 09:28:11.068876 abses-0.6.3.post0/abses/_bases/errors.py
--rw-r--r--   0        0        0      347 2024-05-11 09:28:11.068990 abses-0.6.3.post0/abses/_bases/logging.py
--rw-r--r--   0        0        0     6280 2024-05-11 09:28:11.069510 abses-0.6.3.post0/abses/_bases/modules.py
--rw-r--r--   0        0        0     3075 2024-05-11 09:28:11.069838 abses-0.6.3.post0/abses/_bases/objects.py
--rw-r--r--   0        0        0     1098 2024-05-11 09:28:11.069942 abses-0.6.3.post0/abses/_bases/states.py
--rw-r--r--   0        0        0     9572 2024-05-11 09:28:11.070216 abses-0.6.3.post0/abses/actor.py
--rw-r--r--   0        0        0     4979 2024-05-11 09:28:11.070565 abses-0.6.3.post0/abses/cells.py
--rw-r--r--   0        0        0        0 2024-05-11 14:48:58.011285 abses-0.6.3.post0/abses/conf/__init__.py
--rw-r--r--   0        0        0      297 2024-05-11 14:21:43.684047 abses-0.6.3.post0/abses/conf/default.yaml
--rw-r--r--   0        0        0    17526 2024-05-11 09:28:11.070970 abses-0.6.3.post0/abses/container.py
--rw-r--r--   0        0        0      969 2024-05-11 09:28:11.071255 abses-0.6.3.post0/abses/data.py
--rw-r--r--   0        0        0     8957 2024-05-10 03:24:33.872539 abses-0.6.3.post0/abses/decision.py
--rw-r--r--   0        0        0    15662 2024-05-12 12:06:53.545831 abses-0.6.3.post0/abses/experiment.py
--rw-r--r--   0        0        0     3930 2024-05-11 09:28:11.071776 abses-0.6.3.post0/abses/human.py
--rw-r--r--   0        0        0    19386 2024-05-11 09:28:11.072342 abses-0.6.3.post0/abses/links.py
--rw-r--r--   0        0        0    13666 2024-05-11 09:28:11.072495 abses-0.6.3.post0/abses/main.py
--rw-r--r--   0        0        0     8375 2024-05-11 09:28:11.072683 abses-0.6.3.post0/abses/move.py
--rw-r--r--   0        0        0    12561 2024-05-11 14:49:37.222743 abses-0.6.3.post0/abses/nature.py
--rw-r--r--   0        0        0    28830 2024-05-12 03:13:27.744826 abses-0.6.3.post0/abses/patch.py
--rw-r--r--   0        0        0     6802 2024-05-11 09:28:11.073646 abses-0.6.3.post0/abses/random.py
--rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.6.3.post0/abses/selection.py
--rw-r--r--   0        0        0    11768 2024-05-11 09:28:11.073845 abses-0.6.3.post0/abses/sequences.py
--rw-r--r--   0        0        0    14598 2024-05-11 09:28:11.073992 abses-0.6.3.post0/abses/time.py
--rw-r--r--   0        0        0     5391 2024-05-12 02:43:42.296709 abses-0.6.3.post0/abses/tools/func.py
--rw-r--r--   0        0        0      723 2024-04-17 19:21:17.693370 abses-0.6.3.post0/abses/tools/regex.py
--rw-r--r--   0        0        0     1134 2024-05-12 12:57:47.944073 abses-0.6.3.post0/abses/viz/viz_actors.py
--rw-r--r--   0        0        0     1149 2024-05-11 09:28:11.074327 abses-0.6.3.post0/abses/viz/viz_model.py
--rw-r--r--   0        0        0     4620 2024-05-11 09:28:11.074600 abses-0.6.3.post0/abses/viz/viz_nature.py
--rw-r--r--   0        0        0     6148 2024-04-14 20:25:37.202150 abses-0.6.3.post0/data/.DS_Store
--rw-r--r--   0        0        0  1653872 2023-09-03 00:55:23.536915 abses-0.6.3.post0/data/YR_cities.zip
--rw-r--r--   0        0        0   395561 2023-11-13 06:23:20.897117 abses-0.6.3.post0/data/farmland.tif
--rw-r--r--   0        0        0    84033 2023-09-02 23:31:24.485471 abses-0.6.3.post0/data/irr_lands.csv
--rw-r--r--   0        0        0  6726328 2023-03-03 00:57:27.899017 abses-0.6.3.post0/data/precipitation.nc
--rw-r--r--   0        0        0   189444 2024-05-11 09:28:11.085808 abses-0.6.3.post0/icons/fa-regular-400.otf
--rw-r--r--   0        0        0     2765 2024-05-12 13:09:23.900373 abses-0.6.3.post0/pyproject.toml
--rw-r--r--   0        0        0     7296 1970-01-01 00:00:00.000000 abses-0.6.3.post0/PKG-INFO
+-rw-r--r--   0        0        0    10280 2023-02-23 05:59:56.670150 abses-0.6.4/LICENSE
+drwxr-xr-x   0        0        0        0 2023-10-20 02:43:17.702059 abses-0.6.4/LICENSES/
+-rw-r--r--   0        0        0     6273 2024-04-10 23:24:41.142521 abses-0.6.4/README.md
+-rw-r--r--   0        0        0     1125 2024-05-16 13:00:46.169463 abses-0.6.4/abses/__init__.py
+-rw-r--r--   0        0        0     2598 2024-05-16 08:41:24.081841 abses-0.6.4/abses/_bases/bases.py
+-rw-r--r--   0        0        0     3124 2024-05-16 03:43:18.344259 abses-0.6.4/abses/_bases/components.py
+-rw-r--r--   0        0        0     3128 2024-05-11 09:28:11.068727 abses-0.6.4/abses/_bases/dynamic.py
+-rw-r--r--   0        0        0      298 2024-05-11 09:28:11.068876 abses-0.6.4/abses/_bases/errors.py
+-rw-r--r--   0        0        0     1564 2024-05-16 11:19:52.124908 abses-0.6.4/abses/_bases/logging.py
+-rw-r--r--   0        0        0     6575 2024-05-16 09:25:00.885690 abses-0.6.4/abses/_bases/modules.py
+-rw-r--r--   0        0        0     3157 2024-05-16 09:29:06.415637 abses-0.6.4/abses/_bases/objects.py
+-rw-r--r--   0        0        0     1098 2024-05-11 09:28:11.069942 abses-0.6.4/abses/_bases/states.py
+-rw-r--r--   0        0        0     9755 2024-05-16 07:58:52.452219 abses-0.6.4/abses/actor.py
+-rw-r--r--   0        0        0     4979 2024-05-11 09:28:11.070565 abses-0.6.4/abses/cells.py
+-rw-r--r--   0        0        0        0 2024-05-11 14:48:58.011285 abses-0.6.4/abses/conf/__init__.py
+-rw-r--r--   0        0        0      311 2024-05-16 10:46:33.609412 abses-0.6.4/abses/conf/default.yaml
+-rw-r--r--   0        0        0    17578 2024-05-16 08:31:28.732690 abses-0.6.4/abses/container.py
+-rw-r--r--   0        0        0      969 2024-05-11 09:28:11.071255 abses-0.6.4/abses/data.py
+-rw-r--r--   0        0        0     8957 2024-05-10 03:24:33.872539 abses-0.6.4/abses/decision.py
+-rw-r--r--   0        0        0    16424 2024-05-16 12:59:51.694497 abses-0.6.4/abses/experiment.py
+-rw-r--r--   0        0        0     3872 2024-05-16 06:59:47.771801 abses-0.6.4/abses/human.py
+-rw-r--r--   0        0        0    19386 2024-05-15 07:23:23.061845 abses-0.6.4/abses/links.py
+-rw-r--r--   0        0        0    15588 2024-05-16 11:13:35.757091 abses-0.6.4/abses/main.py
+-rw-r--r--   0        0        0     8375 2024-05-11 09:28:11.072683 abses-0.6.4/abses/move.py
+-rw-r--r--   0        0        0    12661 2024-05-16 09:25:11.727552 abses-0.6.4/abses/nature.py
+-rw-r--r--   0        0        0    28765 2024-05-16 09:25:22.458944 abses-0.6.4/abses/patch.py
+-rw-r--r--   0        0        0     6802 2024-05-11 09:28:11.073646 abses-0.6.4/abses/random.py
+-rw-r--r--   0        0        0     1611 2024-04-04 10:58:12.168183 abses-0.6.4/abses/selection.py
+-rw-r--r--   0        0        0    11767 2024-05-16 08:30:03.748125 abses-0.6.4/abses/sequences.py
+-rw-r--r--   0        0        0    15523 2024-05-16 08:29:09.798671 abses-0.6.4/abses/time.py
+-rw-r--r--   0        0        0     5391 2024-05-12 02:43:42.296709 abses-0.6.4/abses/tools/func.py
+-rw-r--r--   0        0        0      723 2024-04-17 19:21:17.693370 abses-0.6.4/abses/tools/regex.py
+-rw-r--r--   0        0        0     1134 2024-05-12 12:57:47.944073 abses-0.6.4/abses/viz/viz_actors.py
+-rw-r--r--   0        0        0     1149 2024-05-11 09:28:11.074327 abses-0.6.4/abses/viz/viz_model.py
+-rw-r--r--   0        0        0     4620 2024-05-11 09:28:11.074600 abses-0.6.4/abses/viz/viz_nature.py
+-rw-r--r--   0        0        0     6148 2024-04-14 20:25:37.202150 abses-0.6.4/data/.DS_Store
+-rw-r--r--   0        0        0  1653872 2023-09-03 00:55:23.536915 abses-0.6.4/data/YR_cities.zip
+-rw-r--r--   0        0        0   395561 2023-11-13 06:23:20.897117 abses-0.6.4/data/farmland.tif
+-rw-r--r--   0        0        0    84033 2023-09-02 23:31:24.485471 abses-0.6.4/data/irr_lands.csv
+-rw-r--r--   0        0        0  6726328 2023-03-03 00:57:27.899017 abses-0.6.4/data/precipitation.nc
+-rw-r--r--   0        0        0   189444 2024-05-11 09:28:11.085808 abses-0.6.4/icons/fa-regular-400.otf
+-rw-r--r--   0        0        0     2760 2024-05-16 13:00:46.169371 abses-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     7290 1970-01-01 00:00:00.000000 abses-0.6.4/PKG-INFO
```

### Comparing `abses-0.6.3.post0/LICENSE` & `abses-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/README.md` & `abses-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/abses/__init__.py` & `abses-0.6.4/abses/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,17 +25,19 @@
     "ActorsList",
     "PatchCell",
     "perception",
     "alive_required",
     "time_condition",
     "Experiment",
     "load_data",
+    "logger",
 ]
-__version__ = "v0.6.3.post"
+__version__ = "v0.6.4"
 
+from ._bases.logging import logger
 from .actor import Actor, alive_required, perception
 from .container import ActorsList
 from .data import load_data
 from .decision import Decision
 from .experiment import Experiment
 from .human import BaseHuman
 from .main import MainModel
```

### Comparing `abses-0.6.3.post0/abses/_bases/bases.py` & `abses-0.6.4/abses/_bases/bases.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,22 +12,19 @@
 
 The base class implements the observer pattern.
 It allows to observe all attribute changes in the main model.
 """
 
 from __future__ import annotations
 
-import logging
 from abc import ABCMeta
 from typing import List, Optional, Set, Union
 
 from abses.tools.func import make_list
 
-logger = logging.getLogger(__name__)
-
 
 class _Notice:
     """Notice class for the observer pattern."""
 
     __glob_vars__: Set[str] = set()
 
     def __init__(self, observer: Optional[_Observer] = None):
```

### Comparing `abses-0.6.3.post0/abses/_bases/components.py` & `abses-0.6.4/abses/_bases/components.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/abses/_bases/dynamic.py` & `abses-0.6.4/abses/_bases/dynamic.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/abses/_bases/modules.py` & `abses-0.6.4/abses/_bases/modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,25 +19,26 @@
     Generic,
     Iterator,
     List,
     Literal,
     Optional,
     Type,
     TypeVar,
+    cast,
 )
 
 from loguru import logger
 
 from abses._bases.bases import _Notice
 from abses._bases.objects import _BaseObj
 from abses._bases.states import _States
 from abses.tools.func import iter_func
 
 if TYPE_CHECKING:
-    from ..main import MainModel
+    from abses.main import MainModel
 
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
 HowCreation: TypeAlias = Literal["from_resolution", "from_file", "copy_layer"]
@@ -95,43 +96,46 @@
 ModuleType = TypeVar("ModuleType", bound=Module)
 
 
 class _ModuleFactory(Generic[ModuleType]):
     """To create a module."""
 
     methods: List[str] = []
-    default_cls: type[Module] = Module
+    default_cls: Type[Module] = Module
 
     def __init__(self, father) -> None:
         self.father: CompositeModule = father
         self.modules: Dict[str, ModuleType] = {}
 
+    def __str__(self) -> str:
+        return f"{self.father}: {list(self.modules.keys())}"
+
     def __iter__(self) -> Iterator[Module]:
         return iter(self.modules.values())
 
     def __getitem__(self, name: str) -> Module:
         return self.modules[name]
 
     def __contains__(self, name: str | ModuleType) -> bool:
         return name in self.modules or name in self.modules.values()
 
     def __len__(self) -> int:
         return len(self.modules)
 
     def _check_cls(
         self, module_cls: Optional[Type[ModuleType]]
-    ) -> Type[Module]:
+    ) -> Type[ModuleType]:
         """Check if the provided class is a valid module class."""
         if module_cls is None:
-            return self.default_cls
+            return cast(Type[ModuleType], self.default_cls)
         if not issubclass(module_cls, self.default_cls):
             raise TypeError(
                 f"'{module_cls}' not a subclass of {self.default_cls}."
             )
-        return module_cls
+        return cast(Type[ModuleType], module_cls)
 
     @property
     def is_empty(self) -> bool:
         """If the factory is empty."""
         return len(self.modules.keys()) == 0
 
     def _check_name(self, name: str) -> None:
@@ -163,28 +167,31 @@
                 If the module class is not a subclass of Module.
             ValueError:
                 If the creating method is not valid.
 
         Returns:
             The created module.
         """
-        self._check_cls(module_cls=module_class)
+        module_cls = self._check_cls(module_cls=module_class)
         if not how:
-            module = module_class(model=self.father.model, **kwargs)
+            module = module_cls(model=self.father.model, **kwargs)
         elif hasattr(self, how):
-            module = getattr(self, how)(model=self.father.model, **kwargs)
+            module = getattr(self, how)(
+                module_cls=module_cls, model=self.father.model, **kwargs
+            )
         else:
             raise ValueError(
                 f"{how} is not a valid method for creating module."
                 f"Choose from {self.methods} for {self.default_cls}"
             )
         # register as module
         self._check_name(module.name)
         self.modules[module.name] = module
         self.father.attach(module)
+        logger.info(f"{str(self.father)} created module {module.name}.")
         return module
 
 
 # Composite
 class CompositeModule(Module, _States, _Notice):
     """基本的组合模块，可以创建次级模块"""
```

### Comparing `abses-0.6.3.post0/abses/_bases/objects.py` & `abses-0.6.4/abses/_bases/objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Website: https://cv.songshgeo.com/
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional
 
 import mesa
+from loguru import logger
 
 from abses._bases.bases import _Observer
 from abses._bases.components import _Component
 from abses._bases.dynamic import _DynamicVariable
 from abses.time import TimeDriver
 
 if TYPE_CHECKING:
@@ -94,14 +95,15 @@
             function:
                 Function to calculate the dynamic variable.
         """
         var = _DynamicVariable(
             obj=self, name=name, data=data, function=function, **kwargs
         )
         self._dynamic_variables[name] = var
+        logger.info(f"Added dynamic variable '{var}'.")
 
     def dynamic_var(self, attr_name: str) -> Any:
         """Returns output of a dynamic variable.
 
         Parameters:
             attr_name:
                 Dynamic variable's name.
```

### Comparing `abses-0.6.3.post0/abses/_bases/states.py` & `abses-0.6.4/abses/_bases/states.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/abses/actor.py` & `abses-0.6.4/abses/actor.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,15 @@
         mg.GeoAgent.__init__(
             self, unique_id, model=model, geometry=geometry, crs=crs
         )
         _LinkNodeActor.__init__(self)
         self._cell: Optional[PatchCell] = None
         self._decisions: _DecisionFactory = self._setup_decisions()
         self._alive: bool = True
+        self._birth_tick: int = self.time.tick
         self._setup()
 
     def __repr__(self) -> str:
         return f"<{self.breed} [{self.unique_id}]>"
 
     def _setup_decisions(self) -> _DecisionFactory:
         """Decisions that this actor makes."""
@@ -242,14 +243,19 @@
         2. `move.off()`: removes the actor from the current layer.
         3. `move.by()`: moves the actor by a distance.
         4. `move.random()`: moves the actor to a random cell.
         """
         return _Movements(self)
 
     @alive_required
+    def age(self) -> int:
+        """Get the age of the actor."""
+        return self.time.tick - self._birth_tick
+
+    @alive_required
     def get(
         self,
         attr: str,
         target: Optional[TargetName] = None,
     ) -> Any:
         """Gets attribute value from target.
```

### Comparing `abses-0.6.3.post0/abses/cells.py` & `abses-0.6.4/abses/cells.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/abses/container.py` & `abses-0.6.4/abses/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     TYPE_CHECKING,
     Any,
     Callable,
     Iterable,
     Optional,
     Type,
     Union,
+    cast,
 )
 
 import numpy as np
 
 try:
     from typing import TypeAlias
 except ImportError:
@@ -177,15 +178,15 @@
         agents = creator.from_GeoDataFrame(gdf=gdf, unique_id=unique_id)
         self.register(agent_cls)
         self.add(agents)
         return ActorsList(model=self.model, objs=agents)
 
     def new(
         self,
-        breed_cls: Type[Actor],
+        breed_cls: Optional[Type[Actor]] = None,
         num: int = 1,
         singleton: bool = False,
         **kwargs: Any,
     ) -> Union[Actor, ActorsList[Actor]]:
         """Create one or more actors of the given breed class.
 
         Parameters:
@@ -210,31 +211,31 @@
             >>> Actor
 
             actors = model.agents.new(singleton=False)
             >>> type(actors)
             >>> ActorsList
             ```
         """
+        if breed_cls is None:
+            breed_cls = Actor
         # check if the breed class is registered, if not, register it.
         if not self.check_registration(breed_cls):
             self.register(breed_cls)
         # create actors.
         objs = [breed_cls(self._model, **kwargs) for _ in range(num)]
-        logger.info(f"Created {num} actors of breed {breed_cls.__name__}")
+        logger.debug(f"{self} created {num} {breed_cls.__name__}.")
         # add actors to the container and the schedule.
         for agent in objs:
             self.add(agent)
             self.model.schedule.add(agent)
         # return the created actor(s).
         actors_list: ActorsList[Actor] = ActorsList(
             model=self.model, objs=objs
         )
-        if singleton:
-            return objs[0] if num == 1 else actors_list
-        return actors_list
+        return cast(Actor, actors_list.item()) if singleton else actors_list
 
     def get(self, breeds: Breeds = None) -> ActorsList[Actor]:
         """Get all entities of specified breeds to a list.
 
         Parameters:
             breeds:
                 The breed(s) of entities to convert to a list.
```

### Comparing `abses-0.6.3.post0/abses/data.py` & `abses-0.6.4/abses/data.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/abses/decision.py` & `abses-0.6.4/abses/decision.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/abses/experiment.py` & `abses-0.6.4/abses/experiment.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 import pandas as pd
 from hydra import compose, initialize
 from hydra.core.global_hydra import GlobalHydra
 from hydra.core.hydra_config import HydraConfig
 from omegaconf import DictConfig, OmegaConf
 from tqdm.auto import tqdm
 
+from abses._bases.logging import setup_logger_info
 from abses.main import MainModel
 
 Configurations: TypeAlias = DictConfig | str | Dict[str, Any]
 
 
 def convert_to_python_type(value: Any) -> Any:
     """Convert numpy types to python native types.
@@ -90,15 +91,16 @@
 
 class Experiment:
     """Repeated Experiment."""
 
     _instance = None
     folder: Path = Path(os.getcwd())
     hydra_config: DictConfig = DictConfig({})
-    name: Optional[str] = None
+    exp_config: DictConfig = DictConfig({})
+    name: str = "ABSESpyExp"
     final_vars: List[Dict[str, Any]] = []
     model_vars: List[pd.DataFrame] = []
 
     def __new__(cls, *args, **kwargs):
         if not cls._instance:
             cls._instance = super().__new__(cls)
         return cls._instance
@@ -116,15 +118,16 @@
     def _update_config(
         cls,
         cfg: DictConfig,
         repeats: Optional[int] = None,
         number_process: Optional[int] = None,
     ) -> Tuple[int, int]:
         """Loading the configuration of this exp."""
-        exp_config: DictConfig = cfg.get("exp", DictConfig({}))
+        exp_config = cfg.get("exp", DictConfig({}))
+        cls.exp_config = exp_config
         if repeats is None:
             repeats = exp_config.get("repeats", 1)
         if number_process is None:
             number_process = exp_config.get("num_process", 1)
 
         cls.name = exp_config.get("name", "ABSESpyExp")
         if cls.is_hydra_job():
@@ -213,21 +216,42 @@
         """Initialize Hydra with overrides."""
         if self.is_hydra_job():
             return HydraConfig.get().cfg
         with initialize(version_base=None, config_path=str(cfg_path.parent)):
             cfg = compose(config_name=cfg_path.stem, overrides=overrides)
         return cfg
 
+    def _get_logging_mode(self, repeat_id: Optional[int] = None) -> str | bool:
+        log_mode = self.exp_config.get("logging", "once")
+        if log_mode == "once":
+            if repeat_id == 1:
+                logging: bool | str = self.name
+            else:
+                return False
+        elif bool(log_mode) is True:
+            logging = f"{self.name}_{repeat_id}"
+        else:
+            logging = False
+        return logging
+
     def run(
         self, cfg: DictConfig, repeat_id: int, outpath: Optional[Path] = None
     ) -> Tuple[Dict[str, Any], pd.DataFrame]:
         """运行模型一次"""
         if not self._model or not issubclass(self._model, MainModel):
             raise TypeError(f"The model class {self._model} is not valid.")
-        model = self._model(parameters=cfg, run_id=repeat_id, outpath=outpath)
+        # 获取日志
+        logging = self._get_logging_mode(repeat_id=repeat_id)
+        model = self._model(
+            parameters=cfg,
+            run_id=repeat_id,
+            outpath=outpath,
+            logging=logging,
+            experiment=self,
+        )
         model.run_model()
         if model.datacollector.model_reporters:
             df = model.datacollector.get_model_vars_dataframe()
         else:
             df = pd.DataFrame()
         return model.final_report(), df
 
@@ -411,15 +435,15 @@
         """
         cls.final_vars = []
         cls.model_vars = []
         if new_exp:
             cls._instance = None
             cls.folder = Path(os.getcwd())
             cls.hydra_config = DictConfig({})
-            cls.name = None
+            cls.name = "ABSESpyExp"
 
     @classmethod
     def new(cls, model_cls: Optional[Type[MainModel]] = None) -> Experiment:
         """Create a new experiment for the singleton class `Experiment`.
         This method will delete all currently available exp results and settings.
         Then, it initialize a new instance of experiment.
```

### Comparing `abses-0.6.3.post0/abses/human.py` & `abses-0.6.4/abses/human.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
             The agents container of this ABSESpy model.
         collections:
             Actor collections defined.
     """
 
     def __init__(self, model: MainModel[Any, Any], name: Optional[str] = None):
         Module.__init__(self, model, name)
-        logger.info("Initializing a new Human Module...")
         self._collections: Dict[str, Selection] = {}
 
     @property
     def agents(self) -> _AgentsContainer:
         """The agents container of this ABSESpy model."""
         return self.model.agents
```

### Comparing `abses-0.6.3.post0/abses/links.py` & `abses-0.6.4/abses/links.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/abses/main.py` & `abses-0.6.4/abses/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,21 @@
 """
 The main modelling framework of ABSESpy.
 """
 
 from __future__ import annotations
 
 import functools
+import json
 import os
-import sys
 import types
+from datetime import datetime
 from pathlib import Path
 from typing import (
+    TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Generic,
     List,
     Literal,
     Optional,
@@ -34,45 +36,38 @@
 import pandas as pd
 
 try:
     from typing import TypeAlias
 except ImportError:
     from typing_extensions import TypeAlias
 
-from loguru import logger
 from mesa import DataCollector, Model
 from mesa.time import BaseScheduler
 from omegaconf import DictConfig, OmegaConf
 
 from abses import __version__
+from abses._bases.logging import (
+    formatter,
+    log_session,
+    logger,
+    setup_logger_info,
+)
 from abses.actor import Actor
 
 from ._bases.bases import _Notice
 from ._bases.states import _States
 from .container import _AgentsContainer
 from .human import BaseHuman
 from .nature import BaseNature
 from .sequences import ActorsList
 from .time import TimeDriver
 from .viz.viz_model import _VizModel
 
-# Logging configuration
-logger.remove(0)
-logger.add(
-    sys.stderr,
-    format="[{time:YYYY-MM-DD HH:mm:ss}][{module:<15}] | {message}",
-    level="WARNING",
-)
-# 'w' mode in add() method will clean the contents of the logging.log file before writing to it
-logger.add(
-    "logging.log",
-    format="[{time:YYYY-MM-DD HH:mm:ss}][{module:<15}] | {message}",
-    level="DEBUG",
-    mode="w",
-)
+if TYPE_CHECKING:
+    from abses import Experiment
 
 # Dynamically load type hints from users' input type
 N = TypeVar("N", bound=BaseNature)
 H = TypeVar("H", bound=BaseHuman)
 Reporter: TypeAlias = Union[str, Callable[..., Any]]
 SubSystemType: TypeAlias = Literal["model", "nature", "human"]
 SubSystem = Union[
@@ -113,70 +108,118 @@
     def __init__(
         self,
         parameters: DictConfig = DictConfig({}),
         human_class: Optional[Type[H]] = None,
         nature_class: Optional[Type[N]] = None,
         run_id: Optional[int] = None,
         outpath: Optional[Path] = None,
+        experiment: Optional[Experiment] = None,
         **kwargs: Optional[Any],
     ) -> None:
         Model.__init__(self, **kwargs)
         _Notice.__init__(self)
         _States.__init__(self)
-
+        self._exp = experiment
+        self._run_id: Optional[int] = run_id
+        self.outpath = cast(Path, outpath)
+        self._setup_logger(kwargs.get("logging"))
         self.running: bool = True
         self._breeds: Dict[str, Type[Actor]] = {}
         self._containers: List[_AgentsContainer] = []
         self._settings = DictConfig(parameters)
         self._version: str = __version__
+        self._logging_begin()  # logging
         self._check_subsystems(h_cls=human_class, n_cls=nature_class)
         self._agents = _AgentsContainer(
             model=self, max_len=kwargs.get("max_agents")
         )
         self._time = TimeDriver(model=self)
-        self._run_id: Optional[int] = run_id
-        self.outpath = outpath
         self.schedule: BaseScheduler = BaseScheduler(model=self)
         self.initialize_data_collector()
         self._do_each("initialize", order=("nature", "human"))
         self._do_each("set_state", code=1)  # initial state
 
     def __repr__(self) -> str:
         version = self._version
         return f"<{self.name}-{version}({self.state})>"
 
+    def _logging_begin(self) -> None:
+        """Logging the beginning of the model."""
+        # settings = OmegaConf.to_container(self._settings)
+        msg = (
+            f"Model: {self.__class__.__name__}\n"
+            f"ABSESpy version: {__version__}\n"
+            f"Outpath: {self.outpath}\n"
+            # f"Model parameters: {json.dumps(settings, indent=4)}\n"
+        )
+        # logger.bind(data=self._settings).info("Params:")
+        log_session(title="MainModel", msg=msg)
+
+    def _logging_step(self) -> None:
+        if not self.breeds:
+            return
+        agents = self.agents.select({"_birth_tick": self.time.tick})
+        agents_dict = agents.to_dict()
+        lst = [f"{len(lst)} {breed}" for breed, lst in agents_dict.items()]
+        msg = (
+            f"\nIn [tick {self.time.tick - 1}]:"
+            "\n"
+            "Created " + ", ".join(lst) + ""
+        )
+        logger.bind(no_format=True).info(msg)
+
     def _check_subsystems(
         self, h_cls: Optional[Type[H]], n_cls: Optional[Type[N]]
     ) -> None:
         """Check if the subsystems are correctly set."""
         if h_cls is None:
             h_cls = cast(Type[H], BaseHuman)
         else:
             assert issubclass(h_cls, BaseHuman)
         if n_cls is None:
             n_cls = cast(Type[N], BaseNature)
         else:
             assert issubclass(n_cls, BaseNature)
         self._human = h_cls(self)
+        logger.info(f"Human subsystem: {h_cls.__name__}.")
         self._nature = n_cls(self)
+        logger.info(f"Natural subsystem: {n_cls.__name__}.")
 
     def _do_each(
         self,
         _func: str,
         order: SubSystem = ("model", "nature", "human"),
         **kwargs: Any,
     ) -> None:
         _obj = {"model": self, "nature": self.nature, "human": self.human}
         for name in order:
             if name not in _obj:
                 raise ValueError(f"{name} is not a valid component.")
             getattr(_obj[name], _func)(**kwargs)
 
+    def _setup_logger(self, logging: Optional[str] = None) -> None:
+        if not logging:
+            return
+        logging = str(logging).replace(".log", "")
+        logger.add(
+            self.outpath / f"{logging}.log",
+            retention="10 days",
+            rotation="1 day",
+            level="DEBUG",
+            format=formatter,
+        )
+        setup_logger_info(self.exp)
+
+    @property
+    def exp(self) -> Optional[Experiment]:
+        """Returns the associated experiment."""
+        return self._exp
+
     @property
-    def outpath(self) -> Optional[Path]:
+    def outpath(self) -> Path:
         """Output path where to deposit assets."""
         return self._outpath
 
     @outpath.setter
     def outpath(self, path: Optional[Path]) -> None:
         if path is None:
             path = Path(os.getcwd())
@@ -285,45 +328,56 @@
         1. Call `model.setup()` method.
         2. Call `model.step()` method.
         3. Repeating steps, until the end situation is triggered
         4. Call `model.end()` method.
         """
         self._setup()
         while self.running is True:
-            logger.debug(f"Current tick: {self.time.tick}")
-            self._step()
             self.time.go()
+            self._step()
             if self.time.tick == steps:
                 self.running = False
         self._end()
 
     def setup(self) -> None:
         """Users can custom what to do when the model is setup and going to start running."""
 
     def step(self) -> None:
         """A step of the model."""
 
     def end(self) -> None:
         """Users can custom what to do when the model is end."""
 
     def _setup(self) -> None:
-        logger.info(f"Setting up {self.name}...")
         self._do_each("setup", order=("model", "nature", "human"))
         self._do_each("set_state", code=2)
+        msg = (
+            f"Nature: {str(self.nature.modules)}\n"
+            f"Human: {str(self.human.modules)}\n"
+        )
+        log_session(title="Setting-up", msg=msg)
 
     def _step(self) -> None:
         self._do_each("step", order=("model", "nature", "human"))
         self.schedule.step()
         self.datacollector.collect(self)
+        self._logging_step()
 
     def _end(self) -> None:
         self._do_each("end", order=("nature", "human", "model"))
         self._do_each("set_state", code=3)
-        self.final_report()
-        logger.info(f"Ending {self.name}")
+        result = self.final_report()
+        msg = (
+            "The model is ended.\n"
+            f"Total ticks: {self.time.tick}\n"
+            f"Final result: {json.dumps(result, indent=4)}\n"
+        )
+        log_session(title="Ending Run", msg=msg)
+        logger.bind(no_format=True).info(f"{datetime.now()}\n\n\n")
+        logger.remove()
 
     def final_report(self) -> Dict[str, Any]:
         """Report at the end of this model."""
         result = {}
         for k, reporter in self._reports["final"].items():
             if isinstance(reporter, str):
                 value = getattr(self, reporter)
```

### Comparing `abses-0.6.3.post0/abses/move.py` & `abses-0.6.4/abses/move.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/abses/nature.py` & `abses-0.6.4/abses/nature.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
     overload,
 )
 
 import numpy as np
 import pyproj
 import rasterio
 import xarray as xr
-from loguru import logger
 from mesa.space import Coordinate
 
 from abses._bases.modules import CompositeModule, HowCreation
 from abses.cells import PatchCell
 from abses.patch import (
     CRS,
     CellFilter,
@@ -296,18 +295,22 @@
     def __init__(
         self, model: MainModel[Any, Any], name: str = "nature"
     ) -> None:
         CompositeModule.__init__(self, model, name=name)
         self._major_layer: Optional[PatchModule] = None
         self._modules: _PatchModuleFactory = _PatchModuleFactory(self)
 
-        logger.info("Initializing a new Base Nature module...")
-
     def __repr__(self) -> str:
-        return f"<BaseNature [{self.major_layer}]>"
+        major_layer = (
+            self.major_layer.name
+            if self.major_layer is not None
+            else "No major"
+        )
+        flag = "open" if self.opening else "closed"
+        return f"<nature ({major_layer}): {flag}>"
 
     def __getattribute__(self, name: str) -> PatchModule:
         """Get the submodule by name."""
         if name.startswith("_"):
             return super().__getattribute__(name)
         if hasattr(_PatchModuleProtocol, name):
             return getattr(self.major_layer, name)
```

### Comparing `abses-0.6.3.post0/abses/patch.py` & `abses-0.6.4/abses/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,14 @@
 
 
 class _PatchModuleFactory(_ModuleFactory):
     def __init__(self, father) -> None:
         super().__init__(father)
         self.default_cls = PatchModule
 
-    def __repr__(self) -> str:
-        return repr(self.father)
-
     def __getitem__(self, name: str) -> PatchModule:
         return self.modules[name]
 
     def from_resolution(
         self,
         model: MainModel[Any, Any],
         name: Optional[str] = None,
```

### Comparing `abses-0.6.3.post0/abses/random.py` & `abses-0.6.4/abses/random.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/abses/selection.py` & `abses-0.6.4/abses/selection.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/abses/sequences.py` & `abses-0.6.4/abses/sequences.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from abses.viz.viz_actors import _VizNodeList
 
 if TYPE_CHECKING:
     from abses.actor import Actor, TargetName
     from abses.links import _LinkNode
     from abses.main import MainModel
 
-Selection: TypeAlias = Union[str, Iterable[bool], Dict[str, bool]]
+Selection: TypeAlias = Union[str, Iterable[bool], Dict[str, Any]]
 HOW: TypeAlias = Literal["only", "random", "item"]
 Link = TypeVar("Link", bound="_LinkNode")
 
 
 def get_only_agent(agents: ActorsList) -> Actor:
     """Select one agent"""
     if len(agents) == 0:
```

### Comparing `abses-0.6.3.post0/abses/time.py` & `abses-0.6.4/abses/time.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,19 +19,21 @@
     List,
     Optional,
     Union,
     cast,
 )
 
 import pendulum
+from loguru import logger
 from omegaconf import DictConfig
 from pendulum.datetime import DateTime
 from pendulum.duration import Duration
 
 from abses._bases.components import _Component
+from abses._bases.logging import log_session
 
 if TYPE_CHECKING:
     from .main import MainModel
 
 try:
     from typing import Self
 except ImportError:
@@ -147,14 +149,15 @@
         self._model: MainModel[Any, Any] = model
         self._tick: int = 0
         self._start_dt: DateTime = pendulum.instance(datetime.now(), tz=None)
         self._end_dt: Optional[Union[DateTime, int]] = None
         self._duration: Optional[Duration] = None
         self._history: deque = deque()
         self._parse_time_settings()
+        self._logging_setup()
 
     def __repr__(self) -> str:
         if self.ticking_mode == "tick":
             return f"<TimeDriver: tick[{self.tick}]>"
         if self.ticking_mode == "duration":
             return f"<TimeDriver: {self.strftime('%Y-%m-%d %H:%M:%S')}>"
         return f"<TimeDriver: irregular[{self.tick}] {self.strftime('%Y-%m-%d %H:%M:%S')}>"
@@ -164,14 +167,22 @@
 
     def __lt__(self, other: object) -> bool:
         if isinstance(other, (DateTime, datetime)):
             return self.dt < other
         raise NotImplementedError(f"Cannot compare with {other}.")
 
     @property
+    def fmt(self) -> str:
+        """String format of datetime."""
+        hms = ("hours", "minutes", "seconds")
+        if any(getattr(self.duration, item, None) for item in hms):
+            return r"%Y-%m-%d %H:%M:%S"
+        return r"%Y-%m-%d"
+
+    @property
     def should_end(self) -> bool:
         """Should the model end or not."""
         if not self.end_dt:
             return False
         if isinstance(self.end_dt, datetime):
             return self.dt >= self.end_dt
         return self._tick >= self.end_dt
@@ -207,56 +218,70 @@
                 "Ticks cannot be zero unless the ticking mode is 'irregular'."
             )
         if ticks > 1:
             for _ in range(ticks):
                 self.go(ticks=1, **kwargs)
             return
         # tick = 1
+        dt_msg = f" {self.strftime()}" if self.duration else ""
+        tick_msg = f" [tick {self.tick}] "
+        logger.bind(no_format=True).info(
+            "\n" + f"{dt_msg}{tick_msg}".center(30, "-")
+        )
         self._tick += ticks
         if self.ticking_mode == "duration":
             self.dt += self.duration
             self._history.append(self.dt)
         elif self.ticking_mode == "irregular":
             self.dt += pendulum.duration(**kwargs)
             self._history.append(self.dt)
         elif self.ticking_mode != "tick":
             raise ValueError(f"Invalid ticking mode: {self.ticking_mode}")
         # end going
         if self.should_end:
             self._model.running = False
 
-    # def stdout(self) -> None:
-    #     """Print the current time."""
-    #     report = f"tick[{self.tick}] " + self.strftime("%Y-%m-%d %H:%M:%S")
-    #     # logger.info(report)
-    #     sys.stdout.write("\r" + report)
-    #     sys.stdout.flush()
-
     def _parse_time_settings(self) -> None:
         """Setup the time driver."""
         # Parse the start time settings
         self.start_dt = self.params.get("start", None)
-        # logger.debug(f"start_dt: {self.start_dt}")
 
         # Parse the end time settings
         self.end_dt = self.params.get("end", None)
-        # logger.debug(f"end_dt: {self.end_dt}")
 
         # Parse the duration settings
         self.parse_duration(self.params)
-        # logger.debug(f"duration: {self.duration}")
 
         # Parse the irregular settings
         self.irregular: bool = self.params.get("irregular", False)
-        # logger.debug("irregular: {}", self._irregular)
-        # logger.debug("Ticking mode: {}", self.ticking_mode)
 
         self.dt = self.start_dt
         self._history.append(self.dt)
 
+    def _logging_setup(self) -> None:
+        if self.ticking_mode == "duration":
+            end = (
+                self.end_dt.strftime(self.fmt)
+                if isinstance(self.end_dt, datetime)
+                else str(self.end_dt)
+            )
+            msg = (
+                f"Ticking mode: {self.ticking_mode}\n"
+                f"Start time: {self.start_dt.strftime(self.fmt)}\n"
+                f"End time: {end}\n"
+                f"Duration: {self.duration}\n"
+            )
+        else:
+            msg = (
+                f"Ticking mode: {self.ticking_mode}\n"
+                f"Start time: {self.start_dt.strftime(self.fmt)}\n"
+                f"End time: {self.end_dt}\n"
+            )
+        log_session(title="TimeDriver", msg=msg)
+
     @property
     def irregular(self) -> bool:
         """Returns the irregular mode of the time driver."""
         return self._irregular
 
     @irregular.setter
     def irregular(self, value: bool) -> None:
@@ -401,15 +426,19 @@
         return self.dt.weekday()
 
     @property
     def year(self) -> int:
         """Return the year this Period falls on."""
         return self.dt.year
 
-    def strftime(self, fmt: str) -> str:
+    def strftime(self, fmt: Optional[str] = None) -> str:
         """Returns a string representing the current time.
 
         Parameters:
             fmt:
                 An explicit format string of datetime.
         """
-        return self.dt.strftime(fmt)
+        return (
+            self.dt.strftime(self.fmt)
+            if fmt is None
+            else self.dt.strftime(fmt)
+        )
```

### Comparing `abses-0.6.3.post0/abses/tools/func.py` & `abses-0.6.4/abses/tools/func.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/abses/tools/regex.py` & `abses-0.6.4/abses/tools/regex.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/abses/viz/viz_actors.py` & `abses-0.6.4/abses/viz/viz_actors.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/abses/viz/viz_model.py` & `abses-0.6.4/abses/viz/viz_model.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/abses/viz/viz_nature.py` & `abses-0.6.4/abses/viz/viz_nature.py`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/data/.DS_Store` & `abses-0.6.4/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/data/YR_cities.zip` & `abses-0.6.4/data/YR_cities.zip`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/data/farmland.tif` & `abses-0.6.4/data/farmland.tif`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/data/irr_lands.csv` & `abses-0.6.4/data/irr_lands.csv`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/data/precipitation.nc` & `abses-0.6.4/data/precipitation.nc`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/icons/fa-regular-400.otf` & `abses-0.6.4/icons/fa-regular-400.otf`

 * *Files identical despite different names*

### Comparing `abses-0.6.3.post0/pyproject.toml` & `abses-0.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 79
 
 [tool.poetry]
 name = "abses"
-version = "0.6.3.post"
+version = "0.6.4"
 description = "ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour."
 authors = ["Shuang Song <songshgeo@gmail.com>"]
 license = "Apache 2.0 License"
 readme = "README.md"
 include = [
   "icons/fa-regular-400.otf",
   "abses/conf/**/*.yaml",
```

### Comparing `abses-0.6.3.post0/PKG-INFO` & `abses-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abses
-Version: 0.6.3.post0
+Version: 0.6.4
 Summary: ABSESpy makes it easier to build artificial Social-ecological systems with real GeoSpatial datasets and fully incorporate human behaviour.
 License: Apache 2.0 License
 Author: Shuang Song
 Author-email: songshgeo@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: abses Version: 0.6.3.post0 Summary: ABSESpy makes
-it easier to build artificial Social-ecological systems with real GeoSpatial
+Metadata-Version: 2.1 Name: abses Version: 0.6.4 Summary: ABSESpy makes it
+easier to build artificial Social-ecological systems with real GeoSpatial
 datasets and fully incorporate human behaviour. License: Apache 2.0 License
 Author: Shuang Song Author-email: songshgeo@gmail.com Requires-Python:
 >=3.9,<3.12 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: fiona (>1.8) Requires-
 Dist: fontawesome (>=5,<6) Requires-Dist: geopandas (>=0,<1) Requires-Dist:
```

