# Comparing `tmp/compact_json-1.6.1.tar.gz` & `tmp/compact_json-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compact_json-1.6.1.tar", max compression
+gzip compressed data, was "compact_json-1.8.0.tar", max compression
```

## Comparing `compact_json-1.6.1.tar` & `compact_json-1.8.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1050 2022-07-07 06:20:15.071174 compact_json-1.6.1/LICENSE.rst
--rw-r--r--   0        0        0    10954 2023-09-02 08:09:05.797759 compact_json-1.6.1/README.md
--rw-r--r--   0        0        0     1649 2023-09-02 08:50:19.919098 compact_json-1.6.1/pyproject.toml
--rw-r--r--   0        0        0      203 2022-12-18 12:58:26.530149 compact_json-1.6.1/src/compact_json/__init__.py
--rw-r--r--   0        0        0       40 2022-12-27 17:38:43.085582 compact_json-1.6.1/src/compact_json/__main__.py
--rw-r--r--   0        0        0     5571 2023-09-02 08:09:05.800363 compact_json-1.6.1/src/compact_json/_compact_json.py
--rw-r--r--   0        0        0    39596 2023-09-02 09:20:40.436340 compact_json-1.6.1/src/compact_json/formatter.py
--rw-r--r--   0        0        0    11861 1970-01-01 00:00:00.000000 compact_json-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1050 2022-07-07 06:20:15.071174 compact_json-1.8.0/LICENSE.rst
+-rw-r--r--   0        0        0    10966 2024-05-15 14:26:32.072097 compact_json-1.8.0/README.md
+-rw-r--r--   0        0        0     1772 2024-05-15 14:18:31.081851 compact_json-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      238 2024-05-13 18:18:22.485704 compact_json-1.8.0/src/compact_json/__init__.py
+-rw-r--r--   0        0        0       89 2024-05-13 18:16:36.725355 compact_json-1.8.0/src/compact_json/__main__.py
+-rw-r--r--   0        0        0     7504 2024-05-15 14:27:59.353778 compact_json-1.8.0/src/compact_json/_compact_json.py
+-rw-r--r--   0        0        0    41697 2024-05-15 14:19:29.533465 compact_json-1.8.0/src/compact_json/formatter.py
+-rw-r--r--   0        0        0    11907 1970-01-01 00:00:00.000000 compact_json-1.8.0/PKG-INFO
```

### Comparing `compact_json-1.6.1/LICENSE.rst` & `compact_json-1.8.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `compact_json-1.6.1/README.md` & `compact_json-1.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 ```
 
 ## Usage
 
 As a python package, `compact-json` is instantiated with a `Formatter` class that has a range of properties to configure the formatting:
 
 ``` python
+import json
 from compact_json import Formatter, EolStyle
 
 formatter = Formatter()
 formatter.indent_spaces = 2
 formatter.max_inline_complexity = 10
 formatter.json_eol_style = EolStyle.LF
```

### Comparing `compact_json-1.6.1/src/compact_json/_compact_json.py` & `compact_json-1.8.0/src/compact_json/_compact_json.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,132 +5,192 @@
 
 import compact_json
 from compact_json import EolStyle, Formatter, _get_version
 
 logger = logging.getLogger(compact_json.__name__)
 
 
