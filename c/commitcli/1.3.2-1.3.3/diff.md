# Comparing `tmp/commitcli-1.3.2.tar.gz` & `tmp/commitcli-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commitcli-1.3.2.tar", last modified: Mon May 22 07:01:58 2023, max compression
+gzip compressed data, was "commitcli-1.3.3.tar", last modified: Mon May 22 17:22:08 2023, max compression
```

## Comparing `commitcli-1.3.2.tar` & `commitcli-1.3.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-22 07:01:58.776928 commitcli-1.3.2/
--rw-r--r--   0 gallem    (1000) gallem    (1000)     3696 2023-05-22 07:01:58.776928 commitcli-1.3.2/PKG-INFO
-drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-22 07:01:58.764928 commitcli-1.3.2/commitcli/
--rw-r--r--   0 gallem    (1000) gallem    (1000)       48 2022-12-06 16:01:39.000000 commitcli-1.3.2/commitcli/__init__.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)      173 2022-10-01 21:48:20.000000 commitcli-1.3.2/commitcli/__main__.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)     8551 2023-05-22 06:48:45.000000 commitcli-1.3.2/commitcli/commit_message.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)     3487 2023-05-21 08:14:27.000000 commitcli-1.3.2/commitcli/commitcli.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)     6720 2022-12-14 06:25:36.000000 commitcli-1.3.2/commitcli/common.py
-drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-22 07:01:58.768928 commitcli-1.3.2/commitcli.egg-info/
--rw-r--r--   0 gallem    (1000) gallem    (1000)     3696 2023-05-22 07:01:58.000000 commitcli-1.3.2/commitcli.egg-info/PKG-INFO
--rw-r--r--   0 gallem    (1000) gallem    (1000)      694 2023-05-22 07:01:58.000000 commitcli-1.3.2/commitcli.egg-info/SOURCES.txt
--rw-r--r--   0 gallem    (1000) gallem    (1000)        1 2023-05-22 07:01:58.000000 commitcli-1.3.2/commitcli.egg-info/dependency_links.txt
--rw-r--r--   0 gallem    (1000) gallem    (1000)       55 2023-05-22 07:01:58.000000 commitcli-1.3.2/commitcli.egg-info/entry_points.txt
--rw-r--r--   0 gallem    (1000) gallem    (1000)       45 2023-05-22 07:01:58.000000 commitcli-1.3.2/commitcli.egg-info/requires.txt
--rw-r--r--   0 gallem    (1000) gallem    (1000)       42 2023-05-22 07:01:58.000000 commitcli-1.3.2/commitcli.egg-info/top_level.txt
-drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-22 07:01:58.772928 commitcli-1.3.2/common/
--rw-r--r--   0 gallem    (1000) gallem    (1000)       61 2023-04-12 05:50:39.000000 commitcli-1.3.2/common/__init__.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)      169 2023-05-18 06:58:05.000000 commitcli-1.3.2/common/constants.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)      840 2022-11-19 08:13:39.000000 commitcli-1.3.2/common/environment.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)      245 2022-11-19 08:13:17.000000 commitcli-1.3.2/common/logger.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)       98 2023-05-22 06:30:30.000000 commitcli-1.3.2/common/versions.py
-drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-22 07:01:58.772928 commitcli-1.3.2/configmanager/
--rwxr-xr-x   0 gallem    (1000) gallem    (1000)       20 2022-11-06 06:44:56.000000 commitcli-1.3.2/configmanager/__init__.py
--rwxr-xr-x   0 gallem    (1000) gallem    (1000)     4585 2023-05-18 07:04:01.000000 commitcli-1.3.2/configmanager/config.py
--rwxr-xr-x   0 gallem    (1000) gallem    (1000)     4786 2023-05-21 04:25:40.000000 commitcli-1.3.2/configmanager/config_manager.py
--rwxr-xr-x   0 gallem    (1000) gallem    (1000)     1426 2023-05-22 05:19:24.000000 commitcli-1.3.2/configmanager/format_module_manager.py
--rwxr-xr-x   0 gallem    (1000) gallem    (1000)       36 2022-11-06 06:44:56.000000 commitcli-1.3.2/configmanager/test_configmanager.py
--rwxr-xr-x   0 gallem    (1000) gallem    (1000)      336 2022-11-06 06:44:56.000000 commitcli-1.3.2/configmanager/test_format_module_manager.py
-drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-22 07:01:58.776928 commitcli-1.3.2/data/
--rw-r--r--   0 gallem    (1000) gallem    (1000)        0 2023-05-17 06:11:33.000000 commitcli-1.3.2/data/__init__.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)     1272 2023-05-22 06:02:31.000000 commitcli-1.3.2/data/db.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)     2894 2023-05-18 07:53:23.000000 commitcli-1.3.2/data/modules_repository.py
--rw-r--r--   0 gallem    (1000) gallem    (1000)       38 2023-05-22 07:01:58.776928 commitcli-1.3.2/setup.cfg
--rw-r--r--   0 gallem    (1000) gallem    (1000)     1362 2022-12-06 16:04:50.000000 commitcli-1.3.2/setup.py
-drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-22 07:01:58.776928 commitcli-1.3.2/tests/
--rw-r--r--   0 gallem    (1000) gallem    (1000)        0 2022-10-01 21:48:20.000000 commitcli-1.3.2/tests/__init__.py
+drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-22 17:22:08.386080 commitcli-1.3.3/
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     3696 2023-05-22 17:22:08.382080 commitcli-1.3.3/PKG-INFO
+drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-22 17:22:08.374080 commitcli-1.3.3/commitcli/
+-rw-r--r--   0 gallem    (1000) gallem    (1000)       48 2022-12-06 16:01:39.000000 commitcli-1.3.3/commitcli/__init__.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)      173 2022-10-01 21:48:20.000000 commitcli-1.3.3/commitcli/__main__.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     8527 2023-05-22 16:59:17.000000 commitcli-1.3.3/commitcli/commit_message.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     3477 2023-05-22 17:13:43.000000 commitcli-1.3.3/commitcli/commitcli.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     6720 2022-12-14 06:25:36.000000 commitcli-1.3.3/commitcli/common.py
+drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-22 17:22:08.374080 commitcli-1.3.3/commitcli.egg-info/
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     3696 2023-05-22 17:22:08.000000 commitcli-1.3.3/commitcli.egg-info/PKG-INFO
+-rw-r--r--   0 gallem    (1000) gallem    (1000)      694 2023-05-22 17:22:08.000000 commitcli-1.3.3/commitcli.egg-info/SOURCES.txt
+-rw-r--r--   0 gallem    (1000) gallem    (1000)        1 2023-05-22 17:22:08.000000 commitcli-1.3.3/commitcli.egg-info/dependency_links.txt
+-rw-r--r--   0 gallem    (1000) gallem    (1000)       55 2023-05-22 17:22:08.000000 commitcli-1.3.3/commitcli.egg-info/entry_points.txt
+-rw-r--r--   0 gallem    (1000) gallem    (1000)       45 2023-05-22 17:22:08.000000 commitcli-1.3.3/commitcli.egg-info/requires.txt
+-rw-r--r--   0 gallem    (1000) gallem    (1000)       42 2023-05-22 17:22:08.000000 commitcli-1.3.3/commitcli.egg-info/top_level.txt
+drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-22 17:22:08.378080 commitcli-1.3.3/common/
+-rw-r--r--   0 gallem    (1000) gallem    (1000)       61 2023-04-12 05:50:39.000000 commitcli-1.3.3/common/__init__.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)      169 2023-05-18 06:58:05.000000 commitcli-1.3.3/common/constants.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)      840 2022-11-19 08:13:39.000000 commitcli-1.3.3/common/environment.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)      245 2022-11-19 08:13:17.000000 commitcli-1.3.3/common/logger.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)       66 2023-05-22 17:21:54.000000 commitcli-1.3.3/common/versions.py
+drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-22 17:22:08.382080 commitcli-1.3.3/configmanager/
+-rwxr-xr-x   0 gallem    (1000) gallem    (1000)       20 2022-11-06 06:44:56.000000 commitcli-1.3.3/configmanager/__init__.py
+-rwxr-xr-x   0 gallem    (1000) gallem    (1000)     4575 2023-05-22 16:58:04.000000 commitcli-1.3.3/configmanager/config.py
+-rwxr-xr-x   0 gallem    (1000) gallem    (1000)     4751 2023-05-22 17:11:44.000000 commitcli-1.3.3/configmanager/config_manager.py
+-rwxr-xr-x   0 gallem    (1000) gallem    (1000)     1404 2023-05-22 16:59:41.000000 commitcli-1.3.3/configmanager/format_module_manager.py
+-rwxr-xr-x   0 gallem    (1000) gallem    (1000)       36 2022-11-06 06:44:56.000000 commitcli-1.3.3/configmanager/test_configmanager.py
+-rwxr-xr-x   0 gallem    (1000) gallem    (1000)      336 2022-11-06 06:44:56.000000 commitcli-1.3.3/configmanager/test_format_module_manager.py
+drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-22 17:22:08.382080 commitcli-1.3.3/data/
+-rw-r--r--   0 gallem    (1000) gallem    (1000)        0 2023-05-17 06:11:33.000000 commitcli-1.3.3/data/__init__.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     1262 2023-05-22 17:14:09.000000 commitcli-1.3.3/data/db.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     2860 2023-05-22 17:15:24.000000 commitcli-1.3.3/data/modules_repository.py
+-rw-r--r--   0 gallem    (1000) gallem    (1000)       38 2023-05-22 17:22:08.386080 commitcli-1.3.3/setup.cfg
+-rw-r--r--   0 gallem    (1000) gallem    (1000)     1362 2022-12-06 16:04:50.000000 commitcli-1.3.3/setup.py
+drwxr-xr-x   0 gallem    (1000) gallem    (1000)        0 2023-05-22 17:22:08.382080 commitcli-1.3.3/tests/
+-rw-r--r--   0 gallem    (1000) gallem    (1000)        0 2022-10-01 21:48:20.000000 commitcli-1.3.3/tests/__init__.py
```

### Comparing `commitcli-1.3.2/PKG-INFO` & `commitcli-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitcli
-Version: 1.3.2
+Version: 1.3.3
 Summary: commit cli for git with some formats, by default short version of odoo format
 Home-page: https://github.com/marco-gallegos/commit-cli
 Author: Marco A. Gallegos
 Author-email: ma_galeza@hotmail.com
 License: MIT
 Keywords: cli,cc,commit,git,odoo,github,gitlab,bitbucket,conventional commits,semantic commits
 Classifier: Programming Language :: Python :: 3
