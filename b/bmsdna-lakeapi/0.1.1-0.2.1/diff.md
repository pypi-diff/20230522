# Comparing `tmp/bmsdna_lakeapi-0.1.1.tar.gz` & `tmp/bmsdna_lakeapi-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmsdna_lakeapi-0.1.1.tar", max compression
+gzip compressed data, was "bmsdna_lakeapi-0.2.1.tar", max compression
```

## Comparing `bmsdna_lakeapi-0.1.1.tar` & `bmsdna_lakeapi-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1081 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/LICENSE
--rw-r--r--   0        0        0     4722 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/README.md
--rw-r--r--   0        0        0      166 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/api/__init__.py
--rw-r--r--   0        0        0     1135 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/api/api.py
--rw-r--r--   0        0        0      926 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/__init__.py
--rw-r--r--   0        0        0     5347 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_base.py
--rw-r--r--   0        0        0     3601 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_datafusion.py
--rw-r--r--   0        0        0     6908 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_duckdb.py
--rw-r--r--   0        0        0     5670 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_polars.py
--rw-r--r--   0        0        0        0 2023-05-17 10:00:58.844992 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/__init__.py
--rw-r--r--   0        0        0    12190 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/config.py
--rw-r--r--   0        0        0    12625 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/dataframe.py
--rw-r--r--   0        0        0    15576 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/endpoint.py
--rw-r--r--   0        0        0      187 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/env.py
--rw-r--r--   0        0        0     1012 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/log.py
--rw-r--r--   0        0        0     6566 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/model.py
--rw-r--r--   0        0        0     8044 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/response.py
--rw-r--r--   0        0        0     3601 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/route.py
--rw-r--r--   0        0        0     1692 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/types.py
--rw-r--r--   0        0        0     2361 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/uservalidation.py
--rw-r--r--   0        0        0      215 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/yaml.py
--rw-r--r--   0        0        0        0 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/polars_extensions/__init__.py
--rw-r--r--   0        0        0     1847 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/polars_extensions/delta.py
--rw-r--r--   0        0        0      326 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/standalone/__init__.py
--rw-r--r--   0        0        0     1784 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/tools/useradd.py
--rw-r--r--   0        0        0     1095 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/tools/validateschema.py
--rw-r--r--   0        0        0     1804 2023-05-17 10:00:58.848991 bmsdna_lakeapi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6036 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4722 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/README.md
+-rw-r--r--   0        0        0      166 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/api/__init__.py
+-rw-r--r--   0        0        0     1135 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/api/api.py
+-rw-r--r--   0        0        0      926 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/context/__init__.py
+-rw-r--r--   0        0        0     5349 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/context/df_base.py
+-rw-r--r--   0        0        0     3601 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/context/df_datafusion.py
+-rw-r--r--   0        0        0     8721 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/context/df_duckdb.py
+-rw-r--r--   0        0        0     5670 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/context/df_polars.py
+-rw-r--r--   0        0        0        0 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/__init__.py
+-rw-r--r--   0        0        0    12190 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/config.py
+-rw-r--r--   0        0        0    12625 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/dataframe.py
+-rw-r--r--   0        0        0    15707 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/endpoint.py
+-rw-r--r--   0        0        0      187 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/env.py
+-rw-r--r--   0        0        0     1012 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/log.py
+-rw-r--r--   0        0        0     6566 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/model.py
+-rw-r--r--   0        0        0     7822 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/response.py
+-rw-r--r--   0        0        0     3601 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/route.py
+-rw-r--r--   0        0        0     1692 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/types.py
+-rw-r--r--   0        0        0     2361 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/uservalidation.py
+-rw-r--r--   0        0        0      215 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/yaml.py
+-rw-r--r--   0        0        0        0 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/polars_extensions/__init__.py
+-rw-r--r--   0        0        0     1847 2023-05-22 06:46:54.037300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/polars_extensions/delta.py
+-rw-r--r--   0        0        0      326 2023-05-22 06:46:54.041300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/standalone/__init__.py
+-rw-r--r--   0        0        0     1784 2023-05-22 06:46:54.041300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/tools/useradd.py
+-rw-r--r--   0        0        0     1095 2023-05-22 06:46:54.041300 bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/tools/validateschema.py
+-rw-r--r--   0        0        0     1852 2023-05-22 06:46:54.041300 bmsdna_lakeapi-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6036 1970-01-01 00:00:00.000000 bmsdna_lakeapi-0.2.1/PKG-INFO
```

### Comparing `bmsdna_lakeapi-0.1.1/LICENSE` & `bmsdna_lakeapi-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/README.md` & `bmsdna_lakeapi-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/api/api.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/api/api.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/__init__.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/context/__init__.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_base.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/context/df_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
             ds = pa.dataset.dataset(uri, format=file_type)
         elif file_type == "delta":
             dt = DeltaTable(
                 uri,
             )
 
             ds = dt.to_pyarrow_dataset(partitions=partitions)
