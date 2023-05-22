# Comparing `tmp/renus-1.1.4.tar.gz` & `tmp/renus-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renus-1.1.4.tar", last modified: Mon May 15 08:08:00 2023, max compression
+gzip compressed data, was "renus-1.1.5.tar", last modified: Mon May 22 06:20:34 2023, max compression
```

## Comparing `renus-1.1.4.tar` & `renus-1.1.5.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 08:08:00.091553 renus-1.1.4/
--rw-rw-rw-   0        0        0     1539 2022-12-08 07:04:23.000000 renus-1.1.4/LICENSE
--rw-rw-rw-   0        0        0       37 2023-04-20 05:31:47.000000 renus-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      220 2023-05-15 08:08:00.091553 renus-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.532617 renus-1.1.4/renus/
--rw-rw-rw-   0        0        0        0 2023-04-20 05:37:22.000000 renus-1.1.4/renus/__init__.py
--rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.1.4/renus/app.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.560619 renus-1.1.4/renus/commands/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.619617 renus-1.1.4/renus/commands/app/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/app/__init__.py
--rw-rw-rw-   0        0        0     1786 2023-05-03 04:46:26.000000 renus-1.1.4/renus/commands/app/controller.temp
--rw-rw-rw-   0        0        0     1143 2023-05-15 07:03:04.000000 renus-1.1.4/renus/commands/app/model.temp
--rw-rw-rw-   0        0        0      518 2023-03-14 08:51:15.000000 renus-1.1.4/renus/commands/app/route.temp
--rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.1.4/renus/commands/app/run.py
--rw-rw-rw-   0        0        0      211 2022-10-09 08:00:32.000000 renus-1.1.4/renus/commands/app/vue.temp
-drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.644763 renus-1.1.4/renus/commands/backup/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/backup/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.1.4/renus/commands/backup/run.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.654761 renus-1.1.4/renus/commands/copy/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/copy/__init__.py
--rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.1.4/renus/commands/copy/run.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.672132 renus-1.1.4/renus/commands/default/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/default/__init__.py
--rw-rw-rw-   0        0        0     1380 2023-04-30 01:41:46.000000 renus-1.1.4/renus/commands/default/run.py
--rw-rw-rw-   0        0        0     1472 2023-05-15 06:28:58.000000 renus-1.1.4/renus/commands/help.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.707949 renus-1.1.4/renus/commands/install/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/install/__init__.py
--rw-rw-rw-   0        0        0     4079 2023-03-12 17:31:41.000000 renus-1.1.4/renus/commands/install/build.py
--rw-rw-rw-   0        0        0     4042 2023-05-15 07:57:33.000000 renus-1.1.4/renus/commands/install/run.py
--rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.1.4/renus/commands/install/service.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.725527 renus-1.1.4/renus/commands/permission/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/permission/__init__.py
--rw-rw-rw-   0        0        0      763 2023-04-30 01:38:29.000000 renus-1.1.4/renus/commands/permission/run.py
--rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.1.4/renus/commands/run.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:08:00.051537 renus-1.1.4/renus/core/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/__init__.py
--rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.1.4/renus/core/cache.py
--rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/concurrency.py
--rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/config.py
--rw-rw-rw-   0        0        0     2368 2023-05-03 09:54:55.000000 renus-1.1.4/renus/core/cprint.py
--rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.1.4/renus/core/crypt.py
--rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/datastructures.py
--rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.1.4/renus/core/exception.py
--rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.1.4/renus/core/formparsers.py
--rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.1.4/renus/core/injection.py
--rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/log.py
--rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/middleware.py
--rw-rw-rw-   0        0        0    14400 2023-05-15 07:00:53.000000 renus-1.1.4/renus/core/model.py
--rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.1.4/renus/core/request.py
--rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.1.4/renus/core/response.py
--rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.1.4/renus/core/routing.py
--rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.1.4/renus/core/schedule.py
--rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.1.4/renus/core/serialize.py
--rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/status.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:08:00.079555 renus-1.1.4/renus/core/validation/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/validation/__init__.py
--rw-rw-rw-   0        0        0     8909 2023-05-14 05:18:01.000000 renus-1.1.4/renus/core/validation/rules.py
--rw-rw-rw-   0        0        0     3552 2023-05-14 05:22:21.000000 renus-1.1.4/renus/core/validation/validate.py
--rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.1.4/renus/core/websockets.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:08:00.089537 renus-1.1.4/renus/util/
--rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.4/renus/util/__init__.py
--rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.1.4/renus/util/helper.py
-drwxrwxrwx   0        0        0        0 2023-05-15 08:07:59.551618 renus-1.1.4/renus.egg-info/
--rw-rw-rw-   0        0        0      220 2023-05-15 08:07:59.000000 renus-1.1.4/renus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1426 2023-05-15 08:07:59.000000 renus-1.1.4/renus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 08:07:59.000000 renus-1.1.4/renus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-15 08:07:59.000000 renus-1.1.4/renus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 08:08:00.091553 renus-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      334 2023-05-15 08:07:19.000000 renus-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:20:34.572210 renus-1.1.5/
+-rw-rw-rw-   0        0        0     1539 2022-12-08 07:04:23.000000 renus-1.1.5/LICENSE
+-rw-rw-rw-   0        0        0       37 2023-04-20 05:31:47.000000 renus-1.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      220 2023-05-22 06:20:34.570207 renus-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2022-12-05 06:16:54.000000 renus-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.194105 renus-1.1.5/renus/
+-rw-rw-rw-   0        0        0        0 2023-04-20 05:37:22.000000 renus-1.1.5/renus/__init__.py
+-rw-rw-rw-   0        0        0     7705 2022-12-08 08:01:10.000000 renus-1.1.5/renus/app.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.279211 renus-1.1.5/renus/commands/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.460191 renus-1.1.5/renus/commands/app/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/app/__init__.py
+-rw-rw-rw-   0        0        0     1786 2023-05-03 04:46:26.000000 renus-1.1.5/renus/commands/app/controller.temp
+-rw-rw-rw-   0        0        0     1092 2023-05-15 10:24:30.000000 renus-1.1.5/renus/commands/app/model.temp
+-rw-rw-rw-   0        0        0      518 2023-03-14 08:51:15.000000 renus-1.1.5/renus/commands/app/route.temp
+-rw-rw-rw-   0        0        0     4144 2022-10-15 05:56:43.000000 renus-1.1.5/renus/commands/app/run.py
+-rw-rw-rw-   0        0        0      211 2022-10-09 08:00:32.000000 renus-1.1.5/renus/commands/app/vue.temp
+drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.479193 renus-1.1.5/renus/commands/backup/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/backup/__init__.py
+-rw-rw-rw-   0        0        0     1522 2023-04-01 10:04:36.000000 renus-1.1.5/renus/commands/backup/run.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.519241 renus-1.1.5/renus/commands/copy/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/copy/__init__.py
+-rw-rw-rw-   0        0        0     1768 2023-04-01 10:04:36.000000 renus-1.1.5/renus/commands/copy/run.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.554239 renus-1.1.5/renus/commands/default/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/default/__init__.py
+-rw-rw-rw-   0        0        0     1274 2023-05-21 06:32:06.000000 renus-1.1.5/renus/commands/default/run.py
+-rw-rw-rw-   0        0        0     1472 2023-05-15 06:28:58.000000 renus-1.1.5/renus/commands/help.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.609627 renus-1.1.5/renus/commands/install/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/install/__init__.py
+-rw-rw-rw-   0        0        0     3760 2023-05-22 06:18:46.000000 renus-1.1.5/renus/commands/install/build.py
+-rw-rw-rw-   0        0        0     4148 2023-05-22 06:14:27.000000 renus-1.1.5/renus/commands/install/run.py
+-rw-rw-rw-   0        0        0     1025 2023-03-02 07:29:31.000000 renus-1.1.5/renus/commands/install/service.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.647300 renus-1.1.5/renus/commands/permission/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/permission/__init__.py
+-rw-rw-rw-   0        0        0      763 2023-04-30 01:38:29.000000 renus-1.1.5/renus/commands/permission/run.py
+-rw-rw-rw-   0        0        0      372 2022-08-01 09:27:06.000000 renus-1.1.5/renus/commands/run.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:20:34.444233 renus-1.1.5/renus/core/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/__init__.py
+-rw-rw-rw-   0        0        0     5695 2022-09-25 10:11:54.000000 renus-1.1.5/renus/core/cache.py
+-rw-rw-rw-   0        0        0     1442 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/concurrency.py
+-rw-rw-rw-   0        0        0      442 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/config.py
+-rw-rw-rw-   0        0        0     2368 2023-05-03 09:54:55.000000 renus-1.1.5/renus/core/cprint.py
+-rw-rw-rw-   0        0        0     2098 2023-04-15 09:01:12.000000 renus-1.1.5/renus/core/crypt.py
+-rw-rw-rw-   0        0        0     4968 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/datastructures.py
+-rw-rw-rw-   0        0        0     1894 2022-11-21 07:22:01.000000 renus-1.1.5/renus/core/exception.py
+-rw-rw-rw-   0        0        0     8588 2022-09-25 10:17:27.000000 renus-1.1.5/renus/core/formparsers.py
+-rw-rw-rw-   0        0        0     3918 2022-08-10 04:50:38.000000 renus-1.1.5/renus/core/injection.py
+-rw-rw-rw-   0        0        0      647 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/log.py
+-rw-rw-rw-   0        0        0      427 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/middleware.py
+-rw-rw-rw-   0        0        0    15322 2023-05-15 10:26:37.000000 renus-1.1.5/renus/core/model.py
+-rw-rw-rw-   0        0        0     6580 2023-03-12 15:37:00.000000 renus-1.1.5/renus/core/request.py
+-rw-rw-rw-   0        0        0    15219 2023-02-08 08:59:43.000000 renus-1.1.5/renus/core/response.py
+-rw-rw-rw-   0        0        0     7911 2023-01-22 09:11:31.000000 renus-1.1.5/renus/core/routing.py
+-rw-rw-rw-   0        0        0     7256 2022-09-03 10:48:49.000000 renus-1.1.5/renus/core/schedule.py
+-rw-rw-rw-   0        0        0     1448 2023-01-22 09:14:04.000000 renus-1.1.5/renus/core/serialize.py
+-rw-rw-rw-   0        0        0     2933 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/status.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:20:34.534207 renus-1.1.5/renus/core/validation/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/validation/__init__.py
+-rw-rw-rw-   0        0        0     8909 2023-05-14 05:18:01.000000 renus-1.1.5/renus/core/validation/rules.py
+-rw-rw-rw-   0        0        0     3552 2023-05-14 05:22:21.000000 renus-1.1.5/renus/core/validation/validate.py
+-rw-rw-rw-   0        0        0     5857 2022-08-01 09:27:06.000000 renus-1.1.5/renus/core/websockets.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:20:34.566206 renus-1.1.5/renus/util/
+-rw-rw-rw-   0        0        0        0 2022-08-01 09:27:06.000000 renus-1.1.5/renus/util/__init__.py
+-rw-rw-rw-   0        0        0     2348 2023-01-22 09:11:31.000000 renus-1.1.5/renus/util/helper.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:20:33.215105 renus-1.1.5/renus.egg-info/
+-rw-rw-rw-   0        0        0      220 2023-05-22 06:20:32.000000 renus-1.1.5/renus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1426 2023-05-22 06:20:33.000000 renus-1.1.5/renus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 06:20:32.000000 renus-1.1.5/renus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-22 06:20:32.000000 renus-1.1.5/renus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 06:20:34.573167 renus-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      334 2023-05-22 06:19:43.000000 renus-1.1.5/setup.py
```

### Comparing `renus-1.1.4/LICENSE` & `renus-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/app.py` & `renus-1.1.5/renus/app.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/commands/app/controller.temp` & `renus-1.1.5/renus/commands/app/controller.temp`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/commands/app/model.temp` & `renus-1.1.5/renus/commands/app/model.temp`

 * *Files 8% similar despite different names*

