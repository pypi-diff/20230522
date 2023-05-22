# Comparing `tmp/singular_client-0.1.5.tar.gz` & `tmp/singular_client-0.1.6.tar.gz`

## Comparing `singular_client-0.1.5.tar` & `singular_client-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,18 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 singular_client-0.1.5/.DS_Store
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 singular_client-0.1.5/.python-version
--rw-r--r--   0        0        0    40764 2020-02-02 00:00:00.000000 singular_client-0.1.5/ALL Dimensions and Metrics.csv
--rw-r--r--   0        0        0    27890 2020-02-02 00:00:00.000000 singular_client-0.1.5/ALL Dimensions and Metrics.xlsx
--rw-r--r--   0        0        0    40690 2020-02-02 00:00:00.000000 singular_client-0.1.5/all_dimensions_and_metrics.csv
--rw-r--r--   0        0        0    99036 2020-02-02 00:00:00.000000 singular_client-0.1.5/copilot magic documents.png
--rw-r--r--   0        0        0    65639 2020-02-02 00:00:00.000000 singular_client-0.1.5/custom_fields.py
--rw-r--r--   0        0        0    66321 2020-02-02 00:00:00.000000 singular_client-0.1.5/dimensions_and_metrics.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 singular_client-0.1.5/test.json
--rw-r--r--   0        0        0    17741 2020-02-02 00:00:00.000000 singular_client-0.1.5/test_get_custom.pkl
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/__init__.py
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/_bases.py
--rw-r--r--   0        0        0    14536 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/_make_exceptions_module.py
--rw-r--r--   0        0        0   134011 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/_make_fields_module.py
--rw-r--r--   0        0        0     5873 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/api.py
--rwxr-xr-x   0        0        0    14480 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/arguments.py
--rw-r--r--   0        0        0     7433 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/documents.py
--rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/exceptions.py
--rw-r--r--   0        0        0    75071 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/fields.py
--rw-r--r--   0        0        0     4308 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/make_custom_fields_module.py
--rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/utils.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/endpoints/__init__.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/endpoints/governance.py
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/endpoints/links.py
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/endpoints/links_legacy.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/endpoints/monetization.py
--rw-r--r--   0        0        0     9800 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/endpoints/reporting.py
--rw-r--r--   0        0        0     4336 2020-02-02 00:00:00.000000 singular_client-0.1.5/singular_client/endpoints/skan.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 singular_client-0.1.5/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 singular_client-0.1.5/README.md
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 singular_client-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 singular_client-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/__init__.py
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/_bases.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/api.py
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/documents.py
+-rw-r--r--   0        0        0     5479 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/models.py
+-rw-r--r--   0        0        0     2111 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/utils.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/endpoints/__init__.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/endpoints/governance.py
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/endpoints/links.py
+-rw-r--r--   0        0        0     6207 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/endpoints/links_legacy.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/endpoints/monetization.py
+-rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/endpoints/reporting.py
+-rw-r--r--   0        0        0     4188 2020-02-02 00:00:00.000000 singular_client-0.1.6/singular_client/endpoints/skan.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 singular_client-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 singular_client-0.1.6/LICENSE
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 singular_client-0.1.6/README.md
+-rw-r--r--   0        0        0     1434 2020-02-02 00:00:00.000000 singular_client-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 singular_client-0.1.6/PKG-INFO
```

### Comparing `singular_client-0.1.5/singular_client/_bases.py` & `singular_client-0.1.6/singular_client/_bases.py`

 * *Files identical despite different names*

### Comparing `singular_client-0.1.5/singular_client/api.py` & `singular_client-0.1.6/singular_client/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 from __future__ import annotations
 import requests
+import os
 from typing import (
     Optional,
     Literal,
     TYPE_CHECKING,
 )
-import os
-
-from singular_client import TESTING
-from singular_client.documents import *
-from singular_client.arguments import *
 from singular_client._bases import ResponseSchema
 
 if TYPE_CHECKING:
     from singular_client.endpoints import *
 
 
 class SingularAPI:
