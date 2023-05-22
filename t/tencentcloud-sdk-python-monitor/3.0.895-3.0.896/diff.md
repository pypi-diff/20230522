# Comparing `tmp/tencentcloud-sdk-python-monitor-3.0.895.tar.gz` & `tmp/tencentcloud-sdk-python-monitor-3.0.896.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.895.tar", last modified: Fri May 19 02:55:37 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-monitor-3.0.896.tar", last modified: Mon May 22 00:27:57 2023, max compression
```

## Comparing `tencentcloud-sdk-python-monitor-3.0.895.tar` & `tencentcloud-sdk-python-monitor-3.0.896.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/
--rw-r--r--   0 root         (0) root         (0)      749 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/tencentcloud/monitor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/tencentcloud/monitor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/tencentcloud/monitor/v20180724/
--rw-r--r--   0 root         (0) root         (0)    10348 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/tencentcloud/monitor/v20180724/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   144635 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/tencentcloud/monitor/v20180724/monitor_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/tencentcloud/monitor/v20180724/__init__.py
--rw-r--r--   0 root         (0) root         (0)   552994 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/tencentcloud/monitor/v20180724/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/tencentcloud_sdk_python_monitor.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      485 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1679 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1014 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-19 02:55:37.000000 tencentcloud-sdk-python-monitor-3.0.895/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/
+-rw-r--r--   0 root         (0) root         (0)      749 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/tencentcloud/monitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/tencentcloud/monitor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/tencentcloud/monitor/v20180724/
+-rw-r--r--   0 root         (0) root         (0)    10348 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/tencentcloud/monitor/v20180724/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   144635 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/tencentcloud/monitor/v20180724/monitor_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/tencentcloud/monitor/v20180724/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   553846 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/tencentcloud/monitor/v20180724/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/tencentcloud_sdk_python_monitor.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/tencentcloud_sdk_python_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      485 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/tencentcloud_sdk_python_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1679 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/tencentcloud_sdk_python_monitor.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-05-22 00:27:57.000000 tencentcloud-sdk-python-monitor-3.0.896/setup.cfg
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.895/README.rst` & `tencentcloud-sdk-python-monitor-3.0.896/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.895/tencentcloud/monitor/v20180724/errorcodes.py` & `tencentcloud-sdk-python-monitor-3.0.896/tencentcloud/monitor/v20180724/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.895/tencentcloud/monitor/v20180724/monitor_client.py` & `tencentcloud-sdk-python-monitor-3.0.896/tencentcloud/monitor/v20180724/monitor_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-monitor-3.0.895/tencentcloud/monitor/v20180724/models.py` & `tencentcloud-sdk-python-monitor-3.0.896/tencentcloud/monitor/v20180724/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1360,21 +1360,21 @@
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class ConditionsTemp(AbstractModel):
-    """告警条件模版
+    """告警条件模板
 
     """
 
     def __init__(self):
         r"""
-        :param TemplateName: 模版名称
+        :param TemplateName: 模板名称
 注意：此字段可能返回 null，表示取不到有效值。
         :type TemplateName: str
         :param Condition: 指标触发条件
 注意：此字段可能返回 null，表示取不到有效值。
         :type Condition: :class:`tencentcloud.monitor.v20180724.models.AlarmPolicyCondition`
         :param EventCondition: 事件触发条件
 注意：此字段可能返回 null，表示取不到有效值。
@@ -4309,26 +4309,29 @@
         :type UserIds: list of int
         :param GroupIds: 接收组列表
         :type GroupIds: list of int
         :param NoticeIds: 根据通知模板 id 过滤，空数组/不传则不过滤
         :type NoticeIds: list of str
         :param Tags: 模板根据标签过滤
         :type Tags: list of Tag
