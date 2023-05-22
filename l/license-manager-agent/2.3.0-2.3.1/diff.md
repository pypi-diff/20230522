# Comparing `tmp/license_manager_agent-2.3.0.tar.gz` & `tmp/license_manager_agent-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_manager_agent-2.3.0.tar", max compression
+gzip compressed data, was "license_manager_agent-2.3.1.tar", max compression
```

## Comparing `license_manager_agent-2.3.0.tar` & `license_manager_agent-2.3.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       23 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/README.rst
--rw-r--r--   0        0        0        0 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/__init__.py
--rw-r--r--   0        0        0     7388 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/backend_utils.py
--rw-r--r--   0        0        0     3473 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/config.py
--rw-r--r--   0        0        0     1048 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/exceptions.py
--rw-r--r--   0        0        0     4032 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/license_report.py
--rw-r--r--   0        0        0     2000 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/logs.py
--rw-r--r--   0        0        0        0 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/parsing/__init__.py
--rw-r--r--   0        0        0     1732 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/parsing/flexlm.py
--rw-r--r--   0        0        0     3537 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/parsing/lmx.py
--rw-r--r--   0        0        0     4416 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/parsing/lsdyna.py
--rw-r--r--   0        0        0     4758 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/parsing/olicense.py
--rw-r--r--   0        0        0     2197 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/parsing/rlm.py
--rwxr-xr-x   0        0        0     1048 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/reconcile.py
--rw-r--r--   0        0        0    11778 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/reconciliation.py
--rw-r--r--   0        0        0        0 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/server_interfaces/__init__.py
--rw-r--r--   0        0        0     2904 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/server_interfaces/flexlm.py
--rw-r--r--   0        0        0     1665 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/server_interfaces/license_server_interface.py
--rw-r--r--   0        0        0     2751 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/server_interfaces/lmx.py
--rw-r--r--   0        0        0     2727 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/server_interfaces/lsdyna.py
--rw-r--r--   0        0        0     2719 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/server_interfaces/olicense.py
--rw-r--r--   0        0        0     3739 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/server_interfaces/rlm.py
--rw-r--r--   0        0        0     1251 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/utils.py
--rw-r--r--   0        0        0        0 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/workload_managers/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/workload_managers/slurm/__init__.py
--rw-r--r--   0        0        0    10123 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/workload_managers/slurm/cmd_utils.py
--rw-r--r--   0        0        0     1036 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/workload_managers/slurm/common.py
--rw-r--r--   0        0        0     3732 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/workload_managers/slurm/reservations.py
--rw-r--r--   0        0        0     2072 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/workload_managers/slurm/slurmctld_epilog.py
--rw-r--r--   0        0        0     3940 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/lm_agent/workload_managers/slurm/slurmctld_prolog.py
--rw-r--r--   0        0        0     2050 2023-03-06 20:09:18.946208 license_manager_agent-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 license_manager_agent-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/README.rst
+-rw-r--r--   0        0        0        0 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/__init__.py
+-rw-r--r--   0        0        0    10818 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/backend_utils.py
+-rw-r--r--   0        0        0     3473 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/config.py
+-rw-r--r--   0        0        0     1048 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/exceptions.py
+-rw-r--r--   0        0        0     4032 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/license_report.py
+-rw-r--r--   0        0        0     2000 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/logs.py
+-rw-r--r--   0        0        0        0 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/parsing/__init__.py
+-rw-r--r--   0        0        0     1732 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/parsing/flexlm.py
+-rw-r--r--   0        0        0     3537 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/parsing/lmx.py
+-rw-r--r--   0        0        0     4416 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/parsing/lsdyna.py
+-rw-r--r--   0        0        0     4758 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/parsing/olicense.py
+-rw-r--r--   0        0        0     2197 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/parsing/rlm.py
+-rwxr-xr-x   0        0        0     1048 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/reconcile.py
+-rw-r--r--   0        0        0    10660 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/reconciliation.py
+-rw-r--r--   0        0        0        0 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/server_interfaces/__init__.py
+-rw-r--r--   0        0        0     2904 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/server_interfaces/flexlm.py
+-rw-r--r--   0        0        0     1665 2023-05-22 18:46:11.414982 license_manager_agent-2.3.1/lm_agent/server_interfaces/license_server_interface.py
+-rw-r--r--   0        0        0     2751 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/server_interfaces/lmx.py
+-rw-r--r--   0        0        0     2727 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/server_interfaces/lsdyna.py
+-rw-r--r--   0        0        0     2719 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/server_interfaces/olicense.py
+-rw-r--r--   0        0        0     3739 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/server_interfaces/rlm.py
+-rw-r--r--   0        0        0     1251 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/utils.py
+-rw-r--r--   0        0        0        0 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/workload_managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/__init__.py
+-rw-r--r--   0        0        0     8361 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/cmd_utils.py
+-rw-r--r--   0        0        0     1036 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/common.py
+-rw-r--r--   0        0        0     3732 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/reservations.py
+-rw-r--r--   0        0        0     1728 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/slurmctld_epilog.py
+-rw-r--r--   0        0        0     3923 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/slurmctld_prolog.py
+-rw-r--r--   0        0        0     2050 2023-05-22 18:46:11.418982 license_manager_agent-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1053 1970-01-01 00:00:00.000000 license_manager_agent-2.3.1/PKG-INFO
```

### Comparing `license_manager_agent-2.3.0/lm_agent/backend_utils.py` & `license_manager_agent-2.3.1/lm_agent/backend_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 Provide utilities that communicate with the backend.
 """
 import getpass
-import typing
+from typing import Dict, List, Optional, Union
 
 import httpx
 import jwt
-from pydantic import BaseModel, ValidationError
+from pydantic import BaseModel, Field, ValidationError
 
-from lm_agent.config import settings
+from lm_agent.config import PRODUCT_FEATURE_RX, settings
 from lm_agent.exceptions import LicenseManagerAuthTokenError, LicenseManagerBackendConnectionError
 from lm_agent.logs import logger
 
 USER_NAME = getpass.getuser()
 TOKEN_FILE_NAME = f"{USER_NAME}.token"
 
 
-def _load_token_from_cache() -> typing.Union[str, None]:
+def _load_token_from_cache() -> Union[str, None]:
     """
     Looks for and returns a token from a cache file (if it exists).
 
     Returns None if::
     * The token does not exist
     * Can't read the token
     * The token is expired (or will expire within 10 seconds)
