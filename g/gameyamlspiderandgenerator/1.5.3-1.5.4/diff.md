# Comparing `tmp/gameyamlspiderandgenerator-1.5.3.tar.gz` & `tmp/gameyamlspiderandgenerator-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.5.3.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.5.4.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.5.3.tar` & `gameyamlspiderandgenerator-1.5.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.5.3/LICENSE
--rwxr-xr-x   0        0        0     1350 2023-05-20 01:08:55.288767 gameyamlspiderandgenerator-1.5.3/README.md
--rwxr-xr-x   0        0        0      568 2023-05-05 11:54:39.052482 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0     1730 2023-05-20 00:53:28.998905 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      753 2023-05-05 11:54:39.052963 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      235 2023-05-19 14:05:11.849031 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0      901 2023-05-19 15:02:18.997930 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/hook/openai.py
--rwxr-xr-x   0        0        0     3890 2023-05-20 00:56:00.167554 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0      559 2023-05-19 14:05:11.679558 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/hook/validate.py
--rwxr-xr-x   0        0        0       56 2023-05-05 11:54:39.055255 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     3121 2023-05-20 00:57:14.785468 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7096 2023-05-20 00:57:31.872974 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     8006 2023-05-20 00:57:46.796356 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1838 2023-05-20 00:56:00.343108 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     1944 2023-05-05 11:54:39.057708 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2611 2023-05-05 11:54:39.066258 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      265 2023-05-20 00:56:00.262482 gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/util/thread.py
--rwxr-xr-x   0        0        0      719 2023-05-20 01:18:55.728769 gameyamlspiderandgenerator-1.5.3/pyproject.toml
--rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.5.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-05-05 11:54:39.050499 gameyamlspiderandgenerator-1.5.4/LICENSE
+-rwxr-xr-x   0        0        0     1350 2023-05-22 00:40:10.043310 gameyamlspiderandgenerator-1.5.4/README.md
+-rwxr-xr-x   0        0        0      568 2023-05-05 11:54:39.052482 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0     1912 2023-05-22 02:18:45.372264 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      753 2023-05-05 11:54:39.052963 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-05-05 11:54:39.054143 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      235 2023-05-22 00:40:10.045341 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0     1476 2023-05-22 02:04:55.203167 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/hook/openai.py
+-rwxr-xr-x   0        0        0     3890 2023-05-22 00:40:10.056295 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0      559 2023-05-22 00:40:10.056896 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/hook/validate.py
+-rwxr-xr-x   0        0        0       56 2023-05-05 11:54:39.055255 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     3121 2023-05-22 00:40:10.068295 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7008 2023-05-22 02:16:18.462795 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     8006 2023-05-22 00:40:10.090094 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-05-05 11:54:39.056470 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1461 2023-05-05 11:54:39.056789 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1838 2023-05-22 00:40:10.090828 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1953 2023-05-05 14:39:08.995558 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     2138 2023-05-22 02:19:44.858160 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2682 2023-05-22 01:42:34.275139 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      265 2023-05-22 00:40:10.091597 gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/thread.py
+-rwxr-xr-x   0        0        0      719 2023-05-22 02:25:20.115256 gameyamlspiderandgenerator-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0     2478 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.5.4/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.5.3/LICENSE` & `gameyamlspiderandgenerator-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.3/README.md` & `gameyamlspiderandgenerator-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/__init__.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/__main__.py` & `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,37 +7,47 @@
 from .util.plugin_manager import pkg
 import sys
 from loguru import logger
 from gameyamlspiderandgenerator import produce_yaml
 
 parser = argparse.ArgumentParser()
 logger.remove()
-logger.add(sys.stderr, level="ERROR")
+logger.add(sys.stderr, level="INFO")
 parser.add_argument(
     "-f",
     "--config",
     type=str,
     default={"plugin": ["steam", "itchio"], "hook": ["search", "validate"]},
     help="The location of config.yaml (default null)",
 )
 parser.add_argument(
     "-o",
     "--output",
     type=str,
     default=None,
     help="The location of the output file (zip format or yaml format)",
 )
+parser.add_argument(
+    "--fast",
+    action='store_true',
+    default=False,
+    help="Whether to disable all hooks (default: false)",
+)
 parser.add_argument("url", metavar="URL")
 args = parser.parse_args()
 
+
+
 if isinstance(args.config, str):
     with open(args.config) as f:
         setting = safe_load(f)
 else:
     setting = args.config
+if args.fast:
+     setting['hook'] = None
 config.update(setting)
 pkg.__init__()
 yml = produce_yaml(args.url)
 if args.output is None:
     print(yml)
 elif "." not in args.output:
     if args.output == "zip":
```

### Comparing `gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/hook/search.py` & `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/hook/search.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/hook/validate.py` & `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/hook/validate.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,32 +39,28 @@
     def get_thumbnail(self):
         th = self.soup.select_one("#header > img")
         if th is None:
             return None
         return th.attrs["src"]
 
     def get_brief_desc(self):
-        return (
-            pss_dedent(self.data["aggregateRating"]["description"])
-            if "description" in self.data["aggregateRating"]
-            else ""
-        )
+        return self.soup.find("meta", {"name": "twitter:description"}).attrs["content"]
 
     def get_name(self):
         return self.data["name"]
 
     def get_screenshots(self):
         temp = self.soup.select_one("div.columns > div.right_col.column > div.screenshot_list").select('a')
         return [i.attrs['href'] for i in temp]
 
     def get_desc(self):
         return pss_dedent(self.remove_query(html2text(
             str(self.soup.select_one("div.formatted_description.user_formatted")),
             bodywidth=0,
-        )).replace("\n" * 4, "\n").strip())
+        )).replace("\n" * 3, "\n").strip())
 
     def get_platforms(self):
         repl = {
             "Windows": "windows",
             "macOS": "macos",
             "Linux": "linux",
             "Android": "android",
```

### Comparing `gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/config.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/fgi.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,20 @@
 
     def _load(
             self,
             _dir: Literal["plugin", "hook"],
             _type: Union[Type[BasePlugin], Type[BaseHook]],
     ):
         base = __package__.split(".")[0] + "." + _dir
+        if config[_dir] is None:
+            if None not in self["log"]:
+                logger.warning(f"All {_dir}s are disabled")
+                self["log"].append(None)
+            return
+
         for plugin in getattr(config, _dir, []):
             if plugin.startswith("_"):
                 logger.warning(f"Skip loading protected {_dir} {plugin}")
                 continue
             try:
                 package = f"{base}.{plugin}"
                 if plugin in self["log"]:
```

### Comparing `gameyamlspiderandgenerator-1.5.3/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.5.4/gameyamlspiderandgenerator/util/spider.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         将响应内容解析为文本
 
         Proxied for self.response.text
 
         Returns:
             文本
         """
-        return self.response.text
+        return self.response.text.encode(self.response.encoding).decode(self.response.apparent_encoding)
 
     @property
     def status(self) -> int:
         """
         获取响应状态码
 
         Proxied for `self.response.status_code`
```

### Comparing `gameyamlspiderandgenerator-1.5.3/pyproject.toml` & `gameyamlspiderandgenerator-1.5.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.5.3"
+version = "1.5.4"
 description = "A useful tool for generating Furrygameindex yaml files"
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `gameyamlspiderandgenerator-1.5.3/PKG-INFO` & `gameyamlspiderandgenerator-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.5.3
+Version: 1.5.4
 Summary: A useful tool for generating Furrygameindex yaml files
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

