# Comparing `tmp/grote-0.1.8.tar.gz` & `tmp/grote-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grote-0.1.8.tar", max compression
+gzip compressed data, was "grote-0.1.9.tar", max compression
```

## Comparing `grote-0.1.8.tar` & `grote-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2024-01-10 13:50:16.570295 grote-0.1.8/LICENSE
--rw-r--r--   0        0        0     1016 2024-02-03 14:29:00.382226 grote-0.1.8/README.md
--rw-r--r--   0        0        0      428 2024-02-03 13:31:21.215921 grote-0.1.8/grote/__init__.py
--rw-r--r--   0        0        0     2403 2024-04-09 15:48:39.327306 grote-0.1.8/grote/app.py
--rw-r--r--   0        0        0      174 2024-01-10 13:50:16.571335 grote-0.1.8/grote/collections/__init__.py
--rw-r--r--   0        0        0     2903 2024-02-03 13:52:54.947521 grote-0.1.8/grote/collections/base.py
--rw-r--r--   0        0        0     1218 2024-04-10 21:30:35.209116 grote-0.1.8/grote/collections/config.yaml
--rw-r--r--   0        0        0     3962 2024-04-09 15:45:14.921487 grote-0.1.8/grote/collections/load.py
--rw-r--r--   0        0        0     8298 2024-04-10 21:30:05.986989 grote-0.1.8/grote/collections/translate.py
--rw-r--r--   0        0        0     2774 2024-04-10 21:51:22.581671 grote-0.1.8/grote/config.py
--rw-r--r--   0        0        0      299 2024-04-10 21:31:45.750995 grote-0.1.8/grote/config.yaml
--rw-r--r--   0        0        0     9690 2024-02-03 13:44:49.951724 grote-0.1.8/grote/event_logging.py
--rw-r--r--   0        0        0      619 2024-04-09 15:48:39.327445 grote-0.1.8/grote/functions/__init__.py
--rw-r--r--   0        0        0     5543 2024-04-10 21:18:52.959276 grote-0.1.8/grote/functions/load.py
--rw-r--r--   0        0        0     3529 2024-04-10 21:35:57.692323 grote-0.1.8/grote/functions/translate.py
--rw-r--r--   0        0        0      636 2024-04-09 11:50:18.551110 grote-0.1.8/grote/style.py
--rw-r--r--   0        0        0     3659 2024-04-10 21:51:36.927678 grote-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 grote-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-10 13:50:16.570295 grote-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1016 2024-02-03 14:29:00.382226 grote-0.1.9/README.md
+-rw-r--r--   0        0        0      428 2024-02-03 13:31:21.215921 grote-0.1.9/grote/__init__.py
+-rw-r--r--   0        0        0     1331 2024-04-15 13:55:21.523379 grote-0.1.9/grote/app.py
+-rw-r--r--   0        0        0      174 2024-01-10 13:50:16.571335 grote-0.1.9/grote/collections/__init__.py
+-rw-r--r--   0        0        0     3135 2024-04-15 14:06:10.153271 grote-0.1.9/grote/collections/base.py
+-rw-r--r--   0        0        0     1386 2024-04-15 14:17:03.812700 grote-0.1.9/grote/collections/config.yaml
+-rw-r--r--   0        0        0     3962 2024-04-09 15:45:14.921487 grote-0.1.9/grote/collections/load.py
+-rw-r--r--   0        0        0     8596 2024-04-15 14:12:45.901820 grote-0.1.9/grote/collections/translate.py
+-rw-r--r--   0        0        0     2774 2024-04-10 21:51:22.581671 grote-0.1.9/grote/config.py
+-rw-r--r--   0        0        0      299 2024-04-10 21:31:45.750995 grote-0.1.9/grote/config.yaml
+-rw-r--r--   0        0        0     9690 2024-02-03 13:44:49.951724 grote-0.1.9/grote/event_logging.py
+-rw-r--r--   0        0        0      619 2024-04-09 15:48:39.327445 grote-0.1.9/grote/functions/__init__.py
+-rw-r--r--   0        0        0     5871 2024-04-15 14:55:50.690331 grote-0.1.9/grote/functions/load.py
+-rw-r--r--   0        0        0     3529 2024-04-10 21:35:57.692323 grote-0.1.9/grote/functions/translate.py
+-rw-r--r--   0        0        0      636 2024-04-09 11:50:18.551110 grote-0.1.9/grote/style.py
+-rw-r--r--   0        0        0     3659 2024-04-15 14:57:07.057408 grote-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2422 1970-01-01 00:00:00.000000 grote-0.1.9/PKG-INFO
```

### Comparing `grote-0.1.8/LICENSE` & `grote-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `grote-0.1.8/README.md` & `grote-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `grote-0.1.8/grote/collections/base.py` & `grote-0.1.9/grote/collections/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from dataclasses import dataclass
 from functools import wraps
 from pathlib import Path
 from typing import Callable, ClassVar, TypeVar
 
 import gradio as gr
 import yaml