```diff
@@ -16,20 +16,19 @@
         for k, v in doc.items():
             setattr(self, k, v)
 
 
 class {name_camel}(ModelBase,CRUD):
     collection_name="{name_db}"
     document_model=_Base
-    file_remove_func=
+    storage = Storage(None)
 
     def __init__(self,request) -> None:
         super().__init__()
         self.request=request
-        self.file_remove_func = Storage(request).remove
 
     def get(self,police: bool = True) -> typing.List[document_model]:
         return self._get(police)
 
     def first(self,police: bool = True) -> typing.Union[document_model,None]:
         return self._first(police)
```

### Comparing `renus-1.1.4/renus/commands/app/route.temp` & `renus-1.1.5/renus/commands/app/route.temp`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/commands/app/run.py` & `renus-1.1.5/renus/commands/app/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/commands/backup/run.py` & `renus-1.1.5/renus/commands/backup/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/commands/copy/run.py` & `renus-1.1.5/renus/commands/copy/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/commands/default/run.py` & `renus-1.1.5/renus/commands/default/run.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import json
-
-from renus.core.routing import Router
 from renus.util.helper import hash_new_password
 
 
 def run(args):
 
     if args[0]=='super_admin':
         from app.extension.renus.role.model import Role
@@ -23,19 +20,17 @@
         for p in permissions:
             res.append(p['_id'])
         Role('').where({
             'name': 'super_admin'
         }).update({'permission_ids': res,'active':True}, True)
 
         User('').where({
-            'country_code': str(country_code),
-            'phone': str(phone)
+            'phone': str(country_code)+' '+str(phone)
         }).update({
             'name': name,
             'username': 'admin',
             'password':hash_new_password('admin')
         }, True)
         User('').where({
-            'country_code': str(country_code),
-            'phone': str(phone)
+            'phone': str(country_code)+' '+str(phone)
         }).sync_roles(['super_admin'])
         print('Super Admin Created.\nPlease Change username and password.\nusername=admin\npassword=admin')
