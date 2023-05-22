# Comparing `tmp/h2o_mlops_scoring_client-0.0.6b1-py3-none-any.whl.zip` & `tmp/h2o_mlops_scoring_client-0.0.7b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8448 bytes, number of entries: 8
--rw-r--r--  2.0 unx        8 b- defN 23-May-06 00:00 h2o_mlops_scoring_client/VERSION
--rw-r--r--  2.0 unx     9746 b- defN 23-May-05 23:26 h2o_mlops_scoring_client/__init__.py
--rw-r--r--  2.0 unx    12413 b- defN 23-May-05 23:26 h2o_mlops_scoring_client/_utils.py
--rw-r--r--  2.0 unx      228 b- defN 23-May-05 23:26 h2o_mlops_scoring_client/_version.py
--rw-r--r--  2.0 unx     2993 b- defN 23-May-06 00:00 h2o_mlops_scoring_client-0.0.6b1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-06 00:00 h2o_mlops_scoring_client-0.0.6b1.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 23-May-06 00:00 h2o_mlops_scoring_client-0.0.6b1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      737 b- defN 23-May-06 00:00 h2o_mlops_scoring_client-0.0.6b1.dist-info/RECORD
-8 files, 26242 bytes uncompressed, 7134 bytes compressed:  72.8%
+Zip file size: 8741 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        8 b- defN 23-May-22 18:14 h2o_mlops_scoring_client/VERSION
+-rw-r--r--  2.0 unx     9746 b- defN 23-May-18 21:02 h2o_mlops_scoring_client/__init__.py
+-rw-r--r--  2.0 unx    14230 b- defN 23-May-18 21:02 h2o_mlops_scoring_client/_utils.py
+-rw-r--r--  2.0 unx      228 b- defN 23-May-18 21:02 h2o_mlops_scoring_client/_version.py
+-rw-r--r--  2.0 unx     3032 b- defN 23-May-22 18:14 h2o_mlops_scoring_client-0.0.7b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-22 18:14 h2o_mlops_scoring_client-0.0.7b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 23-May-22 18:14 h2o_mlops_scoring_client-0.0.7b1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      737 b- defN 23-May-22 18:14 h2o_mlops_scoring_client-0.0.7b1.dist-info/RECORD
+8 files, 28098 bytes uncompressed, 7427 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: h2o_mlops_scoring_client/_utils.py
 Comment: 
 
 Filename: h2o_mlops_scoring_client/_version.py
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.6b1.dist-info/METADATA
+Filename: h2o_mlops_scoring_client-0.0.7b1.dist-info/METADATA
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.6b1.dist-info/WHEEL
+Filename: h2o_mlops_scoring_client-0.0.7b1.dist-info/WHEEL
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.6b1.dist-info/top_level.txt
+Filename: h2o_mlops_scoring_client-0.0.7b1.dist-info/top_level.txt
 Comment: 
 
-Filename: h2o_mlops_scoring_client-0.0.6b1.dist-info/RECORD
+Filename: h2o_mlops_scoring_client-0.0.7b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## h2o_mlops_scoring_client/VERSION

```diff
@@ -1 +1 @@
-0.0.6b1
+0.0.7b1
```

## h2o_mlops_scoring_client/_utils.py

