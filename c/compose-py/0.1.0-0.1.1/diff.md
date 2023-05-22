# Comparing `tmp/compose-py-0.1.0.tar.gz` & `tmp/compose-py-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compose-py-0.1.0.tar", last modified: Mon May 22 02:24:02 2023, max compression
+gzip compressed data, was "compose-py-0.1.1.tar", last modified: Mon May 22 04:21:30 2023, max compression
```

## Comparing `compose-py-0.1.0.tar` & `compose-py-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,27 @@
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 02:24:02.363970 compose-py-0.1.0/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1070 2023-05-22 02:20:34.000000 compose-py-0.1.0/LICENSE
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     3605 2023-05-22 02:24:02.363970 compose-py-0.1.0/PKG-INFO
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1760 2023-05-22 02:23:26.000000 compose-py-0.1.0/README.md
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 02:24:02.363970 compose-py-0.1.0/compose_py/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      140 2023-05-22 02:20:34.000000 compose-py-0.1.0/compose_py/__init__.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       22 2023-05-22 02:20:34.000000 compose-py-0.1.0/compose_py/_version.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      975 2023-05-22 02:20:34.000000 compose-py-0.1.0/compose_py/_yaml.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     2684 2023-05-22 02:20:34.000000 compose-py-0.1.0/compose_py/dumper.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1882 2023-05-22 02:20:34.000000 compose-py-0.1.0/compose_py/loader.py
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       99 2023-05-22 02:20:34.000000 compose-py-0.1.0/compose_py/model_type.py
-drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 02:24:02.363970 compose-py-0.1.0/compose_py.egg-info/
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     3605 2023-05-22 02:24:02.000000 compose-py-0.1.0/compose_py.egg-info/PKG-INFO
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      334 2023-05-22 02:24:02.000000 compose-py-0.1.0/compose_py.egg-info/SOURCES.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        1 2023-05-22 02:24:02.000000 compose-py-0.1.0/compose_py.egg-info/dependency_links.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      205 2023-05-22 02:24:02.000000 compose-py-0.1.0/compose_py.egg-info/requires.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       11 2023-05-22 02:24:02.000000 compose-py-0.1.0/compose_py.egg-info/top_level.txt
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1078 2023-05-22 02:20:34.000000 compose-py-0.1.0/pyproject.toml
--rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       38 2023-05-22 02:24:02.363970 compose-py-0.1.0/setup.cfg
+drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 04:21:30.623184 compose-py-0.1.1/
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1070 2023-05-22 02:20:34.000000 compose-py-0.1.1/LICENSE
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     3605 2023-05-22 04:21:30.623184 compose-py-0.1.1/PKG-INFO
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1760 2023-05-22 02:23:26.000000 compose-py-0.1.1/README.md
+drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 04:21:30.623184 compose-py-0.1.1/compose_py/
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      140 2023-05-22 02:20:34.000000 compose-py-0.1.1/compose_py/__init__.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       79 2023-05-22 03:42:37.000000 compose-py-0.1.1/compose_py/_types.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       22 2023-05-22 04:21:23.000000 compose-py-0.1.1/compose_py/_version.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      970 2023-05-22 02:37:15.000000 compose-py-0.1.1/compose_py/_yaml.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     2671 2023-05-22 02:36:51.000000 compose-py-0.1.1/compose_py/dumper.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1869 2023-05-22 02:36:53.000000 compose-py-0.1.1/compose_py/loader.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       99 2023-05-22 02:20:34.000000 compose-py-0.1.1/compose_py/model_type.py
+drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 04:21:30.623184 compose-py-0.1.1/compose_py/models_dataclasses/
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1054 2023-05-22 02:20:34.000000 compose-py-0.1.1/compose_py/models_dataclasses/__init__.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)    12265 2023-05-22 04:17:18.000000 compose-py-0.1.1/compose_py/models_dataclasses/_generated.py
+drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 04:21:30.623184 compose-py-0.1.1/compose_py/models_pydantic/
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      972 2023-05-22 02:20:34.000000 compose-py-0.1.1/compose_py/models_pydantic/__init__.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)    15492 2023-05-22 04:17:18.000000 compose-py-0.1.1/compose_py/models_pydantic/_generated.py
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 02:20:34.000000 compose-py-0.1.1/compose_py/py.typed
+drwxrwxr-x   0 igarashi  (1002) igarashi  (1002)        0 2023-05-22 04:21:30.623184 compose-py-0.1.1/compose_py.egg-info/
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     3605 2023-05-22 04:21:30.000000 compose-py-0.1.1/compose_py.egg-info/PKG-INFO
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      541 2023-05-22 04:21:30.000000 compose-py-0.1.1/compose_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)        1 2023-05-22 04:21:30.000000 compose-py-0.1.1/compose_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)      205 2023-05-22 04:21:30.000000 compose-py-0.1.1/compose_py.egg-info/requires.txt
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       11 2023-05-22 04:21:30.000000 compose-py-0.1.1/compose_py.egg-info/top_level.txt
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)     1174 2023-05-22 04:19:03.000000 compose-py-0.1.1/pyproject.toml
+-rw-rw-r--   0 igarashi  (1002) igarashi  (1002)       38 2023-05-22 04:21:30.623184 compose-py-0.1.1/setup.cfg
```

### Comparing `compose-py-0.1.0/LICENSE` & `compose-py-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `compose-py-0.1.0/PKG-INFO` & `compose-py-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compose-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for parsing and loading Compose files
 Author-email: Yuki Igarashi <me@bonprosoft.com>
 License: MIT License
         
         Copyright (c) 2023 Yuki Igarashi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `compose-py-0.1.0/README.md` & `compose-py-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `compose-py-0.1.0/compose_py/_yaml.py` & `compose-py-0.1.1/compose_py/_yaml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-import os
 import pathlib
 import typing
 from typing import Any, Dict, Optional, Type, Union
 
 import yaml
 
+from ._types import Path
+
 DumperType = Any
 
 if typing.TYPE_CHECKING:
     from yaml.cyaml import _CLoader
     from yaml.loader import _Loader
 
     LoaderClass = Union[_Loader, _CLoader]
     LoaderType = Type[LoaderClass]
 else:
     LoaderClass = Any
     LoaderType = Any
 
 
-def ensure_pathlib_obj(p: os.PathLike) -> pathlib.Path:
+def ensure_pathlib_obj(p: Path) -> pathlib.Path:
     return pathlib.Path(p)
 
 
 def load(
-    path: os.PathLike,
+    path: Path,
     *,
     loader: Optional[LoaderType] = None,
 ) -> Dict[str, Any]:
     path = ensure_pathlib_obj(path)
     loader = loader or yaml.SafeLoader
     with path.open("r") as f:
         data: Dict[str, Any] = yaml.load(f, Loader=loader)
         return data
 
 
 def dump(
     obj: Any,
-    path: os.PathLike,
+    path: Path,
     *,
     dumper: Optional[DumperType] = None,
 ) -> None:
     path = ensure_pathlib_obj(path)
     dumper = dumper or yaml.SafeDumper
     with path.open("w") as f:
         yaml.dump(obj, f, Dumper=dumper)
```