@@ -97,54 +97,52 @@
     """
     Extends the httpx.AsyncClient class with automatic token acquisition for requests.
     The token is acquired lazily on the first httpx request issued.
 
     This client should be used for most agent actions.
     """
 
-    _token: typing.Optional[str]
+    _token: Optional[str]
 
     def __init__(self):
         self._token = None
         super().__init__(base_url=settings.BACKEND_BASE_URL, auth=self._inject_token)
 
     def _inject_token(self, request: httpx.Request) -> httpx.Request:
         if self._token is None:
             self._token = acquire_token()
         request.headers["authorization"] = f"Bearer {self._token}"
         return request
 
 
-backend_client = AsyncBackendClient()
-
-
 class SyncBackendClient(httpx.Client):
     """
     Extends the synchronous httpx.Client class with automatic token acquisition for requests.
     The token is acquired lazily on the first httpx request issued.
 
     This client should be used only for the CLI tools.
     """
 
-    _token: typing.Optional[str]
+    _token: Optional[str]
 
     def __init__(self):
         self._token = None
         super().__init__(base_url=settings.BACKEND_BASE_URL, auth=self._inject_token)
 
     def _inject_token(self, request: httpx.Request) -> httpx.Request:
         if self._token is None:
             self._token = acquire_token()
         request.headers["authorization"] = f"Bearer {self._token}"
         return request
 
 
 async def check_backend_health():
     """Hit the API's health-check endpoint to make sure the API is available."""
