# Comparing `tmp/zash-sdk-0.0.8.tar.gz` & `tmp/zash-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zash-sdk-0.0.8.tar", last modified: Mon Jan  9 23:17:49 2023, max compression
+gzip compressed data, was "zash-sdk-0.0.9.tar", last modified: Mon Jan 23 23:59:03 2023, max compression
```

## Comparing `zash-sdk-0.0.8.tar` & `zash-sdk-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2023-01-09 23:17:49.582494 zash-sdk-0.0.8/
--rw-rw-r--   0 efes       (501) staff       (20)    11337 2022-08-18 19:39:58.000000 zash-sdk-0.0.8/LICENSE
--rw-rw-r--   0 efes       (501) staff       (20)      111 2022-08-18 19:39:58.000000 zash-sdk-0.0.8/MANIFEST.in
--rw-r--r--   0 efes       (501) staff       (20)    19267 2023-01-09 23:17:49.582277 zash-sdk-0.0.8/PKG-INFO
--rw-rw-r--   0 efes       (501) staff       (20)    18538 2022-09-08 14:57:27.000000 zash-sdk-0.0.8/README.md
--rw-r--r--   0 efes       (501) staff       (20)      843 2023-01-09 23:17:27.000000 zash-sdk-0.0.8/settings.ini
--rw-r--r--   0 efes       (501) staff       (20)       38 2023-01-09 23:17:49.582541 zash-sdk-0.0.8/setup.cfg
--rw-rw-r--   0 efes       (501) staff       (20)     2541 2022-08-18 19:39:58.000000 zash-sdk-0.0.8/setup.py
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2023-01-09 23:17:49.581166 zash-sdk-0.0.8/zash_sdk/
--rw-r--r--   0 efes       (501) staff       (20)       22 2023-01-09 23:17:27.000000 zash-sdk-0.0.8/zash_sdk/__init__.py
--rw-r--r--   0 efes       (501) staff       (20)     9793 2023-01-09 23:17:27.000000 zash-sdk-0.0.8/zash_sdk/_modidx.py
--rw-r--r--   0 efes       (501) staff       (20)    11067 2023-01-09 23:17:27.000000 zash-sdk-0.0.8/zash_sdk/collection.py
--rw-r--r--   0 efes       (501) staff       (20)     7058 2023-01-09 23:17:27.000000 zash-sdk-0.0.8/zash_sdk/connectors.py
--rw-r--r--   0 efes       (501) staff       (20)      648 2023-01-09 23:17:27.000000 zash-sdk-0.0.8/zash_sdk/graph.py
--rw-r--r--   0 efes       (501) staff       (20)     2135 2023-01-09 23:17:27.000000 zash-sdk-0.0.8/zash_sdk/nft.py
--rw-r--r--   0 efes       (501) staff       (20)      929 2023-01-09 23:17:27.000000 zash-sdk-0.0.8/zash_sdk/zash.py
-drwxr-xr-x   0 efes       (501) staff       (20)        0 2023-01-09 23:17:49.582088 zash-sdk-0.0.8/zash_sdk.egg-info/
--rw-r--r--   0 efes       (501) staff       (20)    19267 2023-01-09 23:17:49.000000 zash-sdk-0.0.8/zash_sdk.egg-info/PKG-INFO
--rw-r--r--   0 efes       (501) staff       (20)      414 2023-01-09 23:17:49.000000 zash-sdk-0.0.8/zash_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 efes       (501) staff       (20)        1 2023-01-09 23:17:49.000000 zash-sdk-0.0.8/zash_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 efes       (501) staff       (20)       38 2023-01-09 23:17:49.000000 zash-sdk-0.0.8/zash_sdk.egg-info/entry_points.txt
--rw-r--r--   0 efes       (501) staff       (20)        1 2022-08-23 16:52:00.000000 zash-sdk-0.0.8/zash_sdk.egg-info/not-zip-safe
--rw-r--r--   0 efes       (501) staff       (20)       84 2023-01-09 23:17:49.000000 zash-sdk-0.0.8/zash_sdk.egg-info/requires.txt
--rw-r--r--   0 efes       (501) staff       (20)        9 2023-01-09 23:17:49.000000 zash-sdk-0.0.8/zash_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2023-01-23 23:59:03.450541 zash-sdk-0.0.9/
+-rw-rw-r--   0 efes       (501) staff       (20)    11337 2022-08-18 19:39:58.000000 zash-sdk-0.0.9/LICENSE
+-rw-rw-r--   0 efes       (501) staff       (20)      111 2022-08-18 19:39:58.000000 zash-sdk-0.0.9/MANIFEST.in
+-rw-r--r--   0 efes       (501) staff       (20)    19267 2023-01-23 23:59:03.450345 zash-sdk-0.0.9/PKG-INFO
+-rw-rw-r--   0 efes       (501) staff       (20)    18538 2022-09-08 14:57:27.000000 zash-sdk-0.0.9/README.md
+-rw-r--r--   0 efes       (501) staff       (20)      843 2023-01-23 23:58:55.000000 zash-sdk-0.0.9/settings.ini
+-rw-r--r--   0 efes       (501) staff       (20)       38 2023-01-23 23:59:03.450578 zash-sdk-0.0.9/setup.cfg
+-rw-rw-r--   0 efes       (501) staff       (20)     2541 2022-08-18 19:39:58.000000 zash-sdk-0.0.9/setup.py
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2023-01-23 23:59:03.449066 zash-sdk-0.0.9/zash_sdk/
+-rw-r--r--   0 efes       (501) staff       (20)       22 2023-01-23 23:58:55.000000 zash-sdk-0.0.9/zash_sdk/__init__.py
+-rw-r--r--   0 efes       (501) staff       (20)    10294 2023-01-23 23:58:55.000000 zash-sdk-0.0.9/zash_sdk/_modidx.py
+-rw-r--r--   0 efes       (501) staff       (20)    12984 2023-01-23 23:58:55.000000 zash-sdk-0.0.9/zash_sdk/collection.py
+-rw-r--r--   0 efes       (501) staff       (20)     7717 2023-01-23 23:58:55.000000 zash-sdk-0.0.9/zash_sdk/connectors.py
+-rw-r--r--   0 efes       (501) staff       (20)      648 2023-01-23 23:58:55.000000 zash-sdk-0.0.9/zash_sdk/graph.py
+-rw-r--r--   0 efes       (501) staff       (20)     2259 2023-01-23 23:58:55.000000 zash-sdk-0.0.9/zash_sdk/nft.py
+-rw-r--r--   0 efes       (501) staff       (20)      929 2023-01-23 23:58:55.000000 zash-sdk-0.0.9/zash_sdk/zash.py
+drwxr-xr-x   0 efes       (501) staff       (20)        0 2023-01-23 23:59:03.450153 zash-sdk-0.0.9/zash_sdk.egg-info/
+-rw-r--r--   0 efes       (501) staff       (20)    19267 2023-01-23 23:59:03.000000 zash-sdk-0.0.9/zash_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 efes       (501) staff       (20)      414 2023-01-23 23:59:03.000000 zash-sdk-0.0.9/zash_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 efes       (501) staff       (20)        1 2023-01-23 23:59:03.000000 zash-sdk-0.0.9/zash_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 efes       (501) staff       (20)       38 2023-01-23 23:59:03.000000 zash-sdk-0.0.9/zash_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 efes       (501) staff       (20)        1 2022-08-23 16:52:00.000000 zash-sdk-0.0.9/zash_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 efes       (501) staff       (20)       84 2023-01-23 23:59:03.000000 zash-sdk-0.0.9/zash_sdk.egg-info/requires.txt
+-rw-r--r--   0 efes       (501) staff       (20)        9 2023-01-23 23:59:03.000000 zash-sdk-0.0.9/zash_sdk.egg-info/top_level.txt
```

### Comparing `zash-sdk-0.0.8/LICENSE` & `zash-sdk-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zash-sdk-0.0.8/PKG-INFO` & `zash-sdk-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zash-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: SDK
 Home-page: https://github.com/zashdev/zash-sdk
 Author: efx
 Author-email: efe@joinzash.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `zash-sdk-0.0.8/README.md` & `zash-sdk-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `zash-sdk-0.0.8/settings.ini` & `zash-sdk-0.0.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = zash-sdk
 lib_name = zash-sdk
