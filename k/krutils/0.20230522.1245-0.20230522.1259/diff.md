# Comparing `tmp/krutils-0.20230522.1245.tar.gz` & `tmp/krutils-0.20230522.1259.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krutils-0.20230522.1245.tar", last modified: Mon May 22 03:45:55 2023, max compression
+gzip compressed data, was "krutils-0.20230522.1259.tar", last modified: Mon May 22 03:59:42 2023, max compression
```

## Comparing `krutils-0.20230522.1245.tar` & `krutils-0.20230522.1259.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 03:45:54.961568 krutils-0.20230522.1245/
--rw-rw-rw-   0        0        0      526 2023-05-22 03:45:54.958896 krutils-0.20230522.1245/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-05-04 06:11:18.000000 krutils-0.20230522.1245/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 03:45:54.805866 krutils-0.20230522.1245/krutils/
--rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230522.1245/krutils/AppErr.py
--rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230522.1245/krutils/CONST.py
--rw-rw-rw-   0        0        0       71 2023-04-11 07:37:54.000000 krutils-0.20230522.1245/krutils/__init__.py
--rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230522.1245/krutils/_dbmgr.py
--rw-rw-rw-   0        0        0     7252 2023-05-22 02:48:58.000000 krutils-0.20230522.1245/krutils/logger.py
--rw-rw-rw-   0        0        0    26748 2023-05-22 03:44:55.000000 krutils-0.20230522.1245/krutils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:45:54.941336 krutils-0.20230522.1245/krutils.egg-info/
--rw-rw-rw-   0        0        0      526 2023-05-22 03:45:54.000000 krutils-0.20230522.1245/krutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      300 2023-05-22 03:45:54.000000 krutils-0.20230522.1245/krutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 03:45:54.000000 krutils-0.20230522.1245/krutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-22 03:45:54.000000 krutils-0.20230522.1245/krutils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 03:45:54.000000 krutils-0.20230522.1245/krutils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 03:45:54.961568 krutils-0.20230522.1245/setup.cfg
--rw-rw-rw-   0        0        0      858 2023-05-22 03:45:53.000000 krutils-0.20230522.1245/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 03:45:54.950662 krutils-0.20230522.1245/test/
--rw-rw-rw-   0        0        0      308 2023-05-22 03:42:17.000000 krutils-0.20230522.1245/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:59:42.799221 krutils-0.20230522.1259/
+-rw-rw-rw-   0        0        0      526 2023-05-22 03:59:42.782029 krutils-0.20230522.1259/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-05-04 06:11:18.000000 krutils-0.20230522.1259/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 03:59:42.604765 krutils-0.20230522.1259/krutils/
+-rw-rw-rw-   0        0        0      455 2022-04-21 08:14:50.000000 krutils-0.20230522.1259/krutils/AppErr.py
+-rw-rw-rw-   0        0        0     1741 2023-04-11 07:38:24.000000 krutils-0.20230522.1259/krutils/CONST.py
+-rw-rw-rw-   0        0        0       71 2023-04-11 07:37:54.000000 krutils-0.20230522.1259/krutils/__init__.py
+-rw-rw-rw-   0        0        0     5471 2023-04-11 07:45:04.000000 krutils-0.20230522.1259/krutils/_dbmgr.py
+-rw-rw-rw-   0        0        0    12538 2023-05-22 03:59:25.000000 krutils-0.20230522.1259/krutils/logger.py
+-rw-rw-rw-   0        0        0    21458 2023-05-22 03:59:08.000000 krutils-0.20230522.1259/krutils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:59:42.756961 krutils-0.20230522.1259/krutils.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-05-22 03:59:42.000000 krutils-0.20230522.1259/krutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      300 2023-05-22 03:59:42.000000 krutils-0.20230522.1259/krutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 03:59:42.000000 krutils-0.20230522.1259/krutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-22 03:59:42.000000 krutils-0.20230522.1259/krutils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 03:59:42.000000 krutils-0.20230522.1259/krutils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 03:59:42.800279 krutils-0.20230522.1259/setup.cfg
+-rw-rw-rw-   0        0        0      858 2023-05-22 03:59:40.000000 krutils-0.20230522.1259/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 03:59:42.776612 krutils-0.20230522.1259/test/
+-rw-rw-rw-   0        0        0      308 2023-05-22 03:42:17.000000 krutils-0.20230522.1259/test/test_logger.py
```

### Comparing `krutils-0.20230522.1245/PKG-INFO` & `krutils-0.20230522.1259/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230522.1245
+Version: 0.20230522.1259
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230522.1245/krutils/CONST.py` & `krutils-0.20230522.1259/krutils/CONST.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1245/krutils/_dbmgr.py` & `krutils-0.20230522.1259/krutils/_dbmgr.py`

 * *Files identical despite different names*

### Comparing `krutils-0.20230522.1245/krutils/utils.py` & `krutils-0.20230522.1259/krutils/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -775,169 +775,14 @@
 
 
 
 
 ##########################################
 ##      LOGGING
 ##########################################