-def command_line_parser():
+def command_line_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
-        description="Format JSON into compact, human readable form"
+        description="Format JSON into compact, human readable form",
     )
     parser.add_argument("-V", "--version", action="store_true")
 
     parser.add_argument(
         "--output",
         "-o",
-        action='append',
+        action="append",
         help="The output file name(s). The number of output file names must match "
-        "the number of input files."
+        "the number of input files.",
+    )
+    parser.add_argument(
+        "--align-expanded-property-names",
+        action="store_true",
+        default=False,
+    )
+    parser.add_argument(
+        "--align-properties",
+        default=False,
+        action="store_true",
+        help="Align property names of expanded dicts",
+    )
+    parser.add_argument(
+        "--always-expand-depth",
+        default="never",
+        choices=["never", "root", "children"],
+        help="Depth at which lists/dicts are always fully expanded",
+    )
+    parser.add_argument(
+        "--bracket-padding",
+        choices=["simple", "nested"],
+        default="nested",
+        help="If nested padding, add spaces inside outside brackes for nested lists/dicts",
+    )
+    parser.add_argument(
+        "--colon-padding",
+        action="store_true",
+        default=True,
+        help="Include a space after property colons",
+    )
+    parser.add_argument(
+        "--comma-padding",
+        action="store_true",
+        default=True,
+        help="Includes a space after commas separating list items and dict properties.",
     )
     parser.add_argument(
         "--crlf",
         default=False,
         action="store_true",
         help="Use Windows-style CRLF line endings",
     )
     parser.add_argument(
-        "--max-inline-length",
-        "-l",
-        metavar="N",
-        type=int,
-        default=50,
-        help="Limit inline elements to N chars, excluding "
-        "indentation and leading property names (default=50)",
+        "--debug",
+        default=False,
+        action="store_true",
+        help="Enable debug logging",
     )
     parser.add_argument(
-        "--max-inline-complexity",
+        "--east-asian-chars",
+        default=False,
+        action="store_true",
+        help="Treat strings as unicode East Asian characters",
+    )
+    parser.add_argument(
+        "--indent",
+        "-i",
         metavar="N",
         type=int,
-        default=2,
-        help="Maximum nesting: 0=basic types, 1=dict/list, 2=all (default=2)",
+        default=4,
+        help="Indent N spaces (default=4)",
+    )
+    parser.add_argument(
+        "--justify-numbers",
+        default=False,
+        action="store_true",
+        help="Right-align numbers with matching precision",
     )
     parser.add_argument(
         "--max-compact-list-complexity",
         metavar="N",
         type=int,
         default=1,
         help="Maximum nesting over multiple lines (default 1)",
     )
     parser.add_argument(
-        "--bracket-padding",
-        choices=["simple", "nested"],
-        default="nested",
-        help="If nested padding, add spaces inside outside brackes for nested lists/dicts",
+        "--max-inline-length",
+        "-l",
+        metavar="N",
+        type=int,
+        default=50,
+        help="Limit inline elements to N chars, excluding "
+        "indentation and leading property names (default=50)",
     )
     parser.add_argument(
-        "--indent",
-        "-i",
+        "--max-inline-complexity",
         metavar="N",
         type=int,
-        default=4,
-        help="Indent N spaces (default=4)",
+        default=2,
+        help="Maximum nesting: 0=basic types, 1=dict/list, 2=all (default=2)",
     )
     parser.add_argument(
-        "--tab-indent", default=False, action="store_true", help="Use tabs to indent"
+        "--multiline-compact-dict",
+        action="store_true",
+        default=False,
+        help="Format dict into multi-line compact style like list",
     )
     parser.add_argument(
-        "--justify-numbers",
+        "--no-ensure-ascii",
         default=False,
         action="store_true",
-        help="Right-align numbers with matching precision",
+        help="Characters will be output as-is without ASCII conversion",
+    )
+    parser.add_argument(
+        "--omit-trailing-whitespace",
+        default=False,
+        action="store_true",
+        help="Remove any trailing whitespace from output lines",
     )
     parser.add_argument(
         "--prefix-string",
         metavar="STRING",
         help="String attached to the beginning of every line",
     )
     parser.add_argument(
-        "--align-properties",
+        "--tab-indent",
         default=False,
         action="store_true",
-        help="Align property names of expanded dicts",
+        help="Use tabs to indent",
     )
     parser.add_argument(
-        "--east-asian-chars",
-        default=False,
-        action="store_true",
-        help="Treat strings as unicode East Asian characters",
-    )
-    parser.add_argument(
-        "--no-ensure-ascii",
-        default=False,
-        action="store_true",
-        help="Characters will be output as-is without ASCII conversion",
+        "--table-dict-minimum-similarity",
+        type=int,
+        default=75,
+        metavar="[0-101]",
+        choices=range(102),
+        help="Inline dict similarity threshold (101 disables table formatting",
     )
     parser.add_argument(
-        "--debug", default=False, action="store_true", help="Enable debug logging"
+        "--table-list-minimum-similarity",
+        type=int,
+        metavar="[0-101]",
+        choices=range(102),
+        default=75,
+        help="Inline list similarity threshold (101 disables table formatting",
     )
 
     parser.add_argument(
         "json",
         nargs="*",
         type=argparse.FileType("r"),
         help='JSON file(s) to parse (or stdin with "-")',
     )
     return parser
 
 
-def main():  # noqa: C901
+def main() -> None:  # noqa: C901, PLR0915, PLR0912
     parser = command_line_parser()
 
-    def die(message):
+    def die(message: str) -> None:
         print(f"{parser.prog}: {message}", file=sys.stderr)
-        exit(1)
+        sys.exit(1)
 
     args = parser.parse_args()
     if args.version:
         print(_get_version())
     elif len(args.json) == 0:
         parser.print_help()
     else:
         formatter = Formatter()
+        formatter.comma_padding = args.comma_padding
+        formatter.colon_padding = args.colon_padding
         formatter.max_inline_length = args.max_inline_length
         formatter.max_inline_complexity = args.max_inline_complexity
         formatter.max_compact_list_complexity = args.max_compact_list_complexity
+        formatter.multiline_compact_dict = args.multiline_compact_dict
         formatter.indent_spaces = args.indent
         if args.crlf:
             formatter.json_eol_style = EolStyle.CRLF
         if args.align_properties:
             formatter.align_expanded_property_names = True
         if args.bracket_padding == "simple":
             formatter.nested_bracket_padding = False
@@ -140,14 +200,15 @@
             formatter.simple_bracket_padding = False
         if args.tab_indent:
             formatter.use_tab_to_indent = True
         if not args.justify_numbers:
             formatter.dont_justify_numbers = False
         if args.prefix_string is not None:
             formatter.prefix_string = args.prefix_string
+        formatter.omit_trailing_whitespace = args.omit_trailing_whitespace
         formatter.east_asian_string_widths = args.east_asian_chars
         formatter.ensure_ascii = not args.no_ensure_ascii
 
         hdlr = logging.StreamHandler()
         hdlr.setFormatter(logging.Formatter("%(levelname)s:%(name)s:%(message)s"))
         logger.addHandler(hdlr)
         if args.debug:
```

### Comparing `compact_json-1.6.1/src/compact_json/formatter.py` & `compact_json-1.8.0/src/compact_json/formatter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,120 +1,137 @@
+"""Compact JSON formatter."""
+
+from __future__ import annotations
+
 import json
 import logging