-version = 0.0.8
+version = 0.0.9
 min_python = 3.7
 license = apache2
 doc_path = _docs
 lib_path = zash_sdk
 nbs_path = .
 recursive = False
 tst_flags = notest
```

### Comparing `zash-sdk-0.0.8/setup.py` & `zash-sdk-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `zash-sdk-0.0.8/zash_sdk/_modidx.py` & `zash-sdk-0.0.9/zash_sdk/_modidx.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,19 @@
                                      'zash_sdk.collection._chain_prefix': ('collection.html#_chain_prefix', 'zash_sdk/collection.py'),
                                      'zash_sdk.collection._fetch_metadata': ('collection.html#_fetch_metadata', 'zash_sdk/collection.py'),
                                      'zash_sdk.collection._fetch_metadatas': ('collection.html#_fetch_metadatas', 'zash_sdk/collection.py'),
                                      'zash_sdk.collection._fetch_socials': ('collection.html#_fetch_socials', 'zash_sdk/collection.py'),
                                      'zash_sdk.collection._fetch_trades': ('collection.html#_fetch_trades', 'zash_sdk/collection.py'),
                                      'zash_sdk.collection._parse_start_end_dates': ( 'collection.html#_parse_start_end_dates',
                                                                                      'zash_sdk/collection.py'),
+                                     'zash_sdk.collection._sqlize_list': ('collection.html#_sqlize_list', 'zash_sdk/collection.py'),
                                      'zash_sdk.collection._timeseries_to_df': ( 'collection.html#_timeseries_to_df',
-                                                                                'zash_sdk/collection.py')},
+                                                                                'zash_sdk/collection.py'),
+                                     'zash_sdk.collection.filter_wash_trades': ( 'collection.html#filter_wash_trades',
+                                                                                 'zash_sdk/collection.py')},
             'zash_sdk.connectors': { 'zash_sdk.connectors.APIConnector': ('connectors.html#apiconnector', 'zash_sdk/connectors.py'),
                                      'zash_sdk.connectors.APIConnector.__init__': ( 'connectors.html#apiconnector.__init__',
                                                                                     'zash_sdk/connectors.py'),
                                      'zash_sdk.connectors.APIConnector.close': ( 'connectors.html#apiconnector.close',
                                                                                  'zash_sdk/connectors.py'),
                                      'zash_sdk.connectors.APIConnector.get': ('connectors.html#apiconnector.get', 'zash_sdk/connectors.py'),
                                      'zash_sdk.connectors.Connector': ('connectors.html#connector', 'zash_sdk/connectors.py'),
@@ -66,14 +69,15 @@
                                      'zash_sdk.connectors.W3Connector.get_token_metadata': ( 'connectors.html#w3connector.get_token_metadata',
                                                                                              'zash_sdk/connectors.py'),
                                      'zash_sdk.connectors._authenticate': ('connectors.html#_authenticate', 'zash_sdk/connectors.py'),
                                      'zash_sdk.connectors._connect_to_redshift': ( 'connectors.html#_connect_to_redshift',
                                                                                    'zash_sdk/connectors.py'),
                                      'zash_sdk.connectors._connect_to_redshift_dev': ( 'connectors.html#_connect_to_redshift_dev',
                                                                                        'zash_sdk/connectors.py'),
+                                     'zash_sdk.connectors._fetch_dev_creds': ('connectors.html#_fetch_dev_creds', 'zash_sdk/connectors.py'),
                                      'zash_sdk.connectors._w3_client': ('connectors.html#_w3_client', 'zash_sdk/connectors.py'),
                                      'zash_sdk.connectors.authenticate': ('connectors.html#authenticate', 'zash_sdk/connectors.py')},
             'zash_sdk.graph': { 'zash_sdk.graph.build_network': ('graph.html#build_network', 'zash_sdk/graph.py'),
                                 'zash_sdk.graph.plot_trade_network': ('graph.html#plot_trade_network', 'zash_sdk/graph.py')},
             'zash_sdk.nft': { 'zash_sdk.nft.NFT': ('nft.html#nft', 'zash_sdk/nft.py'),
                               'zash_sdk.nft.NFT.__init__': ('nft.html#nft.__init__', 'zash_sdk/nft.py'),
                               'zash_sdk.nft.NFT.collection': ('nft.html#nft.collection', 'zash_sdk/nft.py'),
```