-    resp = await backend_client.get("/lm/health")
+    async with AsyncBackendClient() as backend_client:
+        resp = await backend_client.get("/lm/health")
     if resp.status_code != 204:
         logger.error("license-manager-backend health-check failed.")
         raise LicenseManagerBackendConnectionError("Could not connect to the backend health-check endpoint")
 
 
 class BackendConfigurationRow(BaseModel):
     """
@@ -152,18 +150,18 @@
           If the schema changes upstream in a non-reverse-compatible way, this schema should cause errors
           in deserialization.
     """
 
     class Config:
         extra = "ignore"
 
-    id: typing.Optional[int] = None
+    id: Optional[int] = None
     product: str
     features: dict
-    license_servers: typing.List[str]
+    license_servers: List[str]
     license_server_type: str
     grace_time: int
     client_id: str
 
 
 class BackendBookingRow(BaseModel):
     """
@@ -180,51 +178,161 @@
     booked: int
     config_id: int
     lead_host: str
     user_name: str
     cluster_name: str
 
 
+class LicenseBooking(BaseModel):
+    """
+    Structure to represent a license booking.
+    """
+
+    product_feature: str = Field(..., regex=PRODUCT_FEATURE_RX)
+    tokens: int
+    license_server_type: Union[None, str]
+
+
+class LicenseBookingRequest(BaseModel):
+    """
+    Structure to represent a list of license bookings.
+    """
+
+    job_id: int
+    bookings: Union[List, List[LicenseBooking]]
+    user_name: str
+    lead_host: str
+    cluster_name: str
+
+
 async def get_bookings_from_backend(
-    cluster_name: typing.Optional[str] = None,
-) -> typing.List[BackendBookingRow]:
-    bookings: typing.List = []
+    cluster_name: Optional[str] = None,
+) -> List[BackendBookingRow]:
+    bookings: List = []
     try:
-        if cluster_name:
-            resp = await backend_client.get(f"/lm/api/v1/booking/all?cluster_name={cluster_name}")
-        else:
-            resp = await backend_client.get("/lm/api/v1/booking/all")
+        async with AsyncBackendClient() as backend_client:
+            if cluster_name:
+                resp = await backend_client.get(f"/lm/api/v1/booking/all?cluster_name={cluster_name}")
+            else:
+                resp = await backend_client.get("/lm/api/v1/booking/all")
     except httpx.ConnectError as e:
         logger.error(f"Connection failed to backend: {e}")
         return bookings
     for booking in resp.json():
         try:
             bookings.append(BackendBookingRow.parse_obj(booking))
         except ValidationError as err:
             logger.error(f"Wrong format for booking: {str(err)}")
     return bookings
 
 
 async def get_config_id_from_backend(product_feature: str) -> int:
     """Given the product_feature return return the config id."""
     path = "/lm/api/v1/config/"
-    resp = await backend_client.get(path, params={"product_feature": product_feature})
+    async with AsyncBackendClient() as backend_client:
+        resp = await backend_client.get(path, params={"product_feature": product_feature})
     return resp.json()
 
 
-async def get_config_from_backend() -> typing.List[BackendConfigurationRow]:
+async def get_config_from_backend() -> List[BackendConfigurationRow]:
     """Get all config rows from the backend."""
     path = "/lm/api/v1/config/agent/all"
 
     try:
-        resp = await backend_client.get(path)
+        async with AsyncBackendClient() as backend_client:
+            resp = await backend_client.get(path)
     except httpx.ConnectError as e:
         logger.error(f"Connection failed to backend: {backend_client.base_url}{path}: {e}")
         return []
 
     configs = []
     for (i, config_row) in enumerate(resp.json()):
         try:
             configs.append(BackendConfigurationRow.parse_obj(config_row))
         except ValidationError as err:
             logger.error(f"Could not validate config entry at row {i}: {str(err)}")
     return configs
+
+
+async def make_booking_request(lbr: LicenseBookingRequest) -> bool:
+    """Book the feature tokens."""
+
+    features = [
+        {
+            "product_feature": license_booking.product_feature,
+            "booked": license_booking.tokens,
+        }
+        for license_booking in lbr.bookings
+    ]
+
+    logger.debug(f"features: {features}")
+    logger.debug(f"lbr: {lbr}")
+
+    async with AsyncBackendClient() as backend_client:
+        resp = await backend_client.put(
+            "/lm/api/v1/booking/book",
+            json={
+                "job_id": lbr.job_id,
+                "features": features,
+                "user_name": lbr.user_name,
+                "lead_host": lbr.lead_host,
+                "cluster_name": lbr.cluster_name,
+            },
+        )
+
+    if resp.status_code == 200:
+        logger.debug("##### Booking completed successfully #####")
+        return True
+    logger.debug(f"##### Booking failed: {str(resp.content)} #####")
+    return False
+
+
+async def remove_booking_for_job_id(job_id: str) -> bool:
+    """Remove token bookings used by job."""
+
+    # Remove the booking for the job.
+    async with AsyncBackendClient() as backend_client:
+        resp = await backend_client.delete(f"lm/api/v1/booking/book/{job_id}")
+    # Return True if the request to delete the booking was successful.
+    if resp.status_code == 200:
+        return True
+    logger.error(f"{job_id} could not be deleted.")
+    logger.debug(f"response from delete: {resp.__dict__}")
+    return False
+
+
+async def get_all_grace_times() -> Dict[int, int]:
+    """
+    Send GET to /lm/api/v1/config/all.
+    """
+    async with AsyncBackendClient() as backend_client:
+        response = await backend_client.get("/lm/api/v1/config/all")
+    configs = response.json()
+    grace_times = {config["id"]: config["grace_time"] for config in configs}
+    return grace_times
+
+
+async def get_booking_for_job_id(job_id: str) -> Dict:
+    """
+    Return the booking row for the given job_id.
+    """
+    async with AsyncBackendClient() as backend_client:
+        response = await backend_client.get(f"/lm/api/v1/booking/job/{job_id}")
+    return response.json()
+
+
+async def get_bookings_sum_per_cluster(product_feature: str) -> Dict[str, int]:
+    """
+    Get booking sum for a license's bookings in each cluster.
+    """
+    async with AsyncBackendClient() as backend_client:
+        response = await backend_client.get("/lm/api/v1/booking/all")
+    bookings = response.json()
+
+    booking_sum: Dict[str, int] = {}
+
+    for booking in bookings:
+        cluster_name = booking["cluster_name"]
+        if booking["product_feature"] == product_feature:
+            booking_sum[cluster_name] = booking_sum.get(cluster_name, 0) + booking["booked"]
+
+    return booking_sum
```

### Comparing `license_manager_agent-2.3.0/lm_agent/config.py` & `license_manager_agent-2.3.1/lm_agent/config.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/exceptions.py` & `license_manager_agent-2.3.1/lm_agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/license_report.py` & `license_manager_agent-2.3.1/lm_agent/license_report.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/logs.py` & `license_manager_agent-2.3.1/lm_agent/logs.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/parsing/flexlm.py` & `license_manager_agent-2.3.1/lm_agent/parsing/flexlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/parsing/lmx.py` & `license_manager_agent-2.3.1/lm_agent/parsing/lmx.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/parsing/lsdyna.py` & `license_manager_agent-2.3.1/lm_agent/parsing/lsdyna.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/parsing/olicense.py` & `license_manager_agent-2.3.1/lm_agent/parsing/olicense.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/parsing/rlm.py` & `license_manager_agent-2.3.1/lm_agent/parsing/rlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/reconcile.py` & `license_manager_agent-2.3.1/lm_agent/reconcile.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/reconciliation.py` & `license_manager_agent-2.3.1/lm_agent/reconciliation.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,23 @@
 Reconciliation functionality live here.
 """
 import asyncio
 from typing import Dict, List
 
 from httpx import ConnectError
 
