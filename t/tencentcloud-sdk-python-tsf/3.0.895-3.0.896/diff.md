# Comparing `tmp/tencentcloud-sdk-python-tsf-3.0.895.tar.gz` & `tmp/tencentcloud-sdk-python-tsf-3.0.896.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.895.tar", last modified: Fri May 19 03:04:28 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tsf-3.0.896.tar", last modified: Mon May 22 00:36:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tsf-3.0.895.tar` & `tencentcloud-sdk-python-tsf-3.0.896.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/tencentcloud/tsf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/tencentcloud/tsf/v20180326/
--rw-r--r--   0 root         (0) root         (0)    49851 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/tencentcloud/tsf/v20180326/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   195353 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/tencentcloud/tsf/v20180326/tsf_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/tencentcloud/tsf/v20180326/__init__.py
--rw-r--r--   0 root         (0) root         (0)   801873 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/tencentcloud/tsf/v20180326/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/tencentcloud/tsf/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/tencentcloud_sdk_python_tsf.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 03:04:28.000000 tencentcloud-sdk-python-tsf-3.0.895/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/tencentcloud/tsf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/tencentcloud/tsf/v20180326/
+-rw-r--r--   0 root         (0) root         (0)    49851 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/tencentcloud/tsf/v20180326/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   195353 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/tencentcloud/tsf/v20180326/tsf_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/tencentcloud/tsf/v20180326/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   802528 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/tencentcloud/tsf/v20180326/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/tencentcloud/tsf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/tencentcloud_sdk_python_tsf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/tencentcloud_sdk_python_tsf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/tencentcloud_sdk_python_tsf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/tencentcloud_sdk_python_tsf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:36:31.000000 tencentcloud-sdk-python-tsf-3.0.896/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.895/README.rst` & `tencentcloud-sdk-python-tsf-3.0.896/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.895/tencentcloud/tsf/v20180326/errorcodes.py` & `tencentcloud-sdk-python-tsf-3.0.896/tencentcloud/tsf/v20180326/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.895/tencentcloud/tsf/v20180326/tsf_client.py` & `tencentcloud-sdk-python-tsf-3.0.896/tencentcloud/tsf/v20180326/tsf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tsf-3.0.895/tencentcloud/tsf/v20180326/models.py` & `tencentcloud-sdk-python-tsf-3.0.896/tencentcloud/tsf/v20180326/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -22106,24 +22106,36 @@
         :type Priority: int
         :param Description: 规则描述
 注意：此字段可能返回 null，表示取不到有效值。
         :type Description: str
         :param UnitRuleTagList: 规则标签列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type UnitRuleTagList: list of UnitRuleTag
+        :param ItemIndex: 项目id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ItemIndex: int
+        :param CreatedTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreatedTime: str
+        :param UpdatedTime: 修改时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpdatedTime: str
         """
         self.Relationship = None
         self.DestNamespaceId = None
         self.DestNamespaceName = None
         self.Name = None
         self.Id = None
         self.UnitRuleId = None
         self.Priority = None
         self.Description = None
         self.UnitRuleTagList = None
+        self.ItemIndex = None
+        self.CreatedTime = None
+        self.UpdatedTime = None
 
 
     def _deserialize(self, params):
         self.Relationship = params.get("Relationship")
         self.DestNamespaceId = params.get("DestNamespaceId")
         self.DestNamespaceName = params.get("DestNamespaceName")
         self.Name = params.get("Name")
@@ -22133,14 +22145,17 @@
         self.Description = params.get("Description")
         if params.get("UnitRuleTagList") is not None:
             self.UnitRuleTagList = []
             for item in params.get("UnitRuleTagList"):
                 obj = UnitRuleTag()
                 obj._deserialize(item)
                 self.UnitRuleTagList.append(obj)
+        self.ItemIndex = params.get("ItemIndex")
+        self.CreatedTime = params.get("CreatedTime")
+        self.UpdatedTime = params.get("UpdatedTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.895/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tsf-3.0.896/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tsf-3.0.895/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.896/tencentcloud_sdk_python_tsf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.895/PKG-INFO` & `tencentcloud-sdk-python-tsf-3.0.896/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tsf
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Tsf SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tsf-3.0.895/setup.py` & `tencentcloud-sdk-python-tsf-3.0.896/setup.py`

 * *Files identical despite different names*

