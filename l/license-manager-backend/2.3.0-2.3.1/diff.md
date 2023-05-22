# Comparing `tmp/license_manager_backend-2.3.0.tar.gz` & `tmp/license_manager_backend-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "license_manager_backend-2.3.0.tar", max compression
+gzip compressed data, was "license_manager_backend-2.3.1.tar", max compression
```

## Comparing `license_manager_backend-2.3.0.tar` & `license_manager_backend-2.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       25 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/README.rst
--rw-r--r--   0        0        0       60 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/__init__.py
--rw-r--r--   0        0        0      453 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/api/__init__.py
--rw-r--r--   0        0        0     9068 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/api/booking.py
--rw-r--r--   0        0        0     7608 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/api/config.py
--rw-r--r--   0        0        0     9021 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/api/license.py
--rw-r--r--   0        0        0      447 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/api/permissions.py
--rw-r--r--   0        0        0     3585 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/api_schemas.py
--rw-r--r--   0        0        0      464 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/compat.py
--rw-r--r--   0        0        0     1263 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/config.py
--rw-r--r--   0        0        0      209 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/exceptions.py
--rw-r--r--   0        0        0     1754 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/helpers.py
--rw-r--r--   0        0        0     2858 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/main.py
--rw-r--r--   0        0        0     1316 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/security.py
--rw-r--r--   0        0        0     1830 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/storage.py
--rw-r--r--   0        0        0     2541 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/table_schemas.py
--rw-r--r--   0        0        0     1099 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/lm_backend/version.py
--rw-r--r--   0        0        0     2011 2023-03-06 20:09:18.875417 license_manager_backend-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 license_manager_backend-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/README.rst
+-rw-r--r--   0        0        0       60 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/__init__.py
+-rw-r--r--   0        0        0      453 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/api/__init__.py
+-rw-r--r--   0        0        0     9062 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/api/booking.py
+-rw-r--r--   0        0        0     7864 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/api/config.py
+-rw-r--r--   0        0        0     9015 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/api/license.py
+-rw-r--r--   0        0        0     3665 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/api_schemas.py
+-rw-r--r--   0        0        0      464 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/compat.py
+-rw-r--r--   0        0        0     1147 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/config.py
+-rw-r--r--   0        0        0      914 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/constants.py
+-rw-r--r--   0        0        0      209 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/exceptions.py
+-rw-r--r--   0        0        0     1754 2023-05-22 18:46:09.646746 license_manager_backend-2.3.1/lm_backend/helpers.py
+-rw-r--r--   0        0        0     2858 2023-05-22 18:46:09.650746 license_manager_backend-2.3.1/lm_backend/main.py
+-rw-r--r--   0        0        0     1316 2023-05-22 18:46:09.650746 license_manager_backend-2.3.1/lm_backend/security.py
+-rw-r--r--   0        0        0     1830 2023-05-22 18:46:09.650746 license_manager_backend-2.3.1/lm_backend/storage.py
+-rw-r--r--   0        0        0     2541 2023-05-22 18:46:09.650746 license_manager_backend-2.3.1/lm_backend/table_schemas.py
+-rw-r--r--   0        0        0     1099 2023-05-22 18:46:09.650746 license_manager_backend-2.3.1/lm_backend/version.py
+-rw-r--r--   0        0        0     2011 2023-05-22 18:46:09.650746 license_manager_backend-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 license_manager_backend-2.3.1/PKG-INFO
```

### Comparing `license_manager_backend-2.3.0/lm_backend/api/booking.py` & `license_manager_backend-2.3.1/lm_backend/api/booking.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 from asyncio import Lock
 from typing import List, Optional
 
 from fastapi import APIRouter, Depends, HTTPException, Query
 from sqlalchemy.sql import delete, join, select
 
 from lm_backend.api.config import get_config_id_for_product_features
-from lm_backend.api.permissions import Permissions
 from lm_backend.api_schemas import (
     Booking,
     BookingRow,
     BookingRowDetail,
     ConfigurationItem,
     ConfigurationRow,
     LicenseUse,
 )
 from lm_backend.compat import INTEGRITY_CHECK_EXCEPTIONS
