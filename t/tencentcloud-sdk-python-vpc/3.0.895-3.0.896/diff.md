# Comparing `tmp/tencentcloud-sdk-python-vpc-3.0.895.tar.gz` & `tmp/tencentcloud-sdk-python-vpc-3.0.896.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.895.tar", last modified: Fri May 19 03:05:19 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vpc-3.0.896.tar", last modified: Mon May 22 00:37:21 2023, max compression
```

## Comparing `tencentcloud-sdk-python-vpc-3.0.895.tar` & `tencentcloud-sdk-python-vpc-3.0.896.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud_sdk_python_vpc.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)   332171 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/vpc_client.py
--rw-r--r--   0 root         (0) root         (0)    41601 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   851263 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 03:05:19.000000 tencentcloud-sdk-python-vpc-3.0.895/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud_sdk_python_vpc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud_sdk_python_vpc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud_sdk_python_vpc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud_sdk_python_vpc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)   332171 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/vpc_client.py
+-rw-r--r--   0 root         (0) root         (0)    41601 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   851287 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:37:21.000000 tencentcloud-sdk-python-vpc-3.0.896/setup.cfg
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.895/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.896/tencentcloud_sdk_python_vpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.895/README.rst` & `tencentcloud-sdk-python-vpc-3.0.896/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/vpc/v20170312/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1071,15 +1071,15 @@
         r"""
         :param NetworkInterfaceId: 弹性网卡实例ID，例如：eni-m6dyj72l。
         :type NetworkInterfaceId: str
         :param PrivateIpAddresses: 指定的内网IP信息，单次最多指定10个。与SecondaryPrivateIpAddressCount至少提供一个。
         :type PrivateIpAddresses: list of PrivateIpAddressSpecification
         :param SecondaryPrivateIpAddressCount: 新申请的内网IP地址个数，与PrivateIpAddresses至少提供一个。内网IP地址个数总和不能超过配额数，详见<a href="/document/product/576/18527">弹性网卡使用限制</a>。
         :type SecondaryPrivateIpAddressCount: int
-        :param QosLevel: IP服务质量等级，和SecondaryPrivateIpAddressCount配合使用，可选值：PT、AU、AG、DEFAULT，分别代表白金、金、银、默认四个等级。
+        :param QosLevel: IP服务质量等级，和SecondaryPrivateIpAddressCount配合使用，可选值：PT、AU、AG、DEFAULT，分别代表云金、云银、云铜、默认四个等级。
         :type QosLevel: str
         """
         self.NetworkInterfaceId = None
         self.PrivateIpAddresses = None
         self.SecondaryPrivateIpAddressCount = None
         self.QosLevel = None
 
@@ -2942,15 +2942,15 @@
         :type SubnetId: str
         :param InstanceId: 云服务器实例ID。
         :type InstanceId: str
         :param PrivateIpAddresses: 指定的内网IP信息，单次最多指定10个。
         :type PrivateIpAddresses: list of PrivateIpAddressSpecification
         :param SecondaryPrivateIpAddressCount: 新申请的内网IP地址个数，内网IP地址个数总和不能超过配额数。
         :type SecondaryPrivateIpAddressCount: int
-        :param QosLevel: IP服务质量等级，和SecondaryPrivateIpAddressCount配合使用，可选值：PT、AU、AG、DEFAULT，分别代表白金、金、银、默认四个等级。
+        :param QosLevel: IP服务质量等级，和SecondaryPrivateIpAddressCount配合使用，可选值：PT、AU、AG、DEFAULT，分别代表云金、云银、云铜、默认四个等级。
         :type QosLevel: str
         :param SecurityGroupIds: 指定绑定的安全组，例如：['sg-1dd51d']。
         :type SecurityGroupIds: list of str
         :param NetworkInterfaceDescription: 弹性网卡描述，可任意命名，但不得超过60个字符。
         :type NetworkInterfaceDescription: str
         :param Tags: 指定绑定的标签列表，例如：[{"Key": "city", "Value": "shanghai"}]。
         :type Tags: list of Tag
@@ -4264,15 +4264,15 @@
         :type NetworkInterfaceName: str
         :param SubnetId: 弹性网卡所在的子网实例ID，例如：subnet-0ap8nwca。
         :type SubnetId: str
         :param NetworkInterfaceDescription: 弹性网卡描述，可任意命名，但不得超过60个字符。
         :type NetworkInterfaceDescription: str
         :param SecondaryPrivateIpAddressCount: 新申请的内网IP地址个数，内网IP地址个数总和不能超过配额数。
         :type SecondaryPrivateIpAddressCount: int
-        :param QosLevel: IP服务质量等级，和SecondaryPrivateIpAddressCount配合使用，可选值：PT、AU、AG、DEFAULT，分别代表白金、金、银、默认四个等级。
+        :param QosLevel: IP服务质量等级，和SecondaryPrivateIpAddressCount配合使用，可选值：PT、AU、AG、DEFAULT，分别代表云金、云银、云铜、默认四个等级。
         :type QosLevel: str
         :param SecurityGroupIds: 指定绑定的安全组，例如：['sg-1dd51d']。
         :type SecurityGroupIds: list of str
         :param PrivateIpAddresses: 指定的内网IP信息，单次最多指定10个。
         :type PrivateIpAddresses: list of PrivateIpAddressSpecification
         :param Tags: 指定绑定的标签列表，例如：[{"Key": "city", "Value": "shanghai"}]
         :type Tags: list of Tag
@@ -18020,15 +18020,15 @@
 
     """
 
     def __init__(self):
         r"""
         :param NetworkInterfaceIds: 弹性网卡ID，支持批量修改。
         :type NetworkInterfaceIds: list of str
-        :param QosLevel: 服务质量，可选值：PT、AU、AG、DEFAULT，分别代表白金、金、银、默认四个等级。
+        :param QosLevel: 服务质量，可选值：PT、AU、AG、DEFAULT，分别代表云金、云银、云铜、默认四个等级。
         :type QosLevel: str
         :param DirectSendMaxPort: DirectSend端口范围最大值。
         :type DirectSendMaxPort: int
         """
         self.NetworkInterfaceIds = None
         self.QosLevel = None
         self.DirectSendMaxPort = None
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.895/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vpc-3.0.896/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-vpc-3.0.895/PKG-INFO` & `tencentcloud-sdk-python-vpc-3.0.896/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vpc
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Vpc SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vpc-3.0.895/setup.py` & `tencentcloud-sdk-python-vpc-3.0.896/setup.py`

 * *Files identical despite different names*