+import inspect
 from gradio.blocks import BlockContext
 
 T = TypeVar("T", bound="ComponentCollection")
 
 NON_EDITABLE_COMPONENTS = [gr.Markdown, gr.Button]
 
 COMPONENT_CONFIGS = yaml.safe_load(open(Path(__file__).parent / "config.yaml", encoding="utf8"))
@@ -74,15 +75,18 @@
     def state(self, state: gr.State) -> None:
         self._state = state
 
     @classmethod
     def make_component(cls, elem_id: str, **kwargs) -> gr.components.Component:
         if not hasattr(cls, f"get_{elem_id}"):
             raise ValueError(f"Method get_{elem_id} not found for class {cls.__name__}.")
-        return getattr(cls, f"get_{elem_id}")(**kwargs)
+        builder_fn = getattr(cls, f"get_{elem_id}")
+        # Filter kwargs to only pass those that are accepted by the builder function
+        kwargs = {k: v for k, v in kwargs.items() if k in inspect.signature(builder_fn).parameters}
+        return builder_fn(**kwargs)
 
     @classmethod
     @buildmethod
     def build(cls: T, **kwargs) -> T:
         raise NotImplementedError
 
     @abstractmethod
```

### Comparing `grote-0.1.8/grote/collections/config.yaml` & `grote-0.1.9/grote/collections/config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,16 @@
     input_description: "<h3>2. 📝 Input sentences: Upload a file containing source sentences and translations in SOURCE ||| TRANSLATION format</h3>"
     file_label: "Input file"
     sentences_label: "Input sentences"
     sentences_placeholder: "Insert one sentence with format SOURCE ||| TARGET per line..."
     start_button_label: "📝 Start"
 translate:
     source_side_label: "<h3>Source sentences</h3><p>These are the original sentences you need to translate.</p>"
-    target_side_label: "<h3>Translations with&nbsp;<span style='background-color: #fee2e2; color: black;'>potential issues</span></h3><p>Use the green checkmark to remove remaining highlights after editing.</p>"
+    target_side_label: "<h3>Translations with potential issues</h3><p>These are pre-translated sentences that may require editing. Use the green checkmark to remove remaining highlights if needed.</p>"
+    target_side_label_no_highlights: "<h3>Translations with potential issues</h3>"
     reload_button_label: "⬅️ Back to data loading"
     done_button_label: "✅ Done"
     download_button_label: "📥 Download translations"
     source_textbox_label: "Source text"
     target_textbox_label: "Translation"
     legend_label: "Potential issue severity"
+    legend_label_no_highlights: "These are pre-translated sentences that may require editing."
```

### Comparing `grote-0.1.8/grote/collections/load.py` & `grote-0.1.9/grote/collections/load.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.8/grote/collections/translate.py` & `grote-0.1.9/grote/collections/translate.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,26 +47,28 @@
     @classmethod
     def get_source_side_label_cap(cls, value: str | None = None, visible: bool = False) -> gr.Markdown:
         if not value:
             value = TRANS_CFG["source_side_label"]
         return gr.Markdown(value, visible=visible, elem_id="source_side_label_cap")
 
     @classmethod
-    def get_target_side_label_cap(cls, value: str | None = None, visible: bool = False) -> gr.Markdown:
+    def get_target_side_label_cap(cls, value: str | None = None, visible: bool = False, has_highlights: bool = True) -> gr.Markdown:
         if not value:
-            value = TRANS_CFG["target_side_label"]
+            value = TRANS_CFG["target_side_label"] if has_highlights else TRANS_CFG["target_side_label_no_highlights"]
         return gr.Markdown(value, visible=visible, elem_id="target_side_label_cap")
 
     @classmethod
