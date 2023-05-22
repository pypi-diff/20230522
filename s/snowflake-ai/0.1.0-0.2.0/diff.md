# Comparing `tmp/snowflake_ai-0.1.0.tar.gz` & `tmp/snowflake_ai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake_ai-0.1.0.tar", max compression
+gzip compressed data, was "snowflake_ai-0.2.0.tar", max compression
```

## Comparing `snowflake_ai-0.1.0.tar` & `snowflake_ai-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,36 @@
--rwxr-xr-x   0        0        0     1486 2023-04-17 14:09:35.722038 snowflake_ai-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     2407 2023-04-18 04:22:35.355895 snowflake_ai-0.1.0/README.md
--rwxr-xr-x   0        0        0      941 2023-04-18 04:11:03.321235 snowflake_ai-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2023-04-17 14:09:35.975721 snowflake_ai-0.1.0/snowflake_ai/__init__.py
--rwxr-xr-x   0        0        0        0 2023-04-17 14:09:35.979721 snowflake_ai-0.1.0/snowflake_ai/apps/__init__.py
--rwxr-xr-x   0        0        0      116 2023-04-17 14:09:36.009132 snowflake_ai-0.1.0/snowflake_ai/common/__init__.py
--rwxr-xr-x   0        0        0    11740 2023-04-17 14:09:35.993381 snowflake_ai-0.1.0/snowflake_ai/common/data_connect.py
--rwxr-xr-x   0        0        0     8139 2023-04-17 14:09:35.988381 snowflake_ai-0.1.0/snowflake_ai/common/dataframe_factory.py
--rwxr-xr-x   0        0        0     5770 2023-04-17 14:09:35.999381 snowflake_ai-0.1.0/snowflake_ai/common/file_connect.py
--rwxr-xr-x   0        0        0    11213 2023-04-17 14:09:36.005132 snowflake_ai-0.1.0/snowflake_ai/common/snow_connect.py
--rwxr-xr-x   0        0        0        0 2023-04-17 14:09:36.041408 snowflake_ai-0.1.0/snowflake_ai/conf/__init__.py
--rwxr-xr-x   0        0        0     1159 2023-04-17 14:09:36.038408 snowflake_ai-0.1.0/snowflake_ai/conf/app_config.toml
--rwxr-xr-x   0        0        0      158 2023-04-17 14:09:36.076455 snowflake_ai-0.1.0/snowflake_ai/mlops/__init__.py
--rwxr-xr-x   0        0        0      981 2023-04-17 14:09:36.047464 snowflake_ai-0.1.0/snowflake_ai/mlops/flow_context.py
--rwxr-xr-x   0        0        0      742 2023-04-17 14:09:36.053454 snowflake_ai-0.1.0/snowflake_ai/mlops/flow_ops.py
--rwxr-xr-x   0        0        0     2197 2023-04-17 14:09:36.059457 snowflake_ai-0.1.0/snowflake_ai/mlops/flow_pipeline.py
--rwxr-xr-x   0        0        0     1270 2023-04-17 14:09:36.064522 snowflake_ai-0.1.0/snowflake_ai/mlops/flow_test.py
--rwxr-xr-x   0        0        0        0 2023-04-17 14:09:36.067482 snowflake_ai-0.1.0/snowflake_ai/mlops/model_dev.py
--rwxr-xr-x   0        0        0        0 2023-04-17 14:09:36.071454 snowflake_ai-0.1.0/snowflake_ai/mlops/model_serve.py
--rwxr-xr-x   0        0        0      106 2023-04-17 14:09:36.132362 snowflake_ai-0.1.0/snowflake_ai/snowpandas/__init__.py
--rwxr-xr-x   0        0        0     7141 2023-04-17 14:09:36.112671 snowflake_ai-0.1.0/snowflake_ai/snowpandas/data_prep.py
--rwxr-xr-x   0        0        0     2279 2023-04-17 14:09:36.117679 snowflake_ai-0.1.0/snowflake_ai/snowpandas/data_setup.py
--rwxr-xr-x   0        0        0     2186 2023-04-17 14:09:36.122682 snowflake_ai-0.1.0/snowflake_ai/snowpandas/snow_prep.py
--rwxr-xr-x   0        0        0     2664 2023-04-17 14:09:36.127711 snowflake_ai-0.1.0/snowflake_ai/snowpandas/snow_setup.py
--rw-r--r--   0        0        0     3465 1970-01-01 00:00:00.000000 snowflake_ai-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0    13003 2023-04-29 19:34:49.289905 snowflake_ai-0.2.0/LICENSE.txt
+-rwxr-xr-x   0        0        0     2533 2023-05-22 14:27:21.003251 snowflake_ai-0.2.0/README.md
+-rwxr-xr-x   0        0        0     1163 2023-05-22 14:41:51.419797 snowflake_ai-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-04-17 14:09:35.975721 snowflake_ai-0.2.0/snowflake_ai/__init__.py
+-rwxr-xr-x   0        0        0       80 2023-05-13 17:49:10.802511 snowflake_ai-0.2.0/snowflake_ai/apps/__init__.py
+-rwxr-xr-x   0        0        0     5111 2023-05-20 02:49:24.560907 snowflake_ai-0.2.0/snowflake_ai/apps/app_page.py
+-rwxr-xr-x   0        0        0    10544 2023-05-20 05:20:28.322540 snowflake_ai-0.2.0/snowflake_ai/apps/streamlit_app.py
+-rwxr-xr-x   0        0        0     4372 2023-05-16 13:41:57.769513 snowflake_ai-0.2.0/snowflake_ai/apps/tab_registry.py
+-rwxr-xr-x   0        0        0      109 2023-05-14 16:47:27.493709 snowflake_ai-0.2.0/snowflake_ai/common/__init__.py
+-rwxr-xr-x   0        0        0    20726 2023-05-14 15:06:49.134494 snowflake_ai-0.2.0/snowflake_ai/common/app_config.py
+-rwxr-xr-x   0        0        0     6743 2023-05-15 11:58:35.998940 snowflake_ai-0.2.0/snowflake_ai/common/app_connect.py
+-rwxr-xr-x   0        0        0    10343 2023-05-15 14:49:44.315420 snowflake_ai-0.2.0/snowflake_ai/common/data_connect.py
+-rwxr-xr-x   0        0        0     9055 2023-05-20 01:31:31.971625 snowflake_ai-0.2.0/snowflake_ai/common/oauth_connect.py
+-rwxr-xr-x   0        0        0        0 2023-04-17 14:09:36.041408 snowflake_ai-0.2.0/snowflake_ai/conf/__init__.py
+-rwxr-xr-x   0        0        0     5249 2023-05-22 14:24:09.522740 snowflake_ai-0.2.0/snowflake_ai/conf/app_config.toml
+-rwxr-xr-x   0        0        0      152 2023-05-14 19:44:10.088937 snowflake_ai-0.2.0/snowflake_ai/connect/__init__.py
+-rwxr-xr-x   0        0        0     8798 2023-05-20 04:45:57.637455 snowflake_ai-0.2.0/snowflake_ai/connect/authcode_connect.py
+-rwxr-xr-x   0        0        0     3701 2023-05-20 01:16:11.044419 snowflake_ai-0.2.0/snowflake_ai/connect/connect_manager.py
+-rwxr-xr-x   0        0        0     9048 2023-05-15 16:30:51.538940 snowflake_ai-0.2.0/snowflake_ai/connect/dataframe_factory.py
+-rwxr-xr-x   0        0        0     5152 2023-05-05 21:00:10.777186 snowflake_ai-0.2.0/snowflake_ai/connect/file_connect.py
+-rwxr-xr-x   0        0        0    15510 2023-05-14 23:59:19.655555 snowflake_ai-0.2.0/snowflake_ai/connect/snow_connect.py
+-rwxr-xr-x   0        0        0      158 2023-04-17 14:09:36.076455 snowflake_ai-0.2.0/snowflake_ai/mlops/__init__.py
+-rwxr-xr-x   0        0        0     1233 2023-05-05 21:03:32.175401 snowflake_ai-0.2.0/snowflake_ai/mlops/flow_context.py
+-rwxr-xr-x   0        0        0      951 2023-05-01 15:34:06.322421 snowflake_ai-0.2.0/snowflake_ai/mlops/flow_ops.py
+-rwxr-xr-x   0        0        0     2439 2023-05-09 11:59:05.863046 snowflake_ai-0.2.0/snowflake_ai/mlops/flow_pipeline.py
+-rwxr-xr-x   0        0        0     1479 2023-05-01 15:34:17.671701 snowflake_ai-0.2.0/snowflake_ai/mlops/flow_test.py
+-rwxr-xr-x   0        0        0      742 2023-05-22 04:43:32.517483 snowflake_ai-0.2.0/snowflake_ai/mlops/model_dev.py
+-rwxr-xr-x   0        0        0      501 2023-05-01 15:34:30.256772 snowflake_ai-0.2.0/snowflake_ai/mlops/model_serve.py
+-rwxr-xr-x   0        0        0      165 2023-05-21 01:47:43.236204 snowflake_ai-0.2.0/snowflake_ai/snowpandas/__init__.py
+-rwxr-xr-x   0        0        0     8179 2023-05-20 15:35:26.922291 snowflake_ai-0.2.0/snowflake_ai/snowpandas/data_prep.py
+-rwxr-xr-x   0        0        0     3199 2023-05-09 16:36:42.458284 snowflake_ai-0.2.0/snowflake_ai/snowpandas/data_setup.py
+-rwxr-xr-x   0        0        0     1711 2023-05-09 14:38:14.174469 snowflake_ai-0.2.0/snowflake_ai/snowpandas/setup_manager.py
+-rwxr-xr-x   0        0        0    12744 2023-05-21 01:48:22.399687 snowflake_ai-0.2.0/snowflake_ai/snowpandas/snow_encoder.py
+-rwxr-xr-x   0        0        0    19850 2023-05-20 20:33:18.376632 snowflake_ai-0.2.0/snowflake_ai/snowpandas/snow_prep.py
+-rwxr-xr-x   0        0        0     2697 2023-05-09 16:37:09.660283 snowflake_ai-0.2.0/snowflake_ai/snowpandas/snow_setup.py
+-rw-r--r--   0        0        0     3927 1970-01-01 00:00:00.000000 snowflake_ai-0.2.0/PKG-INFO
```

### Comparing `snowflake_ai-0.1.0/README.md` & `snowflake_ai-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
 Snowflake-AI
 =======
 
