# Comparing `tmp/tencentcloud-sdk-python-essbasic-3.0.895.tar.gz` & `tmp/tencentcloud-sdk-python-essbasic-3.0.896.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.895.tar", last modified: Fri May 19 02:50:59 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-essbasic-3.0.896.tar", last modified: Mon May 22 00:23:06 2023, max compression
```

## Comparing `tencentcloud-sdk-python-essbasic-3.0.895.tar` & `tencentcloud-sdk-python-essbasic-3.0.896.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud_sdk_python_essbasic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      678 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      752 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)    15673 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    50895 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   230804 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)     5392 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    53845 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171664 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     1684 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1016 2023-05-19 02:50:58.000000 tencentcloud-sdk-python-essbasic-3.0.895/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:50:59.000000 tencentcloud-sdk-python-essbasic-3.0.895/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud_sdk_python_essbasic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud_sdk_python_essbasic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      678 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud_sdk_python_essbasic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      752 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)    15673 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    50877 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   230804 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    53845 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171664 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1016 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:23:06.000000 tencentcloud-sdk-python-essbasic-3.0.896/setup.cfg
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud_sdk_python_essbasic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud_sdk_python_essbasic.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.895/README.rst` & `tencentcloud-sdk-python-essbasic-3.0.896/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/__init__.py` & `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,18 +299,18 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def ChannelCreateFlowSignUrl(self, request):
-        """创建签署链接，请联系客户经理申请使用
-        该接口用于发起合同后，生成C端签署人的签署链接，点击跳转小程序完成签署
-        注意：该接口目前签署人类型仅支持个人签署方（PERSON）
-        注意：该接口可生成签署链接的C端签署人必须仅有手写签名和时间类型的签署控件
+        """创建个人H5签署链接，请联系客户经理申请使用<br/>
+        该接口用于发起合同后，生成C端签署人的签署链接<br/>
+        注意：该接口目前签署人类型仅支持个人签署方（PERSON）<br/>
+        注意：该接口可生成签署链接的C端签署人必须仅有手写签名和时间类型的签署控件<br/>
 
         :param request: Request instance for ChannelCreateFlowSignUrl.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateFlowSignUrlRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.ChannelCreateFlowSignUrlResponse`
 
         """
         try:
@@ -688,15 +688,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateFlowsByTemplates(self, request):
-        """接口（CreateFlowsByTemplates）用于使用多个模板批量创建签署流程。当前可批量发起合同（签署流程）数量最大为20个。
+        """接口（CreateFlowsByTemplates）用于使用模板批量创建签署流程。当前可批量发起合同（签署流程）数量为1-20个。
         如若在模板中配置了动态表格, 上传的附件必须为A4大小
         合同发起人必须在电子签已经进行实名。
 
         :param request: Request instance for CreateFlowsByTemplates.
         :type request: :class:`tencentcloud.essbasic.v20210526.models.CreateFlowsByTemplatesRequest`
         :rtype: :class:`tencentcloud.essbasic.v20210526.models.CreateFlowsByTemplatesResponse`
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20210526/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.895/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-essbasic-3.0.896/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-essbasic-3.0.895/PKG-INFO` & `tencentcloud-sdk-python-essbasic-3.0.896/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-essbasic
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Essbasic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-essbasic-3.0.895/setup.py` & `tencentcloud-sdk-python-essbasic-3.0.896/setup.py`

 * *Files identical despite different names*