@@ -24,22 +20,21 @@
     our request method and other endpoints, if needed.
 
     AUTHENTICATION
     --------------
     Passing a key is not necessary if an environment variable named `SINGULAR_API_KEY`
     can be found.
     """
+
     base_url = "https://api.singular.net/api/"
     logs = True
     key: str
 
     # Reporting
     combined_report: "CombinedReportEndpoint"
-    network_report: "NetworkReportEndpoint"
-    tracker_report: "TrackerReportEndpoint"
     data_availability: "DataAvailabilityEndpoint"
     report_status: "ReportStatusEndpoint"
     filters: "FiltersEndpoint"
     custom_dimensions: "CustomDimensionsEndpoint"
     cohort_metrics: "CohortMetricsEndpoint"
     conversion_metrics: "ConversionMetricsEndpoint"
     # SKAdNetwork
@@ -71,16 +66,14 @@
             assert key, "No API key provided"
 
         self.key = key
 
         from singular_client import endpoints
 
         self.combined_report = endpoints.CombinedReportEndpoint(self)
-        self.network_report = endpoints.NetworkReportEndpoint(self)
-        self.tracker_report = endpoints.TrackerReportEndpoint(self)
         self.data_availability = endpoints.DataAvailabilityEndpoint(self)
         self.report_status = endpoints.ReportStatusEndpoint(self)
         self.filters = endpoints.FiltersEndpoint(self)
         self.custom_dimensions = endpoints.CustomDimensionsEndpoint(self)
         self.cohort_metrics = endpoints.CohortMetricsEndpoint(self)
         self.conversion_metrics = endpoints.ConversionMetricsEndpoint(self)
         self.skan_raw_report = endpoints.SkanRawReportEndpoint(self)
```

### Comparing `singular_client-0.1.5/singular_client/documents.py` & `singular_client-0.1.6/singular_client/documents.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 """
 Data structures returned by Singular API.
 
 --------------------------------------------------------------------------------
-USED FOR STATIC TYPE CHECKING ONLY. Do not create instances of these classes.
+USED FOR STATIC TYPE CHECKING ONLY. These won't be instantiated.
 --------------------------------------------------------------------------------
 
 Endpoints are type-hinted using these classes as the structure of an individual
 document within a list of documents in a response. They serve two purposes:
 1. Easy access by the user for referencing the expected response data structure
 2. Static type checking. The user's IDE will bark at them or give red underline
    if they try to access an attribute from a response that is not present.