+import re
 import warnings
 from dataclasses import dataclass
 from decimal import Decimal, InvalidOperation
 from enum import Enum, IntEnum, auto
 from functools import lru_cache
-from math import modf
-from pathlib import PosixPath
-from typing import Any, List, Union
+from typing import TYPE_CHECKING, Any
 
 from wcwidth import wcswidth
 
+if TYPE_CHECKING:
+    from pathlib import PosixPath
+
 logger = logging.getLogger(__name__)
 debug = logger.debug
 
 
 @lru_cache(4096)
-def _wcswidth(s):
+def _wcswidth(s: str) -> int:
     return wcswidth(s)
 
 
 class EolStyle(IntEnum):
+    """End of line style enumeration."""
+
     CRLF = auto()
     LF = auto()
 
 
 class JsonValueKind(IntEnum):
+    """JSON token enumeration."""
+
     UNDEFINED = auto()
     DICT = auto()
     LIST = auto()
     STRING = auto()
     INT = auto()
     FLOAT = auto()
     BOOLEAN = auto()
     NULL = auto()
 
 
 class Format(IntEnum):
+    """Format type enumeration."""
+
     INLINE = auto()
     INLINE_TABULAR = auto()
     MULTILINE_COMPACT = auto()
     EXPANDED = auto()
 
 
 class FormattedNode:
-    """Data about a JSON element and how we've formatted it"""
+    """Data about a JSON element and how we've formatted it."""
 
-    def __init__(self):
+    def __init__(self: FormattedNode) -> None:
+        """Initialise a new formating node."""
         self.name = ""
         self.name_length = 0
         self.value = ""
         self.value_length = 0
         self.complexity = 0
         self.depth = 0
         self.kind = JsonValueKind.UNDEFINED
         self.format = Format.INLINE
         self.children: list[FormattedNode] = []
 
-    def cleanup(self):
+    def cleanup(self: FormattedNode) -> None:
+        """Cleanup children."""
         if self.format != Format.INLINE:
             self.children = []
         for child in self.children:
             child.children = []
 
 
-def _fixed_value(value, num_decimals: int):
+def _fixed_value(value: str, num_decimals: int) -> str:
     if "e" in value:
         return value
 
-    if num_decimals > 0:
-        quantize_str = "0." + ("0" * (num_decimals - 1)) + "1"
-    else:
-        quantize_str = "0"
+    quantize_str = "0." + "0" * (num_decimals - 1) + "1" if num_decimals > 0 else "0"
 
     try:
         return str(Decimal(value).quantize(Decimal(quantize_str)))
     except InvalidOperation:  # pragma: no cover
         warnings.warn(
-            f"handled quantize error (please report an issue)", RuntimeWarning
+            "handled quantize error (please report an issue)",
+            RuntimeWarning,
+            stacklevel=2,
         )
         return value
 
 
 class ColumnStats:
     """Used in figuring out how to format properties/list items as columns in a table format."""
 
-    def __init__(self, dont_justify: bool):
+    def __init__(self: ColumnStats, dont_justify: bool) -> None:
+        """Create a new column stats object."""
         debug("ColumnStats()")
         self.dont_justify = dont_justify
         self.prop_name = ""
         self.prop_name_length = 0
         self.order_sum = 0
         self.count = 0
         self.max_value_size = 0
         self.kind = JsonValueKind.NULL
         self.chars_before_dec = 0
         self.chars_after_dec = 0
 
-    def update(self, prop_node: FormattedNode, index: int):
+    def update(self: ColumnStats, prop_node: FormattedNode, index: int) -> None:
         """Add stats about this FormattedNode to this PropertyStats."""
         self.order_sum += index
         self.count += 1
         debug("update()")
         debug(f"  value={prop_node.value}¶")
         debug(f"  max_value_size={self.max_value_size}")
         debug(f"  value_length={prop_node.value_length}")
         self.max_value_size = max([self.max_value_size, prop_node.value_length])
         if self.kind == JsonValueKind.NULL:
             self.kind = prop_node.kind
-        elif self.kind == JsonValueKind.FLOAT and prop_node.kind == JsonValueKind.INT:
-            self.kind = JsonValueKind.FLOAT
-        elif self.kind == JsonValueKind.INT and prop_node.kind == JsonValueKind.FLOAT:
+        elif (
+            self.kind == JsonValueKind.FLOAT
+            and prop_node.kind == JsonValueKind.INT
+            or self.kind == JsonValueKind.INT
+            and prop_node.kind == JsonValueKind.FLOAT
+        ):
             self.kind = JsonValueKind.FLOAT
         elif self.kind != prop_node.kind:
             self.kind = JsonValueKind.UNDEFINED
 
         if prop_node.kind == JsonValueKind.FLOAT:
             if "." in prop_node.value:
                 (whole, frac) = prop_node.value.split(".")
@@ -125,41 +142,43 @@
             debug(f"  chars_after_dec={self.chars_after_dec}")
             debug(f"  chars_before_dec={self.chars_before_dec}")
         elif prop_node.kind == JsonValueKind.INT:
             self.chars_before_dec = max([self.chars_before_dec, len(prop_node.value)])
             debug(f"  chars_before_dec={self.chars_before_dec}")
 
     @property
-    def max_value_size(self):
+    def max_value_size(self: ColumnStats) -> int:
+        """Return max size of a node."""
         if self.dont_justify:
             return self._max_value_size
