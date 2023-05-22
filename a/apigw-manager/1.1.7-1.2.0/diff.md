# Comparing `tmp/apigw_manager-1.1.7-py3-none-any.whl.zip` & `tmp/apigw_manager-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,41 +1,40 @@
-Zip file size: 42048 bytes, number of entries: 39
+Zip file size: 40898 bytes, number of entries: 38
 -rw-r--r--  2.0 unx      760 b- defN 80-Jan-01 00:00 apigw_manager/__init__.py
 -rw-r--r--  2.0 unx      760 b- defN 80-Jan-01 00:00 apigw_manager/apigw/__init__.py
 -rw-r--r--  2.0 unx     1058 b- defN 80-Jan-01 00:00 apigw_manager/apigw/admin.py
 -rw-r--r--  2.0 unx      878 b- defN 80-Jan-01 00:00 apigw_manager/apigw/apps.py
 -rw-r--r--  2.0 unx     5938 b- defN 80-Jan-01 00:00 apigw_manager/apigw/authentication.py
 -rw-r--r--  2.0 unx     3311 b- defN 80-Jan-01 00:00 apigw_manager/apigw/command.py
 -rw-r--r--  2.0 unx     1566 b- defN 80-Jan-01 00:00 apigw_manager/apigw/decorators.py
 -rw-r--r--  2.0 unx     6415 b- defN 80-Jan-01 00:00 apigw_manager/apigw/helper.py
 -rw-r--r--  2.0 unx     2075 b- defN 80-Jan-01 00:00 apigw_manager/apigw/k8s_helper.py
 -rw-r--r--  2.0 unx      760 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/__init__.py
 -rw-r--r--  2.0 unx      760 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/__init__.py
 -rw-r--r--  2.0 unx     1640 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/apply_apigw_permissions.py
--rw-r--r--  2.0 unx     6086 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/create_version_and_release_apigw.py
+-rw-r--r--  2.0 unx     6185 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/create_version_and_release_apigw.py
 -rw-r--r--  2.0 unx     1965 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/fetch_apigw_public_key.py
 -rw-r--r--  2.0 unx     1116 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/fetch_esb_public_key.py
 -rw-r--r--  2.0 unx     1664 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/grant_apigw_permissions.py
 -rw-r--r--  2.0 unx     1598 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/sync_apigw_config.py
 -rw-r--r--  2.0 unx     2401 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/sync_apigw_resources.py
 -rw-r--r--  2.0 unx     1153 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/sync_apigw_stage.py
--rw-r--r--  2.0 unx     1891 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/sync_apigw_strategies.py
 -rw-r--r--  2.0 unx     2393 b- defN 80-Jan-01 00:00 apigw_manager/apigw/management/commands/sync_resource_docs_by_archive.py
 -rw-r--r--  2.0 unx     1915 b- defN 80-Jan-01 00:00 apigw_manager/apigw/migrations/0001_initial.py
 -rw-r--r--  2.0 unx      760 b- defN 80-Jan-01 00:00 apigw_manager/apigw/migrations/__init__.py
 -rw-r--r--  2.0 unx     1270 b- defN 80-Jan-01 00:00 apigw_manager/apigw/models.py
 -rw-r--r--  2.0 unx     6602 b- defN 80-Jan-01 00:00 apigw_manager/apigw/providers.py
 -rw-r--r--  2.0 unx     3907 b- defN 80-Jan-01 00:00 apigw_manager/apigw/utils.py
 -rw-r--r--  2.0 unx      760 b- defN 80-Jan-01 00:00 apigw_manager/apigw/views.py
 -rw-r--r--  2.0 unx      760 b- defN 80-Jan-01 00:00 apigw_manager/core/__init__.py
 -rw-r--r--  2.0 unx     1390 b- defN 80-Jan-01 00:00 apigw_manager/core/configuration.py
 -rw-r--r--  2.0 unx     1441 b- defN 80-Jan-01 00:00 apigw_manager/core/exceptions.py