-
-Tip: Github Copilot will write these for you (including the class name) if you
-paste an example json from documentation into a comment block above the class.
 """
-from typing import TypedDict, List, Optional, Literal, Union, Dict
+from typing import (
+    TypedDict,
+    List,
+    Optional,
+    Literal,
+    Union,
+    Dict,
+)
 
 
 class NameDoc(TypedDict):
     display_name: str
     name: str
 
 
 class IDDoc(TypedDict):
     display_name: str
     id: str
 
 
-class NameDocValues(TypedDict):
+class NameValuesDoc(TypedDict):
     name: str
     display_name: str
     values: List[NameDoc]
 
 
 # Reporting API
 # ==============================================================================
@@ -164,15 +168,15 @@
     deferred_deeplink_enabled: bool
     reengagement_enabled: bool
     click_tracking_link: str
     impression_tracking_link: str
     created_utc: str
     updated_utc: str
     # `status` not included in Create Link response
-    status: str
+    status: Optional[str]
 
 
 class CustomLinkLegacyDoc(TypedDict, total=False):
     custom_source_name: str
     tracker_campaign_name: str
     ios_singular_app_id: int
     ios_app_longname: str
@@ -187,15 +191,15 @@
     other_destination_fallback_url: str
     click_tracking_link: str
     impression_tracking_link: str
     tracking_link_id: int
     created_utc: str
     updated_utc: str
     # `status` not included in Create Link response
-    status: str
+    status: Optional[str]
 
 
 # Ad Monetization API
 # ==============================================================================
 
 
 class AdMonetizationDoc(TypedDict):
@@ -205,74 +209,23 @@
     ad_requests: int
     ad_fill_rate: float
     ad_revenue: float
     source: str
     start_date: str
 
 
-# {
-#       "com.my.app": {
-#           "currency": ​"USD"​, 
-#           "keepalive_interval": ​24​, 
-#           "measurement_period": ​168​, 
-#           "start_ts": ​1601856000​, 
-#           "update_ts": ​1601856000​, 
-#           "version": ​5​, 
-#           "previous_version": ​4​, 
-#           "conversion_model": {
-#               "0": [ 
-#                   {
-#                       "conversion_name": ​"purchase",​ 
-#                       "conversion_type": ​"conversion_events"​, 
-#                       "partner_conversion_name": ​"Partner Purchase"​, 
-#                       "value": ​0
-#                   }, 
-#                   {
-#                       "conversion_name": ​"Add To Cart",​ 
-#                       "conversion_type": ​"conversion_events"​, 
-#                       "partner_conversion_name": ​"Partner Add to Cart"​, 
-#                       "value": ​0
-#                   }, 
-#                   {
-#                       "conversion_name": ​"retention"​, 
-#                       "conversion_type": ​"retention"​, 
-#                       "partner_conversion_name": ​"Partner App Open"​, 
-#                       "value": {"min": ​0​,"max": ​24}
-#                   } 
-#               ],
-#               "1": [ 
-#                   {
-#                       "conversion_name": ​"purchase",​ 
-#                       "conversion_type": ​"conversion_events"​, 
-#                       "partner_conversion_name": ​"Partner Purchase"​, 
-#                       "value": ​0
-#                   },
-
-class ConversionModel(TypedDict):
+class ConversionModelDoc(TypedDict):
     conversion_name: str
     conversion_type: str
     partner_conversion_name: str
     value: Union[int, Dict[str, int]]
 
-class AppConversionModel(TypedDict):
+
+class AppConversionModelDoc(TypedDict):
     currency: str
     keepalive_interval: int
     measurement_period: int
     start_ts: int
     update_ts: int
     version: int
     previous_version: int
-    conversion_model: Dict[str, List[ConversionModel]]
-
-
-
-
-
-
-
-
-
-
-
-
-
-
+    conversion_model: Dict[str, List[ConversionModelDoc]]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `singular_client-0.1.5/singular_client/endpoints/links.py` & `singular_client-0.1.6/singular_client/endpoints/links.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,22 @@
+from typing import (
+    List,
+    Optional,
+    Literal,
+)
 from singular_client._bases import _Endpoint, ResponseDocList
-from singular_client.documents import *
-from singular_client.arguments import *
-from typing import *
+from singular_client.documents import (
+    DomainDoc,
+    AppDoc,
+    PartnerDoc,
+    PartnerAppDoc,
+    CreateLinkDoc,
+    Redirection,
+    LinkDoc,
+)
 from singular_client.utils import _convert_list_arg
 
 
 class DomainsEndpoint(_Endpoint[ResponseDocList[DomainDoc]]):
     endpoint = "v1/singular_links/domains"
     data_path = ["available_domains"]
     res_type = ResponseDocList[DomainDoc]
@@ -103,15 +114,15 @@
 class ViewLinksEndpoint(_Endpoint[ResponseDocList[LinkDoc]]):
     endpoint = "v1/singular_links/links"
     data_path = []
     res_type = ResponseDocList[LinkDoc]
 
     def request(
         self,
-        link_type: Optional[LinkType] = None,
+        link_type: Optional[Literal["custom", "partner", "mobile_web_to_app"]] = None,
         partner_id: Optional[str] = None,
         app_id: Optional[str] = None,
         app_site_id: Optional[str] = None,
         tracking_link_id: Optional[str] = None,
     ):
         return super().request(
             link_type=link_type,
```

### Comparing `singular_client-0.1.5/singular_client/endpoints/links_legacy.py` & `singular_client-0.1.6/singular_client/endpoints/links_legacy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,16 @@
+from typing import Optional, List
 from singular_client._bases import _Endpoint, ResponseDocList
-from singular_client.documents import *
+from singular_client.documents import (
+    AppLegacyDoc,
+    PartnerLegacyDoc,
+    LinkLegacyDoc,
+    CustomLinkLegacyDoc,
+)
 from singular_client.utils import _convert_list_arg
-from typing import *
 
 
 class AppsLegacyEndpoint(_Endpoint[ResponseDocList[AppLegacyDoc]]):
     endpoint = "v1/links/discover_apps"
     data_path = ["available_apps"]
     res_type = ResponseDocList[AppLegacyDoc]
```

### Comparing `singular_client-0.1.5/singular_client/endpoints/monetization.py` & `singular_client-0.1.6/singular_client/endpoints/monetization.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,36 @@
+from typing import Optional, List, Union, Literal
 from singular_client._bases import _Endpoint, ResponseDocList
-from singular_client.documents import *
-from singular_client.arguments import *
-from typing import *
+from singular_client.documents import AdMonetizationDoc
 from singular_client.utils import _convert_list_arg
 
 
 class AdMonetizationEndpoint(_Endpoint[ResponseDocList[AdMonetizationDoc]]):
     endpoint = "v2.0/admonetization/reporting"
     data_path = ["value", "results"]
     res_type = ResponseDocList[AdMonetizationDoc]
 
     def request(
         self,
         start_date: str,
         end_date: Optional[str] = None,
-        time_breakdown: TimeBreakdown = "all",
-        dimensions: Optional[Union[List[AdMonDimension], str]] = None,
-        metrics: Optional[Union[List[AdMonMetric], str]] = None,
+        time_breakdown: Literal["day", "week", "month", "all"] = "all",
+        dimensions: Optional[Union[List[str], str]] = None,
+        metrics: Optional[Union[List[str], str]] = None,
         app: Optional[List[str]] = None,
         source: Optional[List[str]] = None,
         filters: Optional[List[dict]] = None,
-        format: FileFormat = "json",
-        country_code_format: CountryCodeFormat = "iso3",
+        format: Literal["json", "csv"] = "json",
+        country_code_format: Literal["iso3", "iso"] = "iso3",
     ):
         return super().request(
             start_date=start_date,
             end_date=end_date or start_date,
             time_breakdown=time_breakdown,
-            dimensions=_convert_list_arg(dimensions, AD_MON_DIMENSIONS),
-            metrics=_convert_list_arg(metrics, AD_MON_METRICS),
+            dimensions=_convert_list_arg(dimensions),
+            metrics=_convert_list_arg(metrics),
             app=_convert_list_arg(app),
             source=_convert_list_arg(source),
             filters=filters,
             format=format,
             country_code_format=country_code_format,
         )
```

### Comparing `singular_client-0.1.5/singular_client/endpoints/reporting.py` & `singular_client-0.1.6/singular_client/endpoints/reporting.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,62 +15,75 @@
 if status.failed:
     raise Exception("Report failed")
 data = status.read()
 ```
 
 https://support.singular.net/hc/en-us/articles/360045245692-Reporting-API-Reference?navigation_side_bar=true
 """