-# 로그 설정값을 관리
-class _logger_config:
-
-    def __init__(self):
-        ######################
-        # 기본 변수
-
-        # 호출자 인덱스
-        self._CALLER_IDX        = 4;
-
-        # 문자열 치환자
-        self._LOG_SUBSTITUTOR    = "%%";
-
-        # 시스템 로그를 포함하여 출력
-        self.DEBUG_LEVEL_ALL    = _logger_util().get_log_level_index("SYSTEM");
-        # # DB접근 로그를 포함하여 출력
-        self.DEBUG_LEVEL_DB     = _logger_util().get_log_level_index("DB");
-        # # 프로그램 로그를 포함하여 출력
-        self.DEBUG_LEVEL_DEBUG  = _logger_util().get_log_level_index("DEBUG");
-        # # 중요 정보 발생시 출력
-        self.DEBUG_LEVEL_INFO   = _logger_util().get_log_level_index("INFO");
-        # # 오류 발생시 출력
-        self.DEBUG_LEVEL_ERROR  = _logger_util().get_log_level_index("ERROR");
-
-
-        ######################
-        # 설정
-
-        # 파일명 지정
-        self.CONFIG_FILE_PATH = ''
-
-        ######################
-        # 로거 동작 설정
-        ######################
-        # 현재 로그레벨 (최초 생성시 기본로그레벨로 세팅)
-        self.CURR_DEBUG_LEVEL       = _logger_util().get_log_level_index("INFO");
-
-        # 디버깅 출력 방법 : 콘솔 출력 여부
-        self.DEBUG_CONSOLE_PRINT_YN = "Y";
-
-        # 디버깅 출력 방법 : 파일 출력 여부
-        self.DEBUG_FILE_PRINT_YN    = "N";
-
-
-        # 디버깅 출력 방법 : 파일 출력 경로
-        from datetime import datetime
-        self.DEBUG_FILE_DIR_PATH  = "./logs";
-        self.DEBUG_FILE_FILE_NAME  = datetime.now().strftime("%H%M%S") + '.log';
-
-
-
-
-class _logger_util:
-
-    def get_log_level_index(self, level: str) -> int:
-        ''' 로깅 레벨 설정 '''
-        if level == None:
-            return 4
-        elif level == "ERROR":
-            return 4
-        elif level == "INFO":
-            return 3
-        elif level == "DEBUG":
-            return 2
-        elif level == "DB":
-            return 1
-        elif level == "SYSTEM":
-            return 0
-        return 4
-
-    def nvl_dict(self, d: dict, k: str, nv: str) -> str:
-
-        if (d == None):
-            return None
-
-        if (isinstance(d, dict) != True):
-            return None
-
-        if (k == None):
-            return ''
-
-        #import traceback
-        try:
-            v = d[k]
-        except Exception as e:
-            v = nv
-
-        # print (f'v[{v}]')
-
-        return v
-
-    def find_config_file_path(self, start_path: str) -> str:
-        ''' logger 설정 파일을 찾는다 '''
-
-        import os
-
-        curr_dir = os.path.dirname(start_path)
-        CONFIG_FILE_NAME = 'logger.json'
-
-        config_file_path = ""
-        for ii in range(5):
-            # print("seeking..[{0}]th : {1}".format(ii, curr_dir))
-
-            if (os.path.isfile(curr_dir + "/" + CONFIG_FILE_NAME) == True):
-                config_file_path = os.path.join(curr_dir, CONFIG_FILE_NAME)
-                # print("찾았다!", config_file_path)
-                break
-            else:
-                # print("상위로 찾아 올라간다[{0}]->[{1}]".format(curr_dir, os.path.abspath(os.path.join(curr_dir, '..'))))
-                # root까지 확인된 경우 : 더이상 찾을 수 없을 때
-                if (curr_dir == os.path.abspath(os.path.join(curr_dir, '..'))):
-                    # print("못찾았다!")
-                    config_file_path = ''
-                    # raise Exception(CONFIG_FILE_NAME + " 파일을 찾을 수 없습니다.")
-                    break
-                else:
-                    curr_dir = os.path.abspath(os.path.join(curr_dir, '..'))
-
-        # print("get_config_file_path() -> [{0}]".format(config_file_path))
-        return config_file_path
-
-    def parse_config_file(self, config_file_path: str) -> dict():
-        ''' logger 설정 파일을 읽어 config 객체로 변환한다 '''
-
-        # 파일이 존재하는가
-        import os.path
-        if (os.path.isfile(config_file_path) != True):
-            return None
-
-        # 파싱하자
-        import json
-        with open(config_file_path) as _cfp:
-            config_json = json.load(_cfp)
-
-        if config_json == None:
-            return None
-
-        # config 객체 매핑하자
-        parsed_config = _logger_config()
-
-        parsed_config.CONFIG_FILE_PATH = config_file_path
-
-        parsed_config.CURR_DEBUG_LEVEL = self.get_log_level_index(self.nvl_dict(config_json, 'LOG_LEVEL', parsed_config.CURR_DEBUG_LEVEL))
-        parsed_config.DEBUG_CONSOLE_PRINT_YN = self.nvl_dict(config_json, 'LOG_CONSOLE_YN', parsed_config.DEBUG_CONSOLE_PRINT_YN)
-        parsed_config.DEBUG_FILE_PRINT_YN = self.nvl_dict(config_json, 'LOG_FILE_YN', parsed_config.DEBUG_FILE_PRINT_YN)
-        parsed_config.DEBUG_FILE_DIR_PATH = self.nvl_dict(config_json, 'LOG_DIR_PATH', parsed_config.DEBUG_FILE_DIR_PATH)
-        parsed_config.DEBUG_FILE_FILE_NAME = self.nvl_dict(config_json, 'LOG_FILE_NAME', parsed_config.DEBUG_FILE_FILE_NAME)
-
-        # print(parsed_config.__dict__)
-        return parsed_config
-
-
-
-
-
 class logger(____file__):
     '''
     from krutils import utils
     logger = utils.logger(__file__)
 
     or
```

### Comparing `krutils-0.20230522.1245/krutils.egg-info/PKG-INFO` & `krutils-0.20230522.1259/krutils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krutils
-Version: 0.20230522.1245
+Version: 0.20230522.1259
 Summary: Some utils for me.
 Author: bonfireof
 Author-email: bonfireof@gmail.com
 Project-URL: Bug Tracker, https://github.com/bonfireof/krutils
 Project-URL: Documentation, https://github.com/bonfireof/krutils
 Project-URL: Source Code, https://github.com/bonfireof/krutils
 Classifier: Programming Language :: Python :: 3
```

### Comparing `krutils-0.20230522.1245/setup.py` & `krutils-0.20230522.1259/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="krutils",
-    version="0.20230522.1245",
+    version="0.20230522.1259",
     author="bonfireof",
     author_email="bonfireof@gmail.com",
     description="Some utils for me.",
     project_urls={
         "Bug Tracker": "https://github.com/bonfireof/krutils",
         "Documentation": "https://github.com/bonfireof/krutils",
         "Source Code": "https://github.com/bonfireof/krutils",
```