```

### Comparing `renus-1.1.4/renus/commands/help.py` & `renus-1.1.5/renus/commands/help.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/commands/install/build.py` & `renus-1.1.5/renus/commands/install/build.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import os
 
 
 def _add_cls(install, app):
     if install.cls:
         os.makedirs('./app/extension/' + app, exist_ok=True)
         for item in install.cls:
@@ -28,15 +27,15 @@
         os.makedirs('./app/extension/' + app, exist_ok=True)
         with open(f'./app/extension/{app}/route.py', 'w') as file:
             f = 'import ' + install.route + '\n'
             file.write(f)
 
         with open('./routes/index.py', 'r') as file:
             all = file.read()
-            routes = 'import ' + f'app.extension.{app.replace("/",".")}.route' + '\n'
+            routes = 'import ' + f'app.extension.{app.replace("/", ".")}.route' + '\n'
             all = routes + all
             with open('./routes/index.py', 'w') as b:
                 b.write(all)
 
 
 def _add_admin_templates(install):
     with open('./frontend/src/router/admin.js', 'r') as file:
@@ -77,20 +76,11 @@
                                   'file', 'test') + '");')
             all = all.replace('/* {{place new Route user}} */',
                               '/* {{place new Route user}} */\n' + item.get('path', '') + ',')
         with open('./frontend/src/router/index.js', 'w') as b:
             b.write(all)
 
 
