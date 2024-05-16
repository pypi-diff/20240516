# Comparing `tmp/obsidian_to_typst-0.1.1.tar.gz` & `tmp/obsidian_to_typst-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsidian_to_typst-0.1.1.tar", max compression
+gzip compressed data, was "obsidian_to_typst-0.1.2.tar", max compression
```

## Comparing `obsidian_to_typst-0.1.1.tar` & `obsidian_to_typst-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2249 2024-02-26 00:09:06.837145 obsidian_to_typst-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      827 2024-02-25 23:53:08.217951 obsidian_to_typst-0.1.1/README.md
--rw-r--r--   0        0        0       68 2023-12-26 19:31:07.784431 obsidian_to_typst-0.1.1/src/obsidian_to_typst/__init__.py
--rw-r--r--   0        0        0      888 2023-12-28 17:09:49.068405 obsidian_to_typst-0.1.1/src/obsidian_to_typst/document.typ
--rw-r--r--   0        0        0      629 2023-12-26 19:31:07.787026 obsidian_to_typst-0.1.1/src/obsidian_to_typst/obsidian_path.py
--rw-r--r--   0        0        0     3628 2023-12-28 03:45:58.240159 obsidian_to_typst-0.1.1/src/obsidian_to_typst/obsidian_to_typst.py
--rw-r--r--   0        0        0    13562 2024-02-25 23:53:08.226776 obsidian_to_typst-0.1.1/src/obsidian_to_typst/process_markdown.py
--rw-r--r--   0        0        0     1742 1970-01-01 00:00:00.000000 obsidian_to_typst-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      848 2024-05-11 17:51:07.854713 obsidian_to_typst-0.1.2/README.md
+-rw-r--r--   0        0        0     2248 2024-05-12 01:46:05.787967 obsidian_to_typst-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       65 2024-05-11 22:18:00.613969 obsidian_to_typst-0.1.2/src/obsidian_to_typst/__init__.py
+-rw-r--r--   0        0        0      888 2024-05-11 16:59:08.411928 obsidian_to_typst-0.1.2/src/obsidian_to_typst/document.typ
+-rw-r--r--   0        0        0      750 2024-05-12 01:37:37.339987 obsidian_to_typst-0.1.2/src/obsidian_to_typst/obsidian_path.py
+-rw-r--r--   0        0        0     3663 2024-05-11 22:39:44.038387 obsidian_to_typst-0.1.2/src/obsidian_to_typst/obsidian_to_typst.py
+-rw-r--r--   0        0        0    13756 2024-05-16 08:02:52.714568 obsidian_to_typst-0.1.2/src/obsidian_to_typst/process_markdown.py
+-rw-r--r--   0        0        0     1763 1970-01-01 00:00:00.000000 obsidian_to_typst-0.1.2/PKG-INFO
```

### Comparing `obsidian_to_typst-0.1.1/pyproject.toml` & `obsidian_to_typst-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 authors = ["Ryan Bartling <ryan.bartling@gmail.com>"]
 description = "Convert Obsidian vault documents to typst and pdfs"
 license = "MIT"
 name = "obsidian-to-typst"
 readme = "README.md"
 repository = "https://github.com/drbartling/obsidian-to-typst"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.poetry.scripts]
 obsidian-to-typst = "obsidian_to_typst.obsidian_to_typst:main"
 
 [tool.poetry.dependencies]
+python = "^3.9,<3.13"
 click = "^8.1.7"
 colorama = "^0.4.6"
 coloredlogs = "^15.0.1"
 colored-traceback = "^0.3.0"
-pydantic = "^2.5.3"
-python = "^3.9,<3.13"
+pydantic = "^2.7.1"
 
 [tool.poetry.group.dev.dependencies]
 behave = "^1.2.6"
-black = "^23.12.1"
-coverage = "^7.4.0"
+black = "^24.4.2"
+coverage = "^7.5.1"
 devtools = "^0.12.2"
 isort = "^5.13.2"
