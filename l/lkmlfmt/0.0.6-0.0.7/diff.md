# Comparing `tmp/lkmlfmt-0.0.6.tar.gz` & `tmp/lkmlfmt-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lkmlfmt-0.0.6.tar", max compression
+gzip compressed data, was "lkmlfmt-0.0.7.tar", max compression
```

## Comparing `lkmlfmt-0.0.6.tar` & `lkmlfmt-0.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2647 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/README.md
--rw-r--r--   0        0        0       53 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/__init__.py
--rw-r--r--   0        0        0       70 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/__main__.py
--rw-r--r--   0        0        0     2546 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/command.py
--rw-r--r--   0        0        0      100 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/exception.py
--rw-r--r--   0        0        0    11101 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/formatter.py
--rw-r--r--   0        0        0      757 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/lkml.lark
--rw-r--r--   0        0        0       64 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/logger.py
--rw-r--r--   0        0        0     2292 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/parser.py
--rw-r--r--   0        0        0     4806 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/lkmlfmt/template.py
--rw-r--r--   0        0        0      552 2023-05-19 13:34:29.438876 lkmlfmt-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3091 1970-01-01 00:00:00.000000 lkmlfmt-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     2582 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/README.md
+-rw-r--r--   0        0        0       53 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/__main__.py
+-rw-r--r--   0        0        0     2738 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/command.py
+-rw-r--r--   0        0        0      100 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/exception.py
+-rw-r--r--   0        0        0    11547 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/formatter.py
+-rw-r--r--   0        0        0      757 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/lkml.lark
+-rw-r--r--   0        0        0       64 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/logger.py
+-rw-r--r--   0        0        0     2292 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/parser.py
+-rw-r--r--   0        0        0     4251 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/template.py
+-rw-r--r--   0        0        0      534 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2987 1970-01-01 00:00:00.000000 lkmlfmt-0.0.7/PKG-INFO
```

### Comparing `lkmlfmt-0.0.6/README.md` & `lkmlfmt-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: lkmlfmt
+Version: 0.0.7
+Summary: 
+Author: dr666m1
+Author-email: skndr666m1@gmail.com
+Requires-Python: >=3.11,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: lark (>=1.1.5,<2.0.0)
+Requires-Dist: shandy-sqlfmt (>=0.18.1,<0.19.0)
+Description-Content-Type: text/markdown
+
 # lkmlfmt
 lkmlfmt formats your LookML files including embedded SQL and HTML.
 
 ## Installation
 ```sh
 pip install lkmlfmt
 ```
@@ -19,53 +33,39 @@
 from lkmlfmt import fmt
 
 lkml = fmt("""\
 view: view_name {
   derived_table: {
     sql:
     with cte as (
-      select column_name from tablename
+      select col1, col2 from tablename
       where ts between current_date()-7 and current_date())
-    select column_name from cte
+    select {% if true %} col1 {% elsif %} col2 {% endif %} from cte
     ;;
   }
-  dimension: column_name {
-    html:
-{% if value == "foo" %}
-<img src="https://example.com/foo"/>
-{% else %}
-<img src="https://example.com/bar"/>
-{% endif %} ;;
-  }
 }
 """)
 
 assert lkml == """\
 view: view_name {
   derived_table: {
     sql:
       with
         cte as (
-          select column_name
+          select col1, col2
           from tablename
           where ts between current_date() - 7 and current_date()
         )
-      select column_name
+      select
+        {% if true %} col1
+        {% elsif %} col2
+        {% endif %}
       from cte
     ;;
   }
-  dimension: column_name {
-    html:
-      {% if value == "foo" %}
-        <img src="https://example.com/foo"/>
-      {% else %}
-        <img src="https://example.com/bar"/>
-      {% endif %}
-    ;;
-  }
 }
 """
 ```
 
 ## GitHub Actions
 To check if your LookML files are formatted.
 
@@ -112,11 +112,16 @@
 ```
 
 ## Feedback
 I'm not ready to accept pull requests, but your feedback is always welcome.
 If you find any bugs, please feel free to create an issue.
 
 ## See also
