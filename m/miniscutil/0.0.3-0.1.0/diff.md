# Comparing `tmp/miniscutil-0.0.3.tar.gz` & `tmp/miniscutil-0.1.0.tar.gz`

## Comparing `miniscutil-0.0.3.tar` & `miniscutil-0.1.0.tar`

### file list

```diff
@@ -1,29 +1,39 @@
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/__about__.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/__init__.py
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/adapt.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/asyncio_helpers.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/config.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/current.py
--rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/deep.py
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/deepeq.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/dictdiff.py
--rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/dispatch.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/misc.py
--rw-r--r--   0        0        0    12281 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/ofdict.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/sum.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.0.3/miniscutil/type_util.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_classdispatch.py
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_config.py
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_current.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_deepeq.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_humansize.py
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_ofdict.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_typing.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/test_util.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.0.3/tests/snapshots/test_humansize/test_human_size/bytes
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.0.3/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 miniscutil-0.0.3/README.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 miniscutil-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/__about__.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/__init__.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/adapt.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/asyncio_helpers.py
+-rw-r--r--   0        0        0     8959 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/config.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/current.py
+-rw-r--r--   0        0        0    11903 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/deep.py
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/deepeq.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/dictdiff.py
+-rw-r--r--   0        0        0     3469 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/dispatch.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/misc.py
+-rw-r--r--   0        0        0    12454 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/ofdict.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/sum.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/type_util.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/lsp/README.md
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/lsp/__init__.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/lsp/server.py
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/lsp/types.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/rpc/__init__.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/rpc/io_transport.py
+-rw-r--r--   0        0        0    18796 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/rpc/jsonrpc.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/rpc/starlette_ws_transport.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/rpc/transport.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 miniscutil-0.1.0/miniscutil/rpc/websocket_transport.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_classdispatch.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_config.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_current.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_deepeq.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_humansize.py
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_ofdict.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_typing.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/test_util.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 miniscutil-0.1.0/tests/snapshots/test_humansize/test_human_size/bytes
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 miniscutil-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 miniscutil-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 miniscutil-0.1.0/README.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 miniscutil-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 miniscutil-0.1.0/PKG-INFO
```

### Comparing `miniscutil-0.0.3/miniscutil/__init__.py` & `miniscutil-0.1.0/miniscutil/__init__.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/miniscutil/adapt.py` & `miniscutil-0.1.0/miniscutil/adapt.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/miniscutil/asyncio_helpers.py` & `miniscutil-0.1.0/miniscutil/asyncio_helpers.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/miniscutil/config.py` & `miniscutil-0.1.0/miniscutil/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         p = Path(os.environ.get("XDG_CONFIG_HOME", "~/.config"))
     p = p.expanduser().resolve() / app_name
     p.mkdir(exist_ok=True)
     return p
 
 
 def get_app_cache_dir(app_name: str) -> Path:
+    """Returns the path that ths OS wants you to use to place application-specific caching files."""
     if sys.platform == "win32":
         p = Path(os.environ.get("LOCALAPPDATA", "~/.cache"))
     elif sys.platform == "linux":
         p = Path(os.environ.get("XDG_CACHE_HOME", "~/.cache"))
     elif sys.platform == "darwin":  # macos
         p = Path("~/Library/Caches")
     else:
@@ -135,14 +136,85 @@
         key = (key,)
     for k in key:
         j = j[k]
     return j
 
 
 class SecretPersist:
+    """Mixin for managing secrets that live in a config file.
+
+    ## Worked example:
+
+    ```python
+    from pydantic import BaseSettings
+    from miniscutil import SecretPersist, get_app_config_dir
+
+    CONFIG_DIR = get_app_config_dir("my_app")
+
+    class Settings(BaseSettings, SecretPersist):
+        api_key: Optional[SecretStr] = Field(default=None, is_secret=True)
+
+        def get_api_key(self):
+            return self.get_secret("api_key")
+
+        def persist_api_key(self, api_key: str):
+            self.persist_secret("api_key", api_key)
+
+        @property
+        def secrets_file(self) -> Path:
+            return CONFIG_DIR / "secrets.json"
+
+        class Config:
+            env_file = ".env"
+            env_file_encoding = "utf-8"
+
+
+    if __name__ == "__main__":
+       cfg = Settings()
+       k1 = cfg.get_secret('api_key')
+       print(k1)
+       cfg.persist_secret('api_key', 'asdf')
+       k2 = cfg.get_secret('api_key')
+       print(k2)
+
+    ```
+
+    Note that if you want to access the secret, you should use `cfg.get_secret` instead of `cfg.api_key`.
+    The field will still be accessable but if the secret is stored in a config file then it won't automatically access it.
+    Once you have called 'get_secret' the value of `cfg.api_key` will be updated.
+
+    Note also that this means that if there is `api_key` present as an environment variable, this __takes precedence__
+    over the `api_key` field in the secrets file.
+
+    ## Adding multiple secrets for the same key but different configurations
+
+    Often you want to be able to store multiple secret values for different configurations.
+    For example you might need a different API key for dev/prod servers.
+
+    You can set this up by adding `secret_postfix` field to the pydantic config:
+
+    ```
+    class Settings(BaseSettings, SecretPersist):
+        mode : Literal['dev', 'prod'] = Field(default='dev')
+        ...
+        class Config:
+            ...
+            secret_postfix = lambda self: self.mode
+    ```
+
+    Now, when you call `persist_secret`, it will save it in a different slot determined by
+    `secret_postfix`. So now `get_secret`'s return value will depend on whether mode is dev or prod.
+
+    ## Todos
+
+    - [ ] add a warning if the secrets file is overridden
+    - [ ] automatically get the secret from the secret file on field access.
+
+    """
+
     def _get_secret_prelude(self, key: str):
         assert isinstance(self, BaseSettings)
         fields = getattr(self, "__fields__")
         assert key in fields
         field = fields[key]
         assert is_subtype(SecretStr, field.annotation)
         extra = field.field_info.extra
