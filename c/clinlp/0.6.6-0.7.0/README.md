# Comparing `tmp/clinlp-0.6.6.tar.gz` & `tmp/clinlp-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinlp-0.6.6.tar", max compression
+gzip compressed data, was "clinlp-0.7.0.tar", max compression
```

## Comparing `clinlp-0.6.6.tar` & `clinlp-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0    35149 2024-04-24 13:20:39.652059 clinlp-0.6.6/LICENSE
--rw-r--r--   0        0        0    17326 2024-04-24 13:20:39.652059 clinlp-0.6.6/README.md
--rw-r--r--   0        0        0      997 2024-04-24 13:20:39.656059 clinlp-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      465 2024-04-24 13:20:39.656059 clinlp-0.6.6/src/clinlp/__init__.py
--rw-r--r--   0        0        0     7962 2024-04-24 13:20:39.656059 clinlp-0.6.6/src/clinlp/entity.py
--rw-r--r--   0        0        0       48 2024-04-24 13:20:39.656059 clinlp-0.6.6/src/clinlp/exceptions.py
--rw-r--r--   0        0        0     9052 2024-04-24 13:20:39.656059 clinlp-0.6.6/src/clinlp/language.py
--rw-r--r--   0        0        0     1656 2024-04-24 13:20:39.656059 clinlp-0.6.6/src/clinlp/normalizer.py
--rw-r--r--   0        0        0      726 2024-04-24 13:20:39.656059 clinlp-0.6.6/src/clinlp/qualifier/__init__.py
--rw-r--r--   0        0        0    12368 2024-04-24 13:20:39.656059 clinlp-0.6.6/src/clinlp/qualifier/context_algorithm.py
--rw-r--r--   0        0        0     3966 2024-04-24 13:20:39.656059 clinlp-0.6.6/src/clinlp/qualifier/qualifier.py
--rw-r--r--   0        0        0     7214 2024-04-24 13:20:39.656059 clinlp-0.6.6/src/clinlp/qualifier/transformer.py
--rw-r--r--   0        0        0        0 2024-04-24 13:20:39.656059 clinlp-0.6.6/src/clinlp/resources/__init__.py
--rw-r--r--   0        0        0    26538 2024-04-24 13:20:39.656059 clinlp-0.6.6/src/clinlp/resources/context_rules.json
--rw-r--r--   0        0        0     2412 2024-04-24 13:20:39.656059 clinlp-0.6.6/src/clinlp/sentencizer.py
--rw-r--r--   0        0        0     1939 2024-04-24 13:20:39.656059 clinlp-0.6.6/src/clinlp/util.py
--rw-r--r--   0        0        0    18155 1970-01-01 00:00:00.000000 clinlp-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-16 11:48:14.545758 clinlp-0.7.0/LICENSE
+-rw-r--r--   0        0        0    25871 2024-05-16 11:48:14.545758 clinlp-0.7.0/README.md
+-rw-r--r--   0        0        0     1084 2024-05-16 11:48:14.549758 clinlp-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      525 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/exceptions.py
+-rw-r--r--   0        0        0      121 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/ie/__init__.py
+-rw-r--r--   0        0        0     7962 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/ie/entity.py
+-rw-r--r--   0        0        0      740 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/ie/qualifier/__init__.py
+-rw-r--r--   0        0        0    13855 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/ie/qualifier/context_algorithm.py
+-rw-r--r--   0        0        0     4141 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/ie/qualifier/qualifier.py
+-rw-r--r--   0        0        0     7576 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/ie/qualifier/transformer.py
+-rw-r--r--   0        0        0     9053 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/language.py
+-rw-r--r--   0        0        0      123 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/metrics/__init__.py
+-rw-r--r--   0        0        0    22664 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/metrics/ie.py
+-rw-r--r--   0        0        0     1656 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/normalizer.py
+-rw-r--r--   0        0        0        0 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/resources/__init__.py
+-rw-r--r--   0        0        0    38312 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/resources/context_rules.json
+-rw-r--r--   0        0        0     2412 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/sentencizer.py
+-rw-r--r--   0        0        0     2173 2024-05-16 11:48:14.549758 clinlp-0.7.0/src/clinlp/util.py
+-rw-r--r--   0        0        0    26854 1970-01-01 00:00:00.000000 clinlp-0.7.0/PKG-INFO
```

### Comparing `clinlp-0.6.6/LICENSE` & `clinlp-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clinlp-0.6.6/pyproject.toml` & `clinlp-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [tool.poetry]
 name = "clinlp"