-lkmlfmt depends on these awesome formatter and indenter.
+In default, lkmlfmt formats embedded sql using sqlfmt.
 
 * [sqlfmt](https://github.com/tconbeer/sqlfmt)
-* [djhtml](https://github.com/rtts/djhtml)
+
+You can install plugins to change the format of embeded looker expression, sql or html.
+They are distributed under their own licenses, so please check if they are suitable for your purpose.
+
+* [lkmlfmt-djhtml](https://github.com/kitta65/lkmlfmt-djhtml)
+
```

### Comparing `lkmlfmt-0.0.6/lkmlfmt/command.py` & `lkmlfmt-0.0.7/lkmlfmt/command.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,29 +27,39 @@
 @click.option(
     "--log-level",
     type=click.Choice(
         ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"], case_sensitive=False
     ),
     default="WARNING",
 )
-def run(file: list[Path], check: bool, clickhouse: bool, log_level: str) -> None:
+@click.option(
+    "--plugin",
+    "plugins",
+    type=str,
+    multiple=True,
+    default=[],
+    help="A plugin to fmt looker expression, sql or html.",
+)
+def run(
+    file: list[Path], check: bool, clickhouse: bool, log_level: str, plugins: list[str]
+) -> None:
     """Format LookML file(s).
 
     FILE is the LookML file(s) to format (directory is also OK).
     Files which does not end with `.lkml` will be ignored.
     """
     level = getattr(logging, log_level)
     logging.basicConfig(level=level)
 
     modified: list[bool] = []
 
     for f in filter_lkml(file):
         logger.debug(f"formatting {f}")
         before = f.read_text()
-        after = fmt(before, clickhouse)
+        after = fmt(before, clickhouse, plugins)
 
         if before == after:
             click.echo(f"{f} is skipped")
             modified.append(False)
             continue
 
         click.echo(f"{f} is modified")
```

### Comparing `lkmlfmt-0.0.6/lkmlfmt/formatter.py` & `lkmlfmt-0.0.7/lkmlfmt/formatter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
+import importlib
 import re
 from contextlib import contextmanager
-from typing import Any, Generator
+from typing import Generator
 
-from djhtml.lines import Line as DjHTMLLine  # type: ignore
-from djhtml.modes import DjHTML  # type: ignore
 from lark import ParseTree, Token
 from sqlfmt import api
 from sqlfmt.line import Line
 
 from lkmlfmt import parser, template
 from lkmlfmt.exception import LkmlfmtException
 from lkmlfmt.logger import logger
@@ -18,22 +17,23 @@
 ESCAPED_STRING_SINGLE = re.compile(r'"(?P<inner>(.|\n)*?(?<!\\)(\\\\)*?)"')
 ESCAPED_STRING_TRIPLE = re.compile(r'"""(?P<inner>(.|\n)*?(?<!\\)(\\\\)*?)"""')
 NOT_AND_OR = re.compile(r"(?<!\w)(not|and|or)(?!\w)")
 INDENT_WIDTH = 2
 
 
 class LkmlFormatter:
-    def __init__(self, lkml: str, clickhouse: bool) -> None:
+    def __init__(self, lkml: str, clickhouse: bool, plugins: list[str]) -> None:
         self.lkml = lkml
         self.curr_indent = 0
 
         tree, comments = parser.parse(lkml, set_position=True)
         self.tree = tree
         self.comments = comments
         self.mode = api.Mode(dialect_name="clickhouse" if clickhouse else "polyglot")
+        self.plugins = [importlib.import_module(p) for p in plugins]
 
     # NOTE
     # parents take care of self.curr_indent, but children call fmt_indent()
     # parents take care of separator of the children
     def fmt(
         self,
         tree: ParseTree | Token | list[ParseTree | Token] | None = None,
@@ -81,23 +81,19 @@
     def fmt_code_pair(self, pair: ParseTree) -> str:
         lcomments = self.fmt_leading_comments_of(_token(pair.children[0]))
         key = self.fmt(pair.children[0]).lstrip()
         value = str(pair.children[1])
 
         if key.startswith("html"):
             with self.indent():
-                indent = self.curr_indent
-                f: Any = (
-                    lambda s, w: " " * (w * (s.level + indent) + s.offset) + t
-                    if (t := s.text.strip())
-                    else t
-                )
-                # https://github.com/rtts/djhtml/blob/main/djhtml/lines.py
-                DjHTMLLine.indent = f
-                value = _fmt_html(value)
+                formatted = self._try_plugins(value, "fmt_html")
+                if formatted is not None:
+                    value = formatted
+                else:
+                    value = self._fmt_html(value)
 
             if "\n" not in value:
                 return f"{lcomments}{self.fmt_indent()}{key}: {value.lstrip()} ;;"
 
             return f"""{lcomments}{self.fmt_indent()}{key}:
 {value}
 {self.fmt_indent()};;"""
@@ -105,17 +101,25 @@
         # sql_xxx: ... ;; or expression_xxx: ... ;;
         with self.indent():
             # https://docs.python.org/3/library/functions.html#property
             Line.prefix = property(  # type: ignore
                 lambda s: " " * INDENT_WIDTH * (s.depth[0] + self.curr_indent)
             )
             if key.startswith("sql"):
-                value = self._fmt_sql(value)
+                formatted = self._try_plugins(value, "fmt_sql")
+                if formatted is not None:
+                    value = formatted
+                else:
+                    value = self._fmt_sql(value)
             else:
-                value = self._fmt_expr(value)
+                formatted = self._try_plugins(value, "fmt_expr")
+                if formatted is not None:
+                    value = formatted
+                else:
+                    value = self._fmt_expr(value)
 
         if "\n" not in value:
             return f"{lcomments}{self.fmt_indent()}{key}: {value.lstrip()} ;;"
 
         if not value.startswith(" "):  # fallback if sqlfmt does not support
             value = " " * ((self.curr_indent + 1) * INDENT_WIDTH) + value
 
@@ -274,18 +278,22 @@
                 joined += "\n"
 
             joined += "\n"
             joined += self.fmt(t)
 
         return joined
 
+    def _fmt_html(self, html: str) -> str:
+        html = html.lstrip()
+        return " " * INDENT_WIDTH * self.curr_indent + html
+
     def _fmt_sql(self, liquid: str) -> str:
-        jinja, templates, dummies = template.to_jinja(liquid, "sqlfmt")
+        jinja, templates, dummies = template.to_jinja(liquid)
         jinja = api.format_string(jinja, mode=self.mode).rstrip()
-        liquid = template.to_liquid_sqlfmt(jinja, templates, dummies)
+        liquid = template.to_liquid(jinja, templates, dummies)
         return liquid
 
     # NOTE let's rely on sqlfmt for not only sql but also looker expression!
     def _fmt_expr(self, liquid: str) -> str:
         # convert looker expr into sql
         temp = liquid
         temp = temp.replace("case", "lkmlfmt_case")
@@ -307,24 +315,28 @@
                     uppered = NOT_AND_OR.sub(lambda x: x.group(0).upper(), s)
                     expr += uppered
                 case 1:
                     expr += f'"{s}"'
 
         return expr
 
+    def _try_plugins(self, code: str, func: str) -> str | None:
+        for p in self.plugins:
+            if not hasattr(p, func):
+                continue
+            f = getattr(p, func)
+            s = f(code, self.curr_indent)
+            if not isinstance(s, str):
+                raise LkmlfmtException()
+            return s
+        return None
+
 
 def _token(token: Token | ParseTree) -> Token:
     if isinstance(token, Token):
         return token
     raise LkmlfmtException()
 
 
-def _fmt_html(liquid: str) -> str:
-    jinja, templates, dummies = template.to_jinja(liquid, "djhtml")
-    jinja = DjHTML(jinja).indent(2)
-    liquid = template.to_liquid_djhtml(jinja, templates, dummies)
-    return liquid
-
-
-def fmt(lkml: str, clickhouse: bool) -> str:
-    formatter = LkmlFormatter(lkml, clickhouse)
+def fmt(lkml: str, clickhouse: bool = False, plugins: list[str] = []) -> str:
+    formatter = LkmlFormatter(lkml, clickhouse, plugins)
     return formatter.fmt()
```

### Comparing `lkmlfmt-0.0.6/lkmlfmt/lkml.lark` & `lkmlfmt-0.0.7/lkmlfmt/lkml.lark`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.6/lkmlfmt/parser.py` & `lkmlfmt-0.0.7/lkmlfmt/parser.py`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.6/lkmlfmt/template.py` & `lkmlfmt-0.0.7/lkmlfmt/template.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 import re
-from typing import Literal
 
 LIQUID_MARKER = "{{% set LKMLFMT_MARKER = {} %}}"
 TEMPLATE = re.compile(
     r"""(?P<tag>\{%-?\s*(?P<type>#|([a-z]*))([^"'}]*|'[^']*?'|"[^"]*?")*?-?%\})"""
     + r"""|(?P<obj>\{\{([^"'}]*|'[^']*?'|"[^"]*?")*?\}\})"""
     + r"""|(?P<looker>(\$|@)\{[^}]*?\})""",
 )
 DUMMY = re.compile(r"^(?P<lead_n> *?\n)?(?P<indent> *)")
 
-MODE = Literal["sqlfmt", "djhtml"]
 
-
-def to_jinja(liquid: str, mode: MODE = "sqlfmt") -> tuple[str, list[str], list[str]]:
+def to_jinja(liquid: str) -> tuple[str, list[str], list[str]]:
     jinja = ""
     templates = []
     dummies = []
     id_ = 0
     skip_to: str | None = None
 
     while True:
@@ -101,48 +98,32 @@
                 dummy = "{{ var }}"
             # default
             case _:
                 dummy = f"{{% {type_} %}}"
 
         # append results
         marker = LIQUID_MARKER.format(id_)
-        if mode == "sqlfmt":
-            jinja += f"{liquid[: match.start()]}{marker}{dummy}"
-        else:
-            jinja += f"{liquid[: match.start()]}{dummy}{marker}"
+        jinja += f"{liquid[: match.start()]}{marker}{dummy}"
 
         templates.append(match.group(0))
         dummies.append(dummy)
 
         # prepare for next iteration
         liquid = liquid[match.end() :]
         id_ += 1
 
     return jinja, templates, dummies
 
 
-def to_liquid_sqlfmt(jinja: str, templates: list[str], dummies: list[str]) -> str:
+def to_liquid(jinja: str, templates: list[str], dummies: list[str]) -> str:
     for i in range(len(templates)):
         leading, trailing, *_ = jinja.split(LIQUID_MARKER.format(i))
         space, *_ = trailing.split(dummies[i])
         if "\n" in space:
             leading = leading.rstrip("\n ")
         else:
             trailing = trailing.lstrip(" ")
 
         trailing = trailing.replace(dummies[i], templates[i], 1)
         jinja = leading + trailing
 
     return jinja
-
-
-def to_liquid_djhtml(jinja: str, templates: list[str], dummies: list[str]) -> str:
-    liquid = ""
-    trailing = ""
-
-    for i in range(len(templates)):
-        leading, trailing, *_ = jinja.split(f"{dummies[i]}{LIQUID_MARKER.format(i)}")
-        liquid += leading + templates[i]
-        jinja = trailing
-
-    liquid += trailing
-    return liquid
```

### Comparing `lkmlfmt-0.0.6/pyproject.toml` & `lkmlfmt-0.0.7/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "lkmlfmt"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["dr666m1 <skndr666m1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 lkmlfmt = "lkmlfmt.command:run"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 lark = "^1.1.5"
 click = "^8.1.3"
-djhtml = "^3.0.6"
 shandy-sqlfmt = "^0.18.1"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.1"
```