-        elif self.kind == JsonValueKind.FLOAT:
+        if self.kind == JsonValueKind.FLOAT:
             return self.chars_before_dec + self.chars_after_dec + 1
-        elif self.kind == JsonValueKind.INT:
+        if self.kind == JsonValueKind.INT:
             return self.chars_before_dec
-        else:
-            return self._max_value_size
+        return self._max_value_size
 
     @max_value_size.setter
-    def max_value_size(self, v):
+    def max_value_size(self: ColumnStats, v: int) -> None:
+        """Set max size of a node."""
         self._max_value_size = v
 
-    def format_value(self, value: str, value_length: int) -> str:
+    def format_value(self: ColumnStats, value: str, value_length: int) -> str:
+        """Format a value based on its column position."""
         debug("format_value()")
         debug(f"  value={value}¶")
         debug(f"  value_length={value_length}")
         debug(
             "  is_numeric="
             + str(
-                self.kind == JsonValueKind.FLOAT or self.kind == JsonValueKind.INT
-            ).lower()
+                self.kind in (JsonValueKind.FLOAT, JsonValueKind.INT),
+            ).lower(),
         )
 
         if (
-            self.kind == JsonValueKind.FLOAT or self.kind == JsonValueKind.INT
+            self.kind in (JsonValueKind.FLOAT, JsonValueKind.INT)
         ) and not self.dont_justify:
             adjusted_val = _fixed_value(value, self.chars_after_dec)
             total_length = self.chars_before_dec + self.chars_after_dec
             total_length += 1 if self.chars_after_dec > 0 else 0
             debug(f"  adjusted_val={adjusted_val}")
             debug(f"  chars_before_dec={self.chars_before_dec}")
             debug(f"  chars_after_dec={self.chars_after_dec}")
@@ -168,24 +187,24 @@
             return adjusted_val.rjust(total_length)
 
         debug(f"  max_value_size={self.max_value_size}")
         debug(f"  len(value)={len(value)}")
         debug(
             "  value="
             + value.ljust(self.max_value_size - (value_length - len(value)))
-            + "¶"
+            + "¶",
         )
         return value.ljust(self.max_value_size - (value_length - len(value)))
 
 
 @dataclass
 class Formatter:
-    """
-    Class that outputs JSON formatted in a compact, user-readable way. Any given container
-    is formatted in one of three ways:
+    """Class that outputs JSON formatted in a compact, user-readable way.
+
+    Any given container is formatted in one of three ways:
     * Arrays or dicts will be written on a single line, if their contents aren't too
       complex and the resulting line wouldn't be too long.
     * Arrays can be written on multiple lines, with multiple items per line, as long as
       those items aren't too complex.
     * Otherwise, each dict property or list item is written beginning on its own line,
       indented one step deeper than its parent.
 
@@ -261,14 +280,17 @@
 
     east_asian_string_widths
         If True (default is False), format strings using unicodedata.east_asian_width rather
         than simple string lengths
 
     multiline_compact_dict
         If True (default is False), format dict into multi-line compact style like list