-version = "0.6.6"
+version = "0.7.0"
 description = "Performant and production-ready NLP pipelines for clinical text written in Dutch"
 authors = ["UMCU DIT Analytics <analytics@umcutrecht.nl>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 spacy = "^3.5.3"
 intervaltree = "^3.1.0"
 transformers = {extras = ["torch"], version = "^4.30.2"}
 makefun = "^1.15.1"
 pandas = "^2.2.0"
 pydantic = "^2.6.1"
 numpy = "^1.26.4"
+nervaluate = "^0.1.8"
+scikit-learn = "^1.4.2"
 
 [tool.poetry.extras]
 transformers = ["transformers"]
+metrics = ["nervaluate", "scikit-learn"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 ruff = "^0.4.1"
 
 [build-system]
```

### Comparing `clinlp-0.6.6/src/clinlp/entity.py` & `clinlp-0.7.0/src/clinlp/ie/entity.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.6.6/src/clinlp/language.py` & `clinlp-0.7.0/src/clinlp/language.py`

 * *Files 0% similar despite different names*

```diff
@@ -439,13 +439,13 @@
             if meta["clinlp_version"] != clinlp_version:
                 warnings.warn(
                     f"This spaCy model was built with clinlp version "
                     f"{meta['clinlp_version']}, but you currently have version "
                     f"{clinlp_version} installed, potentially leading to unexpected "
                     f"results.",
                     VersionMismatchWarning,
-                    stacklevel=2
+                    stacklevel=2,
                 )
         else:
             meta["clinlp_version"] = clinlp_version
 
         super().__init__(*args, meta=meta, **kwargs)
```

### Comparing `clinlp-0.6.6/src/clinlp/normalizer.py` & `clinlp-0.7.0/src/clinlp/normalizer.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.6.6/src/clinlp/qualifier/context_algorithm.py` & `clinlp-0.7.0/src/clinlp/ie/qualifier/context_algorithm.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,32 +9,33 @@
 from typing import Iterator, Optional, Union
 
 import intervaltree as ivt
 from spacy.language import Language
 from spacy.matcher import Matcher, PhraseMatcher
 from spacy.tokens import Doc, Span
 
-from clinlp.qualifier.qualifier import (
+from clinlp.ie.qualifier.qualifier import (
     ATTR_QUALIFIERS,
     Qualifier,
+    QualifierClass,
     QualifierDetector,
-    QualifierFactory,
 )
-from clinlp.util import clinlp_autocomponent
+from clinlp.util import clinlp_autocomponent, interval_dist
 
 
 class ContextRuleDirection(Enum):
     """
     Direction of a Context rule, as in the original Context Algorithm.
     """
 
     PRECEDING = 1
     FOLLOWING = 2
-    PSEUDO = 3
-    TERMINATION = 4
+    BIDIRECTIONAL = 3
+    PSEUDO = 4
+    TERMINATION = 5
 
 
 @dataclass
 class ContextRule:
     """
     A Context rule, as in the original Context Algorithm.
 
@@ -74,19 +75,25 @@
         """
 
         max_scope = self.rule.max_scope or len(sentence)
 
         if max_scope < 1:
             raise ValueError(f"max_scope must be at least 1, but got {max_scope}")
 
+        scoped_start = max(self.start - max_scope, sentence.start)
+        scoped_end = min(self.end + max_scope, sentence.end)
+
         if self.rule.direction == ContextRuleDirection.PRECEDING:
-            self.scope = (self.start, min(self.end + max_scope, sentence.end))
+            self.scope = (self.start, scoped_end)
 
         elif self.rule.direction == ContextRuleDirection.FOLLOWING:
-            self.scope = (max(self.start - max_scope, sentence.start), self.end)
+            self.scope = (scoped_start, self.end)
+
+        elif self.rule.direction == ContextRuleDirection.BIDIRECTIONAL:
+            self.scope = (scoped_start, scoped_end)
 
 
 _defaults_context_algorithm = {
     "phrase_matcher_attr": "TEXT",
     "load_rules": True,
     "rules": str(
         importlib.resources.files("clinlp.resources").joinpath("context_rules.json")
@@ -125,29 +132,29 @@
     ) -> None:
         self._nlp = nlp
 
         self._matcher = Matcher(self._nlp.vocab)
         self._phrase_matcher = PhraseMatcher(self._nlp.vocab, attr=phrase_matcher_attr)
 
         self.rules = {}
-        self._qualifier_factories = {}
+        self._qualifier_classes = {}
 
         if load_rules:
             if rules is None:
                 raise ValueError(
                     "Did not provide rules. Set `load_rules` to False if you "
                     "want to add `ContextRule` manually."
                 )
 
             rules = self._parse_rules(rules)
             self.add_rules(rules)
 
     @property
-    def qualifier_factories(self) -> dict[str, QualifierFactory]:
-        return self._qualifier_factories
+    def qualifier_classes(self) -> dict[str, QualifierClass]:
+        return self._qualifier_classes
 
     def add_rule(self, rule: ContextRule) -> None:
         """
         Add a rule.
         """
         rule_key = f"rule_{len(self.rules)}"
         self.rules[rule_key] = rule
@@ -169,15 +176,15 @@
         Add multiple rules.
         """
         for rule in rules:
             self.add_rule(rule)
 
     @staticmethod
     def _parse_qualifier(
-        qualifier: str, qualifier_factories: dict[str, QualifierFactory]
+        qualifier: str, qualifier_classes: dict[str, QualifierClass]
     ) -> Qualifier:
         """
         Parse a Qualifier from string.
 
         Args:
             qualifier: The qualifier (e.g. Negation.NEGATED).
 
@@ -190,15 +197,15 @@
             raise ValueError(
                 f"Cannot parse qualifier {qualifier}, please adhere to format "
                 f"{match_regexp} (e.g. NegationQualifier.NEGATED)"
             )
 
         qualifier_class, qualifier = qualifier.split(".")
 
-        return qualifier_factories[qualifier_class].create(value=qualifier)
+        return qualifier_classes[qualifier_class].create(value=qualifier)
 
     @staticmethod
     def _parse_direction(direction: str) -> ContextRuleDirection:
         """
         Parse a Context direction.
 
         Args:
@@ -210,22 +217,20 @@
 
     def _parse_rules(self, rules: Union[str | dict]) -> list[ContextRule]:
         if isinstance(rules, str):
             with open(rules, "rb") as file:
                 rules = json.load(file)
 
         for qualifier in rules["qualifiers"]:
-            self._qualifier_factories[qualifier["name"]] = QualifierFactory(**qualifier)
+            self._qualifier_classes[qualifier["name"]] = QualifierClass(**qualifier)
 
         qualifier_rules = []
 
         for rule in rules["rules"]:
-            qualifier = self._parse_qualifier(
-                rule["qualifier"], self.qualifier_factories
-            )
+            qualifier = self._parse_qualifier(rule["qualifier"], self.qualifier_classes)
             direction = self._parse_direction(rule["direction"])
             max_scope = rule.get("max_scope", None)
 
             qualifier_rules += [
                 ContextRule(pattern, qualifier, direction, max_scope)
                 for pattern in rule["patterns"]
             ]
@@ -273,21 +278,21 @@
 
         for terminate_match in terminations:
             for interval in scopes.overlap(terminate_match.start, terminate_match.end):
                 scopes.remove(interval)
                 match = interval.data
 
                 if (
-                    match.rule.direction == ContextRuleDirection.PRECEDING
+                    match.rule.direction != ContextRuleDirection.FOLLOWING
                     and terminate_match.start >= match.end
                 ):
                     match.scope = (match.scope[0], terminate_match.start)
 
                 if (
-                    match.rule.direction == ContextRuleDirection.FOLLOWING
+                    match.rule.direction != ContextRuleDirection.PRECEDING
                     and terminate_match.end <= match.start
                 ):
                     match.scope = (terminate_match.end, match.scope[1])
 
                 scopes[match.scope[0] : match.scope[1]] = match
 
         return scopes
@@ -301,21 +306,22 @@
         match_scopes = ivt.IntervalTree()
 
         for qualifier_matches in self._group_matched_patterns(
             matched_patterns
         ).values():
             preceding = qualifier_matches[ContextRuleDirection.PRECEDING]
             following = qualifier_matches[ContextRuleDirection.FOLLOWING]
+            bidirectional = qualifier_matches[ContextRuleDirection.BIDIRECTIONAL]
             pseudo = qualifier_matches[ContextRuleDirection.PSEUDO]
             termination = qualifier_matches[ContextRuleDirection.TERMINATION]
 
             qualifier_matches = ivt.IntervalTree()
 
             # Following, preceding
-            for match in preceding + following:
+            for match in preceding + following + bidirectional:
                 qualifier_matches[match.start : match.end] = match
 
             # Pseudo
             for match in pseudo:
                 qualifier_matches.remove_overlap(match.start, match.end)
 
             # Termination
@@ -326,14 +332,42 @@
 
             match_scopes |= self._limit_scopes_from_terminations(
                 qualifier_scopes, termination
             )
 
         return match_scopes
 
+    def _resolve_matched_pattern_conflicts(
+        self, entity: Span, matched_patterns: list[_MatchedContextPattern]
+    ) -> list[_MatchedContextPattern]:
+        if len(matched_patterns) <= 1:
+            return matched_patterns
+
+        grouped_patterns = defaultdict(list)
+        result_patterns = []
+
+        for mp in matched_patterns:
+            grouped_patterns[mp.rule.qualifier.name].append(mp)
+
+        for mp_group in grouped_patterns.values():
+            if len(mp_group) == 1:
+                result_patterns += mp_group
+            else:
+                result_patterns.append(
+                    min(
+                        mp_group,
+                        key=lambda mp: (
+                            interval_dist(entity.start, entity.end, mp.start, mp.end),
+                            -mp.rule.qualifier.priority,
+                        ),
+                    )
+                )
+
+        return result_patterns
+
     def _detect_qualifiers(self, doc: Doc):
         """
         Apply the Context Algorithm to a doc.
         """
 
         if len(self.rules) == 0:
             raise RuntimeError("Cannot match qualifiers without any ContextRule.")
@@ -352,30 +386,37 @@
             for match_id, start, end in matches:
                 rule = self._get_rule_from_match_id(match_id)
 
                 # spacy Matcher handles offset differently than PhraseMatcher,
                 # when applying the matcher to a sentence
                 offset = sentence.start if isinstance(rule.pattern, list) else 0
 
-                pattern = _MatchedContextPattern(
+                matched_pattern = _MatchedContextPattern(
                     rule=self._get_rule_from_match_id(match_id),
                     start=start,
                     end=end,
                     offset=offset,
                 )
 
-                pattern.initialize_scope(sentence)
-                matched_patterns.append(pattern)
+                matched_pattern.initialize_scope(sentence)
+                matched_patterns.append(matched_pattern)
 
             match_scopes = self._compute_match_scopes(matched_patterns)
 
             for ent in sentence.ents:
+                matched_patterns = []
+
                 for match_interval in match_scopes.overlap(ent.start, ent.end):
                     if (ent.start + 1 > match_interval.data.end) or (
                         ent.end < match_interval.data.start + 1
                     ):
-                        self.add_qualifier_to_ent(
-                            ent, match_interval.data.rule.qualifier
-                        )
+                        matched_patterns.append(match_interval.data)
+
+                matched_patterns = self._resolve_matched_pattern_conflicts(
+                    ent, matched_patterns
+                )
+
+                for matched_pattern in matched_patterns:
+                    self.add_qualifier_to_ent(ent, matched_pattern.rule.qualifier)
 
     def __len__(self) -> int:
         return len(self.rules)
```

### Comparing `clinlp-0.6.6/src/clinlp/qualifier/qualifier.py` & `clinlp-0.7.0/src/clinlp/ie/qualifier/qualifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,96 +41,102 @@
 
 
 @dataclass(frozen=True)
 class Qualifier:
     name: str = field(compare=True)
     value: str = field(compare=True)
     is_default: bool = field(compare=True)
+    priority: int = field(default=0, compare=False)
     prob: Optional[float] = field(default=None, compare=False)
 
     def to_dict(self) -> dict:
         return {
             "name": self.name,
             "value": self.value,
             "is_default": self.is_default,
             "prob": self.prob,
         }
 
     def __str__(self) -> str:
         return f"{self.name}.{self.value}"
 
 
-class QualifierFactory:
-    def __init__(self, name: str, values: list[str], default: Optional[str] = None):
+class QualifierClass:
+    def __init__(
+        self,
+        name: str,
+        values: list[str],
+        default: Optional[str] = None,
+        priorities: Optional[dict] = None,
+    ):
         self.name = name
+        self.values = values
         self.default = default or values[0]
+        self.priorities = priorities or {value: n for n, value in enumerate(values)}
 
         if len(set(values)) != len(values):
             raise ValueError(f"Please do not provide any duplicate values ({values})")
 
         if self.default not in values:
             raise ValueError(f"Default {default} not in provided value {values}")
 
-        self.values = values
-
     def create(self, value: Optional[str] = None, **kwargs) -> Qualifier:
         if value is None:
             value = self.default
 
         if value not in self.values:
             raise ValueError(
                 f"The qualifier {self.name} cannot take value '{value}'. "
                 f"Please choose one of {self.values}."
             )
 
         is_default = value == self.default
+        priority = self.priorities[value]
 
-        return Qualifier(name=self.name, value=value, is_default=is_default, **kwargs)
+        return Qualifier(
+            name=self.name,
+            value=value,
+            is_default=is_default,
+            priority=priority,
+            **kwargs,
+        )
 
 
 class QualifierDetector(ABC):
     """For usage as a spaCy pipeline component"""
 
     @property
     @abstractmethod
-    def qualifier_factories(self) -> dict[str, QualifierFactory]:
-        pass
-
-    @abstractmethod
-    def _detect_qualifiers(self, doc: Doc) -> None:
+    def qualifier_classes(self) -> dict[str, QualifierClass]:
         pass
 
     @staticmethod
     def add_qualifier_to_ent(entity: Span, new_qualifier: Qualifier) -> None:
         qualifiers = get_qualifiers(entity)
 
         if qualifiers is None:
             raise RuntimeError(
                 "Cannot add qualifier to entity with non-initialized qualifiers."
             )
 
-        try:
-            old_qualifier = next(
-                iter(q for q in qualifiers if q.name == new_qualifier.name)
-            )
-
-            qualifiers.remove(old_qualifier)
-            qualifiers.add(new_qualifier)
-
-        except StopIteration:
-            qualifiers.add(new_qualifier)
+        qualifiers = {q for q in qualifiers if q.name != new_qualifier.name}
+        qualifiers.add(new_qualifier)
 
         set_qualifiers(entity, qualifiers)
 
     def _initialize_ent_qualifiers(self, entity: Span) -> None:
         if get_qualifiers(entity) is None:
             set_qualifiers(entity, set())
 
-        for _, factory in self.qualifier_factories.items():
-            self.add_qualifier_to_ent(entity, factory.create())
+        for _, qualifier_class in self.qualifier_classes.items():
+            self.add_qualifier_to_ent(entity, qualifier_class.create())
+
+    @abstractmethod
+    def _detect_qualifiers(self, doc: Doc) -> None:
+        pass
 
     def __call__(self, doc: Doc) -> Doc:
         if len(doc.ents) == 0:
             return doc
 
         for ent in doc.ents:
             self._initialize_ent_qualifiers(ent)
```

### Comparing `clinlp-0.6.6/src/clinlp/qualifier/transformer.py` & `clinlp-0.7.0/src/clinlp/ie/qualifier/transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from typing import Callable, Optional, Tuple
 
 import torch
 from spacy import Language
 from spacy.tokens import Doc, Span
 from transformers import AutoTokenizer, RobertaForTokenClassification
 
-from clinlp.qualifier.qualifier import (
+from clinlp.ie.qualifier.qualifier import (
     ATTR_QUALIFIERS,
+    QualifierClass,
     QualifierDetector,
-    QualifierFactory,
 )
 from clinlp.util import clinlp_autocomponent
 
 HF_FROM_PRETRAINED_NEGATION = {
     "pretrained_model_name_or_path": "UMCU/MedRoBERTa.nl_NegationDetection",
     "revision": "83068ba132b6ce38e9f668c1e3ab636f79b774d3",
 }
@@ -27,15 +27,16 @@
     "token_window": 32,
     "strip_entities": True,
     "placeholder": None,
     "prob_aggregator": statistics.mean,
 }
 
 _defaults_negation_transformer = {
-    "negation_threshold": 0.5,
+    "absence_threshold": 0.1,
+    "presence_threshold": 0.9,
 }
 _defaults_experiencer_transformer = {
     "token_window": 64,
     "other_threshold": 0.5,
 }
 
 
@@ -128,54 +129,62 @@
     default_config=_defaults_negation_transformer,
 )
 @clinlp_autocomponent
 class NegationTransformer(QualifierTransformer):
     def __init__(
         self,
         nlp: Language,
-        negation_threshold: float = _defaults_negation_transformer[
-            "negation_threshold"
+        absence_threshold: float = _defaults_negation_transformer["absence_threshold"],
+        presence_threshold: float = _defaults_negation_transformer[
+            "presence_threshold"
         ],
         **kwargs,
     ) -> None:
         self.nlp = nlp
-        self.negation_threshold = negation_threshold
+        self.absence_threshold = absence_threshold
+        self.presence_threshold = presence_threshold
 
         self.tokenizer = AutoTokenizer.from_pretrained(**HF_FROM_PRETRAINED_NEGATION)
         self.model = RobertaForTokenClassification.from_pretrained(
             **HF_FROM_PRETRAINED_NEGATION
         )
 
         super().__init__(**kwargs)
 
     @property
-    def qualifier_factories(self) -> dict[str, QualifierFactory]:
+    def qualifier_classes(self) -> dict[str, QualifierClass]:
         return {
-            "Negation": QualifierFactory(
-                "Negation", ["Affirmed", "Negated"], default="Affirmed"
+            "Presence": QualifierClass(
+                "Presence", ["Absent", "Uncertain", "Present"], default="Present"
             )
         }
 
     def _detect_qualifiers(self, doc: Doc):
         for ent in doc.ents:
             text, ent_start_char, ent_end_char = self._prepare_ent(ent)
 
-            prob = self._predict(
+            prob = 1 - self._predict(
                 text,
                 ent_start_char,
                 ent_end_char,
                 prob_indices=[0, 2],
                 prob_aggregator=self.prob_aggregator,
             )
 
-            if prob > self.negation_threshold:
-                self.add_qualifier_to_ent(
-                    ent,
-                    self.qualifier_factories["Negation"].create("Negated", prob=prob),
-                )
+            if prob <= self.absence_threshold:
+                qualifier_value = "Absent"
+            elif prob >= self.presence_threshold:
+                qualifier_value = "Present"
+            else:
+                qualifier_value = "Uncertain"
+
+            self.add_qualifier_to_ent(
+                ent,
+                self.qualifier_classes["Presence"].create(qualifier_value, prob=prob),
+            )
 
 
 @Language.factory(
     name="clinlp_experiencer_transformer",
     requires=["doc.ents"],
     assigns=[f"span._.{ATTR_QUALIFIERS}"],
     default_config=_defaults_experiencer_transformer,
@@ -195,18 +204,18 @@
         self.model = RobertaForTokenClassification.from_pretrained(
             **HF_FROM_PRETRAINED_EXPERIENCER
         )
 
         super().__init__(**kwargs)
 
     @property
-    def qualifier_factories(self) -> dict[str, QualifierFactory]:
+    def qualifier_classes(self) -> dict[str, QualifierClass]:
         return {
-            "Experiencer": QualifierFactory(
-                "Experiencer", ["Patient", "Other"], default="Patient"
+            "Experiencer": QualifierClass(
+                "Experiencer", ["Patient", "Family"], default="Patient"
             )
         }
 
     def _detect_qualifiers(self, doc: Doc):
         for ent in doc.ents:
             text, ent_start_char, ent_end_char = self._prepare_ent(ent)
 
@@ -217,9 +226,9 @@
                 prob_indices=[1, 3],
                 prob_aggregator=self.prob_aggregator,
             )
 
             if prob > self.other_threshold:
                 self.add_qualifier_to_ent(
                     ent,
-                    self.qualifier_factories["Experiencer"].create("Other", prob=prob),
+                    self.qualifier_classes["Experiencer"].create("Family", prob=prob),
                 )
```

### Comparing `clinlp-0.6.6/src/clinlp/resources/context_rules.json` & `clinlp-0.7.0/src/clinlp/resources/context_rules.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.706885368829592%*

 * *Differences: {"'description'": "'The default set of context rules included in clinlp. Intially based on the "*

 * *                  "psynlp package, further improved since.'",*

 * * "'qualifiers'": "{0: {'name': 'Presence', 'values': ['Absent', 'Uncertain', 'Present'], "*

 * *                 "'default': 'Present', 'priorities': OrderedDict([('Present', 0), ('Uncertain', "*

 * *                 "1), ('Absent', 2)])}, 1: {'name': 'Temporality', 'values': ['Historical', "*

 * *                 "'Current', 'Future'], 'default': 'Current', 'priori […]*

```diff
@@ -1,646 +1,241 @@
 {
-    "description": "A set of context rules intially based on the psynlp package, somewhat tailored on a per use case basis.",
+    "description": "The default set of context rules included in clinlp. Intially based on the psynlp package, further improved since.",
     "name": "default_qualifiers",
     "qualifiers": [
         {
-            "default": "Patient",
-            "name": "Experiencer",
+            "default": "Present",
+            "name": "Presence",
+            "priorities": {
+                "Absent": 2,
+                "Present": 0,
+                "Uncertain": 1
+            },
             "values": [
-                "Patient",
-                "Other"
+                "Absent",
+                "Uncertain",
+                "Present"
             ]
         },
         {
-            "default": "Affirmed",
-            "name": "Negation",
-            "values": [
-                "Affirmed",
-                "Negated"
-            ]
-        },
-        {
-            "default": "Plausible",
-            "name": "Plausibility",
+            "default": "Current",
+            "name": "Temporality",
+            "priorities": {
+                "Current": 0,
+                "Future": 1,
+                "Historical": 2
+            },
             "values": [
-                "Plausible",
-                "Hypothetical"
+                "Historical",
+                "Current",
+                "Future"
             ]
         },
         {
-            "default": "Current",
-            "name": "Temporality",
+            "default": "Patient",
+            "name": "Experiencer",
+            "priorities": {
+                "Family": 2,
+                "Other": 1,
+                "Patient": 0
+            },
             "values": [
-                "Current",
-                "Historical"
+                "Patient",
+                "Family",
+                "Other"
             ]
         }
     ],
     "rules": [
         {
             "direction": "preceding",
-            "patterns": [
-                "familieanamnese",
-                "familie-anamnese",
-                "familie anamnese",
-                "familiair",
-                "familiaire",
-                "familieleden",
-                "familiegeschiedenis",
-                "moederszijde",
-                "vaderszijde",
-                [
-                    {
-                        "LOWER": {
-                            "IN": [
-                                "vader",
-                                "vdr",
-                                "moeder",
-                                "mdr",
-                                "broer",
-                                "broertje",
-                                "zus",
-                                "zusje",
-                                "oom",
-                                "tante",
-                                "neef",
-                                "neefje",
-                                "nicht",
-                                "nichtje",
-                                "opa",
-                                "oma",
-                                "grootvader",
-                                "grootmoeder",
-                                "buurman",
-                                "buurvrouw",
-                                "zoon",
-                                "zoontje",
-                                "dochter",
-                                "dochtertje",
-                                "huisgenoot",
-                                "huisgenote",
-                                "familie",
-                                "broers",
-                                "broertjes",
-                                "zussen",
-                                "zusjes",
-                                "ooms",
-                                "tantes",
-                                "neven",
-                                "neefjes",
-                                "nichten",
-                                "nichtjes",
-                                "zoons",
-                                "zoontjes",
-                                "dochters",
-                                "dochtertjes",
-                                "huisgenoten",
-                                "huisgenotes"
-                            ]
-                        }
-                    }
-                ],
-                [
-                    {
-                        "LOWER": {
-                            "IN": [
-                                "vader",
-                                "vdr",
-                                "moeder",
-                                "mdr",
-                                "broer",
-                                "broertje",
-                                "zus",
-                                "zusje",
-                                "oom",
-                                "tante",
-                                "neef",
-                                "neefje",
-                                "nicht",
-                                "nichtje",
-                                "opa",
-                                "oma",
-                                "grootvader",
-                                "grootmoeder",
-                                "buurman",
-                                "buurvrouw",
-                                "zoon",
-                                "zoontje",
-                                "dochter",
-                                "dochtertje",
-                                "huisgenoot",
-                                "huisgenote",
-                                "familie"
-                            ]
-                        }
-                    },
-                    {
-                        "LOWER": {
-                            "IN": [
-                                "zijn",
-                                "haar"
-                            ]
-                        }
-                    }
-                ],
-                [
-                    {
-                        "LOWER": {
-                            "IN": [
-                                "broers",
-                                "broertjes",
-                                "zussen",
-                                "zusjes",
-                                "ooms",
-                                "tantes",
-                                "neven",
-                                "neefjes",
-                                "nichten",
-                                "nichtjes",
-                                "zoons",
-                                "zoontjes",
-                                "dochters",
-                                "dochtertjes",
-                                "huisgenoten",
-                                "huisgenotes"
-                            ]
-                        }
-                    },
-                    {
-                        "LOWER": "hun"
-                    }
-                ],
-                [
-                    {
-                        "LOWER": {
-                            "IN": [
-                                "vader",
-                                "vdr",
-                                "moeder",
-                                "mdr",
-                                "broer",
-                                "broertje",
-                                "zus",
-                                "zusje",
-                                "oom",
-                                "tante",
-                                "neef",
-                                "neefje",
-                                "nicht",
-                                "nichtje",
-                                "opa",
-                                "oma",
-                                "grootvader",
-                                "grootmoeder",
-                                "buurman",
-                                "buurvrouw",
-                                "zoon",
-                                "zoontje",
-                                "dochter",
-                                "dochtertje",
-                                "huisgenoot",
-                                "huisgenote",
-                                "familie"
-                            ]
-                        }
-                    },
-                    {
-                        "LOWER": "'"
-                    },
-                    {
-                        "LOWER": "s"
-                    }
-                ]
-            ],
-            "qualifier": "Experiencer.Other"
-        },
-        {
-            "direction": "following",
-            "patterns": [
-                "in de familie",
-                "in familie",
-                [
-                    {
-                        "LOWER": "bij"
-                    },
-                    {
-                        "LOWER": {
-                            "IN": [
-                                "vader",
-                                "vdr",
-                                "moeder",
-                                "mdr",
-                                "broer",
-                                "broertje",
-                                "zus",
-                                "zusje",
-                                "oom",
-                                "tante",
-                                "neef",
-                                "neefje",
-                                "nicht",
-                                "nichtje",
-                                "opa",
-                                "oma",
-                                "grootvader",
-                                "grootmoeder",
-                                "buurman",
-                                "buurvrouw",
-                                "zoon",
-                                "zoontje",
-                                "dochter",
-                                "dochtertje",
-                                "huisgenoot",
-                                "huisgenote",
-                                "familie",
-                                "broers",
-                                "broertjes",
-                                "zussen",
-                                "zusjes",
-                                "ooms",
-                                "tantes",
-                                "neven",
-                                "neefjes",
-                                "nichten",
-                                "nichtjes",
-                                "zoons",
-                                "zoontjes",
-                                "dochters",
-                                "dochtertjes",
-                                "huisgenoten",
-                                "huisgenotes"
-                            ]
-                        }
-                    }
-                ]
-            ],
-            "qualifier": "Experiencer.Other"
-        },
-        {
-            "direction": "pseudo",
-            "patterns": [
-                "door familie",
-                "familie",
-                "met familie",
-                "naar familie",
-                [
-                    {
-                        "LOWER": {
-                            "IN": [
-                                "door",
-                                "met",
-                                "naar",
-                                "volgens",
-                                "vertelt",
-                                "vertelde",
-                                "vertellen",
-                                "vertelden"
-                            ]
-                        }
-                    },
-                    {
-                        "LOWER": {
-                            "IN": [
-                                "vader",
-                                "vdr",
-                                "moeder",
-                                "mdr",
-                                "broer",
-                                "broertje",
-                                "zus",
-                                "zusje",
-                                "oom",
-                                "tante",
-                                "neef",
-                                "neefje",
-                                "nicht",
-                                "nichtje",
-                                "opa",
-                                "oma",
-                                "grootvader",
-                                "grootmoeder",
-                                "buurman",
-                                "buurvrouw",
-                                "zoon",
-                                "zoontje",
-                                "dochter",
-                                "dochtertje",
-                                "huisgenoot",
-                                "huisgenote",
-                                "familie",
-                                "broers",
-                                "broertjes",
-                                "zussen",
-                                "zusjes",
-                                "ooms",
-                                "tantes",
-                                "neven",
-                                "neefjes",
-                                "nichten",
-                                "nichtjes",
-                                "zoons",
-                                "zoontjes",
-                                "dochters",
-                                "dochtertjes",
-                                "huisgenoten",
-                                "huisgenotes"
-                            ]
-                        }
-                    }
-                ],
-                [
-                    {
-                        "LOWER": {
-                            "IN": [
-                                "vader",
-                                "vdr",
-                                "moeder",
-                                "mdr",
-                                "broer",
-                                "broertje",
-                                "zus",
-                                "zusje",
-                                "oom",
-                                "tante",
-                                "neef",
-                                "neefje",
-                                "nicht",
-                                "nichtje",
-                                "opa",
-                                "oma",
-                                "grootvader",
-                                "grootmoeder",
-                                "buurman",
-                                "buurvrouw",
-                                "zoon",
-                                "zoontje",
-                                "dochter",
-                                "dochtertje",
-                                "huisgenoot",
-                                "huisgenote",
-                                "familie",
-                                "broers",
-                                "broertjes",
-                                "zussen",
-                                "zusjes",
-                                "ooms",
-                                "tantes",
-                                "neven",
-                                "neefjes",
-                                "nichten",
-                                "nichtjes",
-                                "zoons",
-                                "zoontjes",
-                                "dochters",
-                                "dochtertjes",
-                                "huisgenoten",
-                                "huisgenotes"
-                            ]
-                        }
-                    },
-                    {
-                        "LOWER": {
-                            "IN": [
-                                "belde",
-                                "belden",
-                                "zei",
-                                "zeiden",
-                                "vond",
-                                "vonden",
-                                "vertelt",
-                                "vertelde",
-                                "vertellen",
-                                "vertelden"
-                            ]
-                        }
-                    }
-                ],
-                [
-                    {
-                        "LOWER": {
-                            "IN": [
-                                "vader",
-                                "vdr",
-                                "moeder",
-                                "mdr",
-                                "broer",
-                                "broertje",
-                                "zus",
-                                "zusje",
-                                "oom",
-                                "tante",
-                                "neef",
-                                "neefje",
-                                "nicht",
-                                "nichtje",
-                                "opa",
-                                "oma",
-                                "grootvader",
-                                "grootmoeder",
-                                "buurman",
-                                "buurvrouw",
-                                "zoon",
-                                "zoontje",
-                                "dochter",
-                                "dochtertje",
-                                "huisgenoot",
-                                "huisgenote",
-                                "familie",
-                                "broers",
-                                "broertjes",
-                                "zussen",
-                                "zusjes",
-                                "ooms",
-                                "tantes",
-                                "neven",
-                                "neefjes",
-                                "nichten",
-                                "nichtjes",
-                                "zoons",
-                                "zoontjes",
-                                "dochters",
-                                "dochtertjes",
-                                "huisgenoten",
-                                "huisgenotes"
-                            ]
-                        }
-                    },
-                    {
-                        "LOWER": {
-                            "IN": [
-                                "gaf",
-                                "gaven"
-                            ]
-                        }
-                    },
-                    {
-                        "LOWER": {
-                            "IN": [
-                                "aan"
-                            ]
-                        }
-                    }
-                ]
-            ],
-            "qualifier": "Experiencer.Other"
-        },
-        {
-            "direction": "termination",
-            "patterns": [
-                "beslist",
-                "besloot",
-                "daarnaast",
-                "geen",
-                "hijzelf",
-                "huidig",
-                "klaagt",
-                "niet",
-                "nu",
-                "patient haar",
-                "patient zijn",
-                "patient",
-                "pt haar",
-                "pt zijn",
-                "pt",
-                "rapporteerde",
-                "vandaag",
-                "welke",
-                "zelf",
-                "zijzelf",
-                ","
-            ],
-            "qualifier": "Experiencer.Other"
-        },
-        {
-            "direction": "preceding",
             "max_scope": 5,
             "patterns": [
                 "afwezigheid van",
-                "deed geen",
-                "deed niet",
-                "geen aanwijzing voor",
-                "geen aanwijzingen voor",
-                "geen abnormale",
+                "geen",
+                "geen bevinding van",
+                "geen bevindingen die duiden op",
+                "geen bevindingen van",
+                "geen bewijs dat",
+                "geen bewijs dat suggereert",
                 "geen bewijs voor",
                 "geen klachten van",
-                "geen klachten van",
-                "geen oorzaak van ",
-                "geen reden tot",
-                "geen reden voor",
-                "geen sprake van",
+                "geen mammografisch bewijs van",
+                "geen nieuw",
+                "geen nieuwe",
+                "geen radiografisch bewijs van",
                 "geen suggestie van",
                 "geen teken van",
-                "geen tekenen van",
-                "geen",
-                "is geen",
-                "is niet",
-                "konden geen",
-                "konden niet",
-                "kunnen geen",
-                "kunnen niet",
+                "geen tekenenen van",
+                "had geen",
+                "had niet",
+                "had nooit",
+                "klaagt niet over",
                 "negatief voor",
-                "niet waarschijnlijk",
-                "niet",
+                "niet bekend met",
+                "niet geduid",
+                "niet geduid als",
+                "niet gezien",
+                "noch",
+                "nooit last gehad",
                 "nooit last gehad van",
-                "nooit",
-                "ontkend",
-                "ontkennend",
-                "ontkent",
-                "ontwikkelde geen",
                 "ontwikkelde nooit",
                 "ontwikkelt geen",
+                "ontwikkelt niet",
+                "ontwikkelt nooit",
                 "patient is niet",
+                "patient ontkent",
                 "patient was niet",
+                "sloot haar uit tegen",
+                "sloot haar uit voor",
+                "sloot hem uit tegen",
+                "sloot hem uit voor",
                 "sluit uit",
-                "subklinisch",
-                "subklinische",
-                "toonde geen",
+                "sluiten haar uit tegen",
+                "sluiten haar uit voor",
+                "sluiten hem uit tegen",
+                "sluiten hem uit voor",
+                "tonen geen",
+                "tonen niet",
+                "tonen niet aan",
                 "toonde geen",
-                "uitgesloten",
-                "versus",
+                "uitgesloten tegen",
+                "uitgesloten voor",
+                "vertoont geen",
+                "vertoont niet",
+                "voelde geen",
+                "voelde niet",
+                "voldoende haar uit te sluiten tegen",
+                "voldoende haar uit te sluiten voor",
+                "voldoende hem uit te sluiten tegen",
+                "voldoende hem uit te sluiten voor",
                 "vrij van",
-                "waren geen",
-                "waren niet",
                 "was geen",
                 "was niet",
-                "zijn geen",
-                "zijn niet",
-                "zonder indicatie van ",
+                "weigert",
+                "zonder",
+                "zonder indicatie van",
                 "zonder teken van",
-                "zonder tekenen van",
-                "zonder"
+                "zonder tekenen van"
             ],
-            "qualifier": "Negation.Negated"
+            "qualifier": "Presence.Absent"
         },
         {
             "direction": "following",
             "max_scope": 5,
             "patterns": [
+                "-",
                 "afwezig",
                 "gestaakt",
+                "geweigerd",
+                "is afwezig",
+                "is ontkend",
                 "is uitgesloten",
                 "is verdwenen",
+                "is weer weg",
                 "is weg",
                 "kan worden uitgesloten",
                 "niet aan de orde",
-                "niet aanwezig",
-                "niet gezien",
-                "niet meer",
+                "niet geconstateerd",
+                "niet meer aanwezig",
+                "nooit gehad",
                 "opgelost",
                 "speelt niet",
-                "in complete remissie",
-                "in totale remissie",
-                "waren niet",
-                "was niet",
+                "uitgesloten",
+                "was uitgesloten",
+                "weg",
+                "werd ontkend",
                 "werd uitgesloten",
                 "werden ontkend",
                 "werden uitgesloten",
                 "worden ontkend",
+                "wordt ontkend",
                 "zijn afwezig",
                 "zijn ontkend",
                 "zijn uitgesloten",
                 "zijn verdwenen",
                 "zijn weg"
             ],
-            "qualifier": "Negation.Negated"
+            "qualifier": "Presence.Absent"
+        },
+        {
+            "direction": "bidirectional",
+            "max_scope": 5,
+            "patterns": [
+                "evenmin",
+                "geen aanwijzing voor",
+                "geen aanwijzingen voor",
+                "geen bewijs",
+                "geen last van",
+                "geen sprake van",
+                "is geen",
+                "is niet",
+                "negatief",
+                "niet",
+                "niet aanwezig",
+                "niet meer",
+                "nooit",
+                "nooit ontwikkeld",
+                "ontkend",
+                "ontkennend",
+                "ontkent",
+                "verdween",
+                "verdwenen",
+                "waren niet",
+                "zijn geen",
+                "zijn niet"
+            ],
+            "qualifier": "Presence.Absent"
         },
         {
             "direction": "pseudo",
             "patterns": [
                 "geen afname",
+                "geen antwoord",
                 "geen oorzaak van",
                 "geen toename",
                 "geen verandering",
                 "geen verbetering",
                 "geen verklaring",
                 "geen zekere verandering",
                 "gram negatief",
                 "kan niet",
+                "kon niet",
+                "leek niet",
+                "leken niet",
+                "lijkt niet",
+                "niet aan te tonen",
                 "niet alleen",
+                "niet bekend",
                 "niet besproken",
                 "niet duidelijk",
-                "niet gevraagd",
                 "niet geindiceerd",
-                "niet mogelijk om ",
+                "niet gevraagd",
+                "niet goed",
+                "niet kunnen aantonen",
+                "niet mogelijk",
+                "niet mogelijk om",
                 "niet uit te sluiten",
                 "niet uitgesloten",
                 "niet uitgevraagd",
+                "niet vast te stellen",
+                "niet waarschijnlijk",
                 "niet zeker of",
                 "wel of niet",
                 "zonder effect op",
                 "zonder moeite",
                 "zonder moelijkheid",
-                "zonder verdere",
-                "niet goed"
+                "zonder verdere"
             ],
-            "qualifier": "Negation.Negated"
+            "qualifier": "Presence.Absent"
         },
         {
             "direction": "termination",
             "patterns": [
+                ",",
                 "aangezien er",
                 "afgezien van",
                 "alhoewel",
                 "andere mogelijkheden tot",
                 "andere redenen tot",
                 "andere redenen voor",
                 "behalve",
@@ -676,15 +271,14 @@
                 "soms",
                 "toch",
                 "trigger voor",
                 "uitgezonderd",
                 "voelt zich",
                 "wel",
                 "welke",
-                ",",
                 [
                     {
                         "LOWER": "als",
                         "OP": "?"
                     },
                     {
                         "LOWER": {
@@ -716,116 +310,122 @@
                                 "voor",
                                 "tot"
                             ]
                         }
                     }
                 ]
             ],
-            "qualifier": "Negation.Negated"
+            "qualifier": "Presence.Absent"
         },
         {
             "direction": "preceding",
+            "max_scope": 5,
             "patterns": [
-                "als er",
-                "als",
-                "ambivalent",
                 "beoordelen van",
-                "cave",
+                "differentiaal diagnostisch",
+                "evalueren voor",
+                "gecontroleerd op",
+                "geen weet van",
+                "gescreend op",
+                "kan haar uitsluiten tegen",
+                "kan haar uitsluiten voor",
+                "kan hem uitsluiten tegen",
+                "kan hem uitsluiten voor",
+                "kan uitsluiten tegen",
+                "kan uitsluiten voor",
+                "leek niet",
+                "leken niet",
+                "lijkt niet",
+                "niet zeker of",
+                "observeren van",
+                "rekening houden met",
+                "ter diagnostiek van",
+                "test voor",
+                "vermoeden van",
+                "weet niet van",
+                "wordt gedacht aan"
+            ],
+            "qualifier": "Presence.Uncertain"
+        },
+        {
+            "direction": "following",
+            "max_scope": 5,
+            "patterns": [
+                "?",
+                "dient te worden uitgesloten",
+                "geen antwoord",
+                "kan niet worden uitgesloten",
+                "kon niet worden uitgesloten",
+                "lijkt onwaarschijnlijk",
+                "moet worden uitgesloten",
+                "niet bekend",
+                "niet besproken",
+                "niet gevraagd",
+                "niet uitgevraagd",
+                "zal worden uitgesloten",
+                "zou kunnen worden uitgesloten",
+                "zouden moeten worden uitgesloten",
+                "zullen worden uitgesloten"
+            ],
+            "qualifier": "Presence.Uncertain"
+        },
+        {
+            "direction": "bidirectional",
+            "max_scope": 5,
+            "patterns": [
+                "ambivalent",
                 "dd",
                 "diagnostiek",
-                "differentiaal diagnostisch",
                 "eventueel",
                 "eventuele",
                 "evt",
                 "hypothese",
                 "hypothesen",
                 "hypotheses",
-                "indien er",
-                "indien",
-                "kan indiceren",
-                "kan worden",
-                "kan zijn",
-                "kan",
-                "kans op",
+                "inschatten",
+                "laag ingeschat",
                 "mgl",
-                "mogelijk gerelateerd aan",
+                "minder waarschijnlijk",
                 "mogelijk",
                 "mogelijke",
-                "neiging tot",
-                "niet besproken",
+                "niet aan te tonen",
                 "niet duidelijk",
-                "observeren van",
+                "niet kunnen aantonen",
+                "niet uit te sluiten",
+                "niet uitgesloten",
+                "niet vast te stellen",
+                "niet waarschijnlijk",
                 "onduidelijk",
                 "onwaarschijnlijk",
-                "rekening houden met",
-                "risico op",
                 "screen",
                 "screening",
-                "te verwachten",
+                "second opinion",
+                "ter uitsluiting",
                 "twijfel",
+                "uit te sluiten",
                 "uitsluiten",
                 "verdenking",
                 "vermoedde",
                 "vermoedden",
-                "vermoeden van",
                 "vermoeden",
                 "vermoedt",
-                "verwachte",
                 "voorlopige diagnose",
                 "waarschijnlijk",
-                "wanneer",
                 "wel of niet",
-                "wordt gedacht aan",
-                "zorgen voor",
-                "zou",
-                "werkdiagnose",
-                "dan"
-            ],
-            "qualifier": "Plausibility.Hypothetical"
-        },
-        {
-            "direction": "following",
-            "patterns": [
-                "?",
-                "ambivalent",
-                "kan niet worden uitgesloten",
-                "kan worden",
-                "kan zijn",
-                "kon niet worden uitgesloten",
-                "niet besproken",
-                "niet duidelijk",
-                "niet uitgevraagd",
-                "niet uit te sluiten",
-                "niet waarschijnlijk",
-                "screen",
-                "screening",
-                "onduidelijk",
-                "onwaarschijnijk",
-                "vermoedde",
-                "vermoedden",
-                "waarschijnlijk",
-                "zou worden",
-                "zou zijn"
+                "werkdiagnose"
             ],
-            "qualifier": "Plausibility.Hypothetical"
+            "qualifier": "Presence.Uncertain"
         },
         {
             "direction": "pseudo",
             "patterns": [
-                "als baby",
-                "als kind",
-                "als puber",
-                "als tiener",
                 "dd bij",
-                "geduid als",
-                "kan passen bij",
-                "niet mogelijk",
-                "werkdiagnose voor",
-                "waarschijnlijk bij",
                 "onwaarschijnlijk bij",
+                "waarschijnlijk bij",
+                "werkdiagnose voor",
                 [
                     {
                         "TEXT": {
                             "REGEX": "^\\d+$"
                         }
                     },
                     {
@@ -839,63 +439,171 @@
                     {
                         "TEXT": {
                             "REGEX": "^\\d+$"
                         }
                     }
                 ]
             ],
-            "qualifier": "Plausibility.Hypothetical"
+            "qualifier": "Presence.Uncertain"
         },
         {
             "direction": "termination",
             "patterns": [
-                "aanwezig",
-                "ter preventie",
-                "zeker",
-                "zonder twijfel",
-                ","
+                ",",
+                "aangezien er",
+                "afgezien van",
+                "alhoewel",
+                "andere mogelijkheden tot",
+                "andere redenen tot",
+                "andere redenen voor",
+                "behalve",
+                "behoudens",
+                "bron van",
+                "bron voor",
+                "bronnen van",
+                "bronnen voor",
+                "buiten",
+                "daarentegen",
+                "dat",
+                "desalniettemin",
+                "die",
+                "doch",
+                "etiologie van",
+                "etiologie voor",
+                "hetgeen",
+                "hoewel",
+                "losstaand van",
+                "maar",
+                "naast",
+                "niettemin",
+                "nochtans",
+                "nog",
+                "ofschoon",
+                "ondergeschikt",
+                "reden tot",
+                "reden van",
+                "reden voor",
+                "redenen tot",
+                "redenen voor",
+                "renenen van",
+                "soms",
+                "toch",
+                "trigger voor",
+                "uitgezonderd",
+                "voelt zich",
+                "wel",
+                "welke",
+                [
+                    {
+                        "LOWER": "als",
+                        "OP": "?"
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "de",
+                                "een"
+                            ]
+                        },
+                        "OP": "?"
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "bron",
+                                "bronnen",
+                                "reden",
+                                "redenen",
+                                "oorzaak",
+                                "oorzaken",
+                                "oorsprong",
+                                "etiologie"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "van",
+                                "voor",
+                                "tot"
+                            ]
+                        }
+                    }
+                ]
             ],
-            "qualifier": "Plausibility.Hypothetical"
+            "qualifier": "Presence.Uncertain"
         },
         {
             "direction": "preceding",
             "patterns": [
                 "al bekende",
+                "eerder al",
+                "eerdere",
+                "ex-",
+                "status na"
+            ],
+            "qualifier": "Temporality.Historical"
+        },
+        {
+            "direction": "following",
+            "patterns": [
+                "gehad",
+                "geweest",
+                "heeft gehad",
+                "heeft meegemaakt",
+                "heeft plaatsgehad",
+                "heeft plaatsgevonden",
+                "is gebeurd",
+                "is geweest",
+                "meegemaakt",
+                "opgelost"
+            ],
+            "qualifier": "Temporality.Historical"
+        },
+        {
+            "direction": "bidirectional",
+            "patterns": [
                 "als baby",
                 "als kind",
                 "als puber",
                 "als tiener",
                 "bij eerste presentatie",
                 "destijds",
-                "eerdere",
-                "ex-",
+                "doorgemaakt",
+                "doorgemaakte",
                 "gedocumenteerd",
                 "gedocumenteerde",
-                "geschiedenis van",
                 "geschiedenis",
+                "geschiedenis van",
                 "herinnering",
                 "herinneringen",
+                "in de geschiedenis",
                 "in de kindertijd",
+                "in de psychiatrische voorgeschiedenis",
                 "in de vg",
                 "in de voorgeschiedenis",
                 "in het verleden",
-                "in voorgeschiedenis",
+                "in jeugd",
                 "jaar",
                 "jaren",
                 "maand",
                 "maanden",
                 "niet actueel",
-                "op jong volwassen leeftijd",
+                "op jong volgwassen leeftijd",
                 "op jonge leeftijd",
+                "op jongvolwassen leeftijd",
                 "subacute",
                 "subacuut",
                 "toen",
                 "verleden van",
                 "vg",
                 "voorgeschiedenis",
+                "vorig",
+                "vorige",
                 "vroeger",
                 "werd",
                 [
                     {
                         "LOWER": {
                             "IN": [
                                 "in",
@@ -963,134 +671,183 @@
                         }
                     }
                 ]
             ],
             "qualifier": "Temporality.Historical"
         },
         {
-            "direction": "following",
+            "direction": "pseudo",
             "patterns": [
-                "als baby",
-                "als kind",
-                "als puber",
-                "als tiener",
-                "geweest",
-                "heeft gehad",
-                "heeft meegemaakt",
-                "heeft plaatsgehad",
-                "heeft plaatsgevonden",
-                "in de geschiedenis",
-                "in de kindertijd",
-                "in de psychiatrische voorgeschiedenis",
-                "in de vg",
-                "in de vg",
-                "in de voorgeschiedenis",
-                "in de voorgeschiedenis",
-                "in het verleden",
-                "in jeugd",
-                "in remissie",
-                "in voorgeschiedenis",
-                "in voorgeschiedenis",
-                "is gebeurd",
-                "is geweest",
-                "meegemaakt",
-                "nu in remissie",
-                "op jong volwassen leeftijd",
-                "op jonge leeftijd",
-                "opgelost",
+                "blanco psychiatrische vg",
+                "blanco psychiatrische voorgeschiedenis",
+                "blanco vg",
+                "blanco voorgeschiedenis",
+                "vg blanco",
+                "voorgeschiedenis blanco",
                 [
                     {
                         "LOWER": {
                             "IN": [
-                                "in",
-                                "rond"
+                                "sinds",
+                                "vanaf"
                             ]
                         }
                     },
                     {
                         "TEXT": {
                             "REGEX": "^(19|20)\\d{2}$"
                         }
                     }
                 ],
                 [
                     {
                         "LOWER": {
                             "IN": [
+                                "sinds",
+                                "vanaf"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "1",
+                                "2",
+                                "3",
+                                "4",
+                                "5",
+                                "6",
+                                "7",
+                                "8",
+                                "9",
+                                "10",
+                                "een",
+                                "twee",
+                                "drie",
+                                "vier",
+                                "vijf",
+                                "zes",
+                                "zeven",
+                                "acht",
+                                "negen",
+                                "tien"
+                            ]
+                        },
+                        "OP": "?"
+                    },
+                    {
+                        "TEXT": {
+                            "IN": [
                                 "jaar",
                                 "jaren",
                                 "maand",
                                 "maanden"
                             ]
                         }
-                    },
-                    {
-                        "LOWER": "geleden"
                     }
                 ],
                 [
                     {
-                        "LOWER": "in"
-                    },
-                    {
                         "LOWER": {
                             "IN": [
-                                "januari",
-                                "februari",
-                                "maart",
-                                "april",
-                                "mei",
-                                "juni",
-                                "juli",
-                                "augustus",
-                                "september",
-                                "november",
-                                "december"
+                                "sinds",
+                                "vanaf"
                             ]
                         }
-                    }
-                ],
-                [
-                    {
-                        "LOWER": "in"
                     },
                     {
                         "LOWER": {
                             "IN": [
                                 "januari",
                                 "februari",
                                 "maart",
                                 "april",
                                 "mei",
                                 "juni",
                                 "juli",
                                 "augustus",
                                 "september",
+                                "oktober",
                                 "november",
                                 "december"
                             ]
                         }
+                    },
+                    {
+                        "OP": "?",
+                        "TEXT": {
+                            "REGEX": "^(19|20)\\d{2}$"
+                        }
                     }
                 ]
             ],
             "qualifier": "Temporality.Historical"
         },
         {
+            "direction": "termination",
+            "patterns": [
+                ",",
+                "actueel",
+                "afgenomen",
+                "afname",
+                "nu",
+                "primair",
+                "sinds",
+                "toegenomen",
+                "toename",
+                "vanaf"
+            ],
+            "qualifier": "Temporality.Historical"
+        },
+        {
+            "direction": "preceding",
+            "patterns": [
+                "als",
+                "als de patient",
+                "als er",
+                "als hij",
+                "als zij",
+                "cave",
+                "indien",
+                "indien er",
+                "kans op",
+                "risico op",
+                "ter afwending van",
+                "verwachte",
+                "wanneer",
+                "zorgen voor"
+            ],
+            "qualifier": "Temporality.Future"
+        },
+        {
+            "direction": "following",
+            "patterns": [
+                "kan ontwikkelen"
+            ],
+            "qualifier": "Temporality.Future"
+        },
+        {
+            "direction": "bidirectional",
+            "patterns": [
+                "allergie",
+                "indien nodig",
+                "preventief",
+                "profylactisch",
+                "te verwachten"
+            ],
+            "qualifier": "Temporality.Future"
+        },
+        {
             "direction": "pseudo",
             "patterns": [
-                "blanco psychiatrische vg",
-                "blanco psychiatrische voorgeschiedenis",
-                "blanco vg",
-                "blanco voorgeschiedenis",
-                "lijkt meer",
-                "lijkt minder",
-                "lijkt niet meer",
-                "lijkt niet minder",
-                "vg blanco",
-                "voorgeschiedenis blanco",
+                "als baby",
+                "als kind",
+                "als puber",
+                "als tiener",
+                "geduid als",
                 [
                     {
                         "LOWER": {
                             "IN": [
                                 "sinds",
                                 "vanaf"
                             ]
@@ -1180,27 +937,806 @@
                         "OP": "?",
                         "TEXT": {
                             "REGEX": "^(19|20)\\d{2}$"
                         }
                     }
                 ]
             ],
-            "qualifier": "Temporality.Historical"
+            "qualifier": "Temporality.Future"
         },
         {
             "direction": "termination",
             "patterns": [
+                ",",
                 "actueel",
                 "afgenomen",
                 "afname",
                 "nu",
                 "primair",
                 "sinds",
                 "toegenomen",
                 "toename",
-                "vanaf",
-                ","
+                "vanaf"
             ],
-            "qualifier": "Temporality.Historical"
+            "qualifier": "Temporality.Future"
+        },
+        {
+            "direction": "preceding",
+            "patterns": [
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "broer",
+                                "broers",
+                                "broertje",
+                                "broertjes",
+                                "dochter",
+                                "dochters",
+                                "dochtertje",
+                                "dochtertjes",
+                                "familie",
+                                "grootmoeder",
+                                "grootvader",
+                                "mdr",
+                                "moeder",
+                                "neef",
+                                "neefje",
+                                "neefjes",
+                                "neven",
+                                "nicht",
+                                "nichten",
+                                "nichtje",
+                                "nichtjes",
+                                "oma",
+                                "oom",
+                                "ooms",
+                                "opa",
+                                "tante",
+                                "tantes",
+                                "vader",
+                                "vdr",
+                                "zoon",
+                                "zoons",
+                                "zoontje",
+                                "zoontjes",
+                                "zus",
+                                "zusje",
+                                "zusjes",
+                                "zussen"
+                            ]
+                        }
+                    }
+                ],
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "broer",
+                                "broertje",
+                                "dochter",
+                                "dochtertje",
+                                "familie",
+                                "grootmoeder",
+                                "grootvader",
+                                "mdr",
+                                "moeder",
+                                "neef",
+                                "neefje",
+                                "nicht",
+                                "nichtje",
+                                "oma",
+                                "oom",
+                                "opa",
+                                "tante",
+                                "vader",
+                                "vdr",
+                                "zoon",
+                                "zoontje",
+                                "zus",
+                                "zusje"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "zijn",
+                                "haar"
+                            ]
+                        }
+                    }
+                ],
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "broers",
+                                "broertjes",
+                                "dochters",
+                                "dochtertjes",
+                                "neefjes",
+                                "neven",
+                                "nichten",
+                                "nichtjes",
+                                "ooms",
+                                "tantes",
+                                "zoons",
+                                "zoontjes",
+                                "zusjes",
+                                "zussen"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": "hun"
+                    }
+                ],
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "broer",
+                                "broertje",
+                                "dochter",
+                                "dochtertje",
+                                "familie",
+                                "grootmoeder",
+                                "grootvader",
+                                "mdr",
+                                "moeder",
+                                "neef",
+                                "neefje",
+                                "nicht",
+                                "nichtje",
+                                "oma",
+                                "oom",
+                                "opa",
+                                "tante",
+                                "vader",
+                                "vdr",
+                                "zoon",
+                                "zoontje",
+                                "zus",
+                                "zusje"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": "'"
+                    },
+                    {
+                        "LOWER": "s"
+                    }
+                ]
+            ],
+            "qualifier": "Experiencer.Family"
+        },
+        {
+            "direction": "following",
+            "patterns": [
+                [
+                    {
+                        "LOWER": "bij"
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "broer",
+                                "broers",
+                                "broertje",
+                                "broertjes",
+                                "dochter",
+                                "dochters",
+                                "dochtertje",
+                                "dochtertjes",
+                                "familie",
+                                "grootmoeder",
+                                "grootvader",
+                                "mdr",
+                                "moeder",
+                                "neef",
+                                "neefje",
+                                "neefjes",
+                                "neven",
+                                "nicht",
+                                "nichten",
+                                "nichtje",
+                                "nichtjes",
+                                "oma",
+                                "oom",
+                                "ooms",
+                                "opa",
+                                "tante",
+                                "tantes",
+                                "vader",
+                                "vdr",
+                                "zoon",
+                                "zoons",
+                                "zoontje",
+                                "zoontjes",
+                                "zus",
+                                "zusje",
+                                "zusjes",
+                                "zussen"
+                            ]
+                        }
+                    }
+                ]
+            ],
+            "qualifier": "Experiencer.Family"
+        },
+        {
+            "direction": "bidirectional",
+            "patterns": [
+                "familiair",
+                "familiaire",
+                "familie anamnese",
+                "familie-anamnese",
+                "familieanamnese",
+                "familiegeschiedenis",
+                "familieleden",
+                "in de familie",
+                "in familie",
+                "moederszijde",
+                "vaderszijde"
+            ],
+            "qualifier": "Experiencer.Family"
+        },
+        {
+            "direction": "pseudo",
+            "patterns": [
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "door",
+                                "met",
+                                "naar",
+                                "volgens",
+                                "vertelt",
+                                "vertelde",
+                                "vertellen",
+                                "vertelden"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "broer",
+                                "broers",
+                                "broertje",
+                                "broertjes",
+                                "buurman",
+                                "buurvrouw",
+                                "dochter",
+                                "dochters",
+                                "dochtertje",
+                                "dochtertjes",
+                                "familie",
+                                "grootmoeder",
+                                "grootvader",
+                                "huisgenoot",
+                                "huisgenote",
+                                "huisgenoten",
+                                "huisgenotes",
+                                "mdr",
+                                "moeder",
+                                "neef",
+                                "neefje",
+                                "neefjes",
+                                "neven",
+                                "nicht",
+                                "nichten",
+                                "nichtje",
+                                "nichtjes",
+                                "oma",
+                                "oom",
+                                "ooms",
+                                "opa",
+                                "tante",
+                                "tantes",
+                                "vader",
+                                "vdr",
+                                "zoon",
+                                "zoons",
+                                "zoontje",
+                                "zoontjes",
+                                "zus",
+                                "zusje",
+                                "zusjes",
+                                "zussen"
+                            ]
+                        }
+                    }
+                ],
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "vader",
+                                "vdr",
+                                "moeder",
+                                "mdr",
+                                "broer",
+                                "broertje",
+                                "zus",
+                                "zusje",
+                                "oom",
+                                "tante",
+                                "neef",
+                                "neefje",
+                                "nicht",
+                                "nichtje",
+                                "opa",
+                                "oma",
+                                "grootvader",
+                                "grootmoeder",
+                                "buurman",
+                                "buurvrouw",
+                                "zoon",
+                                "zoontje",
+                                "dochter",
+                                "dochtertje",
+                                "huisgenoot",
+                                "huisgenote",
+                                "familie",
+                                "broers",
+                                "broertjes",
+                                "zussen",
+                                "zusjes",
+                                "ooms",
+                                "tantes",
+                                "neven",
+                                "neefjes",
+                                "nichten",
+                                "nichtjes",
+                                "zoons",
+                                "zoontjes",
+                                "dochters",
+                                "dochtertjes",
+                                "huisgenoten",
+                                "huisgenotes"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "belde",
+                                "belden",
+                                "zei",
+                                "zeiden",
+                                "vond",
+                                "vonden",
+                                "vertelt",
+                                "vertelde",
+                                "vertellen",
+                                "vertelden"
+                            ]
+                        }
+                    }
+                ],
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "vader",
+                                "vdr",
+                                "moeder",
+                                "mdr",
+                                "broer",
+                                "broertje",
+                                "zus",
+                                "zusje",
+                                "oom",
+                                "tante",
+                                "neef",
+                                "neefje",
+                                "nicht",
+                                "nichtje",
+                                "opa",
+                                "oma",
+                                "grootvader",
+                                "grootmoeder",
+                                "buurman",
+                                "buurvrouw",
+                                "zoon",
+                                "zoontje",
+                                "dochter",
+                                "dochtertje",
+                                "huisgenoot",
+                                "huisgenote",
+                                "familie",
+                                "broers",
+                                "broertjes",
+                                "zussen",
+                                "zusjes",
+                                "ooms",
+                                "tantes",
+                                "neven",
+                                "neefjes",
+                                "nichten",
+                                "nichtjes",
+                                "zoons",
+                                "zoontjes",
+                                "dochters",
+                                "dochtertjes",
+                                "huisgenoten",
+                                "huisgenotes"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "gaf",
+                                "gaven"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "aan"
+                            ]
+                        }
+                    }
+                ]
+            ],
+            "qualifier": "Experiencer.Family"
+        },
+        {
+            "direction": "termination",
+            "patterns": [
+                ",",
+                "beslist",
+                "besloot",
+                "daarnaast",
+                "geen",
+                "hijzelf",
+                "huidig",
+                "klaagt",
+                "niet",
+                "nu",
+                "patient",
+                "patient haar",
+                "patient zijn",
+                "pt",
+                "pt haar",
+                "pt zijn",
+                "rapporteerde",
+                "vandaag",
+                "welke",
+                "zelf",
+                "zijzelf"
+            ],
+            "qualifier": "Experiencer.Family"
+        },
+        {
+            "direction": "preceding",
+            "patterns": [
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "buurman",
+                                "buurvrouw",
+                                "huisgenoot",
+                                "huisgenote",
+                                "huisgenoten",
+                                "huisgenotes"
+                            ]
+                        }
+                    }
+                ],
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "buurman",
+                                "buurvrouw",
+                                "huisgenoot",
+                                "huisgenote"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "zijn",
+                                "haar"
+                            ]
+                        }
+                    }
+                ],
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "huisgenoten",
+                                "huisgenotes"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": "hun"
+                    }
+                ],
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "buurman",
+                                "buurvrouw",
+                                "huisgenoot",
+                                "huisgenote"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": "'"
+                    },
+                    {
+                        "LOWER": "s"
+                    }
+                ]
+            ],
+            "qualifier": "Experiencer.Other"
+        },
+        {
+            "direction": "following",
+            "patterns": [
+                [
+                    {
+                        "LOWER": "bij"
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "buurman",
+                                "buurvrouw",
+                                "huisgenoot",
+                                "huisgenote",
+                                "huisgenoten",
+                                "huisgenotes"
+                            ]
+                        }
+                    }
+                ]
+            ],
+            "qualifier": "Experiencer.Other"
+        },
+        {
+            "direction": "pseudo",
+            "patterns": [
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "door",
+                                "met",
+                                "naar",
+                                "volgens",
+                                "vertelt",
+                                "vertelde",
+                                "vertellen",
+                                "vertelden"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "broer",
+                                "broers",
+                                "broertje",
+                                "broertjes",
+                                "buurman",
+                                "buurvrouw",
+                                "dochter",
+                                "dochters",
+                                "dochtertje",
+                                "dochtertjes",
+                                "familie",
+                                "grootmoeder",
+                                "grootvader",
+                                "huisgenoot",
+                                "huisgenote",
+                                "huisgenoten",
+                                "huisgenotes",
+                                "mdr",
+                                "moeder",
+                                "neef",
+                                "neefje",
+                                "neefjes",
+                                "neven",
+                                "nicht",
+                                "nichten",
+                                "nichtje",
+                                "nichtjes",
+                                "oma",
+                                "oom",
+                                "ooms",
+                                "opa",
+                                "tante",
+                                "tantes",
+                                "vader",
+                                "vdr",
+                                "zoon",
+                                "zoons",
+                                "zoontje",
+                                "zoontjes",
+                                "zus",
+                                "zusje",
+                                "zusjes",
+                                "zussen"
+                            ]
+                        }
+                    }
+                ],
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "broer",
+                                "broers",
+                                "broertje",
+                                "broertjes",
+                                "buurman",
+                                "buurvrouw",
+                                "dochter",
+                                "dochters",
+                                "dochtertje",
+                                "dochtertjes",
+                                "familie",
+                                "grootmoeder",
+                                "grootvader",
+                                "huisgenoot",
+                                "huisgenote",
+                                "huisgenoten",
+                                "huisgenotes",
+                                "mdr",
+                                "moeder",
+                                "neef",
+                                "neefje",
+                                "neefjes",
+                                "neven",
+                                "nicht",
+                                "nichten",
+                                "nichtje",
+                                "nichtjes",
+                                "oma",
+                                "oom",
+                                "ooms",
+                                "opa",
+                                "tante",
+                                "tantes",
+                                "vader",
+                                "vdr",
+                                "zoon",
+                                "zoons",
+                                "zoontje",
+                                "zoontjes",
+                                "zus",
+                                "zusje",
+                                "zusjes",
+                                "zussen"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "belde",
+                                "belden",
+                                "zei",
+                                "zeiden",
+                                "vond",
+                                "vonden",
+                                "vertelt",
+                                "vertelde",
+                                "vertellen",
+                                "vertelden"
+                            ]
+                        }
+                    }
+                ],
+                [
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "broer",
+                                "broers",
+                                "broertje",
+                                "broertjes",
+                                "buurman",
+                                "buurvrouw",
+                                "dochter",
+                                "dochters",
+                                "dochtertje",
+                                "dochtertjes",
+                                "familie",
+                                "grootmoeder",
+                                "grootvader",
+                                "huisgenoot",
+                                "huisgenote",
+                                "huisgenoten",
+                                "huisgenotes",
+                                "mdr",
+                                "moeder",
+                                "neef",
+                                "neefje",
+                                "neefjes",
+                                "neven",
+                                "nicht",
+                                "nichten",
+                                "nichtje",
+                                "nichtjes",
+                                "oma",
+                                "oom",
+                                "ooms",
+                                "opa",
+                                "tante",
+                                "tantes",
+                                "vader",
+                                "vdr",
+                                "zoon",
+                                "zoons",
+                                "zoontje",
+                                "zoontjes",
+                                "zus",
+                                "zusje",
+                                "zusjes",
+                                "zussen"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "gaf",
+                                "gaven"
+                            ]
+                        }
+                    },
+                    {
+                        "LOWER": {
+                            "IN": [
+                                "aan"
+                            ]
+                        }
+                    }
+                ]
+            ],
+            "qualifier": "Experiencer.Other"
+        },
+        {
+            "direction": "termination",
+            "patterns": [
+                ",",
+                "beslist",
+                "besloot",
+                "daarnaast",
+                "geen",
+                "hijzelf",
+                "huidig",
+                "klaagt",
+                "niet",
+                "nu",
+                "patient",
+                "patient haar",
+                "patient zijn",
+                "pt",
+                "pt haar",
+                "pt zijn",
+                "rapporteerde",
+                "vandaag",
+                "welke",
+                "zelf",
+                "zijzelf"
+            ],
+            "qualifier": "Experiencer.Other"
         }
     ]
 }
```

### Comparing `clinlp-0.6.6/src/clinlp/sentencizer.py` & `clinlp-0.7.0/src/clinlp/sentencizer.py`

 * *Files identical despite different names*

### Comparing `clinlp-0.6.6/src/clinlp/util.py` & `clinlp-0.7.0/src/clinlp/util.py`

 * *Files 21% similar despite different names*

```diff
@@ -64,7 +64,14 @@
             if (k in component_args or k in component_kwargs)
             and (not isinstance(v, _UnusedArgument))
         }
 
         return cls(**cls_kwargs)
 
     return make_component
+
+
+def interval_dist(start_a: int, end_a: int, start_b: int, end_b: int) -> int:
+    if (end_a < start_a) or (end_b < start_b):
+        raise ValueError("Input malformed interval.")
+
+    return max(0, start_a - end_b, start_b - end_a)
```

### Comparing `clinlp-0.6.6/PKG-INFO` & `clinlp-0.7.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: clinlp
-Version: 0.6.6
+Version: 0.7.0
 Summary: Performant and production-ready NLP pipelines for clinical text written in Dutch
 Author: UMCU DIT Analytics
 Author-email: analytics@umcutrecht.nl
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: metrics
 Provides-Extra: transformers
 Requires-Dist: intervaltree (>=3.1.0,<4.0.0)
 Requires-Dist: makefun (>=1.15.1,<2.0.0)
+Requires-Dist: nervaluate (>=0.1.8,<0.2.0) ; extra == "metrics"
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
+Requires-Dist: scikit-learn (>=1.4.2,<2.0.0) ; extra == "metrics"
 Requires-Dist: spacy (>=3.5.3,<4.0.0)
 Requires-Dist: transformers[torch] (>=4.30.2,<5.0.0) ; extra == "transformers"
 Description-Content-Type: text/markdown
 
 [![test](https://github.com/umcu/clinlp/actions/workflows/test.yml/badge.svg)](https://github.com/umcu/clinlp/actions/workflows/test.yml)
 [![pypi version](https://img.shields.io/pypi/v/clinlp?color=blue)](https://pypi.org/project/clinlp/)
 [![pypi python versions](https://img.shields.io/pypi/pyversions/clinlp)](https://pypi.org/project/clinlp/)
@@ -44,15 +47,15 @@
 ```bash
 pip install clinlp
 ```
 
 ### Example
 ```python
 import spacy
-from clinlp import Term
+from clinlp.ie import Term
 
 nlp = spacy.blank("clinlp")
 
 # Normalization
 nlp.add_pipe("clinlp_normalizer")
 
 # Sentences
@@ -102,18 +105,18 @@
 for ent in doc.ents:
   print(ent, ent._.qualifiers_str)
 ```
 
 * `Preterme` `set()`
 * `<p3` `set()`
 * `bd enigszins verlaagd` `set()`
-* `hypotensie` `{'Experiencer.OTHER'}`
-* `veneus infarkt` `{'Negation.NEGATED'}`
+* `hypotensie` `{'Experiencer.Family'}`
+* `veneus infarkt` `{'Presence.Absent'}`
 * `partus prematurus` `set()`
-* `VI` `{'Plausibility.HYPOTHETICAL'}`
+* `VI` `{'Temporality.Future'}`
 
 ## Citing
 
 If you use `clinlp`, please find the appropriate citation by clicking the Zenodo button below. This should always point you to the current latest release:
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10528055.svg)](https://doi.org/10.5281/zenodo.10528055)
 
@@ -127,15 +130,16 @@
 
 1. [Tokenizer](#tokenizer)
 2. [Normalizer](#normalizer)
 3. [Sentence splitter](#sentence-splitter)
 4. [Entity matcher](#entity-matcher)
 5. [Qualifier detection (negation, historical, etc.)](#qualifier-detection)
     - [Context Algorithm](#context-algorithm)
-    - [Transformer based negation detection](#transformer-based-negation-detection)
+    - [Transformer based detection](#transformer-based-detection)
+6. [Metrics and statistics](#metrics-and-statistics)
 
 ### Tokenizer
 
 The `clinlp` tokenizer is built into the blank model:
 
 ```python
 nlp = spacy.blank("clinlp")
@@ -224,15 +228,15 @@
 entity_matcher = nlp.add_pipe("clinlp_entity_matcher", config={"fuzzy": 1, "fuzzy_min_len": 5})
 ```
 
 #### Terms
 The settings above are described at the matcher level, but can all be overridden at the term level by adding a `Term` to a concept, rather than a literal phrase:
 
 ```python
-from clinlp import Term
+from clinlp.ie import Term
 
 concepts = {
     "sepsis": [
         "sepsis",
         "lijnsepsis",
         Term("early onset", proximity=1),
         Term("late onset", proximity=1),
@@ -319,33 +323,33 @@
         Term("VI", attr="TEXT")
     ]
 }
 ```
 
 ### Qualifier detection
 
-After finding entities, it"s often useful to qualify these entities, e.g.: are they negated or affirmed, historical or current? `clinlp` currently implements two options: the rule-based Context Algorithm, and a transformer-based negation detector. In both cases, the result can be found in the `entity._.qualifiers`, `entity._.qualifiers_dict` and `entity._.qualifiers_str` attributes (including all defaults, e.g. `Affirmed` for `Negation`).   
+After finding entities, it's often useful to qualify these entities, e.g.: are they present or absent, historical or current? `clinlp` currently implements two options: the rule-based Context Algorithm, and a transformer-based negation detector. In both cases, the result can be found in the `entity._.qualifiers`, `entity._.qualifiers_dict` and `entity._.qualifiers_str` attributes (including all defaults, e.g. `Present` for `Presence`). Some clarifications on the framework we use for qualifiers is available under [docs/qualifiers.docx](docs/qualifiers.docx) (will be incorporated in an improved documentation page soon).
 
 #### Context Algorithm
 
-The rule-based [Context Algorithm](https://doi.org/10.1016%2Fj.jbi.2009.05.002) is fairly accurate, and quite transparent and fast. A set of rules, that checks for negation, temporality, plausibility and experiencer, is loaded by default:
+The rule-based [Context Algorithm](https://doi.org/10.1016%2Fj.jbi.2009.05.002) is fairly accurate, and quite transparent and fast. A set of rules, that checks for presence, temporality, and experiencer, is loaded by default:
 
 ```python
 nlp.add_pipe("clinlp_context_algorithm", config={"phrase_matcher_attr": "NORM"})
 ```
 
-A custom set of rules, including different types of qualifiers, can easily be defined. See [`clinlp/resources/context_rules.json`](clinlp/resources/context_rules.json) for an example, and load it as follows:
+A custom set of rules, including different types of qualifiers, can easily be defined. See [`src/clinlp/resources/context_rules.json`](src/clinlp/resources/context_rules.json) for an example, and load it as follows:
 
 ```python
 cm = nlp.add_pipe("clinlp_context_algorithm", config={"rules": "/path/to/my_own_ruleset.json"})
 ```
 
 #### Transformer based detection
 
-`clinlp` also includes a wrapper around some trained transformer models for detector qualifiers, including the negation detector described in [van Es et al, 2022](https://doi.org/10.48550/arxiv.2209.00470). The underlying transformers can be found on [huggingface](https://huggingface.co/UMCU/). The negation detector for instnace is reported as more accurate than the rule-based version (see paper for details), at the cost of less transparency and additional computational cost.
+`clinlp` also includes a wrapper around some trained transformer models for detector qualifiers, including the negation detector described in [van Es et al, 2022](https://doi.org/10.48550/arxiv.2209.00470). The underlying transformers can be found on [huggingface](https://huggingface.co/UMCU/). The negation detector for instance is reported as more accurate than the rule-based version (see paper for details), at the cost of less transparency and additional computational cost.
 
 First, install the additional dependencies:
 
 ```bash
 pip install "clinlp[transformers]"
 ```
 
@@ -354,14 +358,228 @@
 ```python
 _ = nlp.add_pipe("clinlp_negation_transformer")
 _ = nlp.add_pipe("clinlp_experiencer_transformer")
 ```
 
 Some configuration options, like the number of tokens to consider, can be specified in the `config` argument. 
 
+#### Using multiple qualifier detectors together
+
+Multiple qualifier detectors (e.g. `clinlp_context_algorithm` and `clinlp_negation_transformer`) can be used together. However, if there is a qualifier class (e.g. Presence) they both detect, the the component that is added last will erase any qualifiers set by previous detectors, regardless of defaults. It's therefore most efficient to configure different detectors to not detect the same qualifiers, although no errors occur. If the qualifier detectors detect different qualifier classes (e.g. one detects Presence, and the other Experiencer), there is no issue and both qualifier classes will be correctly added to the entities.
+
+### Metrics and statistics
+
+`clinlp` can compute some information extraction related metrics and statistics for annotated datasets. This is done by creating one or more `InfoExtractionDataset`. First install the optional dependencies:
+
+```bash
+pip install clinlp[metrics]
+```
+
+Then:
+
+```python
+from clinlp.metrics import InfoExtractionDataset
+
+# medcattrainer
+import json
+
+with open('medcattrainer_export.json', 'rb') as f:
+    mtrainer_data = json.load(f)
+
+d1 = InfoExtractionDataset.from_medcattrainer(mctrainer_data)
+
+# clinlp
+import clinlp
+import spacy
+
+from model import get_model  # not included
+
+nlp = get_model()
+nlp_docs = nlp.pipe([doc['text'] for doc in data['projects'][0]['documents']])
+
+d2 = InfoExtractionDataset.from_clinlp_docs(nlp_docs)
+
+```
+
+#### Descriptive statistics
+
+Get descriptive statistics for a `Dataset` as follows:
+
+```python
+d1.stats()
+```
+
+Resulting in:
+
+```python
+{'num_docs': 50,
+ 'num_annotations': 513,
+ 'span_counts': {'prematuriteit': 43,
+                 'infectie': 31,
+                 'fototherapie': 25,
+                 'dysmaturiteit': 24,
+                 'IRDS': 20,
+                 'prematuur': 15,
+                 'sepsis': 15,
+                 'hyperbilirubinemie': 14,
+                 'Prematuriteit': 14,
+                 'ROP': 13,
+                 'necrotiserende enterocolitis': 12,
+                 'Prematuur': 11,
+                 'infektie': 11,
+                 'ductus': 11,
+                 'bloeding': 8,
+                 'dysmatuur': 7,
+                 'IUGR': 7,
+                 'Hyperbilirubinemie': 7,
+                 'transfusie': 6,
+                 'hyperbilirubinaemie': 6,
+                 'Dopamine': 6,
+                 'wisseltransfusie': 5,
+                 'premature partus': 5,
+                 'retinopathy of prematurity': 5,
+                 'bloedtransfusie': 5},
+ 'label_counts': {'C0151526_prematuriteit': 94,
+                  'C0020433_hyperbilirubinemie': 68,
+                  'C0243026_sepsis': 63,
+                  'C0015934_intrauterine_groeivertraging': 57,
+                  'C0002871_anemie': 37,
+                  'C0035220_infant_respiratory_distress_syndrome': 25,
+                  'C0035344_retinopathie_van_de_prematuriteit': 21,
+                  'C0520459_necrotiserende_enterocolitis': 18,
+                  'C0013274_patent_ductus_arteriosus': 18,
+                  'C0020649_hypotensie': 18,
+                  'C0559477_perinatale_asfyxie': 18,
+                  'C0270191_intraventriculaire_bloeding': 17,
+                  'C0877064_post_hemorrhagische_ventrikeldilatatie': 13,
+                  'C0014850_oesophagus_atresie': 12,
+                  'C0006287_bronchopulmonale_dysplasie': 9,
+                  'C0031190_persisterende_pulmonale_hypertensie': 7,
+                  'C0015938_macrosomie': 6,
+                  'C0751954_veneus_infarct': 5,
+                  'C0025289_meningitis': 5,
+                  'C0023529_periventriculaire_leucomalacie': 2},
+ 'qualifier_counts': {'Presence': {'Present': 436, 'Uncertain': 34, 'Absent': 30},
+                      'Temporality': {'Current': 473, 'Historical': 18, 'Future': 9},
+                      'Experiencer': {'Patient': 489, 'Family': 9, 'Other': 2}}}
+```
+
+#### Comparison statistics
+
+
+Create a `InfoExtractionMetrics` object as follows:
+
+```python
+from clinlp.metrics import InfoExtractionMetrics
+
+nlp_metrics = InfoExtractionMetrics(d1, d2)
+
+nlp_metrics.entity_metrics()
+```
+
+Will result in:
+```python
+{'ent_type': {'correct': 480,
+              'incorrect': 1,
+              'partial': 0,
+              'missed': 32,
+              'spurious': 21,
+              'possible': 513,
+              'actual': 502,
+              'precision': 0.9561752988047809,
+              'recall': 0.935672514619883,
+              'f1': 0.9458128078817734},
+ 'partial': {'correct': 473,
+             'incorrect': 0,
+             'partial': 8,
+             'missed': 32,
+             'spurious': 21,
+             'possible': 513,
+             'actual': 502,
+             'precision': 0.950199203187251,
+             'recall': 0.9298245614035088,
+             'f1': 0.9399014778325123},
+ 'strict': {'correct': 473,
+            'incorrect': 8,
+            'partial': 0,
+            'missed': 32,
+            'spurious': 21,
+            'possible': 513,
+            'actual': 502,
+            'precision': 0.9422310756972112,
+            'recall': 0.9220272904483431,
+            'f1': 0.9320197044334976},
+ 'exact': {'correct': 473,
+           'incorrect': 8,
+           'partial': 0,
+           'missed': 32,
+           'spurious': 21,
+           'possible': 513,
+           'actual': 502,
+           'precision': 0.9422310756972112,
+           'recall': 0.9220272904483431,
+           'f1': 0.9320197044334976}}
+```
+
+For explanation on the different metrics (`partial`, `exact`, `strict` and `ent_type`), see [Nervaluate documentation](https://github.com/MantisAI/nervaluate).
+
+Then, for metrics on qualifiers, use:
+
+```python
+nlp_metrics.qualifier_info()
+```
+
+Resulting in:
+
+```python
+{'Experiencer': {'metrics': {'n': 460,
+                             'precision': 0.3333333333333333,
+                             'recall': 0.09090909090909091,
+                             'f1': 0.14285714285714288},
+                 'misses': [{'doc.identifier': 'doc_0001',
+                             'annotation': {'text': 'anemie',
+                                            'start': 1849,
+                                            'end': 1855,
+                                            'label': 'C0002871_anemie'},
+                             'true_qualifier': 'Family',
+                             'pred_qualifier': 'Patient'}, ...]},
+ 'Temporality': {'metrics': {'n': 460,
+                             'precision': 0.0,
+                             'recall': 0.0,
+                             'f1': 0.0},
+                 'misses': [{'doc.identifier': 'doc_0001',
+                             'annotation': {'text': 'premature partus',
+                                            'start': 1611,
+                                            'end': 1627,
+                                            'label': 'C0151526_prematuriteit'},
+                             'true_qualifier': 'Current',
+                             'pred_qualifier': 'Historical'}, ...]},
+ 'Plausibility': {'metrics': {'n': 460,
+                              'precision': 0.6486486486486487,
+                              'recall': 0.5217391304347826,
+                              'f1': 0.5783132530120482},
+                  'misses': [{'doc.identifier': 'doc_0001',
+                              'annotation': {'text': 'Groeivertraging',
+                                             'start': 1668,
+                                             'end': 1683,
+                                             'label': 'C0015934_intrauterine_groeivertraging'},
+                              'true_qualifier': 'Current',
+                              'pred_qualifier': 'Future'}, ...]},
+ 'Negation': {'metrics': {'n': 460,
+                          'precision': 0.7692307692307693,
+                          'recall': 0.6122448979591837,
+                          'f1': 0.6818181818181818},
+              'misses': [{'doc.identifier': 'doc_0001',
+                          'annotation': {'text': 'wisseltransfusie',
+                                         'start': 4095,
+                                         'end': 4111,
+                                         'label': 'C0020433_hyperbilirubinemie'},
+                          'true_qualifier': 'Present',
+                          'pred_qualifier': 'Absent'}, ...]}}
+```
 
 ### Where to go from here
 
 We hope to extend `clinlp` with new functionality and more complete documentation in the near future. In the meantime, if any questions or problems arise, we recommend:
 
 * Checking the source code 
 * Getting in touch ([email](mailto:analytics@umcutrecht.nl) | [issue](https://github.com/umcu/clinlp/issues/new))
```

