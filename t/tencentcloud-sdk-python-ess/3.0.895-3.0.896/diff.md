# Comparing `tmp/tencentcloud-sdk-python-ess-3.0.895.tar.gz` & `tmp/tencentcloud-sdk-python-ess-3.0.896.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.895.tar", last modified: Fri May 19 02:50:52 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ess-3.0.896.tar", last modified: Mon May 22 00:23:00 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ess-3.0.895.tar` & `tencentcloud-sdk-python-ess-3.0.896.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/tencentcloud/ess/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)    50642 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    23727 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   222756 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/tencentcloud/ess/v20201111/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/tencentcloud_sdk_python_ess.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/tencentcloud_sdk_python_ess.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:50:52.000000 tencentcloud-sdk-python-ess-3.0.895/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)    50900 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    23727 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   223240 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud_sdk_python_ess.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud_sdk_python_ess.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud_sdk_python_ess.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud_sdk_python_ess.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/tencentcloud_sdk_python_ess.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:23:00.000000 tencentcloud-sdk-python-ess-3.0.896/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ess-3.0.895/README.rst` & `tencentcloud-sdk-python-ess-3.0.896/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.895/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ess-3.0.896/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ess-3.0.895/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/ess_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -345,15 +345,18 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreateFlowSignUrl(self, request):
-        """创建集成页面签署链接，请联系客户经理申请使用
+        """创建个人H5签署链接，请联系客户经理申请使用 <br/>
+        该接口用于发起合同后，生成C端签署人的签署链接 <br/>
+        注意：该接口目前签署人类型仅支持个人签署方（PERSON） <br/>
+        注意：该接口可生成签署链接的C端签署人必须仅有手写签名和时间类型的签署控件<br/>
 
         :param request: Request instance for CreateFlowSignUrl.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreateFlowSignUrlRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreateFlowSignUrlResponse`
 
         """
         try:
@@ -470,15 +473,15 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def CreatePreparedPersonalEsign(self, request):
-        """本接口（CreatePreparedPersonalEsign）用于创建导入个人印章（处方单场景专用，在开通个人自动签之后调用，使用此接口请与客户经理确认）。
+        """本接口（CreatePreparedPersonalEsign）用于创建导入个人印章（处方单场景专用，使用此接口请与客户经理确认）。
 
         :param request: Request instance for CreatePreparedPersonalEsign.
         :type request: :class:`tencentcloud.ess.v20201111.models.CreatePreparedPersonalEsignRequest`
         :rtype: :class:`tencentcloud.ess.v20201111.models.CreatePreparedPersonalEsignResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-ess-3.0.895/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ess-3.0.895/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-ess-3.0.896/tencentcloud/ess/v20201111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2056,15 +2056,15 @@
         :param IdCardType: 身份证件类型:
 ID_CARD 身份证
 PASSPORT 护照
 HONGKONG_AND_MACAO 中国香港
 FOREIGN_ID_CARD 境外身份
 HONGKONG_MACAO_AND_TAIWAN 中国台湾
         :type IdCardType: str
-        :param Mobile: 手机号码
+        :param Mobile: 手机号码；当需要开通自动签时，该参数必传
         :type Mobile: str
         :param EnableAutoSign: 是否开通自动签，该功能需联系运营工作人员开通后使用
         :type EnableAutoSign: bool
         """
         self.UserName = None
         self.IdCardNumber = None
         self.SealImage = None
@@ -3621,25 +3621,33 @@
 class DescribeUserAutoSignStatusResponse(AbstractModel):
     """DescribeUserAutoSignStatus返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param IsOpen: 是否开通
+        :param IsOpen: 是否已开通自动签
         :type IsOpen: bool
+        :param LicenseFrom: 自动签许可生效时间。当且仅当已开通自动签时有值。
+        :type LicenseFrom: int
+        :param LicenseTo: 自动签许可到期时间。当且仅当已开通自动签时有值。
+        :type LicenseTo: int
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self.IsOpen = None
+        self.LicenseFrom = None
+        self.LicenseTo = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
         self.IsOpen = params.get("IsOpen")
+        self.LicenseFrom = params.get("LicenseFrom")
+        self.LicenseTo = params.get("LicenseTo")
         self.RequestId = params.get("RequestId")
 
 
 class DisableUserAutoSignRequest(AbstractModel):
     """DisableUserAutoSign请求参数结构体
 
     """
```

### Comparing `tencentcloud-sdk-python-ess-3.0.895/tencentcloud_sdk_python_ess.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.896/tencentcloud_sdk_python_ess.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.895/PKG-INFO` & `tencentcloud-sdk-python-ess-3.0.896/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ess
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Ess SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ess-3.0.895/setup.py` & `tencentcloud-sdk-python-ess-3.0.896/setup.py`

 * *Files identical despite different names*