+
         else:
             raise Exception(f"Not supported file type {file_type}")
         return ds
 
     @abstractmethod
     def register_arrow(self, name: str, ds: Union[pyarrow.dataset.Dataset, pyarrow.Table]):
         ...
```

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_datafusion.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/context/df_datafusion.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_duckdb.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/context/df_duckdb.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import pypika.queries
 import pypika.terms
 import pypika
 import os
 from datetime import datetime, timezone
 from bmsdna.lakeapi.core.config import SearchConfig
 
+ENABLE_COPY_TO = os.getenv("ENABLE_COPY_TO", "0") == "1"
+
 
 class DuckDBResultData(ResultData):
     def __init__(
         self,
         original_sql: Union[pypika.queries.QueryBuilder, str],
         con: duckdb.DuckDBPyConnection,
     ) -> None:
@@ -56,14 +58,42 @@
 
     def to_arrow_table(self):
         return self.df.arrow()
 
     def to_arrow_recordbatch(self, chunk_size: int = 10000):
         return self.df.fetch_record_batch(chunk_size)
 
+    def write_parquet(self, file_name: str):
+        if not ENABLE_COPY_TO:
+            return super().write_parquet(file_name)
+        query = self.original_sql if isinstance(self.original_sql, str) else self.original_sql.get_sql()
+        full_query = f"COPY ({query}) TO '{file_name}' (FORMAT PARQUET,use_tmp_file False, ROW_GROUP_SIZE 10000)"
+        self.con.execute(full_query)
+
+    def write_nd_json(self, file_name: str):
+        if not ENABLE_COPY_TO:
+            return super().write_nd_json(file_name)
+        query = self.original_sql if isinstance(self.original_sql, str) else self.original_sql.get_sql()
+        full_query = f"COPY ({query}) TO '{file_name}' (FORMAT JSON)"
+        self.con.execute(full_query)
+
+    def write_csv(self, file_name: str, *, separator: str):
+        if not ENABLE_COPY_TO:
+            return super().write_csv(file_name, separator=separator)
+        query = self.original_sql if isinstance(self.original_sql, str) else self.original_sql.get_sql()
+        full_query = f"COPY ({query}) TO '{file_name}' (FORMAT CSV, delim '{separator}', header True)"
+        self.con.execute(full_query)
+
+    def write_json(self, file_name: str):
+        if not ENABLE_COPY_TO:
+            return super().write_json(file_name)
+        query = self.original_sql if isinstance(self.original_sql, str) else self.original_sql.get_sql()
+        full_query = f"COPY ({query}) TO '{file_name}' (FORMAT JSON, Array True)"
+        self.con.execute(full_query)
+
 
 class Match25Term(pypika.terms.Term):
     def __init__(
         self,
         source_view: str,
         field: pypika.terms.Term,
         search_text: str,
@@ -94,15 +124,16 @@
     def __init__(self, con: duckdb.DuckDBPyConnection):
         super().__init__()
         self.con = con
         self.res_con = None
         self.persistance_file_name = None
 
     def register_arrow(self, name: str, ds: Union[pyarrow.dataset.Dataset, pyarrow.Table]):
-        self.con.from_arrow(ds).create_view(name, replace=True)
+        # self.con.from_arrow(ds).create_view(name, replace=True)
+        self.con.register(name, ds)
 
     def close(self):
         pass
 
     def execute_sql(
         self,
         sql: Union[
@@ -135,20 +166,23 @@
         search_columns = []
         for cfg in search_configs:
             search_columns = search_columns + cfg.columns
         scc = ", ".join([f"{sc}" for sc in search_columns])
         pk_name = "__search_id"
         real_query = f"CREATE TABLE search_con.{persistence_name} AS SELECT ROW_NUMBER() OVER () AS __search_id, * FROM {source_view} s"
         persitance_path = os.getenv("TEMP", "/tmp/")
-
         persistance_file_name = os.path.join(persitance_path, persistence_name + ".duckdb")
 
-        if not os.path.exists(persistance_file_name) or datetime.fromtimestamp(
-            os.path.getmtime(persistance_file_name), tz=timezone.utc
-        ) < modified_date.astimezone(timezone.utc):
+        if (
+            not os.path.exists(persistance_file_name)
+            or datetime.fromtimestamp(os.path.getmtime(persistance_file_name), tz=timezone.utc)
+            < modified_date.astimezone(timezone.utc)
+            or datetime.fromtimestamp(os.path.getmtime(persistance_file_name), tz=timezone.utc)
+            < datetime.fromisoformat("2023-05-19T00:00Z")  # before duckdb upgrade
+        ):
             persistance_file_name_temp = persistance_file_name + "_temp"
             if os.path.exists(persistance_file_name_temp):
                 os.remove(persistance_file_name_temp)
             search_con = duckdb.connect(persistance_file_name_temp, read_only=False)
             search_con.commit()  # create empty duck file
             search_con.close()
             self.con.execute(f"ATTACH '{persistance_file_name_temp}' AS search_con")
```

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/context/df_polars.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/context/df_polars.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/config.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/config.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/dataframe.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/endpoint.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,21 +141,25 @@
                         df.query_builder().select(*[pypika.Field(c) for c in partition_columns]).distinct()
                     )
                     partition_values = context.execute_sql(qb).to_arrow_table().to_pylist()
             schema = df.arrow_schema()
             str_cols = [name for name in schema.names if pa.types.is_string(schema.field(name).type)]
 
             str_lengths_df = (
-                context.execute_sql(
-                    df.query_builder().select(
-                        *[fn.Function("MAX", fn.Function("LEN", fn.Field(sc))).as_(sc) for sc in str_cols]
+                (
+                    context.execute_sql(
+                        df.query_builder().select(
+                            *[fn.Function("MAX", fn.Function("LEN", fn.Field(sc))).as_(sc) for sc in str_cols]
+                        )
                     )
+                    .to_arrow_table()
+                    .to_pylist()
                 )
-                .to_arrow_table()
-                .to_pylist()
+                if len(str_cols) > 0
+                else [{}]
             )
             str_lengths = str_lengths_df[0]
 
             def _recursive_get_type(t: Optional[pa.DataType]):
                 if t is None:
                     return None
                 return {
```

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/log.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/log.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/model.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/model.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/response.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import io
 import json
 import mimetypes
 import os
-import tempfile
-import typing
 from enum import Enum
-from typing import Iterable, Union
+from typing import Union
 from uuid import uuid4
 
 import anyio
 import pyarrow as pa
-from fastapi import BackgroundTasks, Request
-from fastapi.concurrency import run_in_threadpool
-from fastapi.responses import Response
+from fastapi import BackgroundTasks
 from starlette.datastructures import URL
-from starlette.responses import FileResponse, StreamingResponse
+from starlette.responses import FileResponse
 
 from bmsdna.lakeapi.context.df_base import ExecutionContext, ResultData
 from bmsdna.lakeapi.core.config import BasicConfig
 from bmsdna.lakeapi.core.log import get_logger
 from bmsdna.lakeapi.core.types import OutputFileType
 
 logger = get_logger(__name__)
@@ -153,33 +149,28 @@
     elif format == OutputFormats.HTML:
         content.to_pandas().to_html(out, index=False)
 
     elif format == OutputFormats.XML:
         content.to_pandas().to_xml(out, index=False, parser="etree")
 
     elif format in (OutputFormats.ARROW_IPC, OutputFormats.ARROW_STREAM):
-        batches = content.to_arrow_recordbatch()
-        with pa.OSFile(out, "wb") as sink:
-            with pa.ipc.new_file(sink, batches.schema) as writer:
-                for batch in batches:
-                    writer.write(batch)
+        with content.to_arrow_recordbatch() as batches:
+            with pa.OSFile(out, "wb") as sink:
+                with pa.ipc.new_file(sink, batches.schema) as writer:
+                    for batch in batches:
+                        writer.write(batch)
 
     elif format == OutputFormats.ND_JSON:
         content.write_nd_json(out)
     elif format == OutputFormats.PARQUET:
         content.write_parquet(out)
     else:
         content.write_json(out)
 
 
-def file_response_generator(path):
-    with open(path, "rb") as f:
-        yield from f
-
-
 async def create_response(
     current_user_name: str,
     url: URL,
     accept: str,
     content: ResultData,
     context: ExecutionContext,
     basic_config: BasicConfig,
@@ -196,15 +187,15 @@
         OutputFormats.ND_JSON,
         OutputFormats.CSV,
         OutputFormats.SEMI_CSV,
         OutputFormats.CSV4EXCEL,
     ]:
         content_dispositiont_type = "inline"
         filename = None
-    path = os.getenv("TEMP", "/tmp") + "/" + str(uuid4()) + extension
+    path = os.path.join(basic_config.temp_folder_path, str(uuid4()) + extension)
     media_type = mimetypes.guess_type("file" + extension)[0]
     write_frame(
         current_user=current_user_name, url=url, content=content, format=format, out=path, basic_config=basic_config
     )
 
     if media_type is not None and format in [
         OutputFormats.JSON,
```

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/route.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/route.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/types.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/types.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/core/uservalidation.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/core/uservalidation.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/polars_extensions/delta.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/polars_extensions/delta.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/tools/useradd.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/tools/useradd.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/bmsdna/lakeapi/tools/validateschema.py` & `bmsdna_lakeapi-0.2.1/bmsdna/lakeapi/tools/validateschema.py`

 * *Files identical despite different names*

### Comparing `bmsdna_lakeapi-0.1.1/pyproject.toml` & `bmsdna_lakeapi-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,63 @@
 [tool.poetry]
 name = "bmsdna-lakeapi"
-version = "0.1.1"
+version = "0.2.1"
 description = ""
 authors = ["DWH Team <you@example.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "bmsdna"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fastapi = "^0.95.1"
 deltalake = "^0.9.0"
 pyyaml = "^6.0"
 aiocache = "^0.12.1"
 pypika = "^0.48.9"
+duckdb = "^0.8.0"
+polars = "^0.17.14"
 
 # schema stuff
 jsonschema = {version = "^4.17.3", optional=true}
 python2jsonschema = { version ="^0.8", optional=true}
-duckdb = "^0.7.1"
-polars = "^0.17.13"
 
 # polars stuff
 xlsx2csv = { version ="^0.8.1", optional = true }
 
 # auth
 argon2-cffi = {version = "^21.3.0", optional=true}
 
 # datafusion
 datafusion = {version = "^24.0.0", optional = true }
 xlsxwriter = "^3.1.0"
 pyjwt = {version = "^2.6.0", optional = true}
 "ruamel.yaml" = {version = "^0.17.26", optional = true}
 
+
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.308"
 black = "^23.3.0"
 uvicorn = "^0.22.0"
+psutil = "^5.9.5"
 
 
 
 
 
 
 [tool.poetry.group.test.dependencies]
 faker = "^18.7.0"
 pytest = "^7.3.1"
 httpx = "^0.24.0"
 pytest-env = "^0.8.1"
 pytest-cov = "^4.0.0"
 pytest-benchmark = "^4.0.0"
 pandas = "^2.0.1"
+pytest-monitor = "^1.6.5"
 
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `bmsdna_lakeapi-0.1.1/PKG-INFO` & `bmsdna_lakeapi-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmsdna-lakeapi
-Version: 0.1.1
+Version: 0.2.1
 Summary: 
 License: MIT
 Author: DWH Team
 Author-email: you@example.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,18 +15,18 @@
 Provides-Extra: polars
 Provides-Extra: schema
 Provides-Extra: useradd
 Requires-Dist: aiocache (>=0.12.1,<0.13.0)
 Requires-Dist: argon2-cffi (>=21.3.0,<22.0.0) ; extra == "auth"
 Requires-Dist: datafusion (>=24.0.0,<25.0.0) ; extra == "datafusion"
 Requires-Dist: deltalake (>=0.9.0,<0.10.0)
-Requires-Dist: duckdb (>=0.7.1,<0.8.0)
+Requires-Dist: duckdb (>=0.8.0,<0.9.0)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0) ; extra == "schema"
-Requires-Dist: polars (>=0.17.13,<0.18.0) ; extra == "polars"
+Requires-Dist: polars (>=0.17.14,<0.18.0) ; extra == "polars"
 Requires-Dist: pyjwt (>=2.6.0,<3.0.0) ; extra == "auth"
 Requires-Dist: pypika (>=0.48.9,<0.49.0)
 Requires-Dist: python2jsonschema (>=0.8,<0.9) ; extra == "schema"
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: ruamel.yaml (>=0.17.26,<0.18.0) ; extra == "useradd"
 Requires-Dist: xlsx2csv (>=0.8.1,<0.9.0) ; extra == "polars"
 Requires-Dist: xlsxwriter (>=3.1.0,<4.0.0)
```