### Comparing `zash-sdk-0.0.8/zash_sdk/collection.py` & `zash-sdk-0.0.9/zash_sdk/collection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,173 +1,233 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../01_collection.ipynb.
 
 # %% auto 0
-__all__ = ['NFTCollection', 'Token']
+__all__ = ['NFTCollection', 'filter_wash_trades', 'Token']
 
 # %% ../01_collection.ipynb 4
 import pandas as pd
 from dateparser import parse as parse_date
 from functools import cache
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from .connectors import Connector
 from fastcore.utils import patch
 from fastcore.basics import basic_repr
 from box import Box
 from operator import attrgetter
 from typing import Callable
 from jinja2 import Template
+from typing import Union
 
 # %% ../01_collection.ipynb 5
 def _parse_start_end_dates(start_time: str, end_time: str = "now") -> tuple[datetime]:
     # ensure you have end_time:
     end_time = end_time or 'now'
     shortcuts = {
         # put more here, but should be convertible to dateparser lib conventions.
         "latest": 'now',
     }
     start_time = str(datetime.utcnow().date()) if start_time == 'today' else start_time
     if start_time in shortcuts: start_time = shortcuts[start_time]
     return parse_date(start_time, settings={'TIMEZONE': 'UTC'}), parse_date(end_time, settings={'TIMEZONE': 'UTC'})
 
 # %% ../01_collection.ipynb 7