-def _add_db(install, app):
-    if install.db:
-        for m, db in install.db.items():
-            m = m.split('.')
-            name = m[-1]
-            m.pop(-1)
-            path = '.'.join(m)
-            model = __import__(path, fromlist=[''])
-            with open(f'extension/{app}/{db}', 'r') as db:
-                d = json.loads(db.read())
-                model = getattr(model, name)('app')
-                for item in d:
-                    model.create(item)
+def _add_config(install):
+    if install.config:
+        with open(f'./config/{install.config[0]}.py', 'w') as b:
+            b.write(open(install.config[1], 'r').read())
```

### Comparing `renus-1.1.4/renus/commands/install/run.py` & `renus-1.1.5/renus/commands/install/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import shutil
 from io import BytesIO
 import zipfile
 from renus.commands.help import bc
 from renus.commands.install.service import request
 
-from renus.commands.install.build import _add_route, _add_admin_templates, _add_index_templates, _add_user_templates, \
-    _add_db, _add_cls, _add_imprt
+from renus.commands.install.build import _add_route, _add_admin_templates, _add_index_templates, _add_user_templates, _add_cls, _add_imprt, _add_config
 
 
 def download(app, version, installed, isUpdate=False):
     if app in installed:
         if isUpdate and installed[app] == version:
             return version
         elif not isUpdate:
@@ -34,15 +33,15 @@
     installed[app] = res.headers['version']
     f = zipfile.ZipFile(BytesIO(res.content))
     shutil.rmtree(f"extension/{app}", True)
     f.extractall(f"extension/{app}")
     if not isUpdate:
         install_app(app, installed)
     else:
-        print(f'{bc.OKBLUE}   updated to version{res.headers["version"]}{bc.ENDC}')
+        print(f'{bc.OKBLUE}   updated to version {res.headers["version"]}{bc.ENDC}')
     return res.headers['version']
 
 
 def rewrite(installed):
     print('   rewrite installed')
     pre_line = ''
     with open('extension/install.py', 'r') as f:
@@ -93,17 +92,22 @@
         print(f'   add {app} index_templates...')
         _add_index_templates(install)
 
     if hasattr(install, 'user_templates'):
         print(f'   add {app} user_templates...')
         _add_user_templates(install)
 
-    if hasattr(install, 'db'):
-        print(f'   add {app} DB...')
-        _add_db(install, app)
+    if hasattr(install, 'config'):
+        print(f'   add {app} config...')
+        _add_config(install)
+
+    if hasattr(install, 'setup'):
+        print(f'   setup {app}...')
+        install.setup()
+
 
 
 def install_all(apps, installed, isUpdate):
     for app, version in apps.items():
         download(app, version, installed, isUpdate)
```

### Comparing `renus-1.1.4/renus/commands/install/service.py` & `renus-1.1.5/renus/commands/install/service.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/commands/permission/run.py` & `renus-1.1.5/renus/commands/permission/run.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/cache.py` & `renus-1.1.5/renus/core/cache.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/concurrency.py` & `renus-1.1.5/renus/core/concurrency.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/cprint.py` & `renus-1.1.5/renus/core/cprint.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/crypt.py` & `renus-1.1.5/renus/core/crypt.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/datastructures.py` & `renus-1.1.5/renus/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/exception.py` & `renus-1.1.5/renus/core/exception.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/formparsers.py` & `renus-1.1.5/renus/core/formparsers.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/injection.py` & `renus-1.1.5/renus/core/injection.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/log.py` & `renus-1.1.5/renus/core/log.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/model.py` & `renus-1.1.5/renus/core/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-import os
+import re
 import typing
 from bson import ObjectId
 from pymongo import MongoClient
 from datetime import datetime
 from renus.core.config import Config
 
+
 class ModelBase:
     _client = MongoClient(Config('database').get('host', '127.0.0.1'),
                           Config('database').get('port', 27017),
                           username=Config('database').get('username', None),
                           password=Config('database').get('password', None))
 
     _database_name = Config('database').get('name', 'renus')
-    collection_name=None
+    collection_name = None
     metro = None
-    file_remove_func=None
+    storage = None
     hidden_fields = []
-    document_model=dict
-    add_time_fields=True
+    document_model = dict
+    add_time_fields = True
+
     def __init__(self) -> None:
         if hasattr(self, '_collection_name'):
             raise RuntimeError('_collection_name has expired. Use collection_name')
+
         self._steps = None
         self._where = None
         self._distinct = None
         self._limit = None
         self._skip = None
         self._sort = None
         self._select = None
@@ -73,36 +76,36 @@
         if self._steps is not None:
             self._steps.append({
                 "$match": where
             })
         else:
             if self._where is None:
                 self._where = {}
-            for k,v in where.items():
+            for k, v in where.items():
                 if k.startswith('$') and k in self._where:
                     if type(v) is list:
-                        self._where[k]+=v
+                        self._where[k] += v
                     else:
-                        self._where[k]={**self._where[k],**v}
+                        self._where[k] = {**self._where[k], **v}
                 else:
                     self._where[k] = v
 
         return self
 
     def count(self, skip=False, limit=False):
         k = {}
         if self._where is not None:
             k['filter'] = self._where
-        else :
+        else:
             k['filter'] = {}
         if skip and self._skip is not None:
             k['skip'] = self._skip
         if limit and self._limit is not None:
             k['limit'] = self._limit
-        
+
         return self.collection().count_documents(**k)
 
     def distinct(self, key: str):
         self._distinct = key
         return self
 
     def limit(self, count: int):
@@ -135,36 +138,36 @@
         else:
             s = [(key_or_list, 1 if asc else -1)]
         if self._steps is not None:
             if type(s) is list:
                 s = {i[0]: i[1] for i in s}
             self._steps.append({"$sort": s})
         else:
-            self._sort=s
+            self._sort = s
         return self
 
     def select(self, *select: [str, typing.Dict]):
         s = {}