+
+    omit_trailing_whitespace
+        If True, strip whitespace at the end of all output lines.
     """
 
     json_eol_style: EolStyle = EolStyle.LF
     max_inline_length: int = 80
     max_inline_complexity: int = 2
     max_compact_list_complexity: int = 1
     nested_bracket_padding: bool = True
@@ -282,74 +304,84 @@
     table_list_minimum_similarity: int = 75
     align_expanded_property_names: bool = False
     dont_justify_numbers: bool = False
     prefix_string: bool = ""
     ensure_ascii: bool = True
     east_asian_string_widths: bool = False
     multiline_compact_dict: bool = False
+    omit_trailing_whitespace: bool = False
 
-    def __post_init__(self):
+    def __post_init__(self: Formatter) -> None:
+        """Init none-datatype fields."""
         self.eol_str = ""
         self.indent_str = ""
         self.padded_comma_str = ""
         self.padded_colon_str = ""
         self.indent_cache = {}
 
-    def str_len(self, s: str) -> int:
+    def str_len(self: Formatter, s: str) -> int:
+        """Return string length supporting east-Asian characters."""
         if not self.east_asian_string_widths or s.isascii():
             return len(s)
         return _wcswidth(s)
 
     def dump(
-        self,
-        obj: Any,
-        output_file: Union[str, PosixPath],
-        newline_at_eof: bool = True,
+        self: Formatter,
+        obj: Any,  # noqa: ANN401
+        output_file: str | PosixPath,
+        newline_at_eof: bool = True,  # noqa: FBT002
     ) -> None:
+        """Write JSON to a file."""
         formatted: str = self.serialize(obj)
         if newline_at_eof:
             formatted += self.eol_str
 
         with open(output_file, "w") as f:
             f.write(formatted)
 
-    def serialize(self, value) -> str:
+    def serialize(self: Formatter, value: str) -> str:
+        """Serialize a value to formatted JSON."""
         self.init_internals()
-        return self.prefix_string + self.format_element(0, value).value
+        value = self.prefix_string + self.format_element(0, value).value
+        if self.omit_trailing_whitespace:
+            value = re.sub(r"\s+$", "", value, flags=re.MULTILINE)
+        return value
 
-    def init_internals(self):
+    def init_internals(self: Formatter) -> None:
         """Set up some intermediate fields for efficiency."""
         self.eol_str = "\r\n" if self.json_eol_style == EolStyle.CRLF else "\n"
         self.indent_str = "\t" if self.use_tab_to_indent else " " * self.indent_spaces
         self.padded_comma_str = ", " if self.comma_padding else ","
         self.padded_colon_str = ": " if self.colon_padding else ":"
 
-    def indent(self, buffer: List[str], depth: int) -> List[str]:
+    def indent(self: Formatter, buffer: list[str], depth: int) -> list[str]:
+        """Indent a list of strings."""
         if depth not in self.indent_cache:
             self.indent_cache[depth] = self.indent_str * depth
         buffer += [self.prefix_string, self.indent_cache[depth]]
         return buffer
 
-    def combine(self, buffer: List[str]) -> str:
+    def combine(self: Formatter, buffer: list[str]) -> str:
+        """Combine a list of strings to a single string."""
         return "".join(buffer)
 
-    def format_element(self, depth: int, element) -> FormattedNode:
-        """Base of recursion. Nearly everything comes through here."""
+    def format_element(self: Formatter, depth: int, element: object) -> FormattedNode:
+        """Root formmatting function for recursion."""
         if isinstance(element, list):
             formatted_item = self.format_list(depth, element)
         elif isinstance(element, dict):
             formatted_item = self.format_dict(depth, element)
         else:
             formatted_item = self.format_simple(depth, element)
 
         formatted_item.cleanup()
         return formatted_item
 
-    def format_simple(self, depth: int, element) -> FormattedNode:
-        """Formats a JSON element other than an list or dict."""
+    def format_simple(self: Formatter, depth: int, element: object) -> FormattedNode:
+        """Format a JSON element other than an list or dict."""
         simple_node = FormattedNode()
         simple_node.value = json.dumps(element, ensure_ascii=self.ensure_ascii)
         simple_node.value_length = self.str_len(simple_node.value)
         simple_node.complexity = 0
         simple_node.depth = depth
 
         if element is None:
@@ -363,17 +395,17 @@
         elif isinstance(element, float):
             simple_node.kind = JsonValueKind.FLOAT
         else:
             simple_node.kind = JsonValueKind.STRING
 
         return simple_node
 
-    def format_list(self, depth: int, element) -> FormattedNode:
-        # Recursively format all of this list's elements.
-        items = list(map(lambda child: self.format_element(depth + 1, child), element))
+    def format_list(self: Formatter, depth: int, element: list) -> FormattedNode:
+        """Recursively format all of this list's elements."""
+        items = [self.format_element(depth + 1, child) for child in element]
         if len(items) == 0:
             return self.empty_list(depth)
 
         item = FormattedNode()
         item.kind = JsonValueKind.LIST
         item.complexity = max([fn.complexity for fn in items]) + 1
         item.depth = depth
@@ -392,29 +424,37 @@
 
         if self.format_list_multiline_compact(item):
             return item
 
         self.format_list_expanded(item)
         return item
 
-    def format_dict(self, depth: int, element: dict) -> FormattedNode:
-        # Recursively format all of this dict's property values.
+    def format_dict(self: Formatter, depth: int, element: dict) -> FormattedNode:
+        """Recursively format all of this dict's property values."""
         items = []
         keys = {}
         for k, v in element.items():
             elem = self.format_element(depth + 1, v)
             if isinstance(k, Enum):
-                k = k.value
+                k = k.value  # noqa: PLW2901
             if not isinstance(k, str):
-                warnings.warn(f"converting key value {k} to string", RuntimeWarning)
-            k = str(k)
+                warnings.warn(
+                    f"converting key value {k} to string",
+                    RuntimeWarning,
+                    stacklevel=2,
+                )
+            k = str(k)  # noqa: PLW2901
             elem.name = json.dumps(k, ensure_ascii=self.ensure_ascii)
             elem.name_length = self.str_len(elem.name)
             if k in keys:
-                warnings.warn(f"duplicate key value {k}", RuntimeWarning)
+                warnings.warn(
+                    f"duplicate key value {k}",
+                    RuntimeWarning,
+                    stacklevel=2,
+                )
                 items[keys[k]] = elem
             else:
                 keys[k] = len(items)
                 items.append(elem)
 
         if len(items) == 0:
             return self.empty_dict(depth)
@@ -436,37 +476,38 @@
 
         if self.format_dict_multiline_compact(item):
             return item
 
         self.format_dict_expanded(item, False)
         return item
 
-    def empty_list(self, depth: int) -> FormattedNode:
+    def empty_list(self: Formatter, depth: int) -> FormattedNode:
+        """Create an empty list node."""
         arr = FormattedNode()
         arr.value = "[]"
         debug("empty_list: value_length = 2")
         arr.value_length = 2
         arr.complexity = 0
         arr.depth = depth
         arr.kind = JsonValueKind.LIST
         arr.format = Format.INLINE
         return arr
 
-    def format_list_inline(self, item: FormattedNode) -> bool:
+    def format_list_inline(self: Formatter, item: FormattedNode) -> bool:
         """Try to format this list in a single line, if possible."""
         if (
             item.depth <= self.always_expand_depth
             or item.complexity > self.max_inline_complexity
         ):
             return False
 
-        if any([fn.format != Format.INLINE for fn in item.children]):
+        if any(fn.format != Format.INLINE for fn in item.children):
             return False
 