--rw-r--r--  2.0 unx     1441 b- defN 80-Jan-01 00:00 apigw_manager/core/fetch.py
+-rw-r--r--  2.0 unx     1643 b- defN 80-Jan-01 00:00 apigw_manager/core/fetch.py
 -rw-r--r--  2.0 unx     4321 b- defN 80-Jan-01 00:00 apigw_manager/core/handler.py
 -rw-r--r--  2.0 unx     1415 b- defN 80-Jan-01 00:00 apigw_manager/core/permission.py
 -rw-r--r--  2.0 unx     1576 b- defN 80-Jan-01 00:00 apigw_manager/core/release.py
--rw-r--r--  2.0 unx     1994 b- defN 80-Jan-01 00:00 apigw_manager/core/sync.py
+-rw-r--r--  2.0 unx     1793 b- defN 80-Jan-01 00:00 apigw_manager/core/sync.py
 -rw-r--r--  2.0 unx     1096 b- defN 80-Jan-01 00:00 apigw_manager/core/utils.py
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 apigw_manager-1.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx     1163 b- defN 80-Jan-01 00:00 apigw_manager-1.1.7.dist-info/METADATA
-?rw-r--r--  2.0 unx     3759 b- defN 16-Jan-01 00:00 apigw_manager-1.1.7.dist-info/RECORD
-39 files, 81846 bytes uncompressed, 35862 bytes compressed:  56.2%
+?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 apigw_manager-1.2.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1107 b- defN 16-Jan-01 00:00 apigw_manager-1.2.0.dist-info/METADATA
+?rw-r--r--  2.0 unx     3638 b- defN 16-Jan-01 00:00 apigw_manager-1.2.0.dist-info/RECORD
+38 files, 79873 bytes uncompressed, 34916 bytes compressed:  56.3%
```

## zipnote {}

```diff
@@ -51,17 +51,14 @@
 
 Filename: apigw_manager/apigw/management/commands/sync_apigw_resources.py
 Comment: 
 
 Filename: apigw_manager/apigw/management/commands/sync_apigw_stage.py
 Comment: 
 
-Filename: apigw_manager/apigw/management/commands/sync_apigw_strategies.py
-Comment: 
-
 Filename: apigw_manager/apigw/management/commands/sync_resource_docs_by_archive.py
 Comment: 
 
 Filename: apigw_manager/apigw/migrations/0001_initial.py
 Comment: 
 
 Filename: apigw_manager/apigw/migrations/__init__.py
@@ -102,17 +99,17 @@
 
 Filename: apigw_manager/core/sync.py
 Comment: 
 
 Filename: apigw_manager/core/utils.py
 Comment: 
 
-Filename: apigw_manager-1.1.7.dist-info/WHEEL
+Filename: apigw_manager-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: apigw_manager-1.1.7.dist-info/METADATA
+Filename: apigw_manager-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: apigw_manager-1.1.7.dist-info/RECORD
+Filename: apigw_manager-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## apigw_manager/apigw/management/commands/create_version_and_release_apigw.py