+def _sqlize_list(l: list): return ','.join(list(map(lambda x: "'" + x + "'", l)))
+
+# %% ../01_collection.ipynb 8
 def _chain_prefix(chain: str):
-    return '' if chain == 'eth' else chain + '_'
-    
-def _build_sol_trade_statement(start_dt:datetime, 
-                           end_dt:datetime, 
-                           collection_address:str='',
-                           mints_only=False,
-                           token_id:str='',
-                           expand_collection=True
-                              ):
-    table = 'sol_trades' if not mints_only else 'sol_mints'
-    # TODO - add expand collections
+    return "" if chain == "eth" else chain + "_"
+
+
+def _build_sol_trade_statement(
+    start_dt: datetime,
+    end_dt: datetime,
+    collection_address: Union[str, list] = "",
+    mints_only=False,
+    token_id: str = "",
+    expand_collection=True,
+):
+    table = "sol_trades" if not mints_only else "sol_mints"
+    collection_addresses = ''
+    if type(collection_address) == list:
+        collection_address, collection_addresses = '', _sqlize_list(collection_address)
+    if ',' in collection_address:
+        # assume this is sqlized
+        collection_address, collection_addresses = '', collection_address
+
     template = """
         SELECT *
         FROM onchain.{{table}}
         WHERE date >= '{{start_date}}' AND date <= '{{end_date}}'
         AND hour >= {{start_hour}} AND hour <= {{end_hour}}
         AND block_time >= {{ start_ts }} AND block_time <= {{ end_ts }}
         {%- if collection_address %}
         AND collection = '{{ collection_address }}'
         {% endif %}
+        {%- if collection_addresses %}
+        AND collection_address IN ({{ collection_addresses }})
+        {% endif %}
         {%- if token_id %}
         AND mint = '{{ token_id }}'
         {% endif %}
     """
-    return Template(template,lstrip_blocks=True,trim_blocks=True, autoescape=True).render(
-        table=table,
-        start_ts=round(start_dt.timestamp()),
-        end_ts=round(end_dt.timestamp()),
-        start_date=start_dt.date(),
-        end_date=end_dt.date(),
-        start_hour=start_dt.hour,
-        end_hour=end_dt.hour,
-        collection_address=collection_address,
-        token_id=token_id).replace('\n','').replace('   ', ' ')
-
-def _build_trade_statement(chain: str, 
-                           start_dt:datetime, 
-                           end_dt:datetime, 
-                           collection_address:str='',
-                           mints_only=False,
-                           token_id:str='',
-                           expand_collection=False,
-                          ):
-    if chain == 'sol':
+    return (
+        Template(template, lstrip_blocks=True, trim_blocks=True, autoescape=True)
+        .render(
+            table=table,
+            start_ts=round(start_dt.timestamp()),
+            end_ts=round(end_dt.timestamp()),
+            start_date=start_dt.date(),
+            end_date=end_dt.date(),
+            start_hour=start_dt.hour,
+            end_hour=end_dt.hour,
+            collection_addresses=collection_addresses,
+            collection_address=collection_address,
+            token_id=token_id,
+        )
+        .replace("\n", "")
+        .replace("   ", " ")
+        .replace("&#39;", "'")
+    )
+
+
+def _build_trade_statement(
+    chain: str,
+    start_dt: datetime,
+    end_dt: datetime,
+    collection_address: Union[str, list] = "",
+    mints_only=False,
+    token_id: str = "",
+    expand_collection=False,
+):
+    if chain == "sol":
         return _build_sol_trade_statement(
             start_dt=start_dt,
             end_dt=end_dt,
             collection_address=collection_address,
             mints_only=mints_only,
             token_id=token_id,
-            expand_collection=expand_collection
+            expand_collection=expand_collection,
         )
     table = f'{_chain_prefix(chain)}{"trades" if not mints_only else "mints"}'
+    collection_addresses = ''
+    if type(collection_address) == list:
+        collection_address, collection_addresses = '', _sqlize_list(collection_address)
+    if ',' in collection_address:
+        # assume this is sqlized
+        collection_address, collection_addresses = '', collection_address
+
     template = """
         SELECT *
         FROM onchain.{{table}}
         WHERE timestamp >= {{ start_ts }} AND timestamp <= {{ end_ts }}
         {%- if collection_address %}
         AND collection_address = '{{ collection_address }}'
         {% endif %}
+        {%- if collection_addresses %}
+        AND collection_address IN ({{ collection_addresses }})
+        {% endif %}
         {%- if token_id %}
         AND token_id = '{{ token_id }}'
         {% endif %}
     """