-from lm_agent.backend_utils import backend_client, get_bookings_from_backend, get_config_id_from_backend
+from lm_agent.backend_utils import (
+    AsyncBackendClient,
+    get_all_grace_times,
+    get_booking_for_job_id,
+    get_bookings_from_backend,
+    get_bookings_sum_per_cluster,
+    get_config_id_from_backend,
+    remove_booking_for_job_id,
+)
 from lm_agent.exceptions import (
     LicenseManagerBackendConnectionError,
     LicenseManagerEmptyReportError,
     LicenseManagerFeatureConfigurationIncorrect,
     LicenseManagerReservationFailure,
 )
 from lm_agent.license_report import report
@@ -29,42 +37,14 @@
     scontrol_show_reservation,
     scontrol_update_reservation,
 )
 
 RECONCILE_URL_PATH = "/lm/api/v1/license/reconcile"
 
 
-async def remove_booked_for_job_id(job_id: str):
-    """
-    Send DELETE to /lm/api/v1/booking/book/{job_id}.
-    """
-    response = await backend_client.delete(f"/lm/api/v1/booking/book/{job_id}")
-    if response.status_code != 200:
-        logger.error(f"{job_id} could not be deleted.")
-        logger.debug(f"response from delete: {response.__dict__}")
-
-
-async def get_all_grace_times() -> Dict[int, int]:
-    """
-    Send GET to /lm/api/v1/config/all.
-    """
-    response = await backend_client.get("/lm/api/v1/config/all")
-    configs = response.json()
-    grace_times = {config["id"]: config["grace_time"] for config in configs}
-    return grace_times
-
-
-async def get_booked_for_job_id(job_id: str) -> Dict:
-    """
-    Return the booking row for the given job_id.
-    """
-    response = await backend_client.get(f"/lm/api/v1/booking/job/{job_id}")
-    return response.json()
-
-
 def get_greatest_grace_time(job_id: str, grace_times: Dict[int, int], booking_rows: List) -> int:
     """
     Find the greatest grace_time for the given job_id.
     """
     greatest_grace_time = -1
     for book in booking_rows:
         if not book:
@@ -96,41 +76,41 @@
     squeue_result = squeue_parser(formatted_squeue_output)
     squeue_running_jobs = get_running_jobs(squeue_result)
 
     grace_times = await get_all_grace_times()
     get_booked_call = []
     for job in squeue_running_jobs:
         job_id = job["job_id"]
-        get_booked_call.append(get_booked_for_job_id(job_id))
+        get_booked_call.append(get_booking_for_job_id(job_id))
 
     booking_rows_for_running_jobs = await asyncio.gather(*get_booked_call)
 
     # get the greatest grace_time for each job
     for job in squeue_running_jobs:
         job_id = job["job_id"]
         greatest_grace_time = get_greatest_grace_time(job_id, grace_times, booking_rows_for_running_jobs)
         # if the running_time is greater than the greatest grace_time, delete the booking for it
         if job["run_time_in_seconds"] > greatest_grace_time and greatest_grace_time != -1:
             logger.debug(f"GRACE_TIME: {greatest_grace_time}, {job_id}")
-            await remove_booked_for_job_id(job_id)
+            await remove_booking_for_job_id(job_id)
     await clean_bookings(squeue_result, cluster_name)
 
 
 async def clean_bookings(squeue_result, cluster_name):
     logger.debug("CLEAN_BOOKINGS: start")
     cluster_bookings = [str(booking.job_id) for booking in await get_bookings_from_backend(cluster_name)]
     if squeue_result is None:
         squeue_result = []
     jobs_not_running = [str(job["job_id"]) for job in squeue_result if job["state"] != "RUNNING"]
     all_jobs_squeue = [str(job["job_id"]) for job in squeue_result]
     delete_booking_call = []
     logger.debug("CLEAN_BOOKINGS: after building lists")
     for job_id in cluster_bookings:
         if job_id in jobs_not_running or job_id not in all_jobs_squeue:
-            delete_booking_call.append(remove_booked_for_job_id(job_id))
+            delete_booking_call.append(remove_booking_for_job_id(job_id))
     logger.debug(f"CLEAN_BOOKINGS: {cluster_bookings}, {jobs_not_running}, {all_jobs_squeue}")
     if not delete_booking_call:
         logger.debug("CLEAN_BOOKINGS: no need to clean")
         return
     await asyncio.gather(*delete_booking_call)
 
 