```

### Comparing `commitcli-1.3.2/commitcli/commit_message.py` & `commitcli-1.3.3/commitcli/commit_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,19 +22,19 @@
     """
     
     def __init__(
         self,
         # format: str = "cc",
         module_manager: ModuleManager,
         configuration_manager: ConfigManager = ConfigManager(),
-        tag: str|None = None,
-        module: str|None = None,
-        header: str|None= None,
-        body: str|None = None,
-        footer: str|None = None,
+        tag: str = None,
+        module: str = None,
+        header: str = None,
+        body: str = None,
+        footer: str = None,
     ):
         """Constructor of the class
 
         Args:
             format (str, optional): format to use. Defaults to "odoo".
             tag (str, optional): tag for the commit string. Defaults to None.
             module (str, optional): module affected for the commit string. Defaults to None.
```

### Comparing `commitcli-1.3.2/commitcli/commitcli.py` & `commitcli-1.3.3/commitcli/commitcli.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     :return: execution status
     :rtype: bool
     """
     can_commit = validate_current_repository()
     if (can_commit is not True):
         return False
     
-    forced_config:dict[str, bool]|None = {
+    forced_config:dict[str, bool] = {
         "avoid_optionals": not nooptionals,
     }
     logger.log("INFO","forced config runing")
     logger.log("INFO", forced_config)
 
     configuration_manager:ConfigManager = ConfigManager(override_config=forced_config)
 
@@ -76,15 +76,15 @@
 
     return message_created
 
 
 def create_commit_message(configuration_manager: ConfigManager, module_manager:ModuleManager, onlylog: bool) -> bool:
     commit_msg:CommitMessage = CommitMessage(configuration_manager=configuration_manager, module_manager=module_manager)
 
-    commit_string:str|None = None
+    commit_string:str = None
     
     try:
         commit_msg.get_answers()
     except KeyboardInterrupt:
         #BUG: this doesn works
         print("cancelling commit.")
     except Exception:
```

### Comparing `commitcli-1.3.2/commitcli/common.py` & `commitcli-1.3.3/commitcli/common.py`

 * *Files identical despite different names*

### Comparing `commitcli-1.3.2/commitcli.egg-info/PKG-INFO` & `commitcli-1.3.3/commitcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commitcli
-Version: 1.3.2
+Version: 1.3.3
 Summary: commit cli for git with some formats, by default short version of odoo format
 Home-page: https://github.com/marco-gallegos/commit-cli
 Author: Marco A. Gallegos
 Author-email: ma_galeza@hotmail.com
 License: MIT
 Keywords: cli,cc,commit,git,odoo,github,gitlab,bitbucket,conventional commits,semantic commits
 Classifier: Programming Language :: Python :: 3
```

### Comparing `commitcli-1.3.2/commitcli.egg-info/SOURCES.txt` & `commitcli-1.3.3/commitcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commitcli-1.3.2/common/environment.py` & `commitcli-1.3.3/common/environment.py`

 * *Files identical despite different names*

### Comparing `commitcli-1.3.2/configmanager/config.py` & `commitcli-1.3.3/configmanager/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     supported_formats: list = [
         "odoo",
         "sgc",
         "cc",
         "free",
     ]
 
-    def __init__(self, config:dict|None = None, signgpg: bool = False, override_config: dict|None = None) -> None:
+    def __init__(self, config:dict = None, signgpg: bool = False, override_config: dict = None) -> None:
         self.config = {
             'format': "cc",
             'signgpg': signgpg,
             'avoid_optionals': override_config['avoid_optionals'] if override_config else False,
             "db": "localfile",
             "db_url": None,
             "db_port": None,
```

### Comparing `commitcli-1.3.2/configmanager/config_manager.py` & `commitcli-1.3.3/configmanager/config_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 
 class ConfigManager(object):
     # data
     # moduleManager:ModuleManager|None
 
     def __init__(
             self, file: str = '.commitclirc',
-            config: Configuration|None = None,
-            override_config:dict|None = None,
+            config: Configuration = None,
+            override_config:dict = None,
         ) -> None:
 
         self._file:str = file
-        self.config:Configuration|None = config
+        self.config:Configuration = config
         self.regex_clave_valor = r'[\D]+[=]{1}[\w.]+'
         self.pattern_regex_clave_valor = re.compile(self.regex_clave_valor)
 
         # some initial starts
         self.init_config(override_config=override_config)
 
 
@@ -53,15 +53,15 @@
         :return: if the file exists on the filesystem
         :rtype: bool
         """
         exist = os.path.exists(file)
         return True if exist else False
 
 