```diff
@@ -18,124 +18,125 @@
 from apigw_manager.core.fetch import Fetcher
 from apigw_manager.core.release import Releaser
 
 
 class Command(DefinitionCommand):
     """API gateway release a version"""
 
-    # 如何判断是否需要创建新版本？
-    # 1.使用配置中的版本号与线上版本进行比较，如果不一致，直接使用配置中的版本号创建新版本
-    # 2.如果配置中的版本号与线上版本一致，为了避免开发者忘记更新版本号的情况，获取同步结果进行判断：
-    #   - 如果有资源变更，使用配置中的版本号（加上当前时间作为元数据）创建新版本
-
     default_namespace = "release"
     Fetcher = Fetcher
     Releaser = Releaser
     ResourceSignatureManager = ResourceSignatureManager
     now_func = datetime.now
 
     def add_arguments(self, parser):
         super().add_arguments(parser)
 
         parser.add_argument("-t", "--title", default=None, help="release title")
         parser.add_argument("-c", "--comment", default="", help="release comment")
         parser.add_argument("-s", "--stage", default=[], nargs="+", help="release stages")
         parser.add_argument("--generate-sdks", default=False, action="store_true", help="with sdks generation")
 
-    def get_version_from_definition(self, definition):
+    def _parse_version_from_definition(self, definition):
         version = definition.get("version")
-        if version:
-            return parse_version(version)
-        return None
+        if not version:
+            return None
 
-    def get_version_from_resource_version(self, resource_version):
+        return parse_version(version)
+
+    def _parse_version_from_resource_version(self, resource_version):
         version = resource_version and resource_version.get("version")
         if not version:
             return None
 
         try:
             return parse_version(version)
         except InvalidVersion:
             return None
 
-    def fix_defined_version(self, defined_version):
+    def _fix_defined_version(self, defined_version):
         if defined_version is None:
             return parse_version("0.0.1")
 
         return defined_version
 
-    def should_create_resource_version(self, manager, api_name, defined_version, latest_version):
+    def _should_create_resource_version(self, manager, api_name, defined_version, latest_version):
         # 版本一致，且没有变更
         if latest_version and defined_version.public == latest_version.public and not manager.is_dirty(api_name):
             return False
         return True
 
-    def get_version_to_be_created(self, defined_version, latest_version):
-        if latest_version is None:
-            return defined_version
-
-        if defined_version <= latest_version:
+    def _get_version_to_be_created(self, defined_version, resource_version_exists):
+        if resource_version_exists:
             now_str = self.now_func().strftime("%Y%m%d%H%M%S")
             return parse_version("%s+%s" % (defined_version.public, now_str))
 
         return defined_version
 
-    def create_resource_version(self, releaser, version, title, comment):
+    def _create_resource_version(self, releaser, version, title, comment):
         return releaser.create_resource_version(
             version=str(version),
             title=title,
             comment=comment,
         )
 
-    def generate_sdks(self, releaser, resource_version, *args, **kwargs):
+    def _check_resource_version_exists(self, fetcher, version):
+        resource_versions = fetcher.list_resource_versions(version=str(version))
+        return resource_versions["count"] != 0
+
+    def _generate_sdks(self, releaser, version, *args, **kwargs):
         try:
-            releaser.generate_sdks(resource_version=resource_version["version"])
+            releaser.generate_sdks(resource_version=version)
         except Exception as err:
             print("warning!! generate sdks failed: %s" % err)
 
     def handle(self, stage, title, comment, generate_sdks, *args, **kwargs):
         configuration = self.get_configuration(**kwargs)
         definition = self.get_definition(**kwargs)
-        defined_version = self.get_version_from_definition(definition)
-        fixed_defined_version = self.fix_defined_version(defined_version)
+        defined_version = self._parse_version_from_definition(definition)
+        fixed_defined_version = self._fix_defined_version(defined_version)
 
         fetcher = self.Fetcher(configuration)
         resource_version = fetcher.latest_resource_version()
-        latest_version = self.get_version_from_resource_version(resource_version)
+        latest_version = self._parse_version_from_resource_version(resource_version)
 
         releaser = self.Releaser(configuration)
         manager = self.ResourceSignatureManager()
         api_name = configuration.api_name
 
-        if self.should_create_resource_version(manager, api_name, fixed_defined_version, latest_version):
-            resource_version = self.create_resource_version(
+        # 如何判断是否需要创建新版本？
+        # 1. 使用配置中的版本号与线上最新版本进行比较，如果版本 public 部分不一致，则需要创建新版本
+        # 2. 如果配置中的版本号与线上最新版本 public 部分一致，为了避免开发者忘记更新版本号的情况，获取同步结果进行判断：
+        #    - 如果有资源变更，则需要创建新版本
+        if self._should_create_resource_version(manager, api_name, fixed_defined_version, latest_version):
+            exists = self._check_resource_version_exists(fetcher, fixed_defined_version)
+            resource_version = self._create_resource_version(
                 releaser=releaser,
-                version=self.get_version_to_be_created(fixed_defined_version, latest_version),
+                version=self._get_version_to_be_created(fixed_defined_version, exists),
                 title=title or definition.get("title", ""),
                 comment=comment or definition.get("comment", ""),
             )
             manager.reset_dirty(api_name)
 
         else:
             generate_sdks = False
-            print("resource_version %s already exists and is the latest, skip creating" % latest_version)
+            print("resource_version %s already exists, skip creating" % latest_version)
 
         result = releaser.release(
-            version=resource_version.get("version", ""),
-            resource_version_name=resource_version["name"],
+            version=resource_version["version"],
             title=title or resource_version.get("title", ""),
             comment=comment or resource_version.get("comment", ""),
             stage_names=stage,
         )
         print(
             "API gateway released %s, title %s, stages %s"
             % (result.get("version"), result["resource_version_title"], result["stage_names"])
         )
 
         # create a sdk when released a new version
         if generate_sdks:
-            self.generate_sdks(
+            self._generate_sdks(
                 releaser=releaser,
-                resource_version=resource_version,
+                version=resource_version["version"],
                 *args,
                 **kwargs,
             )
```