-        if item.complexity >= 2:
+        if item.complexity >= 2:  # noqa: PLR2004
             use_bracket_padding = self.nested_bracket_padding
         else:
             use_bracket_padding = self.simple_bracket_padding
         line_length = 2 + (2 if use_bracket_padding else 0)
         line_length += (len(item.children) - 1) * len(self.padded_comma_str)
         line_length += sum([fn.value_length for fn in item.children])
 
@@ -491,17 +532,19 @@
 
         item.value = self.combine(buffer)
         debug(f"format_list_inline: value_length = {line_length}")
         item.value_length = line_length
         item.format = Format.INLINE
         return True
 
-    def format_list_multiline_compact(self, item: FormattedNode) -> bool:
-        """Try to format this list, spanning multiple lines, but with several items
-        per line, if possible."""
+    def format_list_multiline_compact(self: Formatter, item: FormattedNode) -> bool:
+        """Try to format this list.
+
+        Span multiple lines, but with several items per line, if possible.
+        """
         debug("format_list_multiline_compact()")
         if (
             item.depth <= self.always_expand_depth
             or item.complexity > self.max_compact_list_complexity
         ):
             return False
 
@@ -556,18 +599,20 @@
         self.indent(buffer, item.depth)
         buffer += "]"
 
         item.value = self.combine(buffer)
         item.format = Format.MULTILINE_COMPACT
         return True
 
-    def format_table_list_dict(self, item: FormattedNode) -> bool:
-        """Format this list with one child dict per line, and those dicts
-        padded to line up nicely."""
-        if self.table_dict_minimum_similarity > 100.5:
+    def format_table_list_dict(self: Formatter, item: FormattedNode) -> bool:
+        """Format this list with one child dict per line.
+
+        Those dicts are padded to line up nicely.
+        """
+        if self.table_dict_minimum_similarity > 100.5:  # noqa: PLR2004
             return False
 
         # Gather stats about our children's property order and width, if they're eligible dicts.
         col_stats = self.get_property_stats(item)
         if not col_stats:
             return False
 
@@ -582,20 +627,20 @@
         # children aren't recomputed, so this part isn't recursive.
         for child in item.children:
             self.format_dict_table_row(child, col_stats)
             child.value_length = value_length
 
         if self.format_list_multiline_compact(item):
             return item
-        else:
-            return self.format_list_expanded(item)
+        return self.format_list_expanded(item)
 
-    def format_table_list_list(self, item: FormattedNode) -> bool:
+    def format_table_list_list(self: Formatter, item: FormattedNode) -> bool:
+        """Format a list of lists."""
         debug("format_table_list_list()")
-        if self.table_list_minimum_similarity > 100:
+        if self.table_list_minimum_similarity > 100:  # noqa: PLR2004
             return False
 
         # Gather stats about our children's item widths, if they're eligible lists.
         column_stats = self.get_list_stats(item)
         if not column_stats:
             return False
 
@@ -609,20 +654,21 @@
         # children aren't recomputed, so this part isn't recursive.
         for child in item.children:
             self.format_list_table_row(child, column_stats)
             child.value_length = value_length
 
         if self.format_list_multiline_compact(item):
             return item
-        else:
-            return self.format_list_expanded(item)
+        return self.format_list_expanded(item)
 
     def format_list_table_row(
-        self, item: FormattedNode, column_stats_list: List[ColumnStats]
-    ):
+        self: Formatter,
+        item: FormattedNode,
+        column_stats_list: list[ColumnStats],
+    ) -> None:
         """Format this list in a single line, with padding to line up with siblings."""
         buffer = ["[ "]
 
         debug("format_list_table_row()")
         # Write the elements that actually exist in this list.
         for index, child in enumerate(item.children):
             if index:
@@ -649,17 +695,19 @@
             sum([col.max_value_size for col in column_stats_list])
             + len(self.padded_comma_str) * (len(column_stats_list) - 1)
             + 4
         )
         debug(f"  value={item.value}¶")
         item.format = Format.INLINE_TABULAR
 
