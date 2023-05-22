# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.895.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.896.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.895.tar", last modified: Fri May 19 02:44:55 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.896.tar", last modified: Mon May 22 00:17:10 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.895.tar` & `tencentcloud-sdk-python-cdb-3.0.896.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   151870 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)    18943 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)   529193 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:44:55.000000 tencentcloud-sdk-python-cdb-3.0.895/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/tencentcloud/cdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   150608 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)    18943 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   526122 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/tencentcloud/cdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:17:10.000000 tencentcloud-sdk-python-cdb-3.0.896/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.895/README.rst` & `tencentcloud-sdk-python-cdb-3.0.896/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.896/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1080,41 +1080,14 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
-    def DescribeBackupTables(self, request):
-        """该接口已废弃，需要下线
-
-        本接口(DescribeBackupTables)用于查询指定的数据库的备份数据表名 (已废弃)。
-        旧版本支持全量备份后，用户如果分库表下载逻辑备份文件，需要用到此接口。
-        新版本支持(CreateBackup)创建逻辑备份的时候，直接发起指定库表备份，用户直接下载该备份文件即可。
-
-        :param request: Request instance for DescribeBackupTables.
-        :type request: :class:`tencentcloud.cdb.v20170320.models.DescribeBackupTablesRequest`
-        :rtype: :class:`tencentcloud.cdb.v20170320.models.DescribeBackupTablesResponse`
-
-        """
-        try:
-            params = request._serialize()
-            headers = request.headers
-            body = self.call("DescribeBackupTables", params, headers=headers)
-            response = json.loads(body)
-            model = models.DescribeBackupTablesResponse()
-            model._deserialize(response["Response"])
-            return model
-        except Exception as e:
-            if isinstance(e, TencentCloudSDKException):
-                raise
-            else:
-                raise TencentCloudSDKException(e.message, e.message)
-
-
     def DescribeBackups(self, request):
         """本接口(DescribeBackups)用于查询云数据库实例的备份数据。
 
         :param request: Request instance for DescribeBackups.
         :type request: :class:`tencentcloud.cdb.v20170320.models.DescribeBackupsRequest`
         :rtype: :class:`tencentcloud.cdb.v20170320.models.DescribeBackupsResponse`
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.896/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.896/tencentcloud/cdb/v20170320/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4827,88 +4827,14 @@
                 obj = BackupSummaryItem()
                 obj._deserialize(item)
                 self.Items.append(obj)
         self.TotalCount = params.get("TotalCount")
         self.RequestId = params.get("RequestId")
 
 
-class DescribeBackupTablesRequest(AbstractModel):
-    """DescribeBackupTables请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param InstanceId: 实例ID，格式如：cdb-c1nl9rpv。与云数据库控制台页面中显示的实例ID相同。
-        :type InstanceId: str
-        :param StartTime: 开始时间，格式为：2017-07-12 10:29:20。
-        :type StartTime: str
-        :param DatabaseName: 指定的数据库名。
-        :type DatabaseName: str
-        :param SearchTable: 要查询的数据表名前缀。
-        :type SearchTable: str
-        :param Offset: 分页偏移。
-        :type Offset: int
-        :param Limit: 分页大小，最小值为1，最大值为2000。
-        :type Limit: int
-        """
-        self.InstanceId = None
-        self.StartTime = None
-        self.DatabaseName = None
-        self.SearchTable = None
-        self.Offset = None
-        self.Limit = None
-
-
-    def _deserialize(self, params):
-        self.InstanceId = params.get("InstanceId")
-        self.StartTime = params.get("StartTime")
-        self.DatabaseName = params.get("DatabaseName")
-        self.SearchTable = params.get("SearchTable")
-        self.Offset = params.get("Offset")
-        self.Limit = params.get("Limit")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class DescribeBackupTablesResponse(AbstractModel):
-    """DescribeBackupTables返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param TotalCount: 返回的数据个数。
-        :type TotalCount: int
-        :param Items: 符合条件的数据表数组。
-        :type Items: list of TableName
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.TotalCount = None
-        self.Items = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.TotalCount = params.get("TotalCount")
-        if params.get("Items") is not None:
-            self.Items = []
-            for item in params.get("Items"):
-                obj = TableName()
-                obj._deserialize(item)
-                self.Items.append(obj)
-        self.RequestId = params.get("RequestId")
-
-
 class DescribeBackupsRequest(AbstractModel):
     """DescribeBackups请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -13837,38 +13763,14 @@
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.RequestId = params.get("RequestId")
 
 
-class TableName(AbstractModel):
-    """表名
-
-    """
-
-    def __init__(self):
-        r"""
-        :param TableName: 表名
-        :type TableName: str
-        """
-        self.TableName = None
-
-
-    def _deserialize(self, params):
-        self.TableName = params.get("TableName")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
 class TablePrivilege(AbstractModel):
     """数据库表权限
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.895/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.896/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.895'
+__version__ = '3.0.896'
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.895/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.896/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.895/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.896/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.895/setup.py` & `tencentcloud-sdk-python-cdb-3.0.896/setup.py`

 * *Files identical despite different names*