### Comparing `compose-py-0.1.0/compose_py/dumper.py` & `compose-py-0.1.1/compose_py/dumper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import enum
-import os
 import typing
 from typing import Any, Dict, Optional, TypeVar, cast, overload
 
 from . import _yaml
+from ._types import Path
 from .model_type import ModelType
 
 ComposeSpecification = Any
 TObj = TypeVar("TObj")
 
 if typing.TYPE_CHECKING:
     from typing import Literal
@@ -55,50 +55,50 @@
 
         return models_dataclasses.dump_dict(obj, simplify=simplify)
 
 
 @overload
 def dump_yaml(
     obj: "models_pydantic.ComposeSpecification",
-    path: os.PathLike,
+    path: Path,
     *,
     model: "Literal[ModelType.PYDANTIC]" = ...,
     simplify: bool = ...,
     dumper: Optional[_yaml.DumperType] = ...,
 ) -> None:
     ...
 
 
 @overload
 def dump_yaml(
     obj: "models_dataclasses.ComposeSpecification",
-    path: os.PathLike,
+    path: Path,
     *,
     model: "Literal[ModelType.DATACLASSES]",
     simplify: bool = ...,
     dumper: Optional[_yaml.DumperType] = ...,
 ) -> None:
     ...
 
 
 @overload
 def dump_yaml(
     obj: ComposeSpecification,
-    path: os.PathLike,
+    path: Path,
     *,
     model: ModelType,
     simplify: bool = ...,
     dumper: Optional[_yaml.DumperType] = ...,
 ) -> None:
     ...
 
 
 def dump_yaml(
     obj: ComposeSpecification,
-    path: os.PathLike,
+    path: Path,
     *,
     model: ModelType = ModelType.PYDANTIC,
     simplify: bool = True,
     dumper: Optional[_yaml.DumperType] = None,
 ) -> None:
     data = dump_dict(obj, model=model, simplify=simplify)
     data = replace_enum_with_values(data)