@@ -141,31 +121,14 @@
     filtered_licenses = []
     for license in licenses_to_update:
         if license["product_feature"] in local_licenses:
             filtered_licenses.append(license)
     return filtered_licenses
 
 
-async def get_bookings_sum_per_cluster(product_feature: str) -> Dict[str, int]:
-    """
-    Get booking sum for a license's bookings in each cluster.
-    """
-    response = await backend_client.get("/lm/api/v1/booking/all")
-    bookings = response.json()
-
-    booking_sum: Dict[str, int] = {}
-
-    for booking in bookings:
-        cluster_name = booking["cluster_name"]
-        if booking["product_feature"] == product_feature:
-            booking_sum[cluster_name] = booking_sum.get(cluster_name, 0) + booking["booked"]
-
-    return booking_sum
-
-
 async def create_or_update_reservation(reservation_data):
     """
     Create the reservation if it doesn't exist, otherwise update it.
     If the reservation cannot be updated, delete it and create a new one.
     """
     reservation = await scontrol_show_reservation()
 
@@ -192,15 +155,16 @@
     # Generate report and update the backend
     logger.debug("Reconciling licenses in the backend")
     await update_report()
     logger.debug("Backend licenses reconciliated")
 
     # Fetch from backend the licenses usage information
     logger.debug("Fetching licenses usage information from backend")
-    response = await backend_client.get("/lm/api/v1/license/cluster_update")
+    async with AsyncBackendClient() as backend_client:
+        response = await backend_client.get("/lm/api/v1/license/cluster_update")
     licenses_usage_info = response.json()
     logger.debug("Licenses usage information fetched from backend")
 
     # Filter the licenses to update
     licenses_to_update = await filter_cluster_update_licenses(licenses_usage_info)
     logger.debug(f"Licenses to update: {licenses_to_update}")
 
@@ -219,15 +183,16 @@
         cluster_booking_sum = bookings_per_cluster.get(cluster_name, 0)
         other_cluster_booking_sum = sum(
             [booking for cluster, booking in bookings_per_cluster.items() if cluster != cluster_name]
         )
 
         # Get license configuration from backend
         config_id = await get_config_id_from_backend(product_feature)
-        config = await backend_client.get(f"/lm/api/v1/config/{config_id}")
+        async with AsyncBackendClient() as backend_client:
+            config = await backend_client.get(f"/lm/api/v1/config/{config_id}")
         config = config.json()
 
         license_server_type = config["license_server_type"]
         # Use feature name to get total and limit from feature data in the license config
         try:
             # Get total from new feature format
             total = config["features"][feature].get("total", 0)
@@ -282,19 +247,19 @@
     rep = await report()
     if not rep:
         logger.error(
             "No license data could be collected, check that tools are installed "
             "correctly and the right hosts/ports are configured in settings"
         )
         raise LicenseManagerEmptyReportError("Got an empty response from the license server")
-    client = backend_client
     try:
-        r = await client.patch(RECONCILE_URL_PATH, json=rep)
+        async with AsyncBackendClient() as backend_client:
+            r = await backend_client.patch(RECONCILE_URL_PATH, json=rep)
     except ConnectError as e:
-        logger.error(f"{client.base_url}{RECONCILE_URL_PATH}: {e}")
+        logger.error(f"{backend_client.base_url}{RECONCILE_URL_PATH}: {e}")
         raise LicenseManagerBackendConnectionError("Failed to connect to the backend")
 
     if r.status_code != 200:
         logger.error(f"{r.url}: {r.status_code}!: {r.text}")
         raise LicenseManagerBackendConnectionError(f"Unexpected status code from report: {r.status_code}")
 
     logger.info(f"Forced reconciliation succeeded. backend updated: {len(rep)} feature(s)")