+from typing import (
+    TYPE_CHECKING,
+    Optional,
+    Union,
+    List,
+    Dict,
+    Literal,
+    cast,
+)
 from singular_client._bases import _Endpoint, ResponseDocList
-from singular_client.documents import *
-from singular_client.arguments import *
-from singular_client.fields import *
+from singular_client.documents import (
+    ReportStatusDoc,
+    NameValuesDoc,
+    CohortMetricsDoc,
+    IDDoc,
+    NameDoc,
+    DataConnectorDoc,
+)
 from singular_client.utils import _convert_list_arg
 import json
 import time
 import requests
 import io
-from typing import *
 
 if TYPE_CHECKING:
     from singular_client.api import SingularAPI
     import pandas as pd
 
 
 class ReportStatusResponse:
     """
     Returned by a check on the status of a report, through the ReportStatusEndpoint,
     or indirectly, through the CreateReportResponse object.
 
     Its boolean value is True if the report is done, OR if it has failed.
     """
+
     cached_download: Optional[Union[requests.Response, "pd.DataFrame"]]
     raw: ReportStatusDoc
-    failed = property(lambda x: x.status["status"] == "FAILED")
-    done = property(lambda x: x.status["status"] == "DONE")
-    queued = property(lambda x: x.status["status"] == "QUEUED")
-    started = property(lambda x: x.status["status"] == "STARTED")
-    url = property(lambda x: x.status["download_url"])
+    failed = property(lambda x: x.raw["status"] == "FAILED")
+    done = property(lambda x: x.raw["status"] == "DONE")
+    queued = property(lambda x: x.raw["status"] == "QUEUED")
+    started = property(lambda x: x.raw["status"] == "STARTED")
+    url = property(lambda x: x.raw["download_url"])
 
     def __init__(self, doc: dict):
         self.raw = cast(ReportStatusDoc, doc)
         self.cached_download = None
 
     def __bool__(self) -> bool:
         return self.done or self.failed
 