-pre-commit = "^3.6.0"
-pylint = "^3.0.3"
-pytest = "^7.4.4"
-pytest-cov = "^4.1.0"
+pre-commit = "^3.7.0"
+pylint = "^3.1.0"
+pytest = "^8.2.0"
+pytest-cov = "^5.0.0"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.black]
 exclude = '''
```

### Comparing `obsidian_to_typst-0.1.1/README.md` & `obsidian_to_typst-0.1.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 Install typst using a package manager or `cargo install`
 
 Run `poetry install` and `poetry shell` to install and and activate the python virtual environment.
 
 Than, run `obsidian_to_typst .\examples\feature_guide\Widget.md` to convert the example document to a PDF.  The PDF will be placed in `.\examples\feature_guide\output\Widget.pdf`.
 
 ```powershell
-watchexec.exe -crd500 -e py "isort . && black . && pytest && obsidian_to_typst.cmd .\examples\feature_guide\Widget.md"
+watchexec --clear --restart --debounce 500 --exts py "isort . && black . && pytest && obsidian-to-typst ./examples/feature_guide/Widget.md"
 ```
```

### Comparing `obsidian_to_typst-0.1.1/src/obsidian_to_typst/document.typ` & `obsidian_to_typst-0.1.2/src/obsidian_to_typst/document.typ`

 * *Files identical despite different names*

### Comparing `obsidian_to_typst-0.1.1/src/obsidian_to_typst/obsidian_path.py` & `obsidian_to_typst-0.1.2/src/obsidian_to_typst/obsidian_path.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,7 +18,12 @@
     raise FileNotFoundError(
         f"Unable to locate `{file_name}` under `{VAULT_ROOT}`"
     )
 
 
 def rel_path(path: Path) -> Path:
     return Path(os.path.relpath(path, TEMP_FOLDER))
+
+
+def root_path(path: Path) -> str:
+    path = path.resolve()
+    return os.path.sep + os.path.relpath(path, VAULT_ROOT)
```

### Comparing `obsidian_to_typst-0.1.1/src/obsidian_to_typst/obsidian_to_typst.py` & `obsidian_to_typst-0.1.2/src/obsidian_to_typst/obsidian_to_typst.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,33 +22,35 @@
     type=click.Path(path_type=Path, resolve_path=True),
 )
 @click.option(
     "-t",
     "--template",
     type=click.Path(path_type=Path, resolve_path=True),
 )
-@pydantic.validate_arguments
+@pydantic.validate_call
 def main(filename: Path, template: Optional[Path]):  # pragma: no cover
     colorama.init()
     colored_traceback.add_hook()
     coloredlogs.install(level="INFO")
     try:
         app_main(filename, template)
-    except Exception as e:
+    except Exception as _e:
         logger.critical("Failed to export document to PDF using typst")
         raise
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def app_main(filename: Path, template: Optional[Path]):  # pragma: no cover
+    # pylint: disable=too-many-locals
     obsidian_path.VAULT_ROOT = get_vault_root(filename)
 
     # pylint: disable=protected-access
-    with open(filename, "r", encoding="UTF-8") as f:
+    with filename.open(mode="r", encoding="utf-8") as f:
         text = f.read()
+
     title = get_title(text)
     temp_dir = filename.parent / "temp"
     obsidian_path.TEMP_FOLDER = temp_dir
     temp_dir.mkdir(parents=True, exist_ok=True)
     temp_file = temp_dir / "body.typ"
 
     process_markdown.init_state(temp_dir, filename)
@@ -72,15 +74,15 @@
     args = [
         "typst",
         "compile",
         temp_wrapper,
         "--root",
         obsidian_path.VAULT_ROOT,
     ]
-    logging.info(f"Running `{' '.join([str(a) for a in args])}`")
+    logging.info("Running `%s`", " ".join([str(a) for a in args]))
     try:
         typst_result = subprocess.run(
             args,
             check=True,
             capture_output=False,
             cwd=temp_wrapper.parent,
         )
```

### Comparing `obsidian_to_typst-0.1.1/src/obsidian_to_typst/process_markdown.py` & `obsidian_to_typst-0.1.2/src/obsidian_to_typst/process_markdown.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,87 +10,93 @@
 from obsidian_to_typst import obsidian_path
 
 _logger = logging.getLogger(__name__)
 
 referenced_docs = set()
 docs_embedded = set()
 
+EMBEDDED_IMAGE_REGEX = r"!\[\[([\s_a-zA-Z0-9.]*)\|?([0-9]+)?x?([0-9]+)?]]"
+
 
 @dataclass
 class Indent:
     list_type: str
     depth: str
 
 
 @dataclass
 class State:
+    # pylint: disable=too-many-instance-attributes
     heading_depth: int
+    parent_heading_depth: int
     code_block: Optional[int]
     code_buffer: str
     mermaid_block: Optional[int]
     file: List[Path]
     temp_dir: Optional[Path]
     typst_block: Optional[int]
 
     @classmethod
     def new(cls):
         return cls(
             heading_depth=0,
+            parent_heading_depth=0,
             code_block=None,
             code_buffer="",
             mermaid_block=None,
             file=[],
             temp_dir=None,
             typst_block=None,
         )
 
     def init(self, temp_dir: Path, file: Path):
         self.heading_depth = 0
+        self.parent_heading_depth = 0
         self.code_block = None
         self.code_buffer = ""
         self.mermaid_block = None
         self.file = [file]
         self.temp_dir = temp_dir
         self.typst_block = None
 
 
 STATE: State = State.new()
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def init_state(temp_dir: Path, file: Path) -> None:
     STATE.init(temp_dir, file)
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def obsidian_to_typst(input_text: str) -> str:
     lines = input_text.splitlines()
     lines = [_line_to_typst(i + 1, line) for i, line in enumerate(lines)]
     lines = [line for line in lines if line is not None]
     lines.append("")
     text = "\n".join(lines)
     text = text + cleanup()
     return text
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def _line_to_typst(
     lineno: int,
     line: str,
 ) -> str:
     try:
         return line_to_typst(lineno, line)
     except Exception:  # pragma: no cover
         logging.getLogger(__name__).error(
             "Failed to parse `%s:%s`", STATE.file[-1], lineno
         )
         raise
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def line_to_typst(
     lineno: int,
     line: str,
 ) -> Optional[str]:
     # pylint: disable=too-many-return-statements
 
     if is_code_block_toggle(line):
@@ -104,137 +110,140 @@
         return embed_file(line)
     if line.startswith("#"):
         return line_to_section(line)
     line = string_to_typst(line)
     return line
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def line_to_section(line: str) -> str:
     assert line.startswith("#"), line
     section_lookup = {
         2: "=",
         3: "==",
         4: "===",
         5: "====",
         6: "=====",
     }
     s, line = re.match(r"(#*)\s*(.*)", line).groups()
-    STATE.heading_depth = len(s)
+    STATE.heading_depth = len(s) + STATE.parent_heading_depth
 
     if STATE.heading_depth not in section_lookup:
         return line + "\n\n"
 
     line = string_to_typst(line)
     section_text = f"#heading(level:{STATE.heading_depth - 1})[{line}]"
 
     return section_text
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def is_embedded(line: str) -> bool:
-    return line.startswith("![[") and line.endswith("]]")
+    stripped = line.strip()
+    return stripped.startswith("![[") and stripped.endswith("]]")
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def embed_file(line: str) -> str:
-    if is_markdown(line):
-        return embed_markdown(line)
-    if is_image(line):
-        return embed_image(line)
-    raise Exception(f"Unable to embed {line}")  # pragma: no cover
+    stripped = line.strip()
+    if is_markdown(stripped):
+        return embed_markdown(stripped)
+    if is_image(stripped):
+        return embed_image(stripped)
+    raise Exception(f"Unable to embed {stripped}")  # pragma: no cover
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def is_markdown(line: str) -> bool:
     m = re.match(r"!\[\[(.*)]]", line)
     file_name = m.group(1)
     return Path(file_name).suffix == ""
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def embed_markdown(embed_line: str) -> str:
     m = re.match(r"!\[\[(.*)]]", embed_line)
     file_name = m.group(1)
     assert is_markdown(embed_line), embed_line
 
     file_name = file_name + ".md"
     file = obsidian_path.find_file(file_name)
 
     with open(file, "r", encoding="UTF-8") as f:
         text = f.read()
-    lines = text.splitlines()
-    for i, line in enumerate(lines):
-        if line.startswith("#"):
-            lines[i] = "#" * (STATE.heading_depth - 1) + line
-    text = "\n".join(lines)
 
     STATE.file.append(file)
-    current_depth = STATE.heading_depth
+    current_parent_depth = STATE.parent_heading_depth
+    STATE.parent_heading_depth = STATE.heading_depth - 1
     try:
         result = obsidian_to_typst(text)
     finally:
         STATE.file.pop()
-        STATE.heading_depth = current_depth
+        STATE.heading_depth = STATE.parent_heading_depth + 1
+        STATE.parent_heading_depth = current_parent_depth
 
     ref_label = file_ref_label(file)
     docs_embedded.add(ref_label)
     return file_label(file) + result
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def is_image(line: str) -> bool:
-    m = re.match(r"!\[\[([\s_a-zA-Z0-9.]*)(\|)?([0-9x]+)?]]", line)
+    m = re.match(EMBEDDED_IMAGE_REGEX, line)
     if not m:
         return False
     file_name = m.group(1)
-    return Path(file_name).suffix.lower() in [".png", ".bmp", ".svg"]
+    return Path(file_name).suffix.lower() in [".jpg", ".png", ".bmp", ".svg"]
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def embed_image(line: str) -> str:
     assert is_image(line), line
-    m = re.match(r"!\[\[([\s_a-zA-Z0-9.]*)\|?([0-9]+)?x?([0-9]+)?]]", line)
+    m = re.match(EMBEDDED_IMAGE_REGEX, line)
     if not m:  # pragma: no cover
         raise Exception(line)
     file_name, width, height = m.groups()
-    return include_image(obsidian_path.find_file(file_name), width, height)
+    return include_image(
+        obsidian_path.find_file(file_name),
+        width,
+        height,
+    )
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def include_image(
     image_path: Path, width: Optional[int], height: Optional[int]
 ) -> str:
-    width_text = R"80%" if width is None else f"{int(width/2)}pt"
-    height_text = "" if height is None else f"height:{int(height/2)}pt,"
+    width_text = R"80%" if width is None else f"{int(width / 2)}pt"
+    height_text = "" if height is None else f"height:{int(height / 2)}pt,"
 
-    image_path = obsidian_path.rel_path(image_path)
+    image_path = obsidian_path.root_path(image_path)
     return f'#image("{image_path}",width:{width_text},{height_text})'
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def is_code_block_toggle(line: str) -> bool:
     return re.match(r"\s*```", line) is not None
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def toggle_code_block(
     lineno: int,
     line: str,
 ) -> str:
     # pylint: disable=global-statement
     if not (STATE.code_block or STATE.mermaid_block):
         STATE.code_buffer = ""
         lang = line[3:]
         if "mermaid" == lang:
             STATE.mermaid_block = lineno
             lines = [
                 R"",
                 R"#image(",
-                f'"{STATE.file[-1].stem}_{STATE.mermaid_block}.svg",',
+                f'"{STATE.file[-1].stem}_{STATE.mermaid_block}.png",',
                 R"width: 80%)",
             ]
             return "\n".join(lines)
 
         if "typst" == lang:
             STATE.code_block = lineno
             STATE.typst_block = lineno
@@ -269,74 +278,49 @@
         assert STATE.temp_dir, STATE.temp_dir
         process_mermaid_diagram()
         STATE.mermaid_block = None
         lines = []
     return "\n".join(lines)
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def process_mermaid_diagram():  # pragma: no cover
     assert STATE.temp_dir, STATE.temp_dir
     assert STATE.mermaid_block, STATE.mermaid_block
     assert STATE.file, STATE.file
     mmd_file: Path = (
         STATE.temp_dir / f"{STATE.file[-1].stem}_{STATE.mermaid_block}.mmd"
     )
-    pdf_file = mmd_file.with_suffix(".pdf")
-    img_file = mmd_file.with_suffix(".svg")
+    img_file = mmd_file.with_suffix(".png")
     with open(mmd_file, "w", encoding="UTF-8") as f:
         f.write(STATE.code_buffer)
-    cmd = [
-        "mmdc",
-        "--input",
-        mmd_file,
-        "--output",
-        pdf_file,
-        "--pdfFit",
-    ]
+    cmd_str = (
+        "mmdc "
+        f"--input '{mmd_file}' "
+        f"--output '{img_file}' "
+        "--backgroundColor transparent "
+        "--scale 4 "
+    )
     try:
-        subprocess.run(cmd, shell=True, check=True)
+        subprocess.run(cmd_str, shell=True, check=True)
     except subprocess.CalledProcessError:
         _logger.error(
             "Failed to generate MMD diagram for `%s` with command `%s`.",
             STATE.file[-1],
-            " ".join(
-                [f'"{c}"' if isinstance(c, Path) else str(c) for c in cmd]
-            ),
-        )
-        raise
-    cmd = [
-        "mutool",
-        "draw",
-        "-o",
-        img_file,
-        pdf_file,
-    ]
-    _logger.info(
-        "Calling `%s`",
-        " ".join([f'"{c}"' if isinstance(c, Path) else str(c) for c in cmd]),
-    )
-    try:
-        subprocess.run(cmd, shell=True, check=True)
-    except subprocess.CalledProcessError:
-        _logger.error(
-            "Failed to generate svg file from pdf with command `%s`",
-            " ".join([str(c) for c in cmd]),
+            cmd_str,
         )
         raise
-    temp_img_file = img_file.with_name(img_file.stem + "1" + ".svg")
-    temp_img_file.replace(img_file)
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def sanitize_special_characters(line: str) -> str:
     return re.sub(r"([&$#%{}])(?!.*`)", r"\\\1", line)
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def cleanup():
     assert (
         not STATE.code_block
     ), f"Reached end of file without closing code block from line {STATE.code_block}"
     lines = [""]
     if len(STATE.file) == 1:
         undefined_refs = [
@@ -344,52 +328,63 @@
         ]
         for ref in undefined_refs:
             lines.append(f"<{ref}>")
             _logger.warning("Undefined ref %s", ref)
     return "\n\n.".join(lines)
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def string_to_typst(unprocessed_text: str) -> str:
     logging.getLogger(__name__).debug("unprocessed_text %s", unprocessed_text)
     processed_text = ""
 
-    while unprocessed_text:
-        char = unprocessed_text[0]
-        unprocessed_text = unprocessed_text[1:]
-        if char == "`":
-            pt, unprocessed_text = split_verbatim(unprocessed_text)
-            processed_text += pt
-        elif char == "*":
-            pt, unprocessed_text = split_formatted(unprocessed_text)
-            processed_text += pt
-        elif char == "[":
-            pt, unprocessed_text = split_link(unprocessed_text)
-            processed_text += pt
-        elif char == "^":
-            pt, unprocessed_text = split_reference(unprocessed_text)
-            processed_text += pt
-        elif char == "\\":
-            pt, unprocessed_text = split_escaped_text(unprocessed_text)
-            processed_text += pt
-        else:
-            processed_text += sanitize_special_characters(char)
+    try:
+        while unprocessed_text:
+            char = unprocessed_text[0]
+            unprocessed_text = unprocessed_text[1:]
+            if char == "`":
+                pt, unprocessed_text = split_verbatim(unprocessed_text)
+                processed_text += pt
+            elif char == "*":
+                pt, unprocessed_text = split_formatted(unprocessed_text)
+                processed_text += pt
+            elif char == "[":
+                pt, unprocessed_text = split_link(unprocessed_text)
+                processed_text += pt
+            elif char == "^":
+                pt, unprocessed_text = split_reference(unprocessed_text)
+                processed_text += pt
+            elif char == "\\":
+                pt, unprocessed_text = split_escaped_text(unprocessed_text)
+                processed_text += pt
+            elif char == "!":
+                pt, unprocessed_text = split_embedded_doc(
+                    char + unprocessed_text
+                )
+                processed_text += pt
+            else:
+                processed_text += sanitize_special_characters(char)
+    except Exception:
+        logging.getLogger(__name__).error(
+            "Failed to parse `%s`", unprocessed_text
+        )
+        raise
 
     return processed_text
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def split_verbatim(text: str) -> Tuple[str, str]:
     processed_text = R"`"
     verb_text, unprocessed_text = re.match(r"(.*?`)(.*)", text).groups()
     processed_text += verb_text
     return processed_text, unprocessed_text
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def split_formatted(text: str) -> Tuple[str, str]:
     if text.startswith("*"):
         return split_bold(text)
     return split_italics(text)
 
 
 def split_bold(text: str) -> Tuple[str, str]:
@@ -410,36 +405,36 @@
 
     italic_text = string_to_typst(italic_text)
     processed_text += italic_text
     processed_text += R"_"
     return processed_text, unprocessed_text
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def split_link(text: str) -> Tuple[str, str]:
     return (
         split_markdown_link(text)
         or split_document_link(text)
         or split_paragraph_link(text)
         or (R"\[", text)
     )
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def split_markdown_link(text: str) -> Optional[Tuple[str, str]]:
     m = re.match(r"(.*?)]\((.*?)\)(.*)", text)
     if not m:
         return None
     disp_text, link, unprocessed_text = m.groups()
     disp_text = sanitize_special_characters(disp_text)
     processed_text = f"\\href{{{link}}}{{{disp_text}}}"
     return processed_text, unprocessed_text
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def split_document_link(text: str) -> Optional[Tuple[str, str]]:
     m = re.match(r"\[(.+?)]](.*)", text)
     if not m:
         return None
     link_text, unprocessed_text = m.groups()
 
     m = re.match(r"([a-zA-Z0-9-_\s]+)\|?(.+?)?", link_text)
@@ -452,42 +447,52 @@
     disp_text = (
         sanitize_special_characters(disp_text) if disp_text else doc_name
     )
     processed_text = f"#link(<{doc_ref}>)[{disp_text}]"
     return processed_text, unprocessed_text
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def split_paragraph_link(text: str) -> Optional[Tuple[str, str]]:
     m = re.match(r"\[#\^([a-zA-Z0-9-]+)\|?(.+)]](.*)", text)
     if not m:
         return None
     link, disp_text, unprocessed_text = m.groups()
     disp_text = sanitize_special_characters(disp_text)
     processed_text = f"#link(<{link}>)[{disp_text}]"
     return processed_text, unprocessed_text
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def split_reference(text: str) -> Tuple[str, str]:
     m = re.match(r"([a-zA-Z0-9-]+)$", text)
     if not m:
         return R"^", text
     ref_text = m.groups()[0]
     return f"<{ref_text}>", ""
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def split_escaped_text(text: str) -> Tuple[str, str]:
     escaped_text = "\\" + text[0]
     unprocessed_text = text[1:]
     return escaped_text, unprocessed_text
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
+def split_embedded_doc(text: str) -> tuple((str, str)):
+    if is_image(text):
+        image_splitter = EMBEDDED_IMAGE_REGEX + r"(.*)"
+        m = re.match(image_splitter, text)
+        unprocessed_text = m.groups()[-1]
+        return embed_image(text), unprocessed_text
+    return "!", ""
+
+
+@pydantic.validate_call
 def file_label(file_path: Path) -> str:
     return f"<{file_ref_label(file_path)}>"
 
 
-@pydantic.validate_arguments
+@pydantic.validate_call
 def file_ref_label(file_path: Path) -> str:
     return "file_" + file_path.name.lower().replace(".", "_").replace(" ", "_")
```

### Comparing `obsidian_to_typst-0.1.1/PKG-INFO` & `obsidian_to_typst-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsidian-to-typst
-Version: 0.1.1
+Version: 0.1.2
 Summary: Convert Obsidian vault documents to typst and pdfs
 Home-page: https://github.com/drbartling/obsidian-to-typst
 License: MIT
 Author: Ryan Bartling
 Author-email: ryan.bartling@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: colored-traceback (>=0.3.0,<0.4.0)
 Requires-Dist: coloredlogs (>=15.0.1,<16.0.0)
-Requires-Dist: pydantic (>=2.5.3,<3.0.0)
+Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Project-URL: Repository, https://github.com/drbartling/obsidian-to-typst
 Description-Content-Type: text/markdown
 
 # Obsidian to Typst
 
 This utility attempts to make it easy to convert markdown documents written using obsidian into PDFs.
 
@@ -38,10 +38,10 @@
 Install typst using a package manager or `cargo install`
 
 Run `poetry install` and `poetry shell` to install and and activate the python virtual environment.
 
 Than, run `obsidian_to_typst .\examples\feature_guide\Widget.md` to convert the example document to a PDF.  The PDF will be placed in `.\examples\feature_guide\output\Widget.pdf`.
 
 ```powershell
-watchexec.exe -crd500 -e py "isort . && black . && pytest && obsidian_to_typst.cmd .\examples\feature_guide\Widget.md"
+watchexec --clear --restart --debounce 500 --exts py "isort . && black . && pytest && obsidian-to-typst ./examples/feature_guide/Widget.md"
 ```
```