+from lm_backend.constants import Permissions
 from lm_backend.exceptions import LicenseManagerFeatureConfigurationIncorrect
 from lm_backend.security import guard
 from lm_backend.storage import database, search_clause, sort_clause
 from lm_backend.table_schemas import (
     booking_searchable_fields,
     booking_sortable_fields,
     booking_table,
```

### Comparing `license_manager_backend-2.3.0/lm_backend/api/config.py` & `license_manager_backend-2.3.1/lm_backend/api/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from ast import literal_eval
 from typing import Dict, List, Optional, Union
 
 from armasec import TokenPayload
 from fastapi import APIRouter, Body, Depends, HTTPException, Query, status
 
-from lm_backend.api.permissions import Permissions
 from lm_backend.api_schemas import ConfigurationItem, ConfigurationRow
 from lm_backend.compat import INTEGRITY_CHECK_EXCEPTIONS
+from lm_backend.constants import LicenseServerType, Permissions
 from lm_backend.security import guard
 from lm_backend.storage import database, search_clause, sort_clause
 from lm_backend.table_schemas import config_searchable_fields, config_sortable_fields, config_table
 
 router = APIRouter()
 
 
@@ -73,14 +73,25 @@
     return [
         ConfigurationItem(**item.dict(exclude={"features"}), features=literal_eval(item.features))
         for item in config_rows
     ]
 
 
 @router.get(
+    "/license_server_types",
+    response_model=List[LicenseServerType],
+)
+async def get_license_server_types():
+    """
+    Query database for all configurations.
+    """
+    return [e for e in LicenseServerType]
+
+
+@router.get(
     "/{config_id}",
     response_model=ConfigurationItem,
     dependencies=[Depends(guard.lockdown(Permissions.CONFIG_VIEW))],
 )
 async def get_configuration(config_id: int):
     """
     Get one configuration row based on a given id.
@@ -148,15 +159,15 @@
     dependencies=[Depends(guard.lockdown(Permissions.CONFIG_EDIT))],
 )
 async def update_configuration(
     config_id: int,
     product: Optional[str] = Body(None),
     features: Optional[str] = Body(None),
     license_servers: Optional[List[str]] = Body(None),
-    license_server_type: Optional[str] = Body(None),
+    license_server_type: Optional[LicenseServerType] = Body(None),
     grace_time: Optional[int] = Body(None),
     client_id: Optional[str] = Body(None),
 ):
     """
     Update a configuration row in the database with all of the
     optional arguments provided.
     """
```

### Comparing `license_manager_backend-2.3.0/lm_backend/api/license.py` & `license_manager_backend-2.3.1/lm_backend/api/license.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import asyncio
 from typing import Dict, List, Optional, Sequence, Tuple
 
 from fastapi import APIRouter, Depends, Query
 from sqlalchemy import func
 from sqlalchemy.sql import join, select, update
 
-from lm_backend.api.permissions import Permissions
 from lm_backend.api_schemas import (
     BookingRow,
     LicenseUse,
     LicenseUseBase,
     LicenseUseReconcile,
     LicenseUseReconcileRequest,
     LicenseUseWithBooking,
 )
+from lm_backend.constants import Permissions
 from lm_backend.helpers import LicenseUseSortFieldChecker, LicenseUseWithBookingSortFieldChecker
 from lm_backend.security import guard
 from lm_backend.storage import database, search_clause
 from lm_backend.table_schemas import booking_table, license_searchable_fields, license_table
 
 PRODUCT_FEATURE_RX = r"^.+?\..+$"
 router = APIRouter()
```

### Comparing `license_manager_backend-2.3.0/lm_backend/api_schemas.py` & `license_manager_backend-2.3.1/lm_backend/api_schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 API request and response schemas
 """
 from datetime import datetime
 from typing import List, Optional
 
 from pydantic import BaseModel, Field, validator
 
+from lm_backend.constants import LicenseServerType
+
 
 class ConfigurationRow(BaseModel):
     """
     A configuration row.
     """
 
     id: Optional[int] = Field(None)
     name: Optional[str] = Field(None)
     product: str
     features: str
     license_servers: List[str]
-    license_server_type: str
+    license_server_type: LicenseServerType
     grace_time: int
     client_id: str
 
     class Config:
         orm_mode = True
 
 
@@ -31,15 +33,15 @@
     """
 
     id: Optional[int] = Field(None)
     name: Optional[str] = Field(None)
     product: str
     features: dict
     license_servers: List[str]
-    license_server_type: str
+    license_server_type: LicenseServerType
     grace_time: int
     client_id: str
 
     class Config:
         orm_mode = True
```

### Comparing `license_manager_backend-2.3.0/lm_backend/config.py` & `license_manager_backend-2.3.1/lm_backend/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,12 @@
-from enum import Enum
 from typing import Optional
 
 from pydantic import BaseSettings, Field, HttpUrl
 
-
-class LogLevelEnum(str, Enum):
-    DEBUG = "DEBUG"
-    INFO = "INFO"
-    WARNING = "WARNING"
-    ERROR = "ERROR"
-    CRITICAL = "CRITICAL"
+from lm_backend.constants import LogLevelEnum
 
 
 class Settings(BaseSettings):
     """
     App config.
     """
```

### Comparing `license_manager_backend-2.3.0/lm_backend/helpers.py` & `license_manager_backend-2.3.1/lm_backend/helpers.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.0/lm_backend/main.py` & `license_manager_backend-2.3.1/lm_backend/main.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.0/lm_backend/security.py` & `license_manager_backend-2.3.1/lm_backend/security.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.0/lm_backend/storage.py` & `license_manager_backend-2.3.1/lm_backend/storage.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.0/lm_backend/table_schemas.py` & `license_manager_backend-2.3.1/lm_backend/table_schemas.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.0/lm_backend/version.py` & `license_manager_backend-2.3.1/lm_backend/version.py`

 * *Files identical despite different names*

### Comparing `license_manager_backend-2.3.0/pyproject.toml` & `license_manager_backend-2.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "license-manager-backend"
-version = "2.3.0"
+version = "2.3.1"
 description = "Provides an API for managing license data"
 authors = ["OmniVector Solutions <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/omnivector-solutions/license-manager"
 documentation = "https://omnivector-solutions.github.io/license-manager/"
 packages = [{ include = "lm_backend" }]
```

### Comparing `license_manager_backend-2.3.0/PKG-INFO` & `license_manager_backend-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: license-manager-backend
-Version: 2.3.0
+Version: 2.3.1
 Summary: Provides an API for managing license data
 Home-page: https://github.com/omnivector-solutions/license-manager
 License: MIT
 Author: OmniVector Solutions
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<3.9
 Classifier: License :: OSI Approved :: MIT License
```