## apigw_manager/core/fetch.py

```diff
@@ -20,7 +20,11 @@
         result = self._call_with_cache(self.client.api.get_apigw_public_key, *args, **kwargs)
         return self._parse_result(result, itemgetter("data"))
 
     def latest_resource_version(self, *args, **kwargs):
         """Get the latest resource version"""
         result = self._call(self.client.api.get_latest_resource_version, *args, **kwargs)
         return self._parse_result(result, itemgetter("data"))
+
+    def list_resource_versions(self, *args, **kwargs):
+        result = self._call(self.client.api.list_resource_versions, *args, **kwargs)
+        return self._parse_result(result, itemgetter("data"))
```

## apigw_manager/core/sync.py

```diff
@@ -21,18 +21,14 @@
         result = self._call(self.client.api.sync_api, *args, **kwargs)
         return self._parse_result(result, itemgetter("data"))
 
     def sync_stage_config(self, *args, **kwargs):
         result = self._call(self.client.api.sync_stage, *args, **kwargs)
         return self._parse_result(result, itemgetter("data"))
 
-    def sync_access_strategies(self, *args, **kwargs):
-        result = self._call(self.client.api.sync_access_strategy, *args, **kwargs)
-        return self._parse_result(result, itemgetter("data"))
-
     def sync_resources_config(self, content, *args, **kwargs):
         kwargs["content"] = yaml.dump(dict(content))
 
         result = self._call(self.client.api.sync_resources, *args, **kwargs)
         return self._parse_result(result, itemgetter("data"))
 
     def sync_resource_docs_by_archive(self, *args, **kwargs):
```

## Comparing `apigw_manager-1.1.7.dist-info/METADATA` & `apigw_manager-1.2.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: apigw-manager
-Version: 1.1.7
+Version: 1.2.0
 Summary: 
 Requires-Python: >=3.6.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: cryptography
 Provides-Extra: demo
 Provides-Extra: django
 Provides-Extra: kubernetes
-Requires-Dist: Django (>=1.11.1) ; extra == "django" or extra == "demo"
-Requires-Dist: PyMySQL (>=1.0.2,<2.0.0) ; extra == "demo"
-Requires-Dist: bkapi-bk-apigateway (>=1.0.6,<2.0.0)
+Requires-Dist: Django (>=1.11.1); extra == "django" or extra == "demo"
+Requires-Dist: PyMySQL (>=1.0.2,<2.0.0); extra == "demo"
+Requires-Dist: bkapi-bk-apigateway (>=1.0.11,<2.0.0)
 Requires-Dist: bkapi-client-core (>=1.1.3)