-    def read(self, no_cache: bool = False) -> Optional[Union[dict, "pd.DataFrame"]]:
+    def read(self, no_cache: bool = False) -> Union[dict, "pd.DataFrame"]:
         """
         Download from `status['download_url']`, and read the report without knowing
         whether it is a json or csv report.
         ---
         - If csv, pandas is required.
         - Downloaded response data is cached regardless of whether read errors are raised.
         """
-        if not self:
-            return None
+        assert self.done, "Report must be done to read it."
 
         if self.cached_download and not no_cache:
             res = self.cached_download
         else:
             res = requests.get(self.raw["download_url"])
             self.cached_download = res
         try:
@@ -90,37 +103,35 @@
 
     - Rate limited to 1 request per 10 seconds, per report.
 
     Returns a ReportStatusResponse object, whose boolean value indicates
     whether the report is ready. If True, the report can be downloaded with
     its `.read()` method.
     """
+
     endpoint = "v2.0/get_report_status"
     data_path = ["value"]
     res_type = ReportStatusResponse
     cacheable = False
     request_times: Dict[str, float] = {}
     returns_collection = False
     report_id: str
 
-    def request(self, report_id: str) -> Optional[ReportStatusResponse]:
+    def request(self, report_id: str) -> ReportStatusResponse:
         recent_time = self.request_times.get(report_id, 0)
         if time.time() - recent_time < 10:
-            print(
-                "Please wait at least 10 seconds between report status requests, per report"
-            )
-            return None
+            raise Exception("Rate limited to 1 request per 10 seconds, per report.")
         self.request_times[report_id] = time.time()
         return super().request(report_id=report_id)
 
 
-class FiltersEndpoint(_Endpoint[ResponseDocList[NameDocValues]]):
+class FiltersEndpoint(_Endpoint[ResponseDocList[NameValuesDoc]]):
     endpoint = "v2.0/reporting/filters"
     data_path = ["value", "dimensions"]
-    res_type = ResponseDocList[NameDocValues]
+    res_type = ResponseDocList[NameValuesDoc]
 
 
 class CohortMetricsEndpoint(_Endpoint[CohortMetricsDoc]):
     endpoint = "cohort_metrics"
     data_path = ["value"]
     res_type = CohortMetricsDoc
     returns_collection = False
@@ -142,58 +153,47 @@
     endpoint = "v2.0/data_availability_status"
     data_path = ["value", "data_connectors"]
     res_type = ResponseDocList[DataConnectorDoc]
 
     def request(
         self,
         data_date: str,
-        format: Literal['json', 'csv'] = 'json',
+        format: Literal["json", "csv"] = "json",
         expanded: bool = True,
         display_non_active_sources: bool = False,
     ):
         return super().request(
             format=format,
             data_date=data_date,
             expanded=expanded,
             display_non_active_sources=display_non_active_sources,
         )
 
 
-# ==============================================================================
-
-
 class CreateReportResponse(str):
     api: "SingularAPI"
     # Response gets cached whent the report has failed or completed,
     # so requests can no longer be sent after that.
     cached_status: Optional[ReportStatusResponse]
 
-    def check_status(
-        self, api: Optional["SingularAPI"] = None
-    ) -> Optional[ReportStatusResponse]:
+    def check_status(self, api: Optional["SingularAPI"] = None) -> ReportStatusResponse:
         if hasattr(self, "cached_status") and self.cached_status:
             return self.cached_status
 
         assert api or self.api, "An API must be provided"
         if not api:
             api = self.api
 
         status = api.report_status.request(str(self))
         if status:
             self.cached_status = status
         return status
 
 
-DimensionType = TypeVar("DimensionType")
-MetricType = TypeVar("MetricType")
-
-
-class _AggReportEndpoint(
-    Generic[DimensionType, MetricType], _Endpoint[CreateReportResponse]
-):
+class CombinedReportEndpoint(_Endpoint[CreateReportResponse]):
     """
     This subclass of _Endpoint solves the problem that Singular does not offer a way to
     control which type of data is returned by the 'Create Async Report' endpoint.
 
     The 'Create Async Report' endpoint offers 3 options for the types of data returned,
     but the only way to control which report is returned is by the dimensions and
     metrics provided.
