# Comparing `tmp/tencentcloud-sdk-python-lcic-3.0.895.tar.gz` & `tmp/tencentcloud-sdk-python-lcic-3.0.896.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.895.tar", last modified: Fri May 19 02:54:20 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lcic-3.0.896.tar", last modified: Mon May 22 00:26:32 2023, max compression
```

## Comparing `tencentcloud-sdk-python-lcic-3.0.895.tar` & `tencentcloud-sdk-python-lcic-3.0.896.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/tencentcloud/lcic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/tencentcloud/lcic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)     4414 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)   141851 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)    48649 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/tencentcloud/lcic/v20220817/lcic_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/tencentcloud_sdk_python_lcic.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:54:20.000000 tencentcloud-sdk-python-lcic-3.0.895/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/tencentcloud/lcic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/tencentcloud/lcic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)     4414 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142076 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)    48649 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/tencentcloud/lcic/v20220817/lcic_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/tencentcloud_sdk_python_lcic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/tencentcloud_sdk_python_lcic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/tencentcloud_sdk_python_lcic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/tencentcloud_sdk_python_lcic.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:26:32.000000 tencentcloud-sdk-python-lcic-3.0.896/setup.cfg
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.895/README.rst` & `tencentcloud-sdk-python-lcic-3.0.896/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.895/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-lcic-3.0.896/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.895/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-lcic-3.0.896/tencentcloud/lcic/v20220817/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -950,17 +950,17 @@
 0 不自动连麦（需要手动申请上麦，默认值）
 1 自动连麦
         :type AutoMic: int
         :param TurnOffMic: 释放音视频权限后是否自动取消连麦。可以有以下取值：
 0 自动取消连麦（默认值）
 1 保持连麦状态
         :type TurnOffMic: int
-        :param AudioQuality: 高音质模式。可以有以下取值：
-0 不开启高音质（默认值）
-1 开启高音质
+        :param AudioQuality: 声音音质。可以有以下取值：
+0：流畅模式（默认值），占用更小的带宽、拥有更好的降噪效果，适用于1对1、小班教学、多人音视频会议等场景。
+1：高音质模式，适合需要高保真传输音乐的场景，但降噪效果会被削弱，适用于音乐教学场景。
         :type AudioQuality: int
         :param DisableRecord: 上课后是否禁止自动录制。可以有以下取值：
 0 不禁止录制（自动开启录制，默认值）
 1 禁止录制
 注：如果该配置取值为0，录制将从上课后开始，课堂结束后停止。
         :type DisableRecord: int
         :param Assistants: 助教Id列表。通过[注册用户]接口获取的UserId。指定后该用户在房间内拥有助教权限。
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.895/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-lcic-3.0.896/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lcic-3.0.895/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lcic-3.0.896/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lcic-3.0.895/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.896/tencentcloud_sdk_python_lcic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.895/PKG-INFO` & `tencentcloud-sdk-python-lcic-3.0.896/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lcic
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Lcic SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lcic-3.0.895/setup.py` & `tencentcloud-sdk-python-lcic-3.0.896/setup.py`

 * *Files identical despite different names*