-    def stringline_to_key_value(self, string_line: str = "#comentario") -> tuple[str|None, str|None]:
+    def stringline_to_key_value(self, string_line: str = "#comentario") -> tuple[str, str]:
         """This functions returns the separated values by '=' of a string in 
         format 'some=other'
 
         :param string_line: a string in fomat 'some=other', defaults to "#comentario"
         :type string_line: str, optional
         :return: the values on left and right side of the '=' character
         :rtype: str, str
@@ -72,15 +72,15 @@
             elements = string_line.split("=")
             key= elements[0]
             value= elements[1]
             logger.info(key, value)
         return key, value
 
 
-    def load_file(self, file: str) -> dict|None:
+    def load_file(self, file: str) -> dict:
         """Method to convert the configuration file into a dictionary
 
         :return: dictionary with al the key value files in thee file
         :rtype: dict
         """
         current_file = file
         if self.exist_file(current_file):
@@ -107,15 +107,15 @@
         """
         file = open(self.current_file(), 'w')
         file.write(self.config.get_configuration_file_string())
         file.close()
         return True
 
 
-    def init_config(self, force_reload: bool = False, override_config: dict|None = None) -> bool:
+    def init_config(self, force_reload: bool = False, override_config: dict = None) -> bool:
         """Method to initialize the class, triggering the load of the file or load
         creating a defaul config and save it on the file.
 
         :return: boolean representing the previous existence of the config file
         :rtype: bool
         """
         if self.config is None:
```

### Comparing `commitcli-1.3.2/configmanager/format_module_manager.py` & `commitcli-1.3.3/configmanager/format_module_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,24 +24,24 @@
 
 
 
 class ModuleManager(object):
     """
     File format
     """
-    _file:str|None
-    modules:list[ModuleConfig] | None
+    _file:str
+    modules:list[ModuleConfig]
 
 
     def __init__(self, config) -> None:
-        self._file:str|None = ".ignore.commitcli_modules"
+        self._file:str = ".ignore.commitcli_modules"
         
         modulesRepository = ModulesRepository(config)
         modulesLoaded = modulesRepository.getAll()
-        self.modules:list[ModuleConfig]|None = modulesLoaded
+        self.modules:list[ModuleConfig] = modulesLoaded
 
 
     def update_modules(self):
         pass
 
 
     def get_modules(self) -> list[ModuleConfig]:
```

### Comparing `commitcli-1.3.2/data/db.py` & `commitcli-1.3.3/data/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         :return: if the file exists on the filesystem
         :rtype: bool
         """
         exist = os.path.exists(file)
         return True if exist else False
 
 
-def returnFileDb(filename:str = " nt") -> str|None:
+def returnFileDb(filename:str = " nt") -> str:
     '''This return the full file path'''
     project_file = get_git_root()
     file_name = constants['db']['filename']
     
     if project_file is not None:
         project_file = f"{project_file}{file_name}"
 
@@ -39,12 +39,12 @@
             file = open(project_file, "a")
             file.close()
 
     return project_file
 
 
 
-def GetDatabase (config:Configuration) -> str|None:
+def GetDatabase (config:Configuration) -> str:
     if config.config["db"] == constants["config_names"]["db"]["file"]:
         return returnFileDb()
 
     return None
```

### Comparing `commitcli-1.3.2/data/modules_repository.py` & `commitcli-1.3.3/data/modules_repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 
         if self.db is None:
             raise Exception("we can not determinate the file DB")
         # logger.log('INFO',self.db)
 
     def getAll(self):
-        current_file:str|None = self.db
+        current_file:str = self.db
 
         if current_file is not None:
             modules_file:TextIOWrapper = open(current_file, "r")
             file_content:list[str] = modules_file.readlines()
             modules_file.close()
             moduleList:list = []
 
@@ -77,23 +77,22 @@
 
     def store(self, modules: list[ModuleConfig]):
         pass
 
 
 # repository to expose to the consumers
 class ModulesRepository(IModulesRepository):
-    db:str|None # or new dbs
+    db:str # or new dbs
 
     def __init__(self, config:Configuration) -> None:
         super().__init__()
         self.db_repo = LocalFileDb(config)
 
 
-    def getAll(self) -> list[ModuleConfig]|None:
+    def getAll(self) -> list[ModuleConfig]:
         all = self.db_repo.getAll()
-        print(all)
         return all
         
 
     def store(self):
         pass
```

### Comparing `commitcli-1.3.2/setup.py` & `commitcli-1.3.3/setup.py`

 * *Files identical despite different names*