-        if len(select)==1 and type(select[0]) is dict:
-            s=select[0]
+        if len(select) == 1 and type(select[0]) is dict:
+            s = select[0]
         else:
             for key in select:
                 if type(key) is dict:
                     s = key
                 else:
                     s[key] = 1
 
         if self._steps is not None:
             self._steps.append({'$project': s})
             return self
 
-        self._select=s
+        self._select = s
         return self
 
-    def with_relation(self, collection, local_field, forigen_field, to,single=False):
+    def with_relation(self, collection, local_field, forigen_field, to, single=False):
         if self._steps is not None:
             self._steps.append({
                 "$lookup": {
                     "from": collection,
                     "localField": local_field,
                     "foreignField": forigen_field,
                     "as": to
@@ -193,18 +196,18 @@
         if self._limit is not None:
             find = find.limit(self._limit)
         if self._distinct is not None:
             return find.distinct(self._distinct)
 
         return self.__police(find) if police else list(find)
 
-    def get(self,police: bool = True) -> typing.List[document_model]:
+    def get(self, police: bool = True) -> typing.List[document_model]:
         return self._get(police)
 
-    def _first(self, police: bool = True) -> typing.Union[document_model,None]:
+    def _first(self, police: bool = True) -> typing.Union[document_model, None]:
         self.limit(1)
         res = self.get(police)
         self._limit = None
         if len(res) == 1:
             return res[0]
         return None
 
@@ -217,72 +220,80 @@
 
         if self.add_time_fields and "created_at" not in document:
             document["created_at"] = datetime.utcnow()
 
         id = self.collection().insert_one(document).inserted_id
         document['_id'] = id
         self.boot_event('create', {}, document)
+        self._attach_file(document)
         return document
 
     def create_many(self, documents: typing.List) -> typing.List[ObjectId]:
         if self.add_time_fields:
             for document in documents:
                 if "updated_at" not in document:
                     document["updated_at"] = datetime.utcnow()
 
                 if "created_at" not in document:
                     document["created_at"] = datetime.utcnow()
 
         ids = self.collection().insert_many(documents).inserted_ids
         self.boot_event('create_many', {}, ids)
+        self._attach_file({'_id': 'create_many', 'documents': documents})
         return ids
 
     def update(self, new: dict, upsert=False, get_old=False) -> bool:
         where = self.__ud_gate('update')
         if self.add_time_fields:
             new["updated_at"] = datetime.utcnow()
         d = {"$set": new}
         if self.add_time_fields and "created_at" not in new:
             d["$setOnInsert"] = {'created_at': datetime.utcnow()}
         old = self.collection().find_one_and_update(where, d, upsert=upsert)
         self.boot_event('update', old, new)
+        new['_id'] = old['_id']
+        self._attach_file(new)
         return old if get_old else True
 
     def update_opt(self, new: dict, upsert=False, get_old=False) -> bool:
         where = self.__ud_gate('update')
         if '$set' not in new:
             new['$set'] = {}
         if '$setOnInsert' not in new:
             new['$setOnInsert'] = {}
         if self.add_time_fields:
             new['$set']["updated_at"] = datetime.utcnow()
             new['$setOnInsert']['created_at'] = datetime.utcnow()
         old = self.collection().find_one_and_update(where, new, upsert=upsert)
-        self.boot_event('update', old, {k[1:]:v for k,v in new.items()})
+        self.boot_event('update', old, {k[1:]: v for k, v in new.items()})
+        new['_id'] = old['_id']
+        self._attach_file(new)
         return old if get_old else True
 
     def update_opt_many(self, new: dict, upsert=False, get_old=False) -> bool:
         where = self.__ud_gate('update')
         if '$set' not in new:
             new['$set'] = {}
         if '$setOnInsert' not in new:
             new['$setOnInsert'] = {}
         if self.add_time_fields:
             new['$set']["updated_at"] = datetime.utcnow()
             new['$setOnInsert']['created_at'] = datetime.utcnow()
         old = self.collection().update_many(where, new, upsert=upsert).raw_result
-        self.boot_event('update', old, {k[1:]:v for k,v in new.items()})
+        self.boot_event('update', old, {k[1:]: v for k, v in new.items()})
+        self._attach_file({'_id': 'update_opt_many', 'documents': new})
         return old if get_old else True
 
     def update_many(self, new: dict) -> bool:
         where = self.__ud_gate('update')
         if self.add_time_fields:
             new["updated_at"] = datetime.utcnow()
         old = self.collection().update_many(where, {"$set": new}).raw_result
         self.boot_event('update_many', old, str(new))
+        self._attach_file({'_id': 'update_many', 'documents': new})
         return True
 
     def delete(self, all: bool = False) -> bool:
         where = self.__ud_gate('delete')
         if all is False:
             old = self.collection().find_one_and_delete(where)
             if self.metro is not None:
@@ -294,15 +305,15 @@
             old = self.collection().delete_many(where)
 
             self.boot_event('delete_many', {'deleted_count': old.deleted_count, 'where': str(where)}, {})
 
         return old
 
     def make_visible(self, fields: typing.List):
-        self.visible_fields=fields
+        self.visible_fields = fields
         return self
 
     @staticmethod
     def boot_event(typ: str, old, new):
         pass
 
     @staticmethod
@@ -324,15 +335,15 @@
         if where is not None:
             if '_id' in where:
                 where['_id'] = self.convert_id(where['_id'])
 
         return [where, select]
 
     @staticmethod
-    def cast(document:dict):
+    def cast(document: dict):
         return document
 
     def __cleaner(self, document: dict):
         for field in self.hidden_fields:
             if field in document and field not in self.visible_fields:
                 del document[field]
 
@@ -366,18 +377,19 @@
                 all = self.collection().find(where)
             else:
                 all = [obj]
 
             for item in all:
                 for field, db in self.metro.items():
                     if type(db) is not list:
-                        raise RuntimeError("metro format not true. ex: '_id':[{'collection':'test','field': 'test_id'}]")
+                        raise RuntimeError(
+                            "metro format not true. ex: '_id':[{'collection':'test','field': 'test_id'}]")
                     for d in db:
-                        strg=d.get('storage',False)
-                        c=d.get('collection',False)
+                        strg = d.get('storage', False)
+                        c = d.get('collection', False)
                         if c is not False:
                             if strg:
                                 files = self.collection(c).find({
                                     d['field']: item[field]
                                 })
 
                                 for file in files:
@@ -386,36 +398,51 @@
                                 d['field']: item[field]
                             })
                         elif strg is not False:
                             l = self.__get_links(strg, item)
                             if l:
                                 self._remove_file(l)
 
-
-    def __get_links(self,field:str,doc:dict):
+    def __get_links(self, field: str, doc: dict):
         item = doc.copy()
         p = field.split('.')
         r = None
         for i in p:
             if i not in item:
                 return False
             r = item[i]
             item = item[i]
         return r
 
+    def _attach_file(self, item):
+        if self.storage is None:
+            return
+        links = _links_extractor(item)
+        self.storage.reset().where({
+            'path': {'$in': links}
+        }).update_many({'type': self.collection_name, 'type_id': item['_id']})
+
     def _remove_file(self, links):
+        if self.storage is None:
+            return
         if type(links) is dict:
             links = list(links.values())
         if type(links) is not list:
             links = [links]
 
         for link in links:
             if type(link) is str:
-                self.file_remove_func(link)
+                self.storage.remove(link)
             elif type(link) is dict:
-                self.file_remove_func(link.get('url'))
+                self.storage.remove(link.get('url'))
             else:
                 raise RuntimeError(f"type {link} must be string or dict but its {type(link)}")
 
     @property
     def database_name(self):
         return self._database_name
+
+
+def _links_extractor(txt) -> list:
+    txt = str(txt)
+    s = re.findall("(storage/[^\s]+')", txt)
+    return [i.rstrip("'") for i in s]
```

### Comparing `renus-1.1.4/renus/core/request.py` & `renus-1.1.5/renus/core/request.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/response.py` & `renus-1.1.5/renus/core/response.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/routing.py` & `renus-1.1.5/renus/core/routing.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/schedule.py` & `renus-1.1.5/renus/core/schedule.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/serialize.py` & `renus-1.1.5/renus/core/serialize.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/status.py` & `renus-1.1.5/renus/core/status.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/validation/rules.py` & `renus-1.1.5/renus/core/validation/rules.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/validation/validate.py` & `renus-1.1.5/renus/core/validation/validate.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/core/websockets.py` & `renus-1.1.5/renus/core/websockets.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus/util/helper.py` & `renus-1.1.5/renus/util/helper.py`

 * *Files identical despite different names*

### Comparing `renus-1.1.4/renus.egg-info/SOURCES.txt` & `renus-1.1.5/renus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