```

### Comparing `license_manager_agent-2.3.0/lm_agent/server_interfaces/flexlm.py` & `license_manager_agent-2.3.1/lm_agent/server_interfaces/flexlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/server_interfaces/license_server_interface.py` & `license_manager_agent-2.3.1/lm_agent/server_interfaces/license_server_interface.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/server_interfaces/lmx.py` & `license_manager_agent-2.3.1/lm_agent/server_interfaces/lmx.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/server_interfaces/lsdyna.py` & `license_manager_agent-2.3.1/lm_agent/server_interfaces/lsdyna.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/server_interfaces/olicense.py` & `license_manager_agent-2.3.1/lm_agent/server_interfaces/olicense.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/server_interfaces/rlm.py` & `license_manager_agent-2.3.1/lm_agent/server_interfaces/rlm.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/utils.py` & `license_manager_agent-2.3.1/lm_agent/utils.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/workload_managers/slurm/cmd_utils.py` & `license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/cmd_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 """Utilities that interact with slurm."""
 import asyncio
 import re
 import shlex
 import subprocess
 from typing import List, Optional, Union
 
-from pydantic import BaseModel, Field
-
-from lm_agent.backend_utils import backend_client
-from lm_agent.config import PRODUCT_FEATURE_RX
+from lm_agent.backend_utils import LicenseBooking
 from lm_agent.logs import logger
 from lm_agent.workload_managers.slurm.common import (
     CMD_TIMEOUT,
     ENCODING,
     SACCTMGR_PATH,
     SCONTROL_PATH,
     SQUEUE_PATH,
@@ -32,36 +29,14 @@
         shlex.join([SCONTROL_PATH, "show", f"job={slurm_job_id}"]),
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.STDOUT,
     )
     """
 
 
-class LicenseBooking(BaseModel):
-    """
-    Structure to represent a license booking.
-    """
-
-    product_feature: str = Field(..., regex=PRODUCT_FEATURE_RX)
-    tokens: int
-    license_server_type: Union[None, str]
-
-
-class LicenseBookingRequest(BaseModel):
-    """
-    Structure to represent a list of license bookings.
-    """
-
-    job_id: int
-    bookings: Union[List, List[LicenseBooking]]
-    user_name: str
-    lead_host: str
-    cluster_name: str
-
-
 def _match_requested_license(requested_license: str) -> Union[dict, None]:
     license_regex = re.compile(r"(?P<product>\w+)\.(?P<feature>\w+)@(?P<server_type>\w+)(:(?P<tokens>\d+))?")
 
     matches = license_regex.match(requested_license)
 
     if not matches:
         return None
@@ -105,57 +80,14 @@
             license_server_type=license_server_type,
         )
         required_licenses.append(license_booking)
 
     return required_licenses
 
 
-async def make_booking_request(lbr: LicenseBookingRequest) -> bool:
-    """Book the feature tokens."""
-
-    features = [
-        {
-            "product_feature": license_booking.product_feature,
-            "booked": license_booking.tokens,
-        }
-        for license_booking in lbr.bookings
-    ]
-
-    logger.debug(f"features: {features}")
-    logger.debug(f"lbr: {lbr}")
-
-    resp = await backend_client.put(
-        "/lm/api/v1/booking/book",
-        json={
-            "job_id": lbr.job_id,
-            "features": features,
-            "user_name": lbr.user_name,
-            "lead_host": lbr.lead_host,
-            "cluster_name": lbr.cluster_name,
-        },
-    )
-
-    if resp.status_code == 200:
-        logger.debug("##### Booking completed successfully #####")
-        return True
-    logger.debug(f"##### Booking failed: {str(resp.content)} #####")
-    return False
-
-
-async def reconcile():
-    """Force a reconciliation."""
-    resp = await backend_client.get("/lm/api/v1/license/reconcile")
-
-    if resp.status_code == 200:
-        logger.debug("##### Reconcile completed successfully #####")
-        return True
-    logger.debug(f"##### Reconcile failed {resp.status_code} #####")
-    return False
-
-
 async def get_tokens_for_license(
     product_feature_server: str,
     output_type: str,
 ) -> Optional[int]:
     """
     Return tokens from scontrol output.
     """
```

### Comparing `license_manager_agent-2.3.0/lm_agent/workload_managers/slurm/common.py` & `license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/common.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/workload_managers/slurm/reservations.py` & `license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/reservations.py`

 * *Files identical despite different names*

### Comparing `license_manager_agent-2.3.0/lm_agent/workload_managers/slurm/slurmctld_epilog.py` & `license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/slurmctld_epilog.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,22 @@
 #!/usr/bin/env python3
 """
 The EpilogSlurmctld executable.
 """
 import asyncio
 import sys
 
-from lm_agent.backend_utils import backend_client
+from lm_agent.backend_utils import remove_booking_for_job_id
 from lm_agent.config import settings
 from lm_agent.logs import init_logging, logger
 from lm_agent.reconciliation import update_report
 from lm_agent.workload_managers.slurm.cmd_utils import get_required_licenses_for_job
 from lm_agent.workload_managers.slurm.common import get_job_context
 
 
-async def _remove_booking_for_job(job_id: str) -> bool:
-    """Remove token bookings used by job."""
-
-    # Remove the booking for the job.
-    resp = await backend_client.delete(f"lm/api/v1/booking/book/{job_id}")
-    # Return True if the request to delete the booking was successful.
-    if resp.status_code == 200:
-        return True
-    return False
-
-
 async def epilog():
     # Initialize the logger
     init_logging("slurmctld-epilog")
     job_context = get_job_context()
     job_id = job_context["job_id"]
     job_licenses = job_context["job_licenses"]
 
@@ -48,15 +37,15 @@
 
     if not required_licenses:
         logger.debug("No licenses required, exiting!")
         sys.exit(0)
 
     if len(required_licenses) > 0:
         # Attempt to remove the booking and log the result.
-        booking_removed = await _remove_booking_for_job(job_id)
+        booking_removed = await remove_booking_for_job_id(job_id)
         if booking_removed:
             logger.debug(f"Booking for job id: {job_id} successfully deleted.")
         else:
             logger.debug(f"Booking for job id: {job_id} not removed.")
 
 
 def main():
```

### Comparing `license_manager_agent-2.3.0/lm_agent/workload_managers/slurm/slurmctld_prolog.py` & `license_manager_agent-2.3.1/lm_agent/workload_managers/slurm/slurmctld_prolog.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,19 @@
 Executing this script will result in either an exit(0) or exit(1). Slurm will
 proceed with scheduling the job if the exit status is 0, and will not proceed
 if the exit status is anything other then 0, e.g. 1.
 """
 import asyncio
 import sys
 