-    def format_list_expanded(self, item: FormattedNode) -> bool:
+    def format_list_expanded(self: Formatter, item: FormattedNode) -> bool:
         """Write this list with each element starting on its own line.
-        They might be multiple lines themselves"""
+
+        They might be multiple lines themselves
+        """
         buffer = ["[", self.eol_str]
         first_elem = True
         for child in item.children:
             if not first_elem:
                 buffer += [self.padded_comma_str, self.eol_str]
             self.indent(buffer, child.depth).append(child.value)
             first_elem = False
@@ -667,38 +715,39 @@
         buffer += self.eol_str
         self.indent(buffer, item.depth).append("]")
 
         item.value = self.combine(buffer)
         item.format = Format.EXPANDED
         return True
 
-    def empty_dict(self, depth: int):
+    def empty_dict(self: Formatter, depth: int) -> None:
+        """Create an empty dict node."""
         obj = FormattedNode()
         obj.value = "{}"
         obj.value_length = 2
         obj.complexity = 0
         obj.depth = depth
         obj.kind = JsonValueKind.DICT
         obj.format = Format.INLINE
         return obj
 
-    def format_dict_inline(self, item: FormattedNode) -> bool:
+    def format_dict_inline(self: Formatter, item: FormattedNode) -> bool:
         """Format this dict as a single line, if possible."""
         if (
             item.depth <= self.always_expand_depth
             or item.complexity > self.max_inline_complexity
         ):
             return False
 
-        if any([fn.format != Format.INLINE for fn in item.children]):
+        if any(fn.format != Format.INLINE for fn in item.children):
             return False
 
         use_bracket_padding = (
             self.nested_bracket_padding
-            if item.complexity >= 2
+            if item.complexity >= 2  # noqa: PLR2004
             else self.simple_bracket_padding
         )
 
         line_length = 2 + (2 if use_bracket_padding else 0)
         line_length += len(item.children) * len(self.padded_colon_str)
         line_length += (len(item.children) - 1) * len(self.padded_comma_str)
         line_length += sum([fn.name_length for fn in item.children])
@@ -724,19 +773,23 @@
 
         item.value = self.combine(buffer)
         debug(f"format_dict_inline: value_length = {line_length}")
         item.value_length = line_length
         item.format = Format.INLINE
         return True
 
-    def format_dict_multiline_compact(
-        self, item: FormattedNode, force_expand_prop_names: bool = False
+    def format_dict_multiline_compact(  # noqa: C901
+        self: Formatter,
+        item: FormattedNode,
+        force_expand_prop_names: bool = False,  # noqa: FBT002
     ) -> bool:
-        """Try to format this dict, spanning multiple lines, but with several items
-        per line, if possible."""
+        """Try to format this dict spanning multiple lines.
+
+        This may have several items per line, if possible.
+        """
         debug("format_dict_multiline_compact()")
         if (
             not self.multiline_compact_dict
             or item.depth <= self.always_expand_depth
             or item.complexity > self.max_compact_list_complexity
         ):
             return False
@@ -806,18 +859,20 @@
         self.indent(buffer, item.depth)
         buffer += "}"
 
         item.value = self.combine(buffer)
         item.format = Format.MULTILINE_COMPACT
         return True
 
-    def format_table_dict_dict(self, item: FormattedNode) -> bool:
-        """Format this dict with one child dict per line, and those dicts
-        padded to line up nicely."""
-        if self.table_dict_minimum_similarity > 100:
+    def format_table_dict_dict(self: Formatter, item: FormattedNode) -> bool:
+        """Format this dict with one child dict per line.
+
+        Those dicts are padded to line up nicely.
+        """
+        if self.table_dict_minimum_similarity > 100:  # noqa: PLR2004
             return False
 
         # Gather stats about our children's property order and width, if they're eligible dicts.
         prop_stats = self.get_property_stats(item)
         if not prop_stats:
             return False
 
@@ -832,22 +887,23 @@
         # children aren't recomputed, so this part isn't recursive.
         for child in item.children:
             self.format_dict_table_row(child, prop_stats)
             child.value_length = value_length
 
         if self.format_dict_multiline_compact(item, True):
             return item
-        else:
-            return self.format_dict_expanded(item, True)
+        return self.format_dict_expanded(item, True)
 
-    def format_table_dict_list(self, item: FormattedNode) -> bool:
-        """Format this dict with one child list per line, and those lists padded to
-        line up nicely."""
+    def format_table_dict_list(self: Formatter, item: FormattedNode) -> bool:
+        """Format this dict with one child list per line.
+
+        Those lists are padded to line up nicely.
+        """
         debug("format_table_dict_list()")
-        if self.table_list_minimum_similarity > 100:
+        if self.table_list_minimum_similarity > 100:  # noqa: PLR2004
             return False
 
         # Gather stats about our children's widths, if they're eligible lists.
         column_stats = self.get_list_stats(item)
         if not column_stats:
             return False
 
@@ -861,28 +917,29 @@
         # Their children aren't recomputed, so this part isn't recursive.
         for child in item.children:
             self.format_list_table_row(child, column_stats)
             child.value_length = value_length
 
         if self.format_dict_multiline_compact(item, True):
             return item
-        else:
-            return self.format_dict_expanded(item, True)
+        return self.format_dict_expanded(item, True)
 
     def format_dict_table_row(
-        self, item: FormattedNode, column_stats_list: List[ColumnStats]
-    ):
+        self: Formatter,
+        item: FormattedNode,
+        column_stats_list: list[ColumnStats],
+    ) -> None:
         """Format this dict in a single line, with padding to line up with siblings."""
         # Bundle up each property name, value, quotes, colons, etc., or equivalent empty space.
         highest_non_blank_index = -1
         prop_segment_strings = []
         for col_index, column_stats in enumerate(column_stats_list):
             buffer = []
             filtered_prop_nodes = list(
-                filter(lambda fn: fn.name == column_stats.prop_name, item.children)
+                filter(lambda fn: fn.name == column_stats.prop_name, item.children),
             )
             if len(filtered_prop_nodes) == 0:
                 # This dict doesn't have this particular property. Pad it out.
                 skip_length = (
                     column_stats.prop_name_length
                     + len(self.padded_colon_str)
                     + column_stats.max_value_size
@@ -916,18 +973,22 @@
 
         buffer += " }"
 
         item.value = self.combine(buffer)
         item.format = Format.INLINE_TABULAR
 
     def format_dict_expanded(
-        self, item: FormattedNode, force_expand_prop_names: bool
+        self: Formatter,
+        item: FormattedNode,
+        force_expand_prop_names: bool,
     ) -> bool:
         """Write this dict with each element starting on its own line.