@@ -207,70 +207,53 @@
 
     The user can easily override this type checking if they first join their list
     of columns as a comma-separated string.
     """
 
     endpoint = "v2.0/create_async_report"
     data_path = ["value", "report_id"]
-    available_dimensions: List
-    available_metrics: List
     res_type = CreateReportResponse
     returns_collection = False
     method = "POST"
 
     def request(
         self,
         start_date: str,
-        time_breakdown: TimeBreakdown = "all",
+        time_breakdown: Literal["day", "week", "month", "all"] = "all",
         end_date: Optional[str] = None,
-        dimensions: Optional[Union[List[DimensionType], str]] = None,
-        metrics: Optional[Union[List[MetricType], str]] = None,
+        dimensions: Optional[Union[List[str], str]] = None,
+        metrics: Optional[Union[List[str], str]] = None,
         custom_dimensions: Optional[List[str]] = None,
         cohort_metrics: Optional[List[str]] = None,
         cohort_periods: Optional[List[str]] = None,
         app: Optional[List[str]] = None,
         source: Optional[List[str]] = None,
         filters: Optional[List[dict]] = None,
-        format: FileFormat = "csv",
-        country_code_format: CountryCodeFormat = "iso3",
+        format: Literal["json", "csv"] = "csv",
+        country_code_format: Literal["iso3", "iso"] = "iso3",
         display_alignment: bool = False,
         display_unenriched: bool = False,
     ):
-        dimensions_str = _convert_list_arg(dimensions, self.available_dimensions)
+        dimensions_str = _convert_list_arg(dimensions)
         if custom_dimensions:
-            dimensions_str += _convert_list_arg(custom_dimensions)
+            dimensions_str += "," + _convert_list_arg(custom_dimensions)
         report_id = super().request(
             data=dict(
                 start_date=start_date,
                 end_date=end_date or start_date,
                 time_breakdown=time_breakdown,
                 dimensions=dimensions_str,
-                metrics=_convert_list_arg(metrics, self.available_metrics),
+                metrics=_convert_list_arg(metrics),
                 custom_dimensions=_convert_list_arg(custom_dimensions),
                 cohort_metrics=_convert_list_arg(cohort_metrics),
                 cohort_periods=_convert_list_arg(cohort_periods),
                 app=_convert_list_arg(app),
                 source=_convert_list_arg(source),
                 filters=filters,
                 format=format,
                 country_code_format=country_code_format,
                 display_alignment=display_alignment,
                 display_unenriched=display_unenriched,
             ),
         )
         report_id.api = self.api
         return report_id
-
-
-class CombinedReportEndpoint(_AggReportEndpoint[DimensionInGeneral, MetricInGeneral]):
-    available_dimensions = COMBINED_DIMENSIONS
-    available_metrics = COMBINED_METRICS
-
-
-class NetworkReportEndpoint(_AggReportEndpoint[DimensionInGeneralFromNetwork, MetricInGeneralFromNetwork]):
-    available_dimensions = NETWORK_DIMENSIONS
-    available_metrics = NETWORK_METRICS
-
-
-class TrackerReportEndpoint(_AggReportEndpoint[DimensionInGeneralFromTracker, MetricInGeneralFromTracker]):
-    available_dimensions = TRACKER_DIMENSIONS
-    available_metrics = TRACKER_METRICS
```

### Comparing `singular_client-0.1.5/singular_client/endpoints/skan.py` & `singular_client-0.1.6/singular_client/endpoints/skan.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,68 +2,68 @@
 SKAN Reporting:
     Skan Raw
     Skan
     Skan Events
 
 https://support.singular.net/hc/en-us/articles/360056377792-Singular-SKAdNetwork-API-Reference?navigation_side_bar=true#Create_Async_SKAdNetwork_Raw_Report_Endpoint
 """
+from typing import Literal, Optional, List, Union
 from singular_client._bases import _Endpoint, ResponseDocList
-from singular_client.documents import *
-from singular_client.arguments import *
-from singular_client.fields import *
+from singular_client.documents import NameDoc
 from singular_client.endpoints.reporting import CreateReportResponse
-from typing import *
 from singular_client.utils import _convert_list_arg
 
 
 class SkanEventsEndpoint(_Endpoint[ResponseDocList[NameDoc]]):
     """
     Retrieve a list of available SKAN events for use in Create Async SKAdNetwork
     Report queries. Events are displayed as "display_name" and "name" pairs.
     """
+
     endpoint = "v2.0/skan_events"
     data_path = ["value", "skan_events"]
     res_type = ResponseDocList[NameDoc]
 
 
 class SkanRawReportEndpoint(_Endpoint[CreateReportResponse]):
     """
     Query an asynchronous report for raw SKAdNetwork data collected from postbacks.
     This endpoint provides the number of SKAdNetwork conversions per network and app.
     """