-*Snowflake_AI* is a Snowflake-centric **Enterprise AI/ML** framework with tight integration of popular Python data science libraries, e.g., *Pandas*, *Scikit-Learn*, *Tensorflow*, *Pytorch*, *MLFlow*, etc. This project simplifies the process of integrating your company's Snowflake data with those popular libraries, making it easier to develop and deploy machine learning models.
+*Snowflake_AI* is a Snowflake-centric **Enterprise AI/ML** framework with tight integration of popular Python data science libraries, e.g., *Pandas*, *Scikit-Learn*, *Tensorflow*, *Pytorch*, *MLFlow*, etc. This project simplifies the process of integrating your company's Snowflake data with those popular libraries, making it easier to develop and deploy machine learning models. Currently, this support OAuth and SAML SSO Snowflake Connection, Streamlit Apps development framework and initial Snowpandas.
 
 Installation
 ------
 
 Before getting started, ensure you have *Poetry* installed on your system. You can install Poetry by following the instructions [here](https://python-poetry.org/docs/).
 
 Next, clone [*this*](https://github.com/tonyxliu/snowflake-ai.git) repository and navigate to the project directory (assume you are in bash terminal):
@@ -26,15 +26,15 @@
 Configuration
 -------
 
 Copy the sample configuration file and update the Snowflake connection parameters:
 
 ```bash
 mkdir -p ~/snowflake_ai/conf
-cp snowflake_ai/conf/app_config.toml ~/snowflake-ai/conf/
+cp snowflake_ai/conf/app_config.toml ~/snowflake_ai/conf/
 ```
 
 Edit snowflake_ai/conf/app_config.toml with your Snowflake connection details.
 
 Usage
 ------
```

### Comparing `snowflake_ai-0.1.0/snowflake_ai/common/dataframe_factory.py` & `snowflake_ai-0.2.0/snowflake_ai/connect/dataframe_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-# Copyright (C) 2023 Tony Liu
+# Copyright (c) 2023, Tony Liu
 #
-# This software may be modified and distributed under the terms
-# of the BSD 3-Clause license. See the LICENSE file for details.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# Use, reproduction and distribution of this software in source and 
+# binary forms, with or without modification, are permitted provided that
+# the License terms and conditions are met; you may not use this file
+# except in compliance with the License. See the LICENSE file for details.
 
 """
 This module contains DataFrameFactory class to create Pandas'
 DataFrame or Snowflake DataFrame depending on context.
 """
 
 __author__ = "Tony Liu"
 __email__ = "tony.liu@yahoo.com"
-__license__ = "BSD 3-Clause"
-__version__ = "0.1.0"
+__license__ = "Apache License 2.0"
+__version__ = "0.2.0"
 
 
 import os
 import logging
 from typing import Optional, List, Tuple, Union, Any, Dict
 
 import numpy as np
@@ -28,89 +31,103 @@
 
 from snowflake.snowpark.dataframe import DataFrame as SDF
 from snowflake.snowpark._internal.analyzer.snowflake_plan_node \
     import LogicalPlan
 from snowflake.snowpark import Session
 from snowflake.snowpark.types import StructType
 
-from snowflake_ai.common import DataConnect, SnowConnect, FileConnect
+from snowflake_ai.common import DataConnect
+from snowflake_ai.connect import SnowConnect, FileConnect
 
 
 
 class DataFrameFactory:
     """
-    This class provides uniform dataframe creation interface to create
+    This class provides an uniform dataframe creation interface to create
     a Pandas DataFrame or Snowflake DataFrame instance depending on the
     input context.
 
     To create a dataframe, construct an appropriate DataConnect object and
-    pass it together with data content to this factory class optionally with
-    corresponding schema.
+    pass it to this factory class together with the data content, optionally
+    supplied with the corresponding schema. Note, you can configure Datasets
+    to directly get snowflake or pandas dataframe without using this factory
+    class.
 
     Example 1:
-        from snowflake_ai.common import DataFrameFactory
-
-        # create snowflake dataframe with SnowConnect
-        sdf = DataFrameFactory.create_df(tbl_name, connect)
+        >>> from snowflake_ai.common import DataFrameFactory
+        ...
+        ... # create snowflake dataframe with SnowConnect
+        >>> sdf = DataFrameFactory.create_df(tbl_name, connect)
 
     Example 2:
-        # create snowflake dataframe with SnowConnect
-        sdf = DataFrameFactory.create_df('select col from tbl', connect)
+        ... # create snowflake dataframe with SnowConnect
+        >>> sdf = DataFrameFactory.create_df('select col from tbl', connect)
         
     Example 3:
-        # create pandas dataframe with FileConnect
-        df = DataFrameFactory.create_df(csv_name, connect)
+        ... # create pandas dataframe with FileConnect
+        >>> df = DataFrameFactory.create_df(csv_name, connect)
 
     Example 4:
-        # create pandas dataframe
-        df = DataFrameFactory.create_df([0, 1, 2], columns=['number'])
+        ... # create pandas dataframe
+        >>> df = DataFrameFactory.create_df([0, 1, 2], columns=['number'])
     """
 
     @classmethod
     def create_df(
         cls,
         data: Any, 
-        connect : Optional[DataConnect],
+        connect : Optional[Union[DataConnect, Session]] = None,
         columns: Optional[
             Union[StructType, Tuple, List[str], Axes, None] 
         ] = None,
         index: Optional[Axes] = None,
         dtype: Optional[Dtype] = None, # type: ignore 
     ) -> Union[SDF, DF]:
         """
         Create a Snowflake specific dataframe or Pandas dataframe depending
         on DataConnect types.
 
         Args:
             data (Any): input Snowflake table/view name, or sql statement,
                 or list, tuple, Pandas dataframe, or LogicalPath
-            session (Session): snowflake session
+            connect (DataConnect): SnowConnect or FileConnect object
             columns (StructType | List | Tuple | Axes): dataframe schema
             index (Axes) : pandas dataframe index
             dtype (Dtype) : pandas dataframe data type
 
         Returns:
             DataFrame: Snowflake or Pandas Dataframe
         """
+        session = None
         if isinstance(connect, SnowConnect):
             session = connect.get_connection()
             col = columns
             if isinstance(columns, tuple) or isinstance(columns, np.ndarray):
                 col = list(columns)
             return cls.create_sdf(data, session, col)  # type: ignore
+        
         elif isinstance(connect, FileConnect):
             conn: FileConnect = connect
             if str(data).strip() == "":
-                return pd.read_csv(conn.connection)
+                return pd.read_csv(conn.current_connection)
             else:
                 f = os.path.join(
-                    os.path.dirname(os.path.abspath(str(conn.connection))), 
+                    os.path.dirname(
+                        os.path.abspath(str(conn.current_connection))
+                    ), 
                     str(data)
                 )
                 return pd.read_csv(f)
+        
+        elif isinstance(connect, Session):
+            col = columns
+            if isinstance(columns, tuple) or isinstance(columns, np.ndarray):
+                col = list(columns)
+            return cls.create_sdf(data, connect, col)  # type: ignore
+        
         else:
             return cls.create_pdf(data, columns, index, dtype) # type: ignore
 
 
     @classmethod
     def create_sdf(
         cls,
@@ -131,18 +148,19 @@
 
         Returns:
             DataFrame: Snowflake Dataframe
         """
 
         if session is None and isinstance(data, SDF):
             return data.__copy__()
+        
         elif session is None and not isinstance(data, SDF):
             raise ValueError(
-                "Creation of Snowflake DataFrame requires "\
-                "Snowflake connection session"
+                "DataframeFactory: Creation of Snowflake DataFrame requires"\
+                " Snowflake connection session."
             )
 
         if session is not None and (
             isinstance(data, List) or isinstance(data, tuple) or
             isinstance(data, DF)
         ):
             if columns is None \
@@ -205,15 +223,15 @@
             dtype (Dtype) : dataframe data type
 
         Returns:
             DataFrame: Pandas Dataframe
         """
 
         logger = logging.getLogger(cls.__name__)
-        df = DF()
+        df = DF(data={}, columns=[])
         
         if isinstance(data, SDF):
             df = data.to_pandas()
 
         elif isinstance(data, DF):
             df = data.copy()
             
@@ -222,15 +240,15 @@
             
             if columns is None or isinstance(columns, np.ndarray) or \
                     isinstance(columns, List) or isinstance(columns, tuple):
                 df = cls._create_df(data, index, columns)
 
         else:
             logger.warn(
-                f"SnowDataFrame is initialized with empty Pandas Dataframe"
+                f"Initialization with empty Pandas Dataframe"
             )    
             
         return df
     
 
     @classmethod
     def _create_df(
@@ -243,11 +261,11 @@
     ) -> pd.DataFrame:
         rdf = pd.DataFrame()
         logger = logging.getLogger(cls.__name__)
         try:
             rdf = pd.DataFrame(data, index, columns, dtype, copy)
         except Exception as e:
             logger.exception(
-                "Exception occured in _create_df() when creating "\
-                f"local pandas dataframe: {e}"
+                "DataFrameFactory.create_df(): Exception occured when "\
+                f"creating local pandas dataframe - {e}"
             )
         return rdf
```

### Comparing `snowflake_ai-0.1.0/snowflake_ai/common/snow_connect.py` & `snowflake_ai-0.2.0/snowflake_ai/connect/snow_connect.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,168 +1,249 @@
-# Copyright (C) 2023 Tony Liu
+# Copyright (c) 2023, Tony Liu
 #
-# This software may be modified and distributed under the terms
-# of the BSD 3-Clause license. See the LICENSE file for details.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# Use, reproduction and distribution of this software in source and 
+# binary forms, with or without modification, are permitted provided that
+# the License terms and conditions are met; you may not use this file
+# except in compliance with the License. See the LICENSE file for details.
 
 """
 This module contains SnowConnect class representing a specific Snowflake
 connection.
 """
 
 __author__ = "Tony Liu"
 __email__ = "tony.liu@yahoo.com"
-__license__ = "BSD 3-Clause"
-__version__ = "0.1.0"
+__license__ = "Apache License 2.0"
+__version__ = "0.2.0"
 
 
 import os
+import sys
 import logging
 import types
-from typing import List, Dict, Optional, Union, Iterator
+from typing import List, Dict, Iterator, Optional
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 
 from pandas import DataFrame as DF
 
 from snowflake.snowpark import Session
 from snowflake.snowpark import Row
 from snowflake.snowpark import DataFrame as SDF
 
-from snowflake_ai.common import DataConnect
+from snowflake_ai.common import AppConfig, AppConnect, DataConnect
 
 
 
 class SnowConnect(DataConnect):
     """
     This class provides specific Snowflake connection.
 
     Example:
 
     To use this class, just instantiate SnowConnect as follows:
 
-        from snowflake_ai.common import SnowConnect
-
-        connect: SnowConnect = SnowConnect()
-        session = connect.get_session()
+        >>> from snowflake_ai.common import SnowConnect
+        ... 
+        >>> connect: SnowConnect = SnowConnect()
+        >>> session = connect.get_session()
     """
 
+    T_SNOWFLAKE_CONN = AppConnect.T_SNOWFLAKE_CONN
+    T_AUTH_SNOWFLAKE = AppConnect.T_AUTH_SNOWFLAKE
+    T_AUTH_KEYPAIR = AppConnect.T_AUTH_KEYPAIR
+    T_AUTH_EXT_BROWSER = AppConnect.T_AUTH_EXT_BROWSER
+    T_AUTH_OAUTH = AppConnect.T_AUTH_OAUTH
+
     _logger = logging.getLogger(__name__)
+    _logger.addHandler(logging.StreamHandler(sys.stdout))
 
 
-    def __init__(
-        self,
-        config_dir : Optional[Union[str, None]] = None, 
-        config_file : Optional[Union[str, None]] = None
-    ):
-        super().__init__(config_dir, config_file)
+    def __init__(self, connect_key : Optional[str] = None):
+        super().__init__(connect_key)
         self.logger = SnowConnect._logger
-        self.session = self.get_session()
-
-        # add Snowflake Session methods
-        for method_name in dir(self.session):
-            if not method_name.startswith('_'):
-                method = getattr(self.session, method_name)
-                if isinstance(method, types.MethodType):
-                    setattr(self, method_name, method)
-    
-
-
-
-    def get_session(self) -> Session:
-        """
-        Get this snowflake connection's session. If there is no existing
-        session exists, create a new session.
-
-        Returns:
-            Session: Snowflake connection's session
-        """
-        if not hasattr(self, 'session') or self.session is None:
-            conn = self.get_connection()
-            if (conn is None) or (not isinstance(conn, Session)):
-                raise ValueError(
-                    "SnowConnect.get_session(): "\
-                    "Initialization error, cannot get Session"
-                )
-            self.session = conn
-        return self.session
-    
-
-    def close_session(self):
-        """
-        Close current snowflake connection and session.
-        """
-        self.close_connection()
-
-
-    def close_connection(self) -> int:
-        """
-        Close current snowflake connection and session.
-        """
-        if self.session is not None:
-            self.session.close()
-        return 0
+        
+        if not (self.connect_group == DataConnect.K_DATA_CONN and \
+                self.connect_params):
+            self.logger.error(
+                f"SnowConnect.init(): ConnectType => {self.connect_type};"\
+                f"ConnectGroup => {self.connect_group}; ConnectName => "\
+                f"{self.connect_name}"
+            )
+            raise ValueError(
+                "SnowConnect.init(): SnowConnect configuration Error!"
+            )
+        if (not self.connect_type) or (
+            self.connect_type != AppConfig.T_SNOWFLAKE_CONN
+        ):
+            raise ValueError(
+                f"SnowConnect.init(): Type [{self.connect_type}] Error"
+            )
 
 
     def create_connection(self, params: Dict):
         """
         Create a snowflake connection based on the specific configuration.
         A set of authentication types are supported:
-            snowflake, keypair, oauth (to-do) and externalbrowser (to-do)
+            snowflake, keypair, oauth and externalbrowser
+        Note, user specific connection would be session.
 
         Args:
             params (Dict): Configuration dictionary as input parameters.
 
         Returns:
             object: snowflake connection session
         """
         if params is None:
             raise ValueError(
                 f"SnowConnect.create_connection params cannot be None"
             )
-        auth = ""
+        session = None
         try:
-            auth = params["auth_type"]
-            if auth == "snowflake":
-                self.session = self._do_snowflake_auth(params)
-            elif auth == "keypair":
-                self.logger.debug(f"keypair auth => {params}")
-                self.session = self._do_keypair_auth(params)
-            elif auth == "externalbrowser":
-                self.session = self._do_externalbrowser_auth(params)
-            elif auth == "oauth":
-                self.session = self._do_oauth_auth(params)
+            auth = params[AppConfig.K_AUTH_TYPE]
+            if auth == AppConnect.T_AUTH_SNOWFLAKE:
+                session = self._do_snowflake_auth(params)
+            elif auth == AppConnect.T_AUTH_KEYPAIR:
+                session = self._do_keypair_auth(params)
+            elif auth == AppConnect.T_AUTH_EXT_BROWSER: 
+                # cannot create shared connection
+                self.logger.warning(
+                    "SnowConnect.create_connection(): use create_session "\
+                    "to create externalbrowser enabled connection."
+                )
+            elif auth == AppConnect.T_AUTH_OAUTH:
+                # cannot create shared connection
+                self.logger.warning(
+                    "SnowConnect.create_connection(): use create_session "\
+                    "to create oauth enabled connection."
+                )
         except Exception as e:
             self.logger.exception(
                 f"SnowConnect.create_connection cannot use "\
                 f"auth_type={auth} to creaet snowflake session: {e}"
             )
-        return self.session
+        return session
+
+
+    def get_connection(self, connect_key: Optional[str] = None):
+        """
+        Get lazy created snowflake shared connection.
+
+        Args:
+            connect_key (str): data connect key.
+
+        Returns:
+            object: snowflake connection object, i.e., snowflake session
+        """
+        conn = super().get_connection(connect_key)
+        if conn is not None and (
+            (self.connect_params["type"] != SnowConnect.T_SNOWFLAKE_CONN) \
+            or (not isinstance(conn, Session))
+        ):
+            raise TypeError(
+                f"SnowConnect.get_connection(): Type Error {connect_key}"
+            )
+        return conn
+
+
+    def is_current_active(self) -> bool:
+        """
+        Check whether current Snowflake connection (shared session) is
+        still active or not. 
+        
+        Returns:
+            bool: True if the connection is active, otherwise False
+        """
+        rb = super().is_current_active()
+        try:
+            r = self.dql("select current_role()")           
+            try:
+                pd = next(r)
+                self.logger.info(
+                    "SnowConnect.is_current_active(): Active "
+                    f"connection using role [{pd}]"
+                )
+                if DF(pd).shape[0] > 0:
+                    rb = True
+            except Exception as ee:
+                self.logger.warning(
+                    "SnowConnect.is_current_active(): No Result "\
+                    f"returned [{ee}]"
+                )            
+        except Exception as e:
+            self.logger.warning(
+                f"SnowConnect.is_current_active(): Warning {e}"
+            )
+        return rb
+    
+
+    def create_session(self, ctx: Optional[Dict] = {}) -> Session:
+        """
+        Create snowflake user connection session, or get the existing
+        shared data connection.
+
+        Returns:
+            Session: Snowflake connection's session
+        """
+        conn = self.get_connection()
+        if (conn is not None) and isinstance(conn, Session):
+            return conn
+        else:
+            conn = self.create_connection(self.connect_params)
+        session = conn
+        if session is None:
+            if self.auth_type == self.T_AUTH_EXT_BROWSER:
+                session = self._do_externalbrowser_auth(self.connect_params)
+            elif self.auth_type == self.T_AUTH_OAUTH:
+                session = self._do_oauth(self.connect_params, ctx)
+        return session
+    
+
+    def close_session(self):
+        """
+        Close current snowflake connection and session.
+        """
+        self.close_connection()
+
+
+    def _create_session(self, auth_type: str, conn_params) -> Session:
+        try:
+            session = Session.builder.configs(conn_params).create() 
+            c = session.sql("select current_warehouse(), current_role()")\
+                .collect()
+            self.logger.info(
+                "SnowConnect._create_session() Creation of connection [OK]"\
+                f"Warehouse, Role => {c}"
+            )
+        except Exception as ex:
+            self.logger.exception(
+                "SnowConnect._create_session() Cannot connect to snowflake"\
+                f" Error: {ex} with Auth_Type: {auth_type}"
+            )
+        return session
 
 
     def _do_snowflake_auth(self, params):
         pass_env: str = params["password_env"]
         password = os.environ[pass_env]
-        session = None
         conn_params = {
             "account": params["account"],
             "user": params["user"],
-            "authenticator": "snowflake",
+            "authenticator": self.T_AUTH_SNOWFLAKE,
             "password": password,
             "role": params["role"], 
             "warehouse": params["warehouse"],
             "database": params["database"],
             "schema": params["schema"]
         }
-        try:
-            session = Session.builder.configs(conn_params).create() 
-        except Exception as e:
-            self.logger.exception(
-                f"Cannot connect to snowflake using _do_snowflake_auth(): {e}")
-        return session
+        return self._create_session(
+            SnowConnect.T_AUTH_SNOWFLAKE, conn_params
+        )
 
 
     def _do_keypair_auth(self, params):
         session, pkey, pkb, conn_params = None, None, bytes(), None
         kphrase_env = params["private_key_phrase_env"]
         kphrase = os.environ[kphrase_env]
         kpath_env = params["private_key_path_env"]
@@ -198,44 +279,69 @@
             conn_params = {
                 "account": params["account"],
                 "user": params["user"],
                 "private_key": pkb,
                 "role": params["role"], 
                 "warehouse": params["warehouse"],
                 "database": params["database"],
-                "schema": params["schema"]
+                "schema": params["schema"],
+                "client_session_keep_alive": True,
+                "max_connection_pool" : 20
             }
-            try:
-                session = Session.builder.configs(conn_params).create() 
-                c = session.sql("select current_warehouse(), current_role()")\
-                    .collect()
-                self.logger.info(f"Snowflake connection [OK] => {c}")
-            except Exception as ex:
-                self.logger.exception(
-                    "Cannot connect to snowflake using keyair auth in "\
-                    f"_do_keypair_auth(): {ex}"
-                )
+            session = self._create_session(
+                SnowConnect.T_AUTH_KEYPAIR, conn_params
+            )
         else: 
             raise ValueError(
                 "Cannot read snowflake user private key bytes in "\
-                "_do_keypair_auth()"
+                "SnowConnect._do_keypair_auth()"
             )
         return session
 
 
     def _do_externalbrowser_auth(self, params):
-        pass
-
+        conn_params = {
+            "account": params["account"],
+            "user": params["user"],
+            "authenticator": self.T_AUTH_EXT_BROWSER,
+            "role": params["role"], 
+            "warehouse": params["warehouse"],
+            "database": params["database"],
+            "schema": params["schema"]
+        }
+        return self._create_session(
+            SnowConnect.T_AUTH_EXT_BROWSER, conn_params
+        )
 
-    def _do_oauth_auth(self, params):
-        # TO-DO
-        pass
 
+    def _do_oauth(self, params, ctx: Dict):
+        token = ctx.get("access_token")
+        dtok = ctx.get("decoded_access_token")
+
+        if dtok is not None and dtok:
+            upn:str = dict(dtok).get("upn")
+            upn = upn.upper()
+        
+            conn_params = {
+                "account": params["account"],
+                "user": upn,
+                "authenticator": AppConnect.T_AUTH_OAUTH,
+                "token" : token,
+                "role": params["role"], 
+                "warehouse": params["warehouse"],
+                "database": params["database"],
+                "schema": params["schema"]
+            }
+            return self._create_session(
+                self.T_AUTH_OAUTH, conn_params
+            )
+    
 
-    def ddl(self, sql: str) -> List[Row]:
+    @staticmethod
+    def ddl(session: Session, sql: str) -> List[Row]:
         """
         Excute Data Definition Language statement in Snowflake
         Args:
             sql (str): sql statement string
 
         Returns:
             List[Row]: list of Snowflake Snowpark Rows
@@ -246,54 +352,57 @@
             'set', 'unset'
         }
         matches = [c for c in cmds if sql.upper().startswith(c.upper())]
         if not matches:
             raise ValueError(
                 f"SnowConnect.ddl(): input sql doesn't seem to be DDL [{sql}]"
             )             
-        return self.get_session().sql(sql).collect()
+        return session.sql(sql).collect()
 
 
-    def dml(self, sql: str) -> List[Row]:
+    @staticmethod
+    def dml(session: Session, sql: str) -> List[Row]:
         """
         Excute Data Manupilation Language statement in Snowflake
         Args:
             sql (str): sql statement string
 
         Returns:
             List[Row]: list of Snowflake Snowpark Rows
         """
         cmds =  {'insert', 'update', 'delete', 'call', 'explain'}
         matches = [c for c in cmds if sql.upper().startswith(c.upper())]
         if not matches:
             raise ValueError(
                 f"SnowConnect.dml(): input sql doesn't seem to be DML [{sql}]"
             )             
-        return self.get_session().sql(sql).collect()
+        return session.sql(sql).collect()
 
-    
-    def tcl(self, sql: str) -> List[Row]:
+
+    @staticmethod    
+    def tcl(session: Session, sql: str) -> List[Row]:
         """
         Excute Tranction Control Language statement in Snowflake
         Args:
             sql (str): sql statement string
 
         Returns:
             List[Row]: list of Snowflake Snowpark Rows
         """
         cmds =  {'begin', 'commit', 'rollback', 'savepoint', 'release'}
         matches = [c for c in cmds if sql.upper().startswith(c.upper())]
         if not matches:
             raise ValueError(
                 f"SnowConnect.tcl(): input sql doesn't seem to be TCL [{sql}]"
             )             
-        return self.get_session().sql(sql).collect()
+        return session.sql(sql).collect()
 
-    
-    def dcl(self, sql: str) -> List[Row]:
+
+    @staticmethod    
+    def dcl(session: Session, sql: str) -> List[Row]:
         """
         Excute Data Control Language statement in Snowflake
         Args:
             sql (str): sql statement string
 
         Returns:
             List[Row]: list of Snowflake Snowpark Rows
@@ -303,44 +412,46 @@
             'desc', 'set', 'unset'
         }
         matches = [c for c in cmds if sql.upper().startswith(c.upper())]
         if not matches:
             raise ValueError(
                 f"SnowConnect.dcl(): input sql doesn't seem to be DCL [{sql}]"
             )             
-        return self.get_session().sql(sql).collect()
+        return session.sql(sql).collect()
     
 
-    def dql(self, sql: str) -> Iterator[DF]:
+    @staticmethod
+    def dql(session: Session, sql: str) -> Iterator[DF]:
         """
         Excute Data Query Language (Select) statement in Snowflake
         Args:
             sql (str): sql statement string
 
         Returns:
             Iterator[DF]: Iterator of Pandas DataFrame list
         """
         cmds =  {'select'}
         matches = [c for c in cmds if sql.upper().startswith(c.upper())]
         if not matches:
             raise ValueError(
                 f"SnowConnect.dql(): input sql doesn't seem to be DQL [{sql}]"
             )             
-        return self.get_session().sql(sql).to_pandas_batches()
+        return session.sql(sql).to_pandas_batches()
     
 
-    def sdf(self, sql: str) -> SDF:
+    @staticmethod
+    def sdf(session: Session, sql: str) -> SDF:
         """
         Excute Data Query Language (Select) statement in Snowflake
         Args:
             sql (str): sql statement string
 
         Returns:
             Dataframe: Snowflake Dataframe as result of the query
         """
         cmds =  {'select'}
         matches = [c for c in cmds if sql.upper().startswith(c.upper())]
         if not matches:
             raise ValueError(
                 f"SnowConnect.sdf(): input sql doesn't seem to be DQL [{sql}]"
             )
-        return self.get_session().sql(sql).to_df()
+        return session.sql(sql).to_df()
```

### Comparing `snowflake_ai-0.1.0/snowflake_ai/mlops/flow_context.py` & `snowflake_ai-0.2.0/snowflake_ai/mlops/flow_context.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-# Copyright (C) 2023 Tony Liu
+# Copyright (c) 2023, Tony Liu
 #
-# This software may be modified and distributed under the terms
-# of the BSD 3-Clause license. See the LICENSE file for details.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# Use, reproduction and distribution of this software in source and 
+# binary forms, with or without modification, are permitted provided that
+# the License terms and conditions are met; you may not use this file
+# except in compliance with the License. See the LICENSE file for details.
 
 """
 This module contains FlowContext class representing the context
 of MLOps flow
 """
 
 __author__ = "Tony Liu"
 __email__ = "tony.liu@yahoo.com"
-__license__ = "BSD 3-Clause"
-__version__ = "0.1.0"
+__license__ = "Apache License 2.0"
+__version__ = "0.2.0"
 
 
 import logging
 
 
 
 class FlowContext:
@@ -25,17 +28,17 @@
     historical context sequence), current output, and related
     metadata.
 
     Example:
 
     To use this class, instantiate the initial context:
 
-        from snowflake_ai.mlops import FlowContext
-
-        ctx: FlowContext = FlowContext()
+        >>> from snowflake_ai.mlops import FlowContext
+        ... 
+        >>> ctx: FlowContext = FlowContext()
     """
 
     def __init__(self) -> None:
         self.logger = logging.getLogger(__name__)
         self.direct_input = {}
         self.context_input = []
         self.output = {}
```

### Comparing `snowflake_ai-0.1.0/snowflake_ai/mlops/flow_test.py` & `snowflake_ai-0.2.0/snowflake_ai/mlops/flow_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-#!/usr/bin/env python3
-# Copyright (C) 2023 Tony Liu
+# Copyright (c) 2023, Tony Liu
 #
-# This software may be modified and distributed under the terms
-# of the BSD 3-Clause license. See the LICENSE file for details.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# Use, reproduction and distribution of this software in source and 
+# binary forms, with or without modification, are permitted provided that
+# the License terms and conditions are met; you may not use this file
+# except in compliance with the License. See the LICENSE file for details.
 
 """
 This module contains FlowTest class for testing ML flow targeting
 test/stage domain/environment
 """
 
 __author__ = "Tony Liu"
 __email__ = "tony.liu@yahoo.com"
-__license__ = "BSD 3-Clause"
-__version__ = "0.1.0"
+__license__ = "Apache License 2.0"
+__version__ = "0.2.0"
 
 
 from snowflake_ai.mlops import Pipeline
 
 
 class FlowTest(Pipeline):
     """
```

### Comparing `snowflake_ai-0.1.0/snowflake_ai/snowpandas/data_setup.py` & `snowflake_ai-0.2.0/snowflake_ai/snowpandas/data_setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,115 @@
-# Copyright (C) 2023 Tony Liu
+# Copyright (c) 2023, Tony Liu
 #
-# This software may be modified and distributed under the terms
-# of the BSD 3-Clause license. See the LICENSE file for details.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# Use, reproduction and distribution of this software in source and 
+# binary forms, with or without modification, are permitted provided that
+# the License terms and conditions are met; you may not use this file
+# except in compliance with the License. See the LICENSE file for details.
 
 """
 This module contains DataSetup class for setting-up, initialization,
 configuration, and tearing-down of data Environment
 """
 
 __author__ = "Tony Liu"
 __email__ = "tony.liu@yahoo.com"
-__license__ = "BSD 3-Clause"
-__version__ = "0.1.0"
+__license__ = "Apache License 2.0"
+__version__ = "0.2.0"
 
 
-from typing import Optional
+from typing import Optional, Dict
 from pandas import DataFrame as DF
 
-from snowflake_ai.common import DataConnect, FileConnect, DataFrameFactory
+from snowflake_ai.common import DataConnect
+from snowflake_ai.connect import FileConnect, \
+    SnowConnect, DataFrameFactory
 
 
 
 class DataSetup:
     """
     This class sets up, initializes, configures or tears down
     the data Environment
 
     To use this class, instantiate DataSetup with appropriate DataConnect
     as follows:
 
-        from snowflake_ai.common import FileConnect
-        from snowflake_ai.snowpandas import DataSetup
-
-        conn: FileConnect = FileConnect()
-        setup: DataSetup = DataSetup(conn)
-        df = setup.load_data()
+        >>> from snowflake_ai.common import FileConnect
+        >>> from snowflake_ai.snowpandas import DataSetup
+        ... 
+        >>> conn: FileConnect = FileConnect()
+        >>> setup: DataSetup = DataSetup(conn)
+        >>> df = setup.load_data()
     """
+    def __init__(
+        self, 
+        datasetup_key: str,
+        connect: DataConnect, 
+        data: Optional[Dict[str, DF]] = {}
+    ) -> None:
+        self.datasetup_key = datasetup_key
+        self._connect = connect
+        self._data = data
+        if data is not None:
+            self._data = data
 
-    def __init__(self, connect: DataConnect) -> None:
-        self.__connect = connect
-
-    
 
-    def get_connection(self) -> DataConnect:
+    def get_connect(self) -> DataConnect:
         """
         Get the data connection for the setup.
 
         Returns:
             DataConnect: data connection object for the setup
         """        
-        return self.__connect
+        return self._connect
     
 
     def load_data(self, file_name: Optional[str] = None) -> DF:
         """
         Load pandas dataframe from local-csv file connection.
 
         Returns:
             DataFrame: Pandas dataframe
         """
-        if isinstance(self.__connect, FileConnect):
+        if isinstance(self._connect, FileConnect):
             if (file_name is None) or (file_name.strip() == ""):
-                return DataFrameFactory.create_df(
-                    "", self.__connect
-                )  # type: ignore
+                return DataFrameFactory.create_pdf(
+                    "", self._connect
+                )
             else:
-                df: DF = DataFrameFactory.create_df(
-                    file_name, self.__connect
-                )  # type: ignore
+                df: DF = DataFrameFactory.create_pdf(
+                    file_name, self._connect
+                )
+                
                 df.columns = df.columns.str.strip().str.lower()\
                     .str.replace(' ', '_')
                 return df
+        elif isinstance(self._connect, SnowConnect):
+            pass
         else:
             raise ValueError(
                 "DataSetup Error. Loading File requires FileConnect"
             )
 
 
+    def _load_file_data(self):
+        pass
+
+
+    def _load_snowflake_data(self):
+        pass
+
+
+    def get_data(self) -> Dict[str, DF]:
+        """
+        Get all dataframes for exploration and preparation.
+
+        Returns:
+            Dict: dictionary of dataframes
+        """
+        return self._data
+
+
     def clean_data(self, file_name: Optional[str] = None):
-        # TO-DO: clean up file
-        pass
+        self._data = {}
+        self._connect.close_connection()
```

### Comparing `snowflake_ai-0.1.0/snowflake_ai/snowpandas/snow_setup.py` & `snowflake_ai-0.2.0/snowflake_ai/snowpandas/snow_setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,71 @@
-# Copyright (C) 2023 Tony Liu
+# Copyright (c) 2023, Tony Liu
 #
-# This software may be modified and distributed under the terms
-# of the BSD 3-Clause license. See the LICENSE file for details.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# Use, reproduction and distribution of this software in source and 
+# binary forms, with or without modification, are permitted provided that
+# the License terms and conditions are met; you may not use this file
+# except in compliance with the License. See the LICENSE file for details.
 
 """
 This module contains SnowSetup class specific for setting-up, 
 initialization, configuration, and tearing-down of Snowflake environment
 """
 
 __author__ = "Tony Liu"
 __email__ = "tony.liu@yahoo.com"
-__license__ = "BSD 3-Clause"
-__version__ = "0.1.0"
+__license__ = "Apache License 2.0"
+__version__ = "0.2.0"
 
 
-from typing import Optional
-from snowflake_ai.common import SnowConnect
+from typing import Optional, Dict, Optional
+from snowflake.snowpark import DataFrame as SDF
+
+from snowflake_ai.common import AppConfig
+from snowflake_ai.connect import SnowConnect
 from snowflake_ai.snowpandas import DataSetup
 
 
 
 class SnowSetup(DataSetup):
     """
     This class extends DataSetup for setting-up, initialization,
     configuration, and tearing-down Snowflake specific Environment.
 
     To use this class, instantiate SnowSetup with SnowConnect as follows:
 
-        from snowflake_ai.common import SnowConnect
-        from snowflake_ai.snowpandas import SnowSetup
-
-        conn: SnowConnect = SnowConnect()
-        setup: SnowSetup = SnowSetup(conn)
-        setup.create_stage()
+        >>> from snowflake_ai.common import SnowConnect
+        >>> from snowflake_ai.snowpandas import SnowSetup
+        ... 
+        >>> conn: SnowConnect = SnowConnect()
+        >>> setup: SnowSetup = SnowSetup(conn)
+        >>> setup.create_stage()
     """
+    def __init__(
+            self, datasetup_key: str, 
+            connect: SnowConnect,
+            data: Optional[Dict[str, SDF]] = {}
+    ) -> None:
+        super().__init__(
+            datasetup_key, 
+            connect, 
+            {key: sdf.to_pandas() for key, sdf in data.items()}
+        )
+        self._snow_dfs = data
 
-    def __init__(self, connect: SnowConnect) -> None:
-        super().__init__(connect)
 
-    
-    def get_connection(self) -> SnowConnect:
+    def get_connect(self) -> SnowConnect:
         """
         Get snowflake connection for the setup.
 
         Returns:
             SnowConnect: Snowflake data connection
         """
-        if isinstance(self.__connect, SnowConnect):
-            return self.__connect
+        if isinstance(self._connect, SnowConnect):
+            return self._connect
         else:
             raise TypeError(
                 "SnowSetup should be initialized with SnowConnect"
             )
 
 
     def create_stage(
@@ -65,24 +79,11 @@
         Args:
             stage_name (str): snowflake stage name. if none or empty,
                 use SnowConnect config parameter     
 
         Returns:
             None: succesful creation of snowflake stage
         """
-        if (stage_name is None) or (not stage_name):
-            snow_conn = self.get_connection()
-            stage_keys = [
-                k for k in snow_conn.configs["data"]["connect"]\
-                    [snow_conn.curr_conn_name]["data_setup"].keys() \
-                    if str(k).lower().startswith("stage")
-            ]
-            for sk in stage_keys:
-                stage_name = snow_conn.configs["data"]["connect"]\
-                    [snow_conn.curr_conn_name]["data_setup"][sk]
-                ddl = f"CREATE STAGE IF NOT EXISTS {stage_name}"
-                self.get_connection().ddl(ddl)
-        else:
+        if (stage_name is not None) and (stage_name):
             ddl = f"CREATE STAGE IF NOT EXISTS {stage_name}"
-            self.get_connection().ddl(ddl)
+            self.get_connect().ddl(ddl)
         
-
```

### Comparing `snowflake_ai-0.1.0/PKG-INFO` & `snowflake_ai-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,49 @@
 Metadata-Version: 2.1
 Name: snowflake-ai
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Snowflake centic Enterprise AI/ML framework with tight integration of popular data science libraries
 Home-page: https://github.com/tonyxliu/snowflake-ai#readme
 License: BSD-3-Clause
 Keywords: AI,ML,Snowflake,Enterprise,AI/ML
 Author: Tony Liu
 Author-email: tony.liu@yahoo.com
-Requires-Python: >=3.8.15,<3.9.0
+Requires-Python: >=3.8.10,<3.9.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: altair (==4.1.0)
+Requires-Dist: charset-normalizer (==2.0.4)
+Requires-Dist: click (==8.0.4)
 Requires-Dist: cryptography (>=40.0.1,<40.1.0)
 Requires-Dist: importlib-resources (>=5.12.0,<5.13.0)
+Requires-Dist: markupsafe (==2.1.1)
 Requires-Dist: matplotlib (>=3.7.1,<3.8.0)
-Requires-Dist: numpy (>=1.24.2,<1.25.0)
-Requires-Dist: pandas (>=1.5.2,<1.6.0)
-Requires-Dist: scikit-learn (>=1.2.2,<1.3.0)
-Requires-Dist: snowflake-connector-python (>=3.0.2,<3.1.0)
-Requires-Dist: snowflake-snowpark-python (>=1.2.0,<1.3.0)
+Requires-Dist: mpld3 (>=0.5.7,<0.6.0)
+Requires-Dist: numpy (==1.23.5)
+Requires-Dist: pandas (==1.5.3)
+Requires-Dist: protobuf (==3.19.6)
+Requires-Dist: pyjwt (==2.7.0)
+Requires-Dist: pytz (==2022.7)
+Requires-Dist: requests (==2.28.1)
+Requires-Dist: scikit-learn (==1.2.2)
+Requires-Dist: snowflake-connector-python[pandas] (==3.0.3)
+Requires-Dist: snowflake-snowpark-python (>=1.3.0,<1.4.0)
+Requires-Dist: streamlit (>=1.18.0,<1.19.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 
 Snowflake-AI
 =======
 
-*Snowflake_AI* is a Snowflake-centric **Enterprise AI/ML** framework with tight integration of popular Python data science libraries, e.g., *Pandas*, *Scikit-Learn*, *Tensorflow*, *Pytorch*, *MLFlow*, etc. This project simplifies the process of integrating your company's Snowflake data with those popular libraries, making it easier to develop and deploy machine learning models.
+*Snowflake_AI* is a Snowflake-centric **Enterprise AI/ML** framework with tight integration of popular Python data science libraries, e.g., *Pandas*, *Scikit-Learn*, *Tensorflow*, *Pytorch*, *MLFlow*, etc. This project simplifies the process of integrating your company's Snowflake data with those popular libraries, making it easier to develop and deploy machine learning models. Currently, this support OAuth and SAML SSO Snowflake Connection, Streamlit Apps development framework and initial Snowpandas.
 
 Installation
 ------
 
 Before getting started, ensure you have *Poetry* installed on your system. You can install Poetry by following the instructions [here](https://python-poetry.org/docs/).
 
 Next, clone [*this*](https://github.com/tonyxliu/snowflake-ai.git) repository and navigate to the project directory (assume you are in bash terminal):
@@ -52,15 +62,15 @@
 Configuration
 -------
 
 Copy the sample configuration file and update the Snowflake connection parameters:
 
 ```bash
 mkdir -p ~/snowflake_ai/conf
-cp snowflake_ai/conf/app_config.toml ~/snowflake-ai/conf/
+cp snowflake_ai/conf/app_config.toml ~/snowflake_ai/conf/
 ```
 
 Edit snowflake_ai/conf/app_config.toml with your Snowflake connection details.
 
 Usage
 ------
```