-        They might be multiple lines"""
+
+        They might be multiple lines.
+        """
         max_prop_name_length = max([fn.name_length for fn in item.children])
 
         buffer = ["{", self.eol_str]
         first_item = True
         for prop in item.children:
             if not first_item:
                 buffer += [self.padded_comma_str, self.eol_str]
@@ -942,44 +1003,49 @@
         buffer += self.eol_str
         self.indent(buffer, item.depth).append("}")
 
         item.value = self.combine(buffer)
         item.format = Format.EXPANDED
         return True
 
-    def justify_parallel_numbers(self, item_list: List[FormattedNode]):
-        """If the given nodes are all numbers and not too big or small, format them
-        to the same precision and width."""
-        if len(item_list) < 2 or self.dont_justify_numbers:
+    def justify_parallel_numbers(
+        self: Formatter,
+        item_list: list[FormattedNode],
+    ) -> None:
+        """If the given nodes are all numbers and not too big or small.
+
+        Format them to the same precision and width.
+        """
+        if len(item_list) < 2 or self.dont_justify_numbers:  # noqa: PLR2004
             return
 
         column_stats = ColumnStats(self.dont_justify_numbers)
         for prop_node in item_list:
             column_stats.update(prop_node, 0)
 
-        if (
-            column_stats.kind != JsonValueKind.INT
-            and column_stats.kind != JsonValueKind.FLOAT
-        ):
+        if column_stats.kind not in (JsonValueKind.INT, JsonValueKind.FLOAT):
             return
 
         for prop_node in item_list:
             prop_node.value = column_stats.format_value(
-                prop_node.value, prop_node.value_length
+                prop_node.value,
+                prop_node.value_length,
             )
             debug(
-                f"justify_parallel_numbers: value_length = {column_stats.max_value_size}"
+                f"justify_parallel_numbers: value_length = {column_stats.max_value_size}",
             )
             prop_node.value_length = column_stats.max_value_size
 
-    def get_property_stats(self, item: FormattedNode) -> List[ColumnStats]:
-        """Check if this node's dict children can be formatted as a table, and
-        if so, return stats about their properties, such as max width.
-        Returns None if they're not eligible."""
-        if len(item.children) < 2:
+    def get_property_stats(self: Formatter, item: FormattedNode) -> list[ColumnStats]:
+        """Check if this node's dict children can be formatted as a table.
+
+        If so, return stats about their properties, such as max width.
+        Returns None if they're not eligible.
+        """
+        if len(item.children) < 2:  # noqa: PLR2004
             return None
 
         # Record every property across all dicts, count them, tabulate their
         # order, and find the longest.
         props = {}
         for child in item.children:
             if child.kind != JsonValueKind.DICT or child.format != Format.INLINE:
@@ -1023,26 +1089,26 @@
         # Commas
         line_length += len(self.padded_comma_str) * (len(ordered_props) - 1)
         if line_length > self.max_inline_length:
             return None
 
         return ordered_props
 
-    def get_list_stats(self, item: FormattedNode) -> List[ColumnStats]:
-        """Check if this node's list children can be formatted as a table, and if
-        so, gather stats like max width.
-        Returns None if they're not eligible."""
-        if len(item.children) < 2:
+    def get_list_stats(self: Formatter, item: FormattedNode) -> list[ColumnStats]:
+        """Check if this node's list children can be formatted as a table.
+
+        If so, gather stats like max width.
+        Returns None if they're not eligible.
+        """
+        if len(item.children) < 2:  # noqa: PLR2004
             return None
 
         valid = all(
-            [
-                fn.kind == JsonValueKind.LIST and fn.format == Format.INLINE
-                for fn in item.children
-            ]
+            fn.kind == JsonValueKind.LIST and fn.format == Format.INLINE
+            for fn in item.children
         )
         if not valid:
             return None
 
         number_of_columns = max([len(fn.children) for fn in item.children])
         col_stats_list = [
             ColumnStats(self.dont_justify_numbers) for x in range(number_of_columns)
```

### Comparing `compact_json-1.6.1/PKG-INFO` & `compact_json-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: compact-json
-Version: 1.6.1
+Version: 1.8.0
 Summary: A JSON formatter that produces compact but human-readable
 Home-page: https://github.com/masaccio/compact-json
 License: MIT
 Author: Jon Connell
 Author-email: python@figsandfudge.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: wcwidth (>=0.2.5,<0.3.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: importlib-resources (>=6.1)
+Requires-Dist: setuptools (>=69.0.3)
+Requires-Dist: wcwidth (>=0.2.5,<=0.2.8)
 Project-URL: Documentation, https://github.com/masaccio/compact-json/blob/main/README.md
 Project-URL: Repository, https://github.com/masaccio/compact-json
 Description-Content-Type: text/markdown
 
 # compact-json
 
 [![build:](https://github.com/masaccio/compact-json/actions/workflows/run-all-tests.yml/badge.svg)](https://github.com/masaccio/compact-json/actions/workflows/run-all-tests.yml)
@@ -96,14 +97,15 @@
 ```
 
 ## Usage
 
 As a python package, `compact-json` is instantiated with a `Formatter` class that has a range of properties to configure the formatting:
 
 ``` python
+import json
 from compact_json import Formatter, EolStyle
 
 formatter = Formatter()
 formatter.indent_spaces = 2
 formatter.max_inline_complexity = 10
 formatter.json_eol_style = EolStyle.LF
```