-Requires-Dist: cryptography (>=3.1.1) ; extra == "cryptography"
-Requires-Dist: django-environ (>=0.8.1) ; extra == "demo"
+Requires-Dist: cryptography (>=3.1.1); extra == "cryptography"
+Requires-Dist: django-environ (>=0.8.1); extra == "demo"
 Requires-Dist: future (==0.18.2)
-Requires-Dist: kubernetes ; extra == "kubernetes"
+Requires-Dist: kubernetes; extra == "kubernetes"
 Requires-Dist: packaging (>=21.0)
-Requires-Dist: pyjwt (>=1.6.4) ; extra == "cryptography" or extra == "django" or extra == "demo"
+Requires-Dist: pyjwt (>=1.6.4); extra == "cryptography" or extra == "django" or extra == "demo"
 Requires-Dist: pyyaml (>=5.4.1)
 Requires-Dist: setuptools (>=21.0.0)
 Requires-Dist: urllib3 (>=1.25.3)
```

## Comparing `apigw_manager-1.1.7.dist-info/RECORD` & `apigw_manager-1.2.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -6,34 +6,33 @@
 apigw_manager/apigw/command.py,sha256=rVEgwmjsWhw2JNAKgA7ug10LOO8aV55YMfCo5--cfMY,3311
 apigw_manager/apigw/decorators.py,sha256=MeubyQInAMjklMhSRiffiD0JCER45zh3C6WfJbIg3Bo,1566
 apigw_manager/apigw/helper.py,sha256=lS33XgRfSHjsMrf2G0Fdtl0y7T3PZe4S3JaxI8AVg-E,6415
 apigw_manager/apigw/k8s_helper.py,sha256=PMRte9_svojZnDK9xgXdC5ZXHWRuklswEYVyUi4HwTQ,2075
 apigw_manager/apigw/management/__init__.py,sha256=IrhSBTIdq4nO5gGCVXRwR4rWptnjS6X0iGe53LVHp8g,760
 apigw_manager/apigw/management/commands/__init__.py,sha256=IrhSBTIdq4nO5gGCVXRwR4rWptnjS6X0iGe53LVHp8g,760
 apigw_manager/apigw/management/commands/apply_apigw_permissions.py,sha256=1So9fYO_8TEu4jTX9cvSw16ETyE11I_6Jp--9NyPIqk,1640
-apigw_manager/apigw/management/commands/create_version_and_release_apigw.py,sha256=HNqt0v75WFMNBrXPMNvQafdjBy2JZplq75r6EprJrSU,6086
+apigw_manager/apigw/management/commands/create_version_and_release_apigw.py,sha256=JHoAvF3VifpeOWmjVsv5lVZnWsyIgdAEODFj1jcDDHA,6185
 apigw_manager/apigw/management/commands/fetch_apigw_public_key.py,sha256=1_-2A7PB3ZoONmB9_QaZEcAtaC61d82IotNNNSD0XQU,1965
 apigw_manager/apigw/management/commands/fetch_esb_public_key.py,sha256=qKt_k8SDrTuIr6OgT6yuG8e2KoOOqywP1WUMV8gtqxI,1116
 apigw_manager/apigw/management/commands/grant_apigw_permissions.py,sha256=HpMhVUjewtnCiaoN2DqMHQBrAOuvoPb8vRajh5TAkCo,1664
 apigw_manager/apigw/management/commands/sync_apigw_config.py,sha256=lU0fTJl_tvRwp_uovYcriTTJxoZGKgo5s4zG3_XxRss,1598
 apigw_manager/apigw/management/commands/sync_apigw_resources.py,sha256=49LI43U7HoxmrscuitBQJMrWKssPgeFFC299GQ9rYE8,2401
 apigw_manager/apigw/management/commands/sync_apigw_stage.py,sha256=ql9O_u3PcMvWVgSILSVRIULVgq1vVeuXGedAmXaUBas,1153
