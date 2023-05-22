# Comparing `tmp/tencentcloud-sdk-python-live-3.0.895.tar.gz` & `tmp/tencentcloud-sdk-python-live-3.0.896.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.895.tar", last modified: Fri May 19 02:54:31 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-live-3.0.896.tar", last modified: Mon May 22 00:26:45 2023, max compression
```

## Comparing `tencentcloud-sdk-python-live-3.0.895.tar` & `tencentcloud-sdk-python-live-3.0.896.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/tencentcloud_sdk_python_live.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/tencentcloud_sdk_python_live.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/tencentcloud_sdk_python_live.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/tencentcloud/live/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)   137459 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)    18117 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/tencentcloud/live/v20180801/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   431116 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/tencentcloud/live/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:54:31.000000 tencentcloud-sdk-python-live-3.0.895/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/tencentcloud_sdk_python_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/tencentcloud_sdk_python_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/tencentcloud_sdk_python_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/tencentcloud_sdk_python_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/tencentcloud_sdk_python_live.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/tencentcloud/live/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)   137459 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)    18117 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/tencentcloud/live/v20180801/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   431326 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/tencentcloud/live/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:26:45.000000 tencentcloud-sdk-python-live-3.0.896/setup.cfg
```

### Comparing `tencentcloud-sdk-python-live-3.0.895/tencentcloud_sdk_python_live.egg-info/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.896/tencentcloud_sdk_python_live.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.895/README.rst` & `tencentcloud-sdk-python-live-3.0.896/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.895/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-live-3.0.896/tencentcloud/live/v20180801/live_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.895/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-live-3.0.896/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-live-3.0.895/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-live-3.0.896/tencentcloud/live/v20180801/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8824,38 +8824,42 @@
         :param PornCensorshipNotifyUrl: 鉴黄回调 URL。
         :type PornCensorshipNotifyUrl: str
         :param CallbackKey: 回调 Key，回调 URL 公用，回调签名详见事件消息通知文档。
 [事件消息通知](/document/product/267/32744)。
         :type CallbackKey: str
         :param PushExceptionNotifyUrl: 推流异常回调 URL。
         :type PushExceptionNotifyUrl: str
+        :param AudioAuditNotifyUrl: 音频审核回调 URL。
+        :type AudioAuditNotifyUrl: str
         """
         self.TemplateId = None
         self.TemplateName = None
         self.Description = None
         self.StreamBeginNotifyUrl = None
         self.StreamEndNotifyUrl = None
         self.RecordNotifyUrl = None
         self.SnapshotNotifyUrl = None
         self.PornCensorshipNotifyUrl = None
         self.CallbackKey = None
         self.PushExceptionNotifyUrl = None
+        self.AudioAuditNotifyUrl = None
 
 
     def _deserialize(self, params):
         self.TemplateId = params.get("TemplateId")
         self.TemplateName = params.get("TemplateName")
         self.Description = params.get("Description")
         self.StreamBeginNotifyUrl = params.get("StreamBeginNotifyUrl")
         self.StreamEndNotifyUrl = params.get("StreamEndNotifyUrl")
         self.RecordNotifyUrl = params.get("RecordNotifyUrl")
         self.SnapshotNotifyUrl = params.get("SnapshotNotifyUrl")
         self.PornCensorshipNotifyUrl = params.get("PornCensorshipNotifyUrl")
         self.CallbackKey = params.get("CallbackKey")
         self.PushExceptionNotifyUrl = params.get("PushExceptionNotifyUrl")
+        self.AudioAuditNotifyUrl = params.get("AudioAuditNotifyUrl")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-live-3.0.895/tencentcloud/__init__.py` & `tencentcloud-sdk-python-live-3.0.896/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-live-3.0.895/PKG-INFO` & `tencentcloud-sdk-python-live-3.0.896/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-live
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Live SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-live-3.0.895/setup.py` & `tencentcloud-sdk-python-live-3.0.896/setup.py`

 * *Files identical despite different names*