-    t = Template(template,lstrip_blocks=True,trim_blocks=True, autoescape=True).render(
-        table=table,
-        start_ts=round(start_dt.timestamp()),
-        end_ts=round(end_dt.timestamp()),
-        mints_only=mints_only,
-        collection_address=collection_address,
-        token_id=token_id).replace('\n','').replace('   ', ' ')
+    
+    t = (
+        Template(template, lstrip_blocks=True, trim_blocks=True, autoescape=True)
+        .render(
+            table=table,
+            start_ts=round(start_dt.timestamp()),
+            end_ts=round(end_dt.timestamp()),
+            mints_only=mints_only,
+            collection_addresses=collection_addresses,
+            collection_address=collection_address,
+            token_id=token_id,
+        )
+        .replace("\n", "")
+        .replace("   ", " ")
+        .replace("&#39;", "'")
+    )
     if expand_collection:
         expanded_temp = """
             WITH x as ({{temp}})
             SELECT x.*, y.name, y.slug
             FROM x LEFT JOIN offchain.{{metadata_table}} y
             ON x.collection_address = y.collection_id
         """
-        metadata_table = f'{_chain_prefix(chain)}collection_metadata'
-        return Template(expanded_temp,lstrip_blocks=True,trim_blocks=True).render(
-            temp=t,
-            metadata_table=metadata_table
-        ).replace('\n','').replace('   ', ' ')
+        metadata_table = f"{_chain_prefix(chain)}collection_metadata"
+        return (
+            Template(expanded_temp, lstrip_blocks=True, trim_blocks=True)
+            .render(temp=t, metadata_table=metadata_table)
+            .replace("\n", "")
+            .replace("   ", " ")
+        )
     else:
         return t
 
-# %% ../01_collection.ipynb 9
+# %% ../01_collection.ipynb 10
 @cache
 def __fetch_trades(
     conn: Connector,
     start_dt: datetime,  # start time in UTC. You can use shortcuts like today, yesterday or even clauses such as "1 day/week ago".
     end_dt: datetime,  # default now. Same type as start_time
     chain: str = "eth",
     collection_address: str = "",  # collection address
     token_id: str = "",  # token id
-    mints_only: bool = False, # mints
+    mints_only: bool = False,  # mints
     expand_collection: bool = False,
 ) -> pd.DataFrame:
     return conn.query(
         _build_trade_statement(
             chain,
             start_dt,
             end_dt,
             collection_address=collection_address,
             token_id=token_id,
             mints_only=mints_only,
-            expand_collection=expand_collection
+            expand_collection=expand_collection,
         )
     )
 
 def _fetch_trades(
     conn: Connector,
     start_time: str,  # start time in UTC. You can use shortcuts like today, yesterday or even clauses such as "1 day/week ago".
     end_time: str = "now",  # default now. Same type as start_time
     chain: str = "eth",
-    collection_address: str = "",  # collection address
+    collection_address: Union[str, list] = "",  # collection address
     token_id: str = "",  # token id
     mints_only: bool = False,  # filter for mints if True
-    expand_collection: bool = False, # expand collection columns
+    expand_collection: bool = False,  # expand collection columns
 ) -> pd.DataFrame:
     start_dt, end_dt = _parse_start_end_dates(start_time, end_time=end_time)
     # we cache the one below because "yesterday" etc. style start_time is relative.
+    # this is needed for caching:
+    if type(collection_address) == list:
+        if len(collection_address) > 0:
+            collection_address = (
+                _sqlize_list(collection_address)
+                if len(collection_address) > 1
+                else collection_address[0]
+            )
+        else:
+            collection_address = ''
+        
     return __fetch_trades(
         conn,
         start_dt,
         end_dt,
         chain=chain,
-        collection_address=collection_address,
+        collection_address=(
+            collection_address.lower() if chain != "sol" else collection_address
+        ),
         mints_only=mints_only,
         token_id=token_id,
-        expand_collection=expand_collection
+        expand_collection=expand_collection,
     )
 
+
 @cache
 def _fetch_metadata(conn: Connector, collection_id: str, chain: str = "eth"):
     res = conn.query(
         f"""
         select * from offchain.{_chain_prefix(chain)}collection_metadata
         where collection_id='{collection_id.lower()}'"""
     ).squeeze()
@@ -175,17 +235,19 @@
     for i in [
         "volume_all",
         "volume_daily",
         "volume_weekly",
         "item_count",
         "floor_price",
     ]:
-        if i in res: del res[i]
+        if i in res:
+            del res[i]
     return res
 
+
 @cache
 def _fetch_metadatas(conn: Connector, collection_ids: list[str], chain: str = "eth"):
     cs = ",".join(list(map(lambda i: "'" + i.lower() + "'", collection_id)))
     df = conn.query(
         f"""
         select * from offchain.{_chain_prefix(chain)}collection_metadata
         where collection_id IN ({cs})"""
@@ -202,42 +264,53 @@
         "item_count",
         "floor_price",
     ]:
         if i in res:
             del res[i]
     return res
 
+
 @cache
 def _fetch_socials(conn: Connector, collection_slug: str):
     return conn.get(f"/socials/{collection_slug}").json()
 
-# %% ../01_collection.ipynb 10
+# %% ../01_collection.ipynb 11
 class NFTCollection:
     """NFT Collection objecat"""
     def __init__(self,
                  conn: Connector,
                  collection_id: str, # collection_address e.g. 0xBC4CA0EdA7647A8aB7C2061c2E118A18a936f13D
                  chain: str ='eth'): # chain_id - currently only "eth" or "bnb" allowed
         self._conn, self.chain, self.collection_id = conn, chain, (collection_id.lower() if chain != 'sol' else collection_id)
 
-# %% ../01_collection.ipynb 11
+# %% ../01_collection.ipynb 12
+def filter_wash_trades(trades, filters):
+    if filters == 'all':
+        df = pd.read_csv('./bayc_scc_bsn3.csv')
+        return trades[~trades['hash'].isin(df['hash'])]
+    if filters == ['cycles', 'repeat_trades']:
+        df = pd.read_csv('./bayc_bsn3.csv')
+        return trades[~trades['hash'].isin(df['hash'])]
+
+# %% ../01_collection.ipynb 13
 @patch
 def trades(self: NFTCollection,
            start_time: str, # start time in UTC. You can use shortcuts like today, yesterday or even clauses such as "1 day/week ago".
            end_time: str = 'now', # default now. Same type as start_time 
-           expand_collection: bool = False # expand collection details (name, slug etc.)
-          ):
+           expand_collection: bool = False, # expand collection details (name, slug etc.)
+          ):        
     return _fetch_trades(
         self._conn,
         start_time, 
         end_time=end_time, 
         chain=self.chain,
         collection_address=self.collection_id,
         expand_collection=expand_collection
     )
+
 @patch
 def token(self: NFTCollection, token_id: str): return Token(self._conn, token_id, self.collection_id, chain=self.chain)
 @patch
 def metadata(self: NFTCollection): return _fetch_metadata(self._conn, self.collection_id, chain=self.chain)
 @patch
 def mints(self: NFTCollection,
            start_time: str, # start time in UTC. You can use shortcuts like today, yesterday or even clauses such as "1 day/week ago".
@@ -250,15 +323,15 @@
         end_time=end_time,
         chain=self.chain,
         collection_address=self.collection_id,
         mints_only=True,
         expand_collection=expand_collection
     )
 
-# %% ../01_collection.ipynb 12
+# %% ../01_collection.ipynb 14
 def _timeseries_to_df(timeseries: list) -> pd.DataFrame:
     """turn socials timeseries to pd dataframe"""
     if not timeseries: return timeseries
     _ts = pd.DataFrame([dict(i) for i in timeseries])
     _ts['ts'] = _ts['ts'].apply(pd.to_datetime)
     _ts.set_index('ts')
     return _ts
@@ -268,15 +341,15 @@
     _socials = Box(
         self._conn.get(f'/socials',
                        params={'id':collection_slug, 'chain': self.chain}).json()['social'])
     _socials.discord = _timeseries_to_df(_socials.discord.timeseries)
     _socials.twitter = _timeseries_to_df(_socials.twitter.timeseries)
     return _socials
 
