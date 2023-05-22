# Comparing `tmp/tencentcloud-sdk-python-sqlserver-3.0.895.tar.gz` & `tmp/tencentcloud-sdk-python-sqlserver-3.0.896.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.895.tar", last modified: Fri May 19 02:59:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sqlserver-3.0.896.tar", last modified: Mon May 22 00:31:15 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sqlserver-3.0.895.tar` & `tencentcloud-sdk-python-sqlserver-3.0.896.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/
--rw-r--r--   0 root         (0) root         (0)      755 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud/sqlserver/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud/sqlserver/v20180328/
--rw-r--r--   0 root         (0) root         (0)   104570 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud/sqlserver/v20180328/sqlserver_client.py
--rw-r--r--   0 root         (0) root         (0)     9568 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud/sqlserver/v20180328/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud/sqlserver/v20180328/__init__.py
--rw-r--r--   0 root         (0) root         (0)   335623 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud/sqlserver/v20180328/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud/sqlserver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud_sdk_python_sqlserver.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      505 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1018 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:59:04.000000 tencentcloud-sdk-python-sqlserver-3.0.895/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/
+-rw-r--r--   0 root         (0) root         (0)      755 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud/sqlserver/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud/sqlserver/v20180328/
+-rw-r--r--   0 root         (0) root         (0)   106575 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud/sqlserver/v20180328/sqlserver_client.py
+-rw-r--r--   0 root         (0) root         (0)     9568 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud/sqlserver/v20180328/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud/sqlserver/v20180328/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   349080 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud/sqlserver/v20180328/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud/sqlserver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud_sdk_python_sqlserver.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud_sdk_python_sqlserver.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      505 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud_sdk_python_sqlserver.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud_sdk_python_sqlserver.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:31:15.000000 tencentcloud-sdk-python-sqlserver-3.0.896/setup.cfg
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.895/README.rst` & `tencentcloud-sdk-python-sqlserver-3.0.896/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud/sqlserver/v20180328/sqlserver_client.py` & `tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud/sqlserver/v20180328/sqlserver_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,14 +275,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def CreateCloudDBInstances(self, request):
+        """本接口（CreateCloudDBInstances）用于创建高可用实例(虚拟机版本)。
+
+        :param request: Request instance for CreateCloudDBInstances.
+        :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateCloudDBInstancesRequest`
+        :rtype: :class:`tencentcloud.sqlserver.v20180328.models.CreateCloudDBInstancesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateCloudDBInstances", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateCloudDBInstancesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
+    def CreateCloudReadOnlyDBInstances(self, request):
+        """本接口（CreateCloudReadOnlyDBInstances）用于添加只读副本实例(虚拟机版本)。
+
+        :param request: Request instance for CreateCloudReadOnlyDBInstances.
+        :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateCloudReadOnlyDBInstancesRequest`
+        :rtype: :class:`tencentcloud.sqlserver.v20180328.models.CreateCloudReadOnlyDBInstancesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateCloudReadOnlyDBInstances", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateCloudReadOnlyDBInstancesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def CreateDB(self, request):
         """本接口（CreateDB）用于创建数据库。
 
         :param request: Request instance for CreateDB.
         :type request: :class:`tencentcloud.sqlserver.v20180328.models.CreateDBRequest`
         :rtype: :class:`tencentcloud.sqlserver.v20180328.models.CreateDBResponse`
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud/sqlserver/v20180328/errorcodes.py` & `tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud/sqlserver/v20180328/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud/sqlserver/v20180328/models.py` & `tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud/sqlserver/v20180328/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1234,14 +1234,294 @@
 
 
     def _deserialize(self, params):
         self.FileTaskId = params.get("FileTaskId")
         self.RequestId = params.get("RequestId")
 
 
+class CreateCloudDBInstancesRequest(AbstractModel):
+    """CreateCloudDBInstances请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Zone: 实例可用区，类似ap-guangzhou-1（广州一区）；实例可售卖区域可以通过接口DescribeZones获取
+        :type Zone: str
+        :param Memory: 实例内存大小，单位GB
+        :type Memory: int
+        :param Storage: 实例磁盘大小，单位GB
+        :type Storage: int
+        :param Cpu: 实例核心数
+        :type Cpu: int
+        :param MachineType: 购买实例的宿主机磁盘类型,CLOUD_HSSD-虚拟机加强型SSD云盘，CLOUD_TSSD-虚拟机极速型SSD云盘，CLOUD_BSSD-虚拟机通用型SSD云盘
+        :type MachineType: str
+        :param InstanceChargeType: 付费模式，取值支持 PREPAID（预付费），POSTPAID（后付费）。
+        :type InstanceChargeType: str
+        :param ProjectId: 项目ID
+        :type ProjectId: int
+        :param GoodsNum: 本次购买几个实例，默认值为1。取值不超过10
+        :type GoodsNum: int
+        :param SubnetId: VPC子网ID，形如subnet-bdoe83fa；SubnetId和VpcId需同时设置或者同时不设置
+        :type SubnetId: str
+        :param VpcId: VPC网络ID，形如vpc-dsp338hz；SubnetId和VpcId需同时设置或者同时不设置
+        :type VpcId: str
+        :param Period: 购买实例周期，默认取值为1，表示一个月。取值不超过48
+        :type Period: int
+        :param AutoVoucher: 是否自动使用代金券；1 - 是，0 - 否，默认不使用
+        :type AutoVoucher: int
+        :param VoucherIds: 代金券ID数组，目前单个订单只能使用一张
+        :type VoucherIds: list of str
+        :param DBVersion: sqlserver版本，目前所有支持的版本有：2008R2 (SQL Server 2008 R2 Enterprise)，2012SP3 (SQL Server 2012 Enterprise)，201202 (SQL Server 2012 Standard)，2014SP2 (SQL Server 2014 Enterprise)，201402 (SQL Server 2014 Standard)，2016SP1 (SQL Server 2016 Enterprise)，201602 (SQL Server 2016 Standard)，2017 (SQL Server 2017 Enterprise)，201702 (SQL Server 2017 Standard)，2019 (SQL Server 2019 Enterprise)，201902 (SQL Server 2019 Standard)。每个地域支持售卖的版本不同，可通过DescribeProductConfig接口来拉取每个地域可售卖的版本信息。不填，默认为版本2008R2。
+        :type DBVersion: str
+        :param AutoRenewFlag: 自动续费标志：0-正常续费  1-自动续费，默认为1自动续费。只在购买预付费实例时有效。
+        :type AutoRenewFlag: int
+        :param SecurityGroupList: 安全组列表，填写形如sg-xxx的安全组ID
+        :type SecurityGroupList: list of str
+        :param Weekly: 可维护时间窗配置，以周为单位，表示周几允许维护，1-7分别代表周一到周末
+        :type Weekly: list of int
+        :param StartTime: 可维护时间窗配置，每天可维护的开始时间
+        :type StartTime: str
+        :param Span: 可维护时间窗配置，持续时间，单位：小时
+        :type Span: int
+        :param MultiZones: 是否跨可用区部署，默认值为false
+        :type MultiZones: bool
+        :param ResourceTags: 新建实例绑定的标签集合
+        :type ResourceTags: list of ResourceTag
+        :param Collation: 系统字符集排序规则，默认：Chinese_PRC_CI_AS
+        :type Collation: str
+        :param TimeZone: 系统时区，默认：China Standard Time
+        :type TimeZone: str
+        """
+        self.Zone = None
+        self.Memory = None
+        self.Storage = None
+        self.Cpu = None
+        self.MachineType = None
+        self.InstanceChargeType = None
+        self.ProjectId = None
+        self.GoodsNum = None
+        self.SubnetId = None
+        self.VpcId = None
+        self.Period = None
+        self.AutoVoucher = None
+        self.VoucherIds = None
+        self.DBVersion = None
+        self.AutoRenewFlag = None
+        self.SecurityGroupList = None
+        self.Weekly = None
+        self.StartTime = None
+        self.Span = None
+        self.MultiZones = None
+        self.ResourceTags = None
+        self.Collation = None
+        self.TimeZone = None
+
+
+    def _deserialize(self, params):
+        self.Zone = params.get("Zone")
+        self.Memory = params.get("Memory")
+        self.Storage = params.get("Storage")
+        self.Cpu = params.get("Cpu")
+        self.MachineType = params.get("MachineType")
+        self.InstanceChargeType = params.get("InstanceChargeType")
+        self.ProjectId = params.get("ProjectId")
+        self.GoodsNum = params.get("GoodsNum")
+        self.SubnetId = params.get("SubnetId")
+        self.VpcId = params.get("VpcId")
+        self.Period = params.get("Period")
+        self.AutoVoucher = params.get("AutoVoucher")
+        self.VoucherIds = params.get("VoucherIds")
+        self.DBVersion = params.get("DBVersion")
+        self.AutoRenewFlag = params.get("AutoRenewFlag")
+        self.SecurityGroupList = params.get("SecurityGroupList")
+        self.Weekly = params.get("Weekly")
+        self.StartTime = params.get("StartTime")
+        self.Span = params.get("Span")
+        self.MultiZones = params.get("MultiZones")
+        if params.get("ResourceTags") is not None:
+            self.ResourceTags = []
+            for item in params.get("ResourceTags"):
+                obj = ResourceTag()
+                obj._deserialize(item)
+                self.ResourceTags.append(obj)
+        self.Collation = params.get("Collation")
+        self.TimeZone = params.get("TimeZone")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateCloudDBInstancesResponse(AbstractModel):
+    """CreateCloudDBInstances返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DealName: 订单名称
+        :type DealName: str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DealName = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.DealName = params.get("DealName")
+        self.RequestId = params.get("RequestId")
+
+
+class CreateCloudReadOnlyDBInstancesRequest(AbstractModel):
+    """CreateCloudReadOnlyDBInstances请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 主实例ID，格式如：mssql-3l3fgqn7
+        :type InstanceId: str
+        :param Zone: 实例可用区，类似ap-guangzhou-1（广州一区）；实例可售卖区域可以通过接口DescribeZones获取
+        :type Zone: str
+        :param ReadOnlyGroupType: 只读组类型选项，1-按照一个实例一个只读组的方式发货，2-新建只读组后发货，所有实例都在这个只读组下面， 3-发货的所有实例都在已有的只读组下面
+        :type ReadOnlyGroupType: int
+        :param Memory: 实例内存大小，单位GB
+        :type Memory: int
+        :param Storage: 实例磁盘大小，单位GB
+        :type Storage: int
+        :param Cpu: 实例核心数
+        :type Cpu: int
+        :param MachineType: 购买实例的宿主机磁盘类型,CLOUD_HSSD-虚拟机加强型SSD云盘，CLOUD_TSSD-虚拟机极速型SSD云盘，CLOUD_BSSD-虚拟机通用型SSD云盘
+        :type MachineType: str
+        :param ReadOnlyGroupForcedUpgrade: 0-默认不升级主实例，1-强制升级主实例完成ro部署；主实例为非集群版时需要填1，强制升级为集群版。填1 说明您已同意将主实例升级到集群版实例。
+        :type ReadOnlyGroupForcedUpgrade: int
+        :param ReadOnlyGroupId: ReadOnlyGroupType=3时必填,已存在的只读组ID
+        :type ReadOnlyGroupId: str
+        :param ReadOnlyGroupName: ReadOnlyGroupType=2时必填，新建的只读组名称
+        :type ReadOnlyGroupName: str
+        :param ReadOnlyGroupIsOfflineDelay: ReadOnlyGroupType=2时必填，新建的只读组是否开启延迟剔除功能，1-开启，0-关闭。当只读副本与主实例延迟大于阈值后，自动剔除。
+        :type ReadOnlyGroupIsOfflineDelay: int
+        :param ReadOnlyGroupMaxDelayTime: ReadOnlyGroupType=2 且 ReadOnlyGroupIsOfflineDelay=1时必填，新建的只读组延迟剔除的阈值。
+        :type ReadOnlyGroupMaxDelayTime: int
+        :param ReadOnlyGroupMinInGroup: ReadOnlyGroupType=2 且 ReadOnlyGroupIsOfflineDelay=1时必填，新建的只读组延迟剔除后至少保留只读副本的个数。
+        :type ReadOnlyGroupMinInGroup: int
+        :param InstanceChargeType: 付费模式，取值支持 PREPAID（预付费），POSTPAID（后付费）。
+        :type InstanceChargeType: str
+        :param GoodsNum: 本次购买几个只读实例，默认值为1。
+        :type GoodsNum: int
+        :param SubnetId: VPC子网ID，形如subnet-bdoe83fa；SubnetId和VpcId需同时设置或者同时不设置
+        :type SubnetId: str
+        :param VpcId: VPC网络ID，形如vpc-dsp338hz；SubnetId和VpcId需同时设置或者同时不设置
+        :type VpcId: str
+        :param Period: 购买实例周期，默认取值为1，表示一个月。取值不超过48
+        :type Period: int
+        :param SecurityGroupList: 安全组列表，填写形如sg-xxx的安全组ID
+        :type SecurityGroupList: list of str
+        :param AutoVoucher: 是否自动使用代金券；1 - 是，0 - 否，默认不使用
+        :type AutoVoucher: int
+        :param VoucherIds: 代金券ID数组，目前单个订单只能使用一张
+        :type VoucherIds: list of str
+        :param ResourceTags: 新建实例绑定的标签集合
+        :type ResourceTags: list of ResourceTag
+        :param Collation: 系统字符集排序规则，默认：Chinese_PRC_CI_AS
+        :type Collation: str
+        :param TimeZone: 系统时区，默认：China Standard Time
+        :type TimeZone: str
+        """
+        self.InstanceId = None
+        self.Zone = None
+        self.ReadOnlyGroupType = None
+        self.Memory = None
+        self.Storage = None
+        self.Cpu = None
+        self.MachineType = None
+        self.ReadOnlyGroupForcedUpgrade = None
+        self.ReadOnlyGroupId = None
+        self.ReadOnlyGroupName = None
+        self.ReadOnlyGroupIsOfflineDelay = None
+        self.ReadOnlyGroupMaxDelayTime = None
+        self.ReadOnlyGroupMinInGroup = None
+        self.InstanceChargeType = None
+        self.GoodsNum = None
+        self.SubnetId = None
+        self.VpcId = None
+        self.Period = None
+        self.SecurityGroupList = None
+        self.AutoVoucher = None
+        self.VoucherIds = None
+        self.ResourceTags = None
+        self.Collation = None
+        self.TimeZone = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.Zone = params.get("Zone")
+        self.ReadOnlyGroupType = params.get("ReadOnlyGroupType")
+        self.Memory = params.get("Memory")
+        self.Storage = params.get("Storage")
+        self.Cpu = params.get("Cpu")
+        self.MachineType = params.get("MachineType")
+        self.ReadOnlyGroupForcedUpgrade = params.get("ReadOnlyGroupForcedUpgrade")
+        self.ReadOnlyGroupId = params.get("ReadOnlyGroupId")
+        self.ReadOnlyGroupName = params.get("ReadOnlyGroupName")
+        self.ReadOnlyGroupIsOfflineDelay = params.get("ReadOnlyGroupIsOfflineDelay")
+        self.ReadOnlyGroupMaxDelayTime = params.get("ReadOnlyGroupMaxDelayTime")
+        self.ReadOnlyGroupMinInGroup = params.get("ReadOnlyGroupMinInGroup")
+        self.InstanceChargeType = params.get("InstanceChargeType")
+        self.GoodsNum = params.get("GoodsNum")
+        self.SubnetId = params.get("SubnetId")
+        self.VpcId = params.get("VpcId")
+        self.Period = params.get("Period")
+        self.SecurityGroupList = params.get("SecurityGroupList")
+        self.AutoVoucher = params.get("AutoVoucher")
+        self.VoucherIds = params.get("VoucherIds")
+        if params.get("ResourceTags") is not None:
+            self.ResourceTags = []
+            for item in params.get("ResourceTags"):
+                obj = ResourceTag()
+                obj._deserialize(item)
+                self.ResourceTags.append(obj)
+        self.Collation = params.get("Collation")
+        self.TimeZone = params.get("TimeZone")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateCloudReadOnlyDBInstancesResponse(AbstractModel):
+    """CreateCloudReadOnlyDBInstances返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param DealNames: 订单名称数组
+        :type DealNames: list of str
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.DealNames = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.DealNames = params.get("DealNames")
+        self.RequestId = params.get("RequestId")
+
+
 class CreateDBInstancesRequest(AbstractModel):
     """CreateDBInstances请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.895/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.896/tencentcloud_sdk_python_sqlserver.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.895/PKG-INFO` & `tencentcloud-sdk-python-sqlserver-3.0.896/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sqlserver
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Sqlserver SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sqlserver-3.0.895/setup.py` & `tencentcloud-sdk-python-sqlserver-3.0.896/setup.py`

 * *Files identical despite different names*