-from lm_agent.backend_utils import get_config_from_backend
+from lm_agent.backend_utils import LicenseBookingRequest, get_config_from_backend, make_booking_request
 from lm_agent.config import settings
 from lm_agent.logs import init_logging, logger
 from lm_agent.reconciliation import update_report
-from lm_agent.workload_managers.slurm.cmd_utils import (
-    LicenseBookingRequest,
-    get_required_licenses_for_job,
-    make_booking_request,
-)
+from lm_agent.workload_managers.slurm.cmd_utils import get_required_licenses_for_job
 from lm_agent.workload_managers.slurm.common import get_job_context
 
 
 async def prolog():
     """The PrologSlurmctld for the license-manager-agent."""
     # Initialize the logger
     init_logging("slurmctld-prolog")
```

### Comparing `license_manager_agent-2.3.0/pyproject.toml` & `license_manager_agent-2.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "license-manager-agent"
-version = "2.3.0"
+version = "2.3.1"
 description = "Provides an agent for interacting with license manager"
 authors = ["OmniVector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/license-manager"
 documentation = "https://omnivector-solutions.github.io/license-manager/"
 packages = [{ include = "lm_agent" }]
```

### Comparing `license_manager_agent-2.3.0/PKG-INFO` & `license_manager_agent-2.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-manager-agent
-Version: 2.3.0
+Version: 2.3.1
 Summary: Provides an agent for interacting with license manager
 Home-page: https://github.com/omnivector-solutions/license-manager
 License: MIT
 Author: OmniVector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<3.9
 Classifier: License :: OSI Approved :: MIT License
```