-# %% ../01_collection.ipynb 13
+# %% ../01_collection.ipynb 15
 class Token:
     __repr__= basic_repr(['collection_id', 'token_id', 'token_type', 'chain'])
     def __init__(self, conn: Connector, token_id: str, collection_id:str, chain:str='eth', token_type='721'):
         self._conn, self.token_id, self.chain, self.token_type = conn, token_id, chain, token_type
         self.collection_id = collection_id
     def trades(self: 'Token',
            start_time: str, # start time in UTC. You can use shortcuts like today, yesterday or even clauses such as "1 day/week ago".
```

### Comparing `zash-sdk-0.0.8/zash_sdk/connectors.py` & `zash-sdk-0.0.9/zash_sdk/connectors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../00_connectors.ipynb.
 
 # %% auto 0
 __all__ = ['aws_client_config', 'client', 'ci_client', 'BASE_URL', 'VERSION', 'DEFAULT_CHAIN', 'PERIODS', 'URI',
            'IPFS_PUB_GATEWAY', 'authenticate', 'RSConnector', 'APIConnector', 'W3Connector', 'Connector']
 
-# %% ../00_connectors.ipynb 4
+# %% ../00_connectors.ipynb 3
 import redshift_connector
 import boto3
+import json
 import requests
 import uuid
 import pandas as pd
 from functools import cache
 from redshift_connector import Connection
 from botocore.exceptions import ClientError
 from botocore.config import Config
@@ -24,14 +25,21 @@
 from box import Box
 
 # %% ../00_connectors.ipynb 5
 aws_client_config = Config(region_name="eu-west-1")
 client = boto3.client("cognito-idp", config=aws_client_config)
 ci_client = boto3.client("cognito-identity", config=aws_client_config)
 
+def _fetch_dev_creds():
+    """fetch api_key and db_user from parameter store"""
+    ssm = boto3.client('ssm')
+    return json.loads(ssm.get_parameter(
+        Name='sdk-admin-creds',
+    )['Parameter']['Value'])
+
 @cache
 def _authenticate(username, api_key):
     auth_res = client.initiate_auth(
         ClientId="377phvhgdn23vsor2ndafu02ek",
         AuthFlow="USER_PASSWORD_AUTH",
         AuthParameters={
             "USERNAME": username,
@@ -45,31 +53,35 @@
     }
 
     identity_id = ci_client.get_id(
         IdentityPoolId="eu-west-1:1b1ee2fe-2476-414c-9b29-993a56efb136",
         Logins=_logins,
     )["IdentityId"]
 
-    return ci_client.get_credentials_for_identity(
-        IdentityId=identity_id,
-        Logins=_logins,
-    )["Credentials"]
+    return {
+        **ci_client.get_credentials_for_identity(
+            IdentityId=identity_id,
+            Logins=_logins)["Credentials"],
+        'username': username,
+        'api_key': api_key
+    }
 def _connect_to_redshift(creds):
     return redshift_connector.connect(
         iam=True,
         database="prod",
-        db_user="pete",
+        db_user=creds['username'],
         cluster_identifier="redshift-cluster-1",
         access_key_id=creds["AccessKeyId"],
         secret_access_key=creds["SecretKey"],
         session_token=creds["SessionToken"],
         region="eu-west-1",
     )
 def _connect_to_redshift_dev():
     return _connect_to_redshift({
+        'username': _fetch_dev_creds()['db_user'],
         "AccessKeyId": None,
         "SecretKey": None,
         "SessionToken": None
     })
 def authenticate(
     username: str,  # username, usually your email
     api_key: str,  # generated api_key, you can request one from zash.sh
@@ -89,58 +101,68 @@
 # %% ../00_connectors.ipynb 6
 class RSConnector:
     """Redshift connector"""
     def __init__(self, username: str, api_key: str):
         self._conn = authenticate(username, api_key)
         self.username, self.api_key = username, api_key
     def refresh(self):
+        self.close()
         self._conn = authenticate(self.username, self.api_key)
     def _fetch(self, statement: str):
-        with self._conn.cursor() as cur:
+        try:
+            cur = self._conn.cursor()
             cur.execute(statement)
-            return cur.fetch_dataframe()
+            df = cur.fetch_dataframe()
+            cur.close()
+            return df
+        except Exception as e:
+            # maybe add more details
+            self._conn.rollback()
+            cur.close()
+            raise e
     def query(self, statement: str):
         try:
             return self._fetch(statement)
         except ClientError as e:
             if not len(e.args): raise e
             if "ExpiredToken" in e.args[0]:
                 print('Session expired, reauthenticating...')
                 self.refresh()
                 return self._fetch(statement)
     def close(self):
         self._conn.close()
 
-# %% ../00_connectors.ipynb 8
+# %% ../00_connectors.ipynb 9
 BASE_URL = "https://api.zash.sh"
 VERSION = "v2"
 DEFAULT_CHAIN = "eth"
 PERIODS = {"1d", "1w", "1m", "all"}
 
 class APIConnector:
     """Zash API connector. See [API docs](https://zashapi.readme.io) for more details."""
     def __init__(self, base_url: str = BASE_URL, api_key: str = "") -> None:
         self._session = requests.Session()
-        api_key = 'wwCThCi1Q45Fk6C7zAHGJ9PAIy05vMpP5GzXp6vq' if api_key == 'your_api_key' else api_key
+        api_key = _fetch_dev_creds()['api_key'] if api_key == 'your_api_key' else api_key
         self._session.headers.update({"X-API-Key": api_key})
         self.base_url = base_url
         self.product = "nft"
         self.base_path = urljoin(base_url, f"{VERSION}/{self.product}")
     @delegates(requests.Session.get)
     def get(self, 
             path: str, # API path that is after the product (i.e nft), i.e. /socials/bayc
             *args, **kwargs):
         if not path.startswith('/'): path = '/' + path
         return self._session.get(self.base_path + path, *args, **kwargs)
     def close(self): self._session.close()
 
-# %% ../00_connectors.ipynb 11
+# %% ../00_connectors.ipynb 12
 URI = {
     'bnb': 'https://bsc-dataseed2.binance.org',
-    'eth':'https://mainnet.infura.io/v3/e750204167004ae3b1d6a48241d8dcd2'
+    'eth':'https://mainnet.infura.io/v3/e750204167004ae3b1d6a48241d8dcd2',
+    'matic':'https://polygon-mainnet.infura.io/v3/e750204167004ae3b1d6a48241d8dcd2'
 }
 IPFS_PUB_GATEWAY = 'https://ipfs.io'
 _nft_metadata_abi = [{"inputs":[{"internalType":"uint256","name":"tokenId","type":"uint256"}],"name":"tokenURI","outputs":[{"internalType":"string","name":"","type":"string"}],"stateMutability":"view","type":"function"}]
 def _w3_client(uri, chain):
     if chain == "eth":
         return Web3(Web3.HTTPProvider(uri))
     elif chain == "bnb":
@@ -164,15 +186,15 @@
         if token_uri.strip().startswith('ipfs'):
             token_uri = token_uri.replace('ipfs://', f'{IPFS_PUB_GATEWAY}/ipfs/')
         return Box({
             'uri': token_uri,
             **requests.get(token_uri).json()
         })
 
-# %% ../00_connectors.ipynb 14
+# %% ../00_connectors.ipynb 15
 class Connector:
     def __init__(self, username: str, api_key:str):
         self._rs_connector, self._api_connector = RSConnector(username, api_key), APIConnector(api_key=api_key)
     @delegates(RSConnector.query)
     def query(self, *args, **kwargs): return self._rs_connector.query(*args, **kwargs)
     @delegates(APIConnector.get)
     def get(self, *args, **kwargs): return self._api_connector.get(*args, **kwargs)
```

### Comparing `zash-sdk-0.0.8/zash_sdk/graph.py` & `zash-sdk-0.0.9/zash_sdk/graph.py`

 * *Files identical despite different names*

### Comparing `zash-sdk-0.0.8/zash_sdk/nft.py` & `zash-sdk-0.0.9/zash_sdk/nft.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,18 +21,19 @@
     def mints(self,
            start_time: str, # start time in UTC. You can use shortcuts like today, yesterday or even clauses such as "1 day/week ago".
            end_time: str = '' # default now. Same type as start_time 
           )-> pd.DataFrame: # pandas dataframe with each row as a trade
         return _fetch_trades(self._conn, start_time, end_time=end_time, chain=self.chain, mints_only=True)
     def trades(self,
                start_time: str, # start time in UTC. You can use shortcuts like today, yesterday or even clauses such as "1 day/week ago".
-               end_time: str = '', # default now. Same type as start_time 
+               end_time: str = '', # default now. Same type as start_time
+               filter_collections=[], # collections to filter for when fetching trades
                expand_collection: bool = False # expand collection column with collection details (i.e. slug, name)
               )-> pd.DataFrame: # pandas dataframe with each row as a trade
-        return _fetch_trades(self._conn, start_time, end_time=end_time, chain=self.chain, expand_collection=expand_collection)
+        return _fetch_trades(self._conn, start_time, end_time=end_time, chain=self.chain, expand_collection=expand_collection,collection_address=filter_collections)
     def collection(self, 
                collection_id: str # collection_address with checksum (e.g. 0xBC4CA0EdA7647A8aB7C2061c2E118A18a936f13D)
               ) -> NFTCollection: 
         return NFTCollection(self._conn, collection_id, chain=self.chain)
 
 # %% ../02_nft.ipynb 10
 @patch
```

### Comparing `zash-sdk-0.0.8/zash_sdk/zash.py` & `zash-sdk-0.0.9/zash_sdk/zash.py`

 * *Files identical despite different names*

### Comparing `zash-sdk-0.0.8/zash_sdk.egg-info/PKG-INFO` & `zash-sdk-0.0.9/zash_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zash-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: SDK
 Home-page: https://github.com/zashdev/zash-sdk
 Author: efx
 Author-email: efe@joinzash.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