+        :param OnCallFormIDs: 值班列表
+        :type OnCallFormIDs: list of str
         """
         self.Module = None
         self.PageNumber = None
         self.PageSize = None
         self.Order = None
         self.OwnerUid = None
         self.Name = None
         self.ReceiverType = None
         self.UserIds = None
         self.GroupIds = None
         self.NoticeIds = None
         self.Tags = None
+        self.OnCallFormIDs = None
 
 
     def _deserialize(self, params):
         self.Module = params.get("Module")
         self.PageNumber = params.get("PageNumber")
         self.PageSize = params.get("PageSize")
         self.Order = params.get("Order")
@@ -4340,14 +4343,15 @@
         self.NoticeIds = params.get("NoticeIds")
         if params.get("Tags") is not None:
             self.Tags = []
             for item in params.get("Tags"):
                 obj = Tag()
                 obj._deserialize(item)
                 self.Tags.append(obj)
+        self.OnCallFormIDs = params.get("OnCallFormIDs")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -4420,15 +4424,15 @@
         :param Field: 排序字段，例如按照最后修改时间排序，Field: "UpdateTime"
         :type Field: str
         :param Order: 排序顺序：升序：ASC  降序：DESC
         :type Order: str
         :param ProjectIds: 策略所属项目的id数组，可在此页面查看
 [项目管理](https://console.cloud.tencent.com/project)
         :type ProjectIds: list of int
-        :param NoticeIds: 通知模版的id列表，可查询通知模版列表获取。
+        :param NoticeIds: 通知模板的id列表，可查询通知模板列表获取。
 可使用 [查询通知模板列表](https://cloud.tencent.com/document/product/248/51280) 接口查询。
         :type NoticeIds: list of str
         :param RuleTypes: 根据触发条件筛选 不传展示全部策略 STATIC=展示静态阈值策略 DYNAMIC=展示动态阈值策略
         :type RuleTypes: list of str
         :param Enable: 告警启停筛选，[1]：启用   [0]：停止，全部[0, 1]
         :type Enable: list of int
         :param NotBindingNoticeRule: 传 1 查询未配置通知规则的告警策略；不传或传其他数值，查询所有策略。
@@ -4437,20 +4441,24 @@
         :type InstanceGroupId: int
         :param NeedCorrespondence: 是否需要策略与入参过滤维度参数的对应关系，1：是  0：否，默认为0
         :type NeedCorrespondence: int
         :param TriggerTasks: 按照触发任务（例如弹性伸缩）过滤策略。最多10个
         :type TriggerTasks: list of AlarmPolicyTriggerTask
         :param OneClickPolicyType: 根据一键告警策略筛选 不传展示全部策略 ONECLICK=展示一键告警策略 NOT_ONECLICK=展示非一键告警策略
         :type OneClickPolicyType: list of str
-        :param NotBindAll: 根据全部对象过滤，1代表需要过滤掉全部对象，0则无需过滤
+        :param NotBindAll: 返回结果过滤掉绑定全部对象的策略，1代表需要过滤，0则无需过滤
         :type NotBindAll: int
-        :param NotInstanceGroup: 根据实例对象过滤，1代表需要过滤掉有实例对象，0则无需过滤
+        :param NotInstanceGroup: 返回结果过滤掉关联实例为实例分组的策略，1代表需要过滤，0则无需过滤
         :type NotInstanceGroup: int
         :param Tags: 策略根据标签过滤
         :type Tags: list of Tag
+        :param PromInsId: prom实例id，自定义指标策略时会用到
+        :type PromInsId: str
+        :param ReceiverOnCallFormIDs: 根据排班表搜索
+        :type ReceiverOnCallFormIDs: list of str
         """
         self.Module = None
         self.PageNumber = None
         self.PageSize = None
         self.PolicyName = None
         self.MonitorTypes = None
         self.Namespaces = None
@@ -4468,14 +4476,16 @@
         self.InstanceGroupId = None
         self.NeedCorrespondence = None
         self.TriggerTasks = None
         self.OneClickPolicyType = None
         self.NotBindAll = None
         self.NotInstanceGroup = None
         self.Tags = None
+        self.PromInsId = None
+        self.ReceiverOnCallFormIDs = None
 
 
     def _deserialize(self, params):
         self.Module = params.get("Module")
         self.PageNumber = params.get("PageNumber")
         self.PageSize = params.get("PageSize")
         self.PolicyName = params.get("PolicyName")
@@ -4505,14 +4515,16 @@
         self.NotInstanceGroup = params.get("NotInstanceGroup")
         if params.get("Tags") is not None:
             self.Tags = []
             for item in params.get("Tags"):
                 obj = Tag()
                 obj._deserialize(item)
                 self.Tags.append(obj)
+        self.PromInsId = params.get("PromInsId")
+        self.ReceiverOnCallFormIDs = params.get("ReceiverOnCallFormIDs")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -15982,28 +15994,32 @@
         :type NeedPhoneArriveNotice: int
         :param PhoneCallType: 电话拨打类型 SYNC=同时拨打 CIRCLE=轮询拨打 不指定时默认是轮询
 注意：此字段可能返回 null，表示取不到有效值。
         :type PhoneCallType: str
         :param Weekday: 通知周期 1-7表示周一到周日
 注意：此字段可能返回 null，表示取不到有效值。
         :type Weekday: list of int
+        :param OnCallFormIDs: 值班表id列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OnCallFormIDs: list of str
         """
         self.ReceiverType = None
         self.StartTime = None
         self.EndTime = None
         self.NoticeWay = None
         self.UserIds = None
         self.GroupIds = None
         self.PhoneOrder = None
         self.PhoneCircleTimes = None
         self.PhoneInnerInterval = None
         self.PhoneCircleInterval = None
         self.NeedPhoneArriveNotice = None
         self.PhoneCallType = None
         self.Weekday = None
+        self.OnCallFormIDs = None
 
 
     def _deserialize(self, params):
         self.ReceiverType = params.get("ReceiverType")
         self.StartTime = params.get("StartTime")
         self.EndTime = params.get("EndTime")
         self.NoticeWay = params.get("NoticeWay")
@@ -16012,14 +16028,15 @@
         self.PhoneOrder = params.get("PhoneOrder")
         self.PhoneCircleTimes = params.get("PhoneCircleTimes")
         self.PhoneInnerInterval = params.get("PhoneInnerInterval")
         self.PhoneCircleInterval = params.get("PhoneCircleInterval")
         self.NeedPhoneArriveNotice = params.get("NeedPhoneArriveNotice")
         self.PhoneCallType = params.get("PhoneCallType")
         self.Weekday = params.get("Weekday")
+        self.OnCallFormIDs = params.get("OnCallFormIDs")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.895/tencentcloud/__init__.py` & `tencentcloud-sdk-python-monitor-3.0.896/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-monitor-3.0.895/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.896/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.895/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO` & `tencentcloud-sdk-python-monitor-3.0.896/tencentcloud_sdk_python_monitor.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-monitor
-Version: 3.0.895
+Version: 3.0.896
 Summary: Tencent Cloud Monitor SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-monitor-3.0.895/setup.py` & `tencentcloud-sdk-python-monitor-3.0.896/setup.py`

 * *Files identical despite different names*