```

### Comparing `miniscutil-0.0.3/miniscutil/current.py` & `miniscutil-0.1.0/miniscutil/current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/miniscutil/deep.py` & `miniscutil-0.1.0/miniscutil/deep.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/miniscutil/deepeq.py` & `miniscutil-0.1.0/miniscutil/deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/miniscutil/dispatch.py` & `miniscutil-0.1.0/miniscutil/dispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/miniscutil/misc.py` & `miniscutil-0.1.0/miniscutil/misc.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/miniscutil/ofdict.py` & `miniscutil-0.1.0/miniscutil/ofdict.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     Type,
     TypeVar,
     Union,
     get_args,
     get_origin,
 )
 import logging
+
+from pydantic import ValidationError
 from .dispatch import classdispatch
 from .type_util import as_list, as_newtype, as_optional, as_set, is_optional
 
 try:
     from typing import TypeGuard
 except ImportError:
     from typing_extensions import TypeGuard
@@ -417,12 +419,15 @@
 
     @todict.register(BaseModel)
     def _todict_model(x: BaseModel):
         return x.dict()
 
     @ofdict.register(BaseModel)
     def _ofdict_model(ModelCls: type[BaseModel], item):
-        return ModelCls.parse_obj(item)
+        try:
+            return ModelCls.parse_obj(item)
+        except ValidationError as e:
+            raise TypeError(f"Model {ModelCls.__name__} is invalid: {e}") from e
 
     # [todo] pydantic validation types like EmailStr, SecretStr etc
 except ImportError:
     pass
```

### Comparing `miniscutil-0.0.3/miniscutil/sum.py` & `miniscutil-0.1.0/miniscutil/sum.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/miniscutil/type_util.py` & `miniscutil-0.1.0/miniscutil/type_util.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/tests/test_classdispatch.py` & `miniscutil-0.1.0/tests/test_classdispatch.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/tests/test_config.py` & `miniscutil-0.1.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/tests/test_current.py` & `miniscutil-0.1.0/tests/test_current.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/tests/test_deepeq.py` & `miniscutil-0.1.0/tests/test_deepeq.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/tests/test_ofdict.py` & `miniscutil-0.1.0/tests/test_ofdict.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/tests/test_typing.py` & `miniscutil-0.1.0/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/.gitignore` & `miniscutil-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/LICENSE.txt` & `miniscutil-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/README.md` & `miniscutil-0.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -12,22 +12,7 @@
 - `dispatch.py` hijacks the dispatcher used by `functools.singledispatch` as its own class. This is used to implement a `classdispatch` decorator that can accept a type as argument.
 - `adapt`, an implementation of [PEP-246](https://peps.python.org/pep-0246/#specification)
 - `ofdict.py` converts to and from a json-like object `JsonLike = Union[str, int, float, bool, type(None), list[JsonLike], dict[str, JsonLike]]`. It overlaps a lot with `attrs`, `cattrs` and `pydantic` libraries.
 - `deep.py` implements a deepcopy-like reduction system for traversing, mapping and serializing arbitrary python objects.
 - `deepeq.py` implements a deep-equality algorithm.
 - `current.py` is a base class for implementing the singleton pattern.
 - `sum.py` discriminated sum type.
-
-**Table of Contents**
-
-- [Installation](#installation)
-- [License](#license)
-
-## Installation
-
-```console
-pip install miniscutil
-```
-
-## License
-
-`miniscutil` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `miniscutil-0.0.3/pyproject.toml` & `miniscutil-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `miniscutil-0.0.3/PKG-INFO` & `miniscutil-0.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniscutil
-Version: 0.0.3
+Version: 0.1.0
 Project-URL: Documentation, https://github.com/EdAyers/sss/miniscutil#readme
 Project-URL: Issues, https://github.com/EdAyers/sss/miniscutil/issues
 Project-URL: Source, https://github.com/EdAyers/sss/miniscutil
 Author-email: "E.W.Ayers" <contact@edayers.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -35,22 +35,7 @@
 - `dispatch.py` hijacks the dispatcher used by `functools.singledispatch` as its own class. This is used to implement a `classdispatch` decorator that can accept a type as argument.
 - `adapt`, an implementation of [PEP-246](https://peps.python.org/pep-0246/#specification)
 - `ofdict.py` converts to and from a json-like object `JsonLike = Union[str, int, float, bool, type(None), list[JsonLike], dict[str, JsonLike]]`. It overlaps a lot with `attrs`, `cattrs` and `pydantic` libraries.
 - `deep.py` implements a deepcopy-like reduction system for traversing, mapping and serializing arbitrary python objects.
 - `deepeq.py` implements a deep-equality algorithm.
 - `current.py` is a base class for implementing the singleton pattern.
 - `sum.py` discriminated sum type.
-
-**Table of Contents**
-
-- [Installation](#installation)
-- [License](#license)
-
-## Installation
-
-```console
-pip install miniscutil
-```
-
-## License
-
-`miniscutil` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