```

### Comparing `compose-py-0.1.0/compose_py/loader.py` & `compose-py-0.1.1/compose_py/loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import os
 import typing
 from typing import Any, Dict, Optional, overload
 
 from . import _yaml
+from ._types import Path
 from .model_type import ModelType
 
 ComposeSpecification = Any
 
 if typing.TYPE_CHECKING:
     from typing import Literal
 
@@ -49,43 +49,43 @@
         from . import models_dataclasses
 
         return models_dataclasses.load_dict(data)
 
 
 @overload
 def load_yaml(
-    path: os.PathLike,
+    path: Path,
     *,
     model: "Literal[ModelType.PYDANTIC]" = ...,
     loader: Optional[_yaml.LoaderType] = ...,
 ) -> "models_pydantic.ComposeSpecification":
     ...
 
 
 @overload
 def load_yaml(
-    path: os.PathLike,
+    path: Path,
     *,
     model: "Literal[ModelType.DATACLASSES]",
     loader: Optional[_yaml.LoaderType] = ...,
 ) -> "models_dataclasses.ComposeSpecification":
     ...
 
 
 @overload
 def load_yaml(
-    path: os.PathLike,
+    path: Path,
     *,
     model: ModelType,
     loader: Optional[_yaml.LoaderType] = ...,
 ) -> ComposeSpecification:
     ...
 
 
 def load_yaml(
-    path: os.PathLike,
+    path: Path,
     *,
     model: ModelType = ModelType.PYDANTIC,
     loader: Optional[_yaml.LoaderType] = None,
 ) -> ComposeSpecification:
     data = _yaml.load(path, loader=loader)
     return load_dict(data, model=model)
```

### Comparing `compose-py-0.1.0/compose_py.egg-info/PKG-INFO` & `compose-py-0.1.1/compose_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compose-py
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python library for parsing and loading Compose files
 Author-email: Yuki Igarashi <me@bonprosoft.com>
 License: MIT License
         
         Copyright (c) 2023 Yuki Igarashi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `compose-py-0.1.0/pyproject.toml` & `compose-py-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -39,12 +39,16 @@
   "isort==5.12.0",
   "mypy==1.3.0",
   "pysen==0.10.4",
   "pytest==7.3.1",
   "types-PyYAML==6.0.12.9",
 ]
 
-[tool.setuptools]
-packages = ["compose_py"]
+[tool.setuptools.packages.find]
+exclude = ["build", "tests"]
+namespaces = false
+
+[tool.setuptools.package-data]
+"compose_py" = ["py.typed"]
 
 [tool.setuptools.dynamic]
 version = {attr = "compose_py._version.__version__"}
```