+
     endpoint = "v2.0/create_async_skadnetwork_raw_report"
     data_path = ["value", "report_id"]
-    available_dimensions = SKAN_RAW_DIMENSIONS
-    available_metrics = SKAN_RAW_METRICS
     res_type = CreateReportResponse
     returns_collection = False
     method = "POST"
 
     def request(
         self,
         start_date: str,
-        time_breakdown: TimeBreakdown = "all",
+        time_breakdown: Literal["day", "week", "month", "all"] = "all",
         end_date: Optional[str] = None,
-        skadnetwork_date_type: SkadDateType = "skan_postback_date",
-        dimensions: Optional[Union[List[DimensionInSkanRaw], str]] = None,
-        metrics: Optional[Union[List[MetricInSkanRaw], str]] = None,
+        skadnetwork_date_type: Literal[
+            "skan_postback_date", "estimated_install_date"
+        ] = "skan_postback_date",
+        dimensions: Optional[Union[List[str], str]] = None,
+        metrics: Optional[Union[List[str], str]] = None,
         app: Optional[List[str]] = None,
         source: Optional[List[str]] = None,
         filters: Optional[List[dict]] = None,
-        format: FileFormat = "csv",
-        country_code_format: CountryCodeFormat = "iso3",
+        format: Literal["json", "csv"] = "csv",
+        country_code_format: Literal["iso3", "iso"] = "iso3",
     ):
         report_id = super().request(
             data=dict(
                 start_date=start_date,
                 end_date=end_date or start_date,
                 time_breakdown=time_breakdown,
                 skadnetwork_date_type=skadnetwork_date_type,
-                dimensions=_convert_list_arg(dimensions, self.available_dimensions),
-                metrics=_convert_list_arg(metrics, self.available_metrics),
+                dimensions=_convert_list_arg(dimensions),
+                metrics=_convert_list_arg(metrics),
                 app=_convert_list_arg(app),
                 source=_convert_list_arg(source),
                 filters=filters,
                 format=format,
                 country_code_format=country_code_format,
             ),
         )
@@ -73,40 +73,41 @@
 
 class SkanReportEndpoint(_Endpoint[CreateReportResponse]):
     """
     Generate an asynchronous report query for SKAdNetwork data combined with ad network
     and tracker data. Use it to measure metrics like CPI, click-through rate,
     etc., for SKAdNetwork campaigns, grouped by network and/or campaign.
     """
+
     endpoint = "v2.0/create_async_skadnetwork_report"
     data_path = ["value", "report_id"]
     res_type = CreateReportResponse
-    available_dimensions = SKAN_DIMENSIONS
-    available_metrics = SKAN_METRICS
     returns_collection = False
     method = "POST"
 
     def request(
         self,
         start_date: str,
-        time_breakdown: TimeBreakdown = "all",
+        time_breakdown: Literal["day", "week", "month", "all"] = "all",
         end_date: Optional[str] = None,
-        skadnetwork_date_type: SkadDateType = "skan_postback_date",
-        dimensions: Optional[Union[List[DimensionInSkan], str]] = None,
-        metrics: Optional[Union[List[MetricInSkan], str]] = None,
+        skadnetwork_date_type: Literal[
+            "skan_postback_date", "estimated_install_date"
+        ] = "skan_postback_date",
+        dimensions: Optional[Union[List[str], str]] = None,
+        metrics: Optional[Union[List[str], str]] = None,
         skan_events: Optional[List[str]] = None,
-        format: FileFormat = "csv",
+        format: Literal["json", "csv"] = "csv",
     ):
         report_id = super().request(
             data=dict(
                 start_date=start_date,
                 end_date=end_date or start_date,
                 time_breakdown=time_breakdown,
                 skadnetwork_date_type=skadnetwork_date_type,
-                dimensions=_convert_list_arg(dimensions, self.available_dimensions),
-                metrics=_convert_list_arg(metrics, self.available_metrics),
+                dimensions=_convert_list_arg(dimensions),
+                metrics=_convert_list_arg(metrics),
                 skan_events=_convert_list_arg(skan_events),
                 format=format,
             ),
         )
         report_id.api = self.api
         return report_id
```