```diff
@@ -21,23 +21,27 @@
 
     BIGQUERY = "Google BigQuery table"
     CSV = "CSV file"
     JDBC_QUERY = "SQL query through JDBC connection"
     JDBC_TABLE = "SQL table through JDBC connection"
     ORC = "ORC file"
     PARQUET = "Parquet file"
+    SNOWFLAKE_QUERY = "Snowflake query"
+    SNOWFLAKE_TABLE = "Snowflake table"
 
 
 _format_config: _Dict[Format, _Dict[str, str]] = {
     Format.BIGQUERY: {"format": "bigquery"},
     Format.CSV: {"format": "csv", "header": "true", "inferschema": "true"},
     Format.JDBC_QUERY: {"format": "jdbc"},
     Format.JDBC_TABLE: {"format": "jdbc"},
     Format.ORC: {"format": "orc"},
     Format.PARQUET: {"format": "parquet"},
+    Format.SNOWFLAKE_QUERY: {"format": "net.snowflake.spark.snowflake"},
+    Format.SNOWFLAKE_TABLE: {"format": "net.snowflake.spark.snowflake"},
 }
 
 
 class WriteMode(_enum.Enum):
     """Write modes for sink."""
 
     APPEND = "Append to existing files"
@@ -244,19 +248,30 @@
 
         def score_pandas_dataframe_spark(
             iterator: _Iterator[_pandas.DataFrame],
         ) -> _Iterator[_pandas.DataFrame]:
             for pdf in iterator:
                 yield self.score_pandas_dataframe(pdf, id_column)
 
-        input_columns = [id_column] + [c["name"] for c in self.schema["inputFields"]]
+        id_column_schema = sdf.schema[id_column]
+        if isinstance(id_column_schema.dataType, _pyspark_sql_types.DecimalType):
+            id_column_schema.dataType = _pyspark_sql_types.FloatType()
+        input_schema = _pyspark_sql_types.StructType(
+            [id_column_schema] + [f for f in self.schema_spark_input]
+        )
         output_schema = _pyspark_sql_types.StructType(
-            [sdf.schema[id_column]] + [f for f in self.schema_spark_output]
+            [id_column_schema] + [f for f in self.schema_spark_output]
+        )
+        sdf = sdf.select(
+            *[
+                sdf[f"{column.name}"].cast(f"{column.dataType.typeName()}")
+                for column in input_schema
+            ]
         )
-        scores = sdf.select(input_columns).mapInPandas(
+        scores = sdf.mapInPandas(
             score_pandas_dataframe_spark, schema=output_schema  # type: ignore
         )
         # ^ mypy says incompatible type and I don't know how to fix it
 
         return scores
 
 
@@ -296,27 +311,42 @@
     source_data: str,
     source_format: Format,
     source_config: _Optional[_Dict[str, str]] = None,
 ) -> _pyspark_sql.DataFrame:
     _source_config = _copy.copy(_format_config[source_format])
     if source_config:
         _source_config.update(source_config)
-    if source_format == Format.JDBC_QUERY:
+    if source_format in [Format.JDBC_QUERY, Format.SNOWFLAKE_QUERY]:
         _source_config["query"] = source_data
-    if source_format == Format.JDBC_TABLE:
+    if source_format in [Format.JDBC_TABLE, Format.SNOWFLAKE_TABLE]:
         _source_config["dbtable"] = source_data
     if source_format in [
         Format.JDBC_QUERY,
         Format.JDBC_TABLE,
     ] and not _source_config.get("url"):
         raise RuntimeError("JDBC connection URL required for source.")
+    if source_format in [Format.SNOWFLAKE_QUERY, Format.SNOWFLAKE_TABLE]:
+        required_sf_options = {
+            "sfDatabase",
+            "sfPassword",
+            "sfURL",
+            "sfUser",
+            "sfWarehouse",
+        }
+        missing_sf_options = required_sf_options.difference(_source_config.keys())
+        if missing_sf_options:
+            raise RuntimeError(
+                f"Snowflake option(s) {missing_sf_options} required for source."
+            )
 
     if source_format in [
         Format.JDBC_QUERY,
         Format.JDBC_TABLE,
+        Format.SNOWFLAKE_QUERY,
+        Format.SNOWFLAKE_TABLE,
     ]:
         return spark.read.load(**_source_config)
     else:
         return spark.read.load(source_data, **_source_config)
 
 
 def write_sink(
@@ -325,26 +355,41 @@
     sink_format: Format,
     sink_write_mode: WriteMode,
     sink_config: _Optional[_Dict[str, str]] = None,
 ) -> None:
     _sink_config = _copy.copy(_format_config[sink_format])
     if sink_config:
         _sink_config.update(sink_config)
-    if sink_format == Format.JDBC_QUERY:
+    if sink_format in [Format.JDBC_QUERY, Format.SNOWFLAKE_QUERY]:
         _sink_config["query"] = sink_location
-    if sink_format == Format.JDBC_TABLE:
+    if sink_format in [Format.JDBC_TABLE, Format.SNOWFLAKE_TABLE]:
         _sink_config["dbtable"] = sink_location
     if sink_format in [
         Format.JDBC_QUERY,
         Format.JDBC_TABLE,
     ] and not _sink_config.get("url"):
         raise RuntimeError("JDBC connection URL required for sink.")
+    if sink_format in [Format.SNOWFLAKE_QUERY, Format.SNOWFLAKE_TABLE]:
+        required_sf_options = {
+            "sfDatabase",
+            "sfPassword",
+            "sfURL",
+            "sfUser",
+            "sfWarehouse",
+        }
+        missing_sf_options = required_sf_options.difference(_sink_config.keys())
+        if missing_sf_options:
+            raise RuntimeError(
+                f"Snowflake option(s) {missing_sf_options} required for sink."
+            )
 
     mode = _copy.copy(_write_mode[sink_write_mode])
 
     if sink_format in [
         Format.JDBC_QUERY,
         Format.JDBC_TABLE,
+        Format.SNOWFLAKE_QUERY,
+        Format.SNOWFLAKE_TABLE,
     ]:
         scored_sdf.write.mode(mode).save(**_sink_config)
     else:
         scored_sdf.write.mode(mode).save(sink_location, **_sink_config)
```

## Comparing `h2o_mlops_scoring_client-0.0.6b1.dist-info/METADATA` & `h2o_mlops_scoring_client-0.0.7b1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h2o-mlops-scoring-client
-Version: 0.0.6b1
+Version: 0.0.7b1
 Summary: A Python client library to simplify robust mini-batch scoring against an H2O MLOps scoring endpoint.
 Author: H2O.ai
 Author-email: support@h2o.ai
 License: Proprietary License
 Project-URL: Documentation, https://docs.h2o.ai/mlops/mlops-scoring-client/overview
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/markdown
@@ -82,16 +82,18 @@
 
 The MLOps scoring client can read and write:
 
 - CSV
 - Parquet
 - ORC
 - BigQuery tables
-- JDBC tables
 - JDBC queries
+- JDBC tables
+- Snowflake queries
+- Snowflake tables
 
 If there's a file type you would like to see supported, please let us know.
 
 ### I want model monitoring for batch scoring, can I do that?
 
 Yes. The MLOps Scoring Client uses MLOps scoring endpoints which are automatically monitored.
```