-apigw_manager/apigw/management/commands/sync_apigw_strategies.py,sha256=E3mP_pPJ4S4nPxLM9JTQemvIip_e9LXR7hG7BnE4vug,1891
 apigw_manager/apigw/management/commands/sync_resource_docs_by_archive.py,sha256=V1ZG43A4LqjH42LlT59ySiY-ROjz-ojLkKTlFqSabU8,2393
 apigw_manager/apigw/migrations/0001_initial.py,sha256=6EJOCcS4jYBgROzmkDKQKIQyo4ZBay11RZuK3bBC7U8,1915
 apigw_manager/apigw/migrations/__init__.py,sha256=IrhSBTIdq4nO5gGCVXRwR4rWptnjS6X0iGe53LVHp8g,760
 apigw_manager/apigw/models.py,sha256=Eu8udmsrxXV1obEoy9gTtFeNV2RZdOnG48Wcri3BX7s,1270
 apigw_manager/apigw/providers.py,sha256=EbpNpXcqTS7fRXa2VxA7fmOMy3wDWbxeeTl6xS6YbP0,6602
 apigw_manager/apigw/utils.py,sha256=vP8gPnV_s71MeBy3QGTtdBNrOoVpYA_PDyZ-YN1agKM,3907
 apigw_manager/apigw/views.py,sha256=IrhSBTIdq4nO5gGCVXRwR4rWptnjS6X0iGe53LVHp8g,760
 apigw_manager/core/__init__.py,sha256=IrhSBTIdq4nO5gGCVXRwR4rWptnjS6X0iGe53LVHp8g,760
 apigw_manager/core/configuration.py,sha256=UTIRuoSxx6H2HG4mLIMNtcY282r0N4RkU-POfUIGMVQ,1390
 apigw_manager/core/exceptions.py,sha256=mKGaLRrdqHGuf3iAOizSqOvTr-pnybq9RHaUAe2weBk,1441
-apigw_manager/core/fetch.py,sha256=CgJUBT5J3kjmBx_dmmcYRjica2Kn2eG_2w0wXUaGqtk,1441
+apigw_manager/core/fetch.py,sha256=3SabZhCMh7F5DlC_SJkDHrJVAR6mhHLekO8z-gMV3zc,1643
 apigw_manager/core/handler.py,sha256=lYxhfBaJ_fQOKRrREOyWqcqRDTP5Hyc1G0DRh_OtTyU,4321
 apigw_manager/core/permission.py,sha256=RGvGbL60WZ9I0mzXnTHoEmUwP3AKlwysOV-nipdN0rk,1415
 apigw_manager/core/release.py,sha256=zu17zfYegBFx3MEpt2GjsSWEKvHd0B63IYplqtycGOc,1576
-apigw_manager/core/sync.py,sha256=bnpaq6_OeKkcal3AVap8HECMx9PPRTBEhKJbgnF0i-U,1994
+apigw_manager/core/sync.py,sha256=iTmPDmBS_s-wIB5t94Lk-cpapqC-yayWQgK9xY1cpno,1793
 apigw_manager/core/utils.py,sha256=Em36ItO907rdziRYJizl540P-09aAXeprOSow60mCxc,1096
-apigw_manager-1.1.7.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-apigw_manager-1.1.7.dist-info/METADATA,sha256=_8DnfyeJih31q1syOR9Lw29OfNdFksNAsAWXplz3mdk,1163
-apigw_manager-1.1.7.dist-info/RECORD,,
+apigw_manager-1.2.0.dist-info/WHEEL,sha256=DA86_h4QwwzGeRoz62o1svYt5kGEXpoUTuTtwzoTb30,83
+apigw_manager-1.2.0.dist-info/METADATA,sha256=QQluyhcwi_ltwSGpNhYkykELOQ5rez3ivK8wlZJVCbM,1107
+apigw_manager-1.2.0.dist-info/RECORD,,
```