-    def get_target_side_legend_cap(cls, value: str | None = None, visible: bool = False) -> gr.Markdown:
-        if not value and cfg.tag_labels and cfg.tag_colors:
+    def get_target_side_legend_cap(cls, value: str | None = None, visible: bool = False, has_highlights: bool = True) -> gr.Markdown:
+        if not value and cfg.tag_labels and cfg.tag_colors and has_highlights:
             value = f"<b>{TRANS_CFG['legend_label']}:</b>" + "".join(
                 f'<span style="background-color:{color}; margin-left: 0.5em; color: black; padding: 0px 5px;">{label}</span>'
                 for label, color in zip(cfg.tag_labels, cfg.tag_colors)
             )
+        elif not value and not has_highlights:
+            value = TRANS_CFG['legend_label_no_highlights']
         return gr.Markdown(value, visible=visible, elem_id="target_side_legend_cap")
 
     @classmethod
     def get_reload_btn(cls, visible: bool = False) -> gr.Button:
         return gr.Button(TRANS_CFG["reload_button_label"], variant="secondary", elem_id="reload_btn", visible=visible)
 
     @classmethod
@@ -91,14 +93,15 @@
     def get_textbox_txt(
         cls,
         type: Literal["source", "target"],
         id: int,
         value: str | Callable = "",
         visible: bool = False,
         lines: int = 2,
+        has_highlights: bool = True
     ) -> gr.components.Textbox | HighlightedTextbox:
         if type == "source":
             return gr.Textbox(
                 label=TRANS_CFG["source_textbox_label"],
                 lines=lines,
                 elem_id=f"{type}_{id}_txt",
                 value=value,
@@ -123,15 +126,15 @@
                 label=TRANS_CFG["target_textbox_label"],
                 elem_id=f"{type}_{id}_txt",
                 interactive=True,
                 show_label=False,
                 show_legend=False,
                 combine_adjacent=True,
                 visible=visible,
-                show_remove_tags_button=True,
+                show_remove_tags_button=has_highlights,
                 color_map=color_map,
             )
 
     @classmethod
     @buildmethod
     def build(
         cls: TranslateComponents,
```

### Comparing `grote-0.1.8/grote/config.py` & `grote-0.1.9/grote/config.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.8/grote/event_logging.py` & `grote-0.1.9/grote/event_logging.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.8/grote/functions/__init__.py` & `grote-0.1.9/grote/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.8/grote/functions/load.py` & `grote-0.1.9/grote/functions/load.py`

 * *Files 23% similar despite different names*

```diff
@@ -50,32 +50,36 @@
 
     if not all(" ||| " in s for s in sentences_txt):
         raise gr.Error("ERROR: Sentences must match the format SOURCE ||| TARGET")
 
     source_sentences = [sent.split(" ||| ")[0] for sent in sentences_txt]
     target_sentences = [sent.split(" ||| ")[1] for sent in sentences_txt]
     # Check wellformedness of source and target sentences (highlights allowed in target sentences only)
-    find_tag_pattern = rf"(<\/?[{'|'.join(cfg.allowed_tags)}]>)"
+    find_tag_pattern = rf"(<\/?(?:{'|'.join(cfg.allowed_tags)})>)"
+    open_tags = [f"<{tag}>" for tag in cfg.allowed_tags]
+    close_tags = [f"</{tag}>" for tag in cfg.allowed_tags]
     source_matches = [(m.group(0),) + m.span() for m in re.finditer(find_tag_pattern, "\n".join(source_sentences))]
     if len(source_matches) > 0:
         raise gr.Error("ERROR: Source sentences cannot contain highlights.")
+    state["_has_highlights"] = False
     for tgt_sent_idx, target_sentence in enumerate(target_sentences, start=1):
         target_matches = [(m.group(0),) + m.span() for m in re.finditer(find_tag_pattern, target_sentence)]
         num_matches = len(target_matches)
         if num_matches > 0:
             if num_matches % 2 != 0:
                 raise gr.Error(f"ERROR: Target sentence {tgt_sent_idx} contains an unclosed highlight.")
             for curr_match_idx, match in enumerate(target_matches, start=1):
-                if (curr_match_idx % 2 != 0 and not match[0].startswith("</")) or (
-                    curr_match_idx % 2 == 0 and match[0].startswith("</")
+                if (curr_match_idx % 2 != 0 and match[0] not in open_tags) or (
+                    curr_match_idx % 2 == 0 and match[0] not in close_tags
                 ):
                     raise gr.Error(
                         f"ERROR: Target sentence {tgt_sent_idx} contains an invalid highlight ({curr_match_idx},"
                         f" {match[0]})."
                     )
+            state["_has_highlights"] = True
     state["login_code_txt"] = login_code_txt
     state["file_in"] = None
     state["_filename"] = Path(file_in.name).stem if file_in is not None else "grote_sentences.txt"
     state["sentences_txt"] = sentences_txt
     return state
 
 
@@ -90,26 +94,26 @@
     lc_components = []
     for lc_elem_id in lc_state.keys():
         if not lc_elem_id.startswith("_"):
             lc_components.append(LoadComponents.make_component(lc_elem_id, visible=False))
     tc_components = []
     for tc_elem_id in tc_state.keys():
         if not tc_elem_id.startswith("_") and not tc_elem_id.endswith("_txt"):
-            tc_components.append(TranslateComponents.make_component(tc_elem_id, visible=True))
+            tc_components.append(TranslateComponents.make_component(tc_elem_id, visible=True, has_highlights=lc_state["_has_highlights"]))
     for tc_elem_id in [k for k in tc_state.keys() if k.endswith("_txt")]:
         txt_type, txt_id, _ = tc_elem_id.split("_")
         if int(txt_id) < len(source_sentences):
             if txt_type == "source":
                 curr_sent = source_sentences[int(txt_id)]
             elif txt_type == "target":
                 curr_sent = target_sentences[int(txt_id)]
-            tc_components.append(TranslateComponents.get_textbox_txt(txt_type, txt_id, curr_sent, visible=True))
+            tc_components.append(TranslateComponents.get_textbox_txt(txt_type, txt_id, curr_sent, visible=True, has_highlights=lc_state["_has_highlights"]))
             tc_state[f"{txt_type}_{txt_id}_txt"] = curr_sent
         else:
-            tc_components.append(TranslateComponents.get_textbox_txt(txt_type, txt_id, "", visible=False))
+            tc_components.append(TranslateComponents.get_textbox_txt(txt_type, txt_id, "", visible=False, has_highlights=lc_state["_has_highlights"]))
     n_hid = cfg.max_num_sentences - num_sentences
     return (
         [TranslateComponents.get_textboxes_col(visible=True)]
         + [lc_state]
         + lc_components
         + [tc_state]
         + tc_components
```

### Comparing `grote-0.1.8/grote/functions/translate.py` & `grote-0.1.9/grote/functions/translate.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.8/grote/style.py` & `grote-0.1.9/grote/style.py`

 * *Files identical despite different names*

### Comparing `grote-0.1.8/pyproject.toml` & `grote-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.6.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "grote"
-version = "0.1.8"
+version = "0.1.9"
 description = "Groningen Translation Environment"
 readme = "README.md"
 authors = ["Gabriele Sarti"]
 maintainers = ["Gabriele Sarti <gabriele.sarti996@gmail.com>"]
 license = "Apache Software License 2.0"
 repository = "https://github.com/gsarti/grote"
 homepage = "https://github.com/gsarti/grote"
@@ -37,15 +37,15 @@
 "grote" = "grote.app:main"
 
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 
 gradio = "^4.26.0"
-gradio_highlightedtextbox = "^0.0.11"
+gradio_highlightedtextbox = "^0.0.12"
 toml = "^0.10.2"
 
 ipykernel = { version = "^6.19.2", optional = true }
 ipywidgets = { version = "^8.0.0rc2", optional = true }
 jupyterlab = { version = "^4.0.7", optional = true }
 
 [tool.poetry.group.lint.dependencies]
```

### Comparing `grote-0.1.8/PKG-INFO` & `grote-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grote
-Version: 0.1.8
+Version: 0.1.9
 Summary: Groningen Translation Environment
 Home-page: https://github.com/gsarti/grote
 License: Apache Software License 2.0
 Keywords: translation environment,gradio
 Author: Gabriele Sarti
 Maintainer: Gabriele Sarti
 Maintainer-email: gabriele.sarti996@gmail.com
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Provides-Extra: notebook
 Requires-Dist: gradio (>=4.26.0,<5.0.0)
-Requires-Dist: gradio_highlightedtextbox (>=0.0.11,<0.0.12)
+Requires-Dist: gradio_highlightedtextbox (>=0.0.12,<0.0.13)
 Requires-Dist: ipykernel (>=6.19.2,<7.0.0) ; extra == "notebook"
 Requires-Dist: ipywidgets (>=8.0.0rc2,<9.0.0) ; extra == "notebook"
 Requires-Dist: jupyterlab (>=4.0.7,<5.0.0) ; extra == "notebook"
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: Repository, https://github.com/gsarti/grote
 Description-Content-Type: text/markdown
```

