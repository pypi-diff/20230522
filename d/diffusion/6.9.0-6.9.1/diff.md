# Comparing `tmp/diffusion-6.9.0-1-py3-none-any.whl.zip` & `tmp/diffusion-6.9.1-1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,107 +1,113 @@
-Zip file size: 172011 bytes, number of entries: 105
--rw-r--r--  2.0 unx      248 b- defN 23-Jan-04 09:40 diffusion/__init__.py
--rw-r--r--  2.0 unx      739 b- defN 23-Jan-04 09:40 diffusion/exceptions.py
--rw-r--r--  2.0 unx     3731 b- defN 23-Jan-04 09:40 diffusion/datatypes/__init__.py
--rw-r--r--  2.0 unx      494 b- defN 23-Jan-04 09:40 diffusion/datatypes/exceptions.py
--rw-r--r--  2.0 unx      652 b- defN 23-Jan-04 09:40 diffusion/datatypes/complex/__init__.py
--rw-r--r--  2.0 unx     2053 b- defN 23-Jan-04 09:40 diffusion/datatypes/complex/jsondatatype.py
--rw-r--r--  2.0 unx      214 b- defN 23-Jan-04 09:40 diffusion/datatypes/complex/recorddatatype.py
--rw-r--r--  2.0 unx      204 b- defN 23-Jan-04 09:40 diffusion/datatypes/complex/routingdatatype.py
--rw-r--r--  2.0 unx      204 b- defN 23-Jan-04 09:40 diffusion/datatypes/complex/unknowndatatype.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-04 09:40 diffusion/datatypes/foundation/__init__.py
--rw-r--r--  2.0 unx     7795 b- defN 23-Jan-04 09:40 diffusion/datatypes/foundation/abstract.py
--rw-r--r--  2.0 unx     1850 b- defN 23-Jan-04 09:40 diffusion/datatypes/foundation/datatype.py
--rw-r--r--  2.0 unx     1088 b- defN 23-Jan-04 09:40 diffusion/datatypes/primitives/__init__.py
--rw-r--r--  2.0 unx     2095 b- defN 23-Jan-04 09:40 diffusion/datatypes/primitives/binarydatatype.py
--rw-r--r--  2.0 unx      366 b- defN 23-Jan-04 09:40 diffusion/datatypes/primitives/doubledatatype.py
--rw-r--r--  2.0 unx      988 b- defN 23-Jan-04 09:40 diffusion/datatypes/primitives/int64datatype.py
--rw-r--r--  2.0 unx     1602 b- defN 23-Jan-04 09:40 diffusion/datatypes/primitives/primitivedatatype.py
--rw-r--r--  2.0 unx      234 b- defN 23-Jan-04 09:40 diffusion/datatypes/primitives/stringdatatype.py
--rw-r--r--  2.0 unx    11467 b- defN 23-Jan-04 09:40 diffusion/datatypes/timeseries/__init__.py
--rw-r--r--  2.0 unx    18779 b- defN 23-Jan-04 09:40 diffusion/datatypes/timeseries/time_series_event.py
--rw-r--r--  2.0 unx     2089 b- defN 23-Jan-04 09:40 diffusion/datatypes/timeseries/time_series_event_metadata.py
--rw-r--r--  2.0 unx     1645 b- defN 23-Jan-04 09:40 diffusion/datatypes/timeseries/types.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-04 09:40 diffusion/features/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-04 09:40 diffusion/features/control/__init__.py
--rw-r--r--  2.0 unx     7734 b- defN 23-Jan-04 09:40 diffusion/features/control/metrics/__init__.py
--rw-r--r--  2.0 unx     1138 b- defN 23-Jan-04 09:40 diffusion/features/control/metrics/collector.py
--rw-r--r--  2.0 unx     5218 b- defN 23-Jan-04 09:40 diffusion/features/control/metrics/session_metrics.py
--rw-r--r--  2.0 unx     5046 b- defN 23-Jan-04 09:40 diffusion/features/control/metrics/topic_metrics.py
--rw-r--r--  2.0 unx     9508 b- defN 23-Jan-04 09:40 diffusion/features/control/session_trees/__init__.py
--rw-r--r--  2.0 unx     1334 b- defN 23-Jan-04 09:40 diffusion/features/control/session_trees/branch_mapping.py
--rw-r--r--  2.0 unx     3332 b- defN 23-Jan-04 09:40 diffusion/features/control/session_trees/branch_mapping_table.py
--rw-r--r--  2.0 unx     1031 b- defN 23-Jan-04 09:40 diffusion/features/control/session_trees/invalid_branch_mapping_exception.py
--rw-r--r--  2.0 unx    16865 b- defN 23-Jan-04 09:40 diffusion/features/timeseries/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-04 09:40 diffusion/features/timeseries/query/__init__.py
--rw-r--r--  2.0 unx     6760 b- defN 23-Jan-04 09:40 diffusion/features/timeseries/query/query_result.py
--rw-r--r--  2.0 unx    51194 b- defN 23-Jan-04 09:40 diffusion/features/timeseries/query/range_query.py
--rw-r--r--  2.0 unx    27026 b- defN 23-Jan-04 09:40 diffusion/features/timeseries/query/range_query_parameters.py
--rw-r--r--  2.0 unx     3456 b- defN 23-Jan-04 09:40 diffusion/features/timeseries/query/range_query_request.py
--rw-r--r--  2.0 unx    11170 b- defN 23-Jan-04 09:40 diffusion/features/timeseries/query/range_query_result.py
--rw-r--r--  2.0 unx    12427 b- defN 23-Jan-04 09:40 diffusion/features/topics/__init__.py
--rw-r--r--  2.0 unx     8127 b- defN 23-Jan-04 09:40 diffusion/features/topics/selectors.py
--rw-r--r--  2.0 unx     2731 b- defN 23-Jan-04 09:40 diffusion/features/topics/streams.py
--rw-r--r--  2.0 unx      424 b- defN 23-Jan-04 09:40 diffusion/features/topics/details/__init__.py
--rw-r--r--  2.0 unx    43714 b- defN 23-Jan-04 09:40 diffusion/features/topics/details/topic_specification.py
--rw-r--r--  2.0 unx     4692 b- defN 23-Jan-04 09:40 diffusion/features/topics/update/__init__.py
--rw-r--r--  2.0 unx     4573 b- defN 23-Jan-04 09:40 diffusion/features/topics/update/constraint_factory.py
--rw-r--r--  2.0 unx    12226 b- defN 23-Jan-04 09:40 diffusion/features/topics/update/constraints.py
--rw-r--r--  2.0 unx     4096 b- defN 23-Jan-04 09:40 diffusion/handlers/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-04 09:40 diffusion/internal/__init__.py
--rw-r--r--  2.0 unx      677 b- defN 23-Jan-04 09:40 diffusion/internal/components.py
--rw-r--r--  2.0 unx     1246 b- defN 23-Jan-04 09:40 diffusion/internal/encoder.py
--rw-r--r--  2.0 unx      507 b- defN 23-Jan-04 09:40 diffusion/internal/exceptions.py
--rw-r--r--  2.0 unx    12047 b- defN 23-Jan-04 09:40 diffusion/internal/utils.py
--rw-r--r--  2.0 unx      452 b- defN 23-Jan-04 09:40 diffusion/internal/encoded_data/__init__.py
--rw-r--r--  2.0 unx     2628 b- defN 23-Jan-04 09:40 diffusion/internal/encoded_data/abstract.py
--rw-r--r--  2.0 unx      494 b- defN 23-Jan-04 09:40 diffusion/internal/encoded_data/exceptions.py
--rw-r--r--  2.0 unx     1928 b- defN 23-Jan-04 09:40 diffusion/internal/encoded_data/generics.py
--rw-r--r--  2.0 unx     4912 b- defN 23-Jan-04 09:40 diffusion/internal/encoded_data/scalars.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jan-04 09:40 diffusion/internal/generated/__init__.py
--rw-r--r--  2.0 unx    10365 b- defN 23-Jan-04 09:40 diffusion/internal/generated/services.py
--rw-r--r--  2.0 unx     6965 b- defN 23-Jan-04 09:40 diffusion/internal/protocol/__init__.py
--rw-r--r--  2.0 unx     9658 b- defN 23-Jan-04 09:40 diffusion/internal/protocol/conversations.py
--rw-r--r--  2.0 unx     2518 b- defN 23-Jan-04 09:40 diffusion/internal/protocol/exceptions.py
--rw-r--r--  2.0 unx     8325 b- defN 23-Jan-04 09:40 diffusion/internal/protocol/message_types.py
--rw-r--r--  2.0 unx    11585 b- defN 23-Jan-04 09:40 diffusion/internal/protocol/properties.py
--rw-r--r--  2.0 unx     1128 b- defN 23-Jan-04 09:40 diffusion/internal/serialisers/__init__.py
--rw-r--r--  2.0 unx     2721 b- defN 23-Jan-04 09:40 diffusion/internal/serialisers/attrs.py
--rw-r--r--  2.0 unx    13067 b- defN 23-Jan-04 09:40 diffusion/internal/serialisers/base.py
--rw-r--r--  2.0 unx     6990 b- defN 23-Jan-04 09:40 diffusion/internal/serialisers/compound.py
--rw-r--r--  2.0 unx      901 b- defN 23-Jan-04 09:40 diffusion/internal/serialisers/dataclass_model.py
--rw-r--r--  2.0 unx    11433 b- defN 23-Jan-04 09:40 diffusion/internal/serialisers/generic_model.py
--rw-r--r--  2.0 unx     1844 b- defN 23-Jan-04 09:40 diffusion/internal/serialisers/pydantic.py
--rw-r--r--  2.0 unx    39211 b- defN 23-Jan-04 09:40 diffusion/internal/serialisers/spec.py
--rw-r--r--  2.0 unx     3240 b- defN 23-Jan-04 09:40 diffusion/internal/serialisers/timeseries.py
--rw-r--r--  2.0 unx      688 b- defN 23-Jan-04 09:40 diffusion/internal/services/__init__.py
--rw-r--r--  2.0 unx    14200 b- defN 23-Jan-04 09:40 diffusion/internal/services/abstract.py
--rw-r--r--  2.0 unx      406 b- defN 23-Jan-04 09:40 diffusion/internal/services/exceptions.py
--rw-r--r--  2.0 unx     2001 b- defN 23-Jan-04 09:40 diffusion/internal/services/locator.py
--rw-r--r--  2.0 unx     6822 b- defN 23-Jan-04 09:40 diffusion/internal/services/messaging.py
--rw-r--r--  2.0 unx     1769 b- defN 23-Jan-04 09:40 diffusion/internal/services/session.py
--rw-r--r--  2.0 unx     5667 b- defN 23-Jan-04 09:40 diffusion/internal/services/topics.py
--rw-r--r--  2.0 unx     6646 b- defN 23-Jan-04 09:40 diffusion/internal/session/__init__.py
--rw-r--r--  2.0 unx     8506 b- defN 23-Jan-04 09:40 diffusion/internal/session/connection.py
--rw-r--r--  2.0 unx     1678 b- defN 23-Jan-04 09:40 diffusion/internal/session/credentials.py
--rw-r--r--  2.0 unx     4292 b- defN 23-Jan-04 09:40 diffusion/internal/session/error_reason.py
--rw-r--r--  2.0 unx     8161 b- defN 23-Jan-04 09:40 diffusion/internal/session/exception_handler.py
--rw-r--r--  2.0 unx     7483 b- defN 23-Jan-04 09:40 diffusion/internal/topics/__init__.py
--rw-r--r--  2.0 unx      311 b- defN 23-Jan-04 09:40 diffusion/internal/topics/constraints.py
--rw-r--r--  2.0 unx     2192 b- defN 23-Jan-04 09:40 diffusion/internal/validation/__init__.py
--rw-r--r--  2.0 unx     1923 b- defN 23-Jan-04 09:40 diffusion/internal/validation/pydantic.py
--rw-r--r--  2.0 unx    10373 b- defN 23-Jan-04 09:40 diffusion/messaging/__init__.py
--rw-r--r--  2.0 unx    13206 b- defN 23-Jan-04 09:40 diffusion/session/__init__.py
--rw-r--r--  2.0 unx     5509 b- defN 23-Jan-04 09:40 diffusion/session/exceptions.py
--rw-r--r--  2.0 unx     2166 b- defN 23-Jan-04 09:40 diffusion/session/retry_strategy.py
--rw-r--r--  2.0 unx     1223 b- defN 23-Jan-04 09:40 diffusion/session/session_container_factory.py
--rw-r--r--  2.0 unx    12135 b- defN 23-Jan-04 09:40 diffusion/session/session_factory.py
--rw-r--r--  2.0 unx      424 b- defN 23-Jan-04 09:40 diffusion/session/locks/__init__.py
--rw-r--r--  2.0 unx     2112 b- defN 23-Jan-04 09:40 diffusion/session/locks/session_lock_acquisition.py
--rw-r--r--  2.0 unx      805 b- defN 23-Jan-04 09:40 diffusion/session/locks/session_lock_request.py
--rw-r--r--  2.0 unx      710 b- defN 23-Jan-04 09:40 diffusion/session/locks/session_lock_request_cancellation.py
--rw-r--r--  2.0 unx    14842 b- defN 23-Jan-04 09:40 diffusion/session/locks/session_locks.py
--rw-r--r--  2.0 unx     1646 b- defN 23-Jan-04 09:40 diffusion-6.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx      102 b- defN 23-Jan-04 09:40 diffusion-6.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jan-04 09:40 diffusion-6.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    10356 b- defN 23-Jan-04 09:40 diffusion-6.9.0.dist-info/RECORD
-105 files, 605565 bytes uncompressed, 155113 bytes compressed:  74.4%
+Zip file size: 179966 bytes, number of entries: 111
+-rw-rw-rw-  2.0 unx      248 b- defN 23-Mar-28 09:10 diffusion/__init__.py
+-rw-rw-rw-  2.0 unx      739 b- defN 23-Mar-28 09:10 diffusion/exceptions.py
+-rw-rw-rw-  2.0 unx     3781 b- defN 23-Mar-28 09:10 diffusion/datatypes/__init__.py
+-rw-rw-rw-  2.0 unx      494 b- defN 23-Mar-28 09:10 diffusion/datatypes/exceptions.py
+-rw-rw-rw-  2.0 unx      652 b- defN 23-Mar-28 09:10 diffusion/datatypes/complex/__init__.py
+-rw-rw-rw-  2.0 unx     2053 b- defN 23-Mar-28 09:10 diffusion/datatypes/complex/jsondatatype.py
+-rw-rw-rw-  2.0 unx      214 b- defN 23-Mar-28 09:10 diffusion/datatypes/complex/recorddatatype.py
+-rw-rw-rw-  2.0 unx      204 b- defN 23-Mar-28 09:10 diffusion/datatypes/complex/routingdatatype.py
+-rw-rw-rw-  2.0 unx      204 b- defN 23-Mar-28 09:10 diffusion/datatypes/complex/unknowndatatype.py
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Mar-28 09:10 diffusion/datatypes/foundation/__init__.py
+-rw-rw-rw-  2.0 unx     7795 b- defN 23-Mar-28 09:10 diffusion/datatypes/foundation/abstract.py
+-rw-rw-rw-  2.0 unx     1850 b- defN 23-Mar-28 09:10 diffusion/datatypes/foundation/datatype.py
+-rw-rw-rw-  2.0 unx     1088 b- defN 23-Mar-28 09:10 diffusion/datatypes/primitives/__init__.py
+-rw-rw-rw-  2.0 unx     2095 b- defN 23-Mar-28 09:10 diffusion/datatypes/primitives/binarydatatype.py
+-rw-rw-rw-  2.0 unx      366 b- defN 23-Mar-28 09:10 diffusion/datatypes/primitives/doubledatatype.py
+-rw-rw-rw-  2.0 unx      988 b- defN 23-Mar-28 09:10 diffusion/datatypes/primitives/int64datatype.py
+-rw-rw-rw-  2.0 unx     1602 b- defN 23-Mar-28 09:10 diffusion/datatypes/primitives/primitivedatatype.py
+-rw-rw-rw-  2.0 unx      234 b- defN 23-Mar-28 09:10 diffusion/datatypes/primitives/stringdatatype.py
+-rw-rw-rw-  2.0 unx    11467 b- defN 23-Mar-28 09:10 diffusion/datatypes/timeseries/__init__.py
+-rw-rw-rw-  2.0 unx    19412 b- defN 23-Mar-28 09:10 diffusion/datatypes/timeseries/time_series_event.py
+-rw-rw-rw-  2.0 unx     2997 b- defN 23-Mar-28 09:10 diffusion/datatypes/timeseries/time_series_event_metadata.py
+-rw-rw-rw-  2.0 unx     1645 b- defN 23-Mar-28 09:10 diffusion/datatypes/timeseries/types.py
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Mar-28 09:10 diffusion/features/__init__.py
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Mar-28 09:10 diffusion/features/control/__init__.py
+-rw-rw-rw-  2.0 unx     8750 b- defN 23-Mar-28 09:10 diffusion/features/control/metrics/__init__.py
+-rw-rw-rw-  2.0 unx     1138 b- defN 23-Mar-28 09:10 diffusion/features/control/metrics/collector.py
+-rw-rw-rw-  2.0 unx     5218 b- defN 23-Mar-28 09:10 diffusion/features/control/metrics/session_metrics.py
+-rw-rw-rw-  2.0 unx     5158 b- defN 23-Mar-28 09:10 diffusion/features/control/metrics/topic_metrics.py
+-rw-rw-rw-  2.0 unx     9508 b- defN 23-Mar-28 09:10 diffusion/features/control/session_trees/__init__.py
+-rw-rw-rw-  2.0 unx     1334 b- defN 23-Mar-28 09:10 diffusion/features/control/session_trees/branch_mapping.py
+-rw-rw-rw-  2.0 unx     3409 b- defN 23-Mar-28 09:10 diffusion/features/control/session_trees/branch_mapping_table.py
+-rw-rw-rw-  2.0 unx     1031 b- defN 23-Mar-28 09:10 diffusion/features/control/session_trees/invalid_branch_mapping_exception.py
+-rw-rw-rw-  2.0 unx    17686 b- defN 23-Mar-28 09:10 diffusion/features/timeseries/__init__.py
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Mar-28 09:10 diffusion/features/timeseries/query/__init__.py
+-rw-rw-rw-  2.0 unx     6760 b- defN 23-Mar-28 09:10 diffusion/features/timeseries/query/query_result.py
+-rw-rw-rw-  2.0 unx    49729 b- defN 23-Mar-28 09:10 diffusion/features/timeseries/query/range_query.py
+-rw-rw-rw-  2.0 unx      710 b- defN 23-Mar-28 09:10 diffusion/features/timeseries/query/range_query_parameters.py
+-rw-rw-rw-  2.0 unx    12515 b- defN 23-Mar-28 09:10 diffusion/features/topics/__init__.py
+-rw-rw-rw-  2.0 unx     8127 b- defN 23-Mar-28 09:10 diffusion/features/topics/selectors.py
+-rw-rw-rw-  2.0 unx     2731 b- defN 23-Mar-28 09:10 diffusion/features/topics/streams.py
+-rw-rw-rw-  2.0 unx      424 b- defN 23-Mar-28 09:10 diffusion/features/topics/details/__init__.py
+-rw-rw-rw-  2.0 unx    43807 b- defN 23-Mar-28 09:10 diffusion/features/topics/details/topic_specification.py
+-rw-rw-rw-  2.0 unx     4557 b- defN 23-Mar-28 09:10 diffusion/features/topics/update/__init__.py
+-rw-rw-rw-  2.0 unx     4573 b- defN 23-Mar-28 09:10 diffusion/features/topics/update/constraint_factory.py
+-rw-rw-rw-  2.0 unx    13539 b- defN 23-Mar-28 09:10 diffusion/features/topics/update/constraints.py
+-rw-rw-rw-  2.0 unx     4096 b- defN 23-Mar-28 09:10 diffusion/handlers/__init__.py
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Mar-28 09:10 diffusion/internal/__init__.py
+-rw-rw-rw-  2.0 unx      677 b- defN 23-Mar-28 09:10 diffusion/internal/components.py
+-rw-rw-rw-  2.0 unx     1246 b- defN 23-Mar-28 09:10 diffusion/internal/encoder.py
+-rw-rw-rw-  2.0 unx      507 b- defN 23-Mar-28 09:10 diffusion/internal/exceptions.py
+-rw-rw-rw-  2.0 unx    12064 b- defN 23-Mar-28 09:10 diffusion/internal/utils.py
+-rw-rw-rw-  2.0 unx      452 b- defN 23-Mar-28 09:10 diffusion/internal/encoded_data/__init__.py
+-rw-rw-rw-  2.0 unx     4234 b- defN 23-Mar-28 09:10 diffusion/internal/encoded_data/abstract.py
+-rw-rw-rw-  2.0 unx      494 b- defN 23-Mar-28 09:10 diffusion/internal/encoded_data/exceptions.py
+-rw-rw-rw-  2.0 unx     1928 b- defN 23-Mar-28 09:10 diffusion/internal/encoded_data/generics.py
+-rw-rw-rw-  2.0 unx     4912 b- defN 23-Mar-28 09:10 diffusion/internal/encoded_data/scalars.py
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Mar-28 09:10 diffusion/internal/generated/__init__.py
+-rw-rw-rw-  2.0 unx    10827 b- defN 23-Mar-28 09:10 diffusion/internal/generated/services.py
+-rw-rw-rw-  2.0 unx     6965 b- defN 23-Mar-28 09:10 diffusion/internal/protocol/__init__.py
+-rw-rw-rw-  2.0 unx     9658 b- defN 23-Mar-28 09:10 diffusion/internal/protocol/conversations.py
+-rw-rw-rw-  2.0 unx     2518 b- defN 23-Mar-28 09:10 diffusion/internal/protocol/exceptions.py
+-rw-rw-rw-  2.0 unx     8325 b- defN 23-Mar-28 09:10 diffusion/internal/protocol/message_types.py
+-rw-rw-rw-  2.0 unx    11585 b- defN 23-Mar-28 09:10 diffusion/internal/protocol/properties.py
+-rw-rw-rw-  2.0 unx     1501 b- defN 23-Mar-28 09:10 diffusion/internal/serialisers/__init__.py
+-rw-rw-rw-  2.0 unx     2619 b- defN 23-Mar-28 09:10 diffusion/internal/serialisers/attrs.py
+-rw-rw-rw-  2.0 unx    18544 b- defN 23-Mar-28 09:10 diffusion/internal/serialisers/base.py
+-rw-rw-rw-  2.0 unx     7541 b- defN 23-Mar-28 09:10 diffusion/internal/serialisers/compound.py
+-rw-rw-rw-  2.0 unx    13422 b- defN 23-Mar-28 09:10 diffusion/internal/serialisers/generic_model.py
+-rw-rw-rw-  2.0 unx      786 b- defN 23-Mar-28 09:10 diffusion/internal/serialisers/primitives.py
+-rw-rw-rw-  2.0 unx     1712 b- defN 23-Mar-28 09:10 diffusion/internal/serialisers/pydantic.py
+-rw-rw-rw-  2.0 unx    42379 b- defN 23-Mar-28 09:10 diffusion/internal/serialisers/spec.py
+-rw-rw-rw-  2.0 unx     4071 b- defN 23-Mar-28 09:10 diffusion/internal/serialisers/timeseries.py
+-rw-rw-rw-  2.0 unx      688 b- defN 23-Mar-28 09:10 diffusion/internal/services/__init__.py
+-rw-rw-rw-  2.0 unx    13677 b- defN 23-Mar-28 09:10 diffusion/internal/services/abstract.py
+-rw-rw-rw-  2.0 unx      406 b- defN 23-Mar-28 09:10 diffusion/internal/services/exceptions.py
+-rw-rw-rw-  2.0 unx     2001 b- defN 23-Mar-28 09:10 diffusion/internal/services/locator.py
+-rw-rw-rw-  2.0 unx     6822 b- defN 23-Mar-28 09:10 diffusion/internal/services/messaging.py
+-rw-rw-rw-  2.0 unx     1769 b- defN 23-Mar-28 09:10 diffusion/internal/services/session.py
+-rw-rw-rw-  2.0 unx     5667 b- defN 23-Mar-28 09:10 diffusion/internal/services/topics.py
+-rw-rw-rw-  2.0 unx     6646 b- defN 23-Mar-28 09:10 diffusion/internal/session/__init__.py
+-rw-rw-rw-  2.0 unx     8506 b- defN 23-Mar-28 09:10 diffusion/internal/session/connection.py
+-rw-rw-rw-  2.0 unx     1678 b- defN 23-Mar-28 09:10 diffusion/internal/session/credentials.py
+-rw-rw-rw-  2.0 unx     4292 b- defN 23-Mar-28 09:10 diffusion/internal/session/error_reason.py
+-rw-rw-rw-  2.0 unx     8161 b- defN 23-Mar-28 09:10 diffusion/internal/session/exception_handler.py
+-rw-rw-rw-  2.0 unx      424 b- defN 23-Mar-28 09:10 diffusion/internal/session/locks/__init__.py
+-rw-rw-rw-  2.0 unx     1360 b- defN 23-Mar-28 09:10 diffusion/internal/session/locks/session_lock_acquisition.py
+-rw-rw-rw-  2.0 unx      805 b- defN 23-Mar-28 09:10 diffusion/internal/session/locks/session_lock_request.py
+-rw-rw-rw-  2.0 unx      710 b- defN 23-Mar-28 09:10 diffusion/internal/session/locks/session_lock_request_cancellation.py
+-rw-rw-rw-  2.0 unx      424 b- defN 23-Mar-28 09:10 diffusion/internal/timeseries/__init__.py
+-rw-rw-rw-  2.0 unx      424 b- defN 23-Mar-28 09:10 diffusion/internal/timeseries/query/__init__.py
+-rw-rw-rw-  2.0 unx     2363 b- defN 23-Mar-28 09:10 diffusion/internal/timeseries/query/range_query.py
+-rw-rw-rw-  2.0 unx    27383 b- defN 23-Mar-28 09:10 diffusion/internal/timeseries/query/range_query_parameters.py
+-rw-rw-rw-  2.0 unx     3556 b- defN 23-Mar-28 09:10 diffusion/internal/timeseries/query/range_query_request.py
+-rw-rw-rw-  2.0 unx    10765 b- defN 23-Mar-28 09:10 diffusion/internal/timeseries/query/range_query_result.py
+-rw-rw-rw-  2.0 unx     7618 b- defN 23-Mar-28 09:10 diffusion/internal/topics/__init__.py
+-rw-rw-rw-  2.0 unx      311 b- defN 23-Mar-28 09:10 diffusion/internal/topics/constraints.py
+-rw-rw-rw-  2.0 unx     2192 b- defN 23-Mar-28 09:10 diffusion/internal/validation/__init__.py
+-rw-rw-rw-  2.0 unx     1923 b- defN 23-Mar-28 09:10 diffusion/internal/validation/pydantic.py
+-rw-rw-rw-  2.0 unx    10373 b- defN 23-Mar-28 09:10 diffusion/messaging/__init__.py
+-rw-rw-rw-  2.0 unx    13266 b- defN 23-Mar-28 09:10 diffusion/session/__init__.py
+-rw-rw-rw-  2.0 unx     5509 b- defN 23-Mar-28 09:10 diffusion/session/exceptions.py
+-rw-rw-rw-  2.0 unx     2166 b- defN 23-Mar-28 09:10 diffusion/session/retry_strategy.py
+-rw-rw-rw-  2.0 unx     1223 b- defN 23-Mar-28 09:10 diffusion/session/session_container_factory.py
+-rw-rw-rw-  2.0 unx    12135 b- defN 23-Mar-28 09:10 diffusion/session/session_factory.py
+-rw-rw-rw-  2.0 unx      424 b- defN 23-Mar-28 09:10 diffusion/session/locks/__init__.py
+-rw-rw-rw-  2.0 unx      929 b- defN 23-Mar-28 09:10 diffusion/session/locks/session_lock_acquisition.py
+-rw-rw-rw-  2.0 unx    14937 b- defN 23-Mar-28 09:10 diffusion/session/locks/session_locks.py
+-rw-rw-rw-  2.0 unx     1706 b- defN 23-Mar-28 09:10 diffusion-6.9.1.dist-info/METADATA
+-rw-rw-rw-  2.0 unx      102 b- defN 23-Mar-28 09:10 diffusion-6.9.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       10 b- defN 23-Mar-28 09:10 diffusion-6.9.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    11009 b- defN 23-Mar-28 09:10 diffusion-6.9.1.dist-info/RECORD
+111 files, 628255 bytes uncompressed, 161980 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -105,20 +105,14 @@
 
 Filename: diffusion/features/timeseries/query/range_query.py
 Comment: 
 
 Filename: diffusion/features/timeseries/query/range_query_parameters.py
 Comment: 
 
-Filename: diffusion/features/timeseries/query/range_query_request.py
-Comment: 
-
-Filename: diffusion/features/timeseries/query/range_query_result.py
-Comment: 
-
 Filename: diffusion/features/topics/__init__.py
 Comment: 
 
 Filename: diffusion/features/topics/selectors.py
 Comment: 
 
 Filename: diffusion/features/topics/streams.py
@@ -201,18 +195,18 @@
 
 Filename: diffusion/internal/serialisers/base.py
 Comment: 
 
 Filename: diffusion/internal/serialisers/compound.py
 Comment: 
 
-Filename: diffusion/internal/serialisers/dataclass_model.py
+Filename: diffusion/internal/serialisers/generic_model.py
 Comment: 
 
-Filename: diffusion/internal/serialisers/generic_model.py
+Filename: diffusion/internal/serialisers/primitives.py
 Comment: 
 
 Filename: diffusion/internal/serialisers/pydantic.py
 Comment: 
 
 Filename: diffusion/internal/serialisers/spec.py
 Comment: 
@@ -252,14 +246,44 @@
 
 Filename: diffusion/internal/session/error_reason.py
 Comment: 
 
 Filename: diffusion/internal/session/exception_handler.py
 Comment: 
 
+Filename: diffusion/internal/session/locks/__init__.py
+Comment: 
+
+Filename: diffusion/internal/session/locks/session_lock_acquisition.py
+Comment: 
+
+Filename: diffusion/internal/session/locks/session_lock_request.py
+Comment: 
+
+Filename: diffusion/internal/session/locks/session_lock_request_cancellation.py
+Comment: 
+
+Filename: diffusion/internal/timeseries/__init__.py
+Comment: 
+
+Filename: diffusion/internal/timeseries/query/__init__.py
+Comment: 
+
+Filename: diffusion/internal/timeseries/query/range_query.py
+Comment: 
+
+Filename: diffusion/internal/timeseries/query/range_query_parameters.py
+Comment: 
+
+Filename: diffusion/internal/timeseries/query/range_query_request.py
+Comment: 
+
+Filename: diffusion/internal/timeseries/query/range_query_result.py
+Comment: 
+
 Filename: diffusion/internal/topics/__init__.py
 Comment: 
 
 Filename: diffusion/internal/topics/constraints.py
 Comment: 
 
 Filename: diffusion/internal/validation/__init__.py
@@ -288,29 +312,23 @@
 
 Filename: diffusion/session/locks/__init__.py
 Comment: 
 
 Filename: diffusion/session/locks/session_lock_acquisition.py
 Comment: 
 
-Filename: diffusion/session/locks/session_lock_request.py
-Comment: 
-
-Filename: diffusion/session/locks/session_lock_request_cancellation.py
-Comment: 
-
 Filename: diffusion/session/locks/session_locks.py
 Comment: 
 
-Filename: diffusion-6.9.0.dist-info/METADATA
+Filename: diffusion-6.9.1.dist-info/METADATA
 Comment: 
 
-Filename: diffusion-6.9.0.dist-info/WHEEL
+Filename: diffusion-6.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: diffusion-6.9.0.dist-info/top_level.txt
+Filename: diffusion-6.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: diffusion-6.9.0.dist-info/RECORD
+Filename: diffusion-6.9.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## diffusion/datatypes/__init__.py

```diff
@@ -95,19 +95,19 @@
                    `DataType` subclass, which is returned unchanged.
 
     Raises:
         `UnknownDataTypeError`: If the corresponding data type was not found.
 
     Examples:
         >>> get('string')
-        <class 'diffusion.datatypes.simple.StringDataType'>
+        <class 'diffusion.datatypes.primitives.stringdatatype.StringDataType'>
         >>> get(INT64)
-        <class 'diffusion.datatypes.simple.Int64DataType'>
+        <class 'diffusion.datatypes.primitives.int64datatype.Int64DataType'>
         >>> get(15)
-        <class 'diffusion.datatypes.complex.JsonDataType'>
+        <class 'diffusion.datatypes.complex.jsondatatype.JsonDataType'>
     """
     if isinstance(data_type, str):
         data_type = getattr(_dt_module, data_type.strip().upper(), None)
     if isinstance(data_type, int):
         data_type = _indexed_data_types.get(data_type)
     if isinstance(data_type, TopicSpecification):
         return data_type.topic_type
```

## diffusion/datatypes/timeseries/time_series_event.py

```diff
@@ -1,8 +1,8 @@
-#   Copyright (c) 2022 Push Technology Ltd., All Rights Reserved.
+#   Copyright (c) 2022-2023 Push Technology Ltd., All Rights Reserved.
 #
 #   Use is subject to license terms.
 #
 #  NOTICE: All information contained herein is, and remains the
 #  property of Push Technology. The intellectual and technical
 #  concepts contained herein are proprietary to Push Technology and
 #  may be covered by U.S. and Foreign Patents, patents in process, and
@@ -19,20 +19,19 @@
 from pydantic import StrictInt
 
 from diffusion.datatypes.timeseries.types import (
     VT,
     VT_other,
     TimeSeriesValueType,
 )
+from diffusion.internal.serialisers.base import ChoiceProvider
+from diffusion.internal.serialisers.generic_model import GenericModel
 from diffusion.internal.validation import StrictNonNegativeInt
 
-try:
-    from typing import final  # type: ignore
-except ImportError:
-    from typing_extensions import final  # type: ignore
+from typing_extensions import final, Literal  # type: ignore
 from io import BytesIO
 
 import pydantic
 import stringcase
 
 from diffusion.datatypes import AbstractDataType
 from diffusion.datatypes.foundation.abstract import (
@@ -61,22 +60,27 @@
 
     def __int__(self):
         return self.value
 
     @functools.lru_cache(maxsize=None)
     def get_type(
         self,
-    ) -> typing.Type["Event_Variants"]:
-
-        return typing.cast(typing.Type[Event_Variants], Content.mapping.get(self))
+    ) -> typing.Type["Event"]:
+        for x in (OriginalEvent, EditEvent, AuthorEncoding, Offsets):
+            if (
+                typing.cast(ChoiceProvider, typing.cast(GenericModel, x).Config).id()
+                == self
+            ):
+                return typing.cast(typing.Type[Event], x)
+        raise RuntimeError(f"Cannot convert {self} to an Event class")
 
     @classmethod
     def from_int(
         cls, event_type: int
-    ) -> typing.Optional[typing.Type["Event_Variants"]]:
+    ) -> typing.Optional[typing.Type["Event"]]:
         if event_type not in cls.__members__.values():
             return None
         ev = cls(event_type)
         return ev.get_type()
 
     @classmethod
     @typing.overload
@@ -92,25 +96,18 @@
     ) -> typing.Optional[EventType]:
         return cls._from_type(tp)
 
     @classmethod
     @functools.lru_cache(maxsize=None)
     def _from_type(
         cls, tp: typing.Union[typing.Hashable, typing.Type[Event_Variants]]
-    ) -> typing.Optional[EventType]:
+    ) -> EventType:
         if not inspect.isclass(tp):
             tp = type(tp)
-        return next(
-            iter(
-                name
-                for name, tp_match in Content.mapping.items()
-                if issubclass(tp, tp_match)
-            ),
-            None,
-        )
+        return typing.cast(EventType, tp.Config.id())
 
 
 Event_T = typing.TypeVar("Event_T", bound="Event")
 
 
 class EventTypeFactory(typing.Generic[VT]):
     @classmethod
@@ -124,15 +121,15 @@
         #    return cls
         type_name = typing.cast(AbstractDataType, val_type).type_name
         return typing.cast(
             typing.Type[Event_T],
             type(
                 f"{model_cls.__name__}{stringcase.pascalcase(type_name)}",
                 (model_cls,),
-                {"_value_type": val_type, "type_name": f"event-{type_name}"},
+                {"_value_type": val_type, "type_name": f"event-{type_name}"}
             ),
         )
 
     @classmethod
     def of(
         cls, model_cls: typing.Type[Event], val_type: typing.Type[VT_other]
     ) -> typing.Type[Event[VT_other]]:
@@ -156,19 +153,23 @@
     value: typing.Optional[VT] = pydantic.Field()
     """ Value of event payload """
 
     _value_type: typing.ClassVar[type]
 
     encoder: typing.Type[Encoder] = DefaultEncoder
 
-    class Config(MarshalledModel.Config):
+    class Config(MarshalledModel.Config, ChoiceProvider[EventType]):
         allow_mutation = False
         frozen = True
         alias_generator = None
 
+        @classmethod
+        def id(cls) -> EventType:
+            raise NotImplementedError()
+
     @property
     def is_original_event(self):
         """
         Flag indicating whether this is an original event
         """
         return not self.is_edit_event
 
@@ -395,27 +396,32 @@
     def edit_author_code(self):
         return self.metadata.author
 
 
 @final
 class OriginalEvent(typing.Generic[VT], Event[VT]):
     class Config(Event.Config):
+        @classmethod
+        def id(cls) -> Literal[EventType.ORIGINAL_EVENT]:
+            return EventType.ORIGINAL_EVENT
+
         alias = "range-query-original-event"
 
         @classmethod
         def attr_mappings_all(cls, modelcls):
             return {
                 "range-query-original-event": {
-                    "rq-time-series-event-metadata.sequence": "original_sequence",
+                    "rq-time-series-event-metadata.time-series-sequence": "original_sequence",
                     "rq-time-series-event-metadata.timestamp": "original_timestamp",
                     "rq-time-series-event-metadata.author-code.bytes": "original_author_code",
                     "value": "value",
                 },
                 "original-event": {
-                    "original-event.time-series-event-metadata.sequence": "original_sequence",
+                    "original-event.time-series-event-metadata.time-series-sequence":
+                        "original_sequence",
                     "original-event.time-series-event-metadata.timestamp": "original_timestamp",
                     "original-event.time-series-event-metadata.author": "original_author",
                     "original-event.value": "value",
                 },
             }
 
     @classmethod
@@ -458,40 +464,45 @@
         Args:
             stream: the input stream
 
 
         Returns:
             the event that was read from the stream
         """
-        return cls.Config.read(cls, stream, "original-event")
+        return cls.Config.read(cls, stream, cls.Config.serialiser("original-event"))
 
 
 @final
 class EditEvent(typing.Generic[VT], Event[VT]):
     class Config(Event.Config):
+        @classmethod
+        def id(cls):
+            return EventType.EDIT_EVENT
+
         alias = "range-query-edit-event"
         # fmt: off
         mappings = {
             "range-query-edit-event": {
-                "rq-time-series-event-metadata.sequence": "original_sequence",
+                "rq-time-series-event-metadata.time-series-sequence": "original_sequence",
                 "rq-time-series-event-metadata.timestamp": "original_timestamp",
                 "rq-time-series-event-metadata.author-code.bytes": "original_author_code",
-                "range-query-original-event.rq-time-series-event-metadata.sequence":
+                "range-query-original-event.rq-time-series-event-metadata.time-series-sequence":
                     "edit_sequence",
                 "range-query-original-event.rq-time-series-event-metadata.timestamp":
                     "edit_timestamp",
                 "range-query-original-event.rq-time-series-event-metadata.author-code.bytes":
                     "edit_author_code",
                 "range-query-original-event.value": "value",
             },
             "edit-event": {
-                "time-series-event-metadata.sequence": "original_sequence",
+                "time-series-event-metadata.time-series-sequence": "original_sequence",
                 "time-series-event-metadata.timestamp": "original_timestamp",
                 "time-series-event-metadata.author": "original_author",
-                "original-event.time-series-event-metadata.sequence": "edit_sequence",
+                "original-event.time-series-event-metadata.time-series-sequence":
+                    "edit_sequence",
                 "original-event.time-series-event-metadata.timestamp": "edit_timestamp",
                 "original-event.time-series-event-metadata.author": "edit_author",
                 "original-event.value": "value",
             },
         }
         # fmt: on
 
@@ -546,28 +557,32 @@
         Args:
             stream: the input stream
 
         Returns:
             the event that was read from the stream
         """
         # return cls.from_bytes(bytes(stream), sys.byteorder)
-        return cls.Config.read(cls, stream, serialiser="edit-event")
+        return cls.Config.read(cls, stream, serialiser=cls.Config.serialiser("edit-event"))
 
 
 @final
 class Offsets(MarshalledModel):
-    class Config(MarshalledModel.Config):
+    class Config(MarshalledModel.Config, ChoiceProvider):
+        @classmethod
+        def id(cls) -> int:
+            return EventType.METADATA_OFFSETS
+
         alias = "range-query-metadata-offsets"
         frozen = True
 
         @classmethod
         def attr_mappings_all(cls, modelcls):
             return {
                 "range-query-metadata-offsets": {
-                    "sequence": "sequence",
+                    "time-series-sequence": "sequence",
                     "timestamp": "timestamp",
                 }
             }
 
     sequence: StrictNonNegativeInt = 0
 
     timestamp: StrictInt = 0
@@ -587,15 +602,19 @@
         if not original_event:
             return None
         return original_event.offset(self)
 
 
 @final
 class AuthorEncoding(MarshalledModel):
-    class Config(MarshalledModel.Config):
+    class Config(MarshalledModel.Config, ChoiceProvider):
+        @classmethod
+        def id(cls) -> int:
+            return EventType.AUTHOR_ENCODING
+
         alias = "range-query-author-encoding"
         alias_generator = None
 
         @classmethod
         def attr_mappings_all(cls, modelcls):
             return {
                 "range-query-author-encoding": {
@@ -605,16 +624,7 @@
             }
 
     author_code: bytes
     author: str
 
 
 Event_Variants = typing.Union["OriginalEvent", "EditEvent", "Offsets", "AuthorEncoding"]
-
-
-class Content(object):
-    mapping = {
-        EventType.ORIGINAL_EVENT: OriginalEvent,
-        EventType.EDIT_EVENT: EditEvent,
-        EventType.METADATA_OFFSETS: Offsets,
-        EventType.AUTHOR_ENCODING: AuthorEncoding,
-    }
```

## diffusion/datatypes/timeseries/time_series_event_metadata.py

```diff
@@ -1,7 +1,17 @@
+#  Copyright (c) 2022-2023 Push Technology Ltd., All Rights Reserved.
+#
+#  Use is subject to license terms.
+#
+#  NOTICE: All information contained herein is, and remains the
+#  property of Push Technology. The intellectual and technical
+#  concepts contained herein are proprietary to Push Technology and
+#  may be covered by U.S. and Foreign Patents, patents in process, and
+#  are protected by trade secret or copyright law.
+
 from __future__ import annotations
 
 import typing
 
 from diffusion.internal.serialisers.pydantic import MarshalledModel
 
 if typing.TYPE_CHECKING:
@@ -51,16 +61,24 @@
         alias = "time-series-event-metadata"
         allow_mutation = False
         frozen = True
 
         @classmethod
         def attr_mappings_all(cls, modelcls):
             return {
-                "time-series-event-metadata": {},
-                "time-series-update-response": {},
+                "time-series-event-metadata": {
+                    "time-series-event-metadata.time-series-sequence": "sequence",
+                    "time-series-event-metadata.timestamp": "timestamp",
+                    "time-series-event-metadata.author": "author",
+                },
+                "time-series-update-response": {
+                    "time-series-event-metadata.time-series-sequence": "sequence",
+                    "time-series-event-metadata.timestamp": "timestamp",
+                    "time-series-event-metadata.author": "author",
+                },
             }
 
     def offset(self, offsets: Offsets) -> EventMetadata:
         return self.copy(
             update={
                 "timestamp": self.timestamp + offsets.timestamp,
                 "sequence": self.sequence + offsets.sequence,
```

## diffusion/features/control/metrics/__init__.py

```diff
@@ -1,27 +1,55 @@
-#  Copyright (c) 2021, 2022 Push Technology Ltd., All Rights Reserved.
+#  Copyright (c) 2021-2023 Push Technology Ltd., All Rights Reserved.
 #
 #  Use is subject to license terms.
 #
 #  NOTICE: All information contained herein is, and remains the
 #  property of Push Technology. The intellectual and technical
 #  concepts contained herein are proprietary to Push Technology and
 #  may be covered by U.S. and Foreign Patents, patents in process, and
 #  are protected by trade secret or copyright law.
-
+from __future__ import annotations
 import typing
 
 from diffusion.features.control.metrics.collector import MetricCollector
 from diffusion.features.control.metrics.session_metrics import SessionMetricCollector
 from diffusion.features.control.metrics.topic_metrics import TopicMetricCollector
 from diffusion.internal.components import Component
 from diffusion.internal.protocol.conversations import ResponseHandler
 from diffusion.internal.protocol.exceptions import InvalidSessionFilterError
+from diffusion.internal.serialisers.base import Serialiser
+from diffusion.internal.serialisers.pydantic import MarshalledModel
 from diffusion.internal.services.abstract import ServiceValue
 from diffusion.internal.utils import validate_member_arguments
+if typing.TYPE_CHECKING:
+    from diffusion.internal.serialisers.generic_model import Model_Variants
+
+
+class ListTopicMetricCollectors(MarshalledModel):
+    entries: typing.List[TopicMetricCollector]
+
+    class Config(MarshalledModel.Config):
+        @classmethod
+        def decode(
+            cls,
+            item,
+            modelcls: typing.Type[Model_Variants],
+            model_key: str,
+            serialiser: Serialiser = None,
+        ):
+            serialiser = cls.check_serialiser(serialiser)
+            return cls.decode_complex(item, modelcls, model_key, serialiser)
+
+        @classmethod
+        def attr_mappings_all(cls, modelcls):
+            return {
+                "protocol24-topic-metric-collectors": {
+                    "protocol24-topic-metric-collectors": "entries"
+                }
+            }
 
 
 class Metrics(Component):
     """
     This feature allows a client to configure metric collectors.
 
     Diffusion servers provide metrics which are made available in several ways:-
@@ -87,16 +115,17 @@
         or topic metric collectors (`list_topic_metric_collectors`),
         a session needs the `VIEW_SERVER` global permission.
 
     # Accessing the feature
 
     This feature may be obtained from a `Session` as follows:
 
-    ```python
-    metrics: Metrics = session.metrics()
+    ```pycon
+    >>> metrics: Metrics = session.metrics
+
     ```
     """
     @validate_member_arguments
     async def put_session_metric_collector(self, collector: SessionMetricCollector) -> None:
         """
         Add a session metric collector, replacing any with the same name.
 
@@ -182,16 +211,18 @@
         Returns:
               a list of current topic metric collectors.
 
         Raises:
             ServerDisconnectedError: if the session is
                 disconnected.
         """
-        result = await self.services.LIST_TOPIC_METRIC_COLLECTORS.invoke(self.session)
-        return [TopicMetricCollector.from_tuple(x) for x in result[0]]
+        result = await self.services.LIST_TOPIC_METRIC_COLLECTORS.invoke(
+            self.session, response_type=ListTopicMetricCollectors
+        )
+        return result.entries
 
     @validate_member_arguments
     async def remove_topic_metric_collector(self, name: str) -> None:
         """
         Removes any topic metric collector with the given name, if it exists.
 
         Args:
```

## diffusion/features/control/metrics/topic_metrics.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2021, 2022 Push Technology Ltd., All Rights Reserved.
+#  Copyright (c) 2021-2023 Push Technology Ltd., All Rights Reserved.
 #
 #  Use is subject to license terms.
 #
 #  NOTICE: All information contained herein is, and remains the
 #  property of Push Technology. The intellectual and technical
 #  concepts contained herein are proprietary to Push Technology and
 #  may be covered by U.S. and Foreign Patents, patents in process, and
@@ -34,127 +34,124 @@
     (True if grouping by topic type)
     """
 
     group_by_path_prefix_parts: pydantic.NonNegativeInt = 0
     """
     The number of leading parts of the topic path to group by.
     """
+
     class Config(MetricCollector.Config):
-        alias = "topic-metric-collector"
+        frozen = True
+        alias = "protocol24-topic-metric-collector"
 
 
 class TopicMetricCollectorBuilder(BuilderBase[TopicMetricCollector]):
     """
     A topic metric collector builder.
 
     This creates instances of `TopicMetricCollector` that can be supplied to
     Metrics.put_topic_metric_collector.
     """
-    Self = typing.TypeVar('Self', bound=BuilderBase[TopicMetricCollector])
+
+    Self = typing.TypeVar("Self", bound=BuilderBase[TopicMetricCollector])
 
     @validate_member_arguments
-    def export_to_prometheus(
-            self: Self, export: bool
-    ) -> Self:
+    def group_by_topic_type(self: Self, group_by_topic_type: bool) -> Self:
         """
-        Specifies whether the metric collector should export metrics to
-        Prometheus or not.
+        Specifies whether the metric collector should group by topic
+        type.
 
-        The default is that metrics are not exported to Prometheus.
+        By default a topic metric collector does not group by topic type.
 
         Args:
-            export:
-                True to export metrics to Prometheus
+            group_by_topic_type:
+                True to indicate that the collector
+                should group by topic type
 
         Returns:
             this builder
         """
-        self._target.exports_to_prometheus = export
+        self._target = self._target.copy(
+            update=dict(groups_by_topic_type=group_by_topic_type)
+        )
         return self
 
     @validate_member_arguments
-    def group_by_topic_type(
-            self: Self, group_by_topic_type: bool
-    ) -> Self:
+    def group_by_path_prefix_parts(self: Self, parts: pydantic.NonNegativeInt) -> Self:
         """
-        Specifies whether the metric collector should group by topic
-        type.
+        Specifies the number of leading parts of the topic path the
+        metric collector should use to group results.
+        Since 6.8.
 
-        By default a topic metric collector does not group by topic type.
+        By default a topic metric collector does not group by the topic
+        path prefix. If a positive number of parts is specified, it
+        will enable grouping.
 
         Args:
-            group_by_topic_type:
-                True to indicate that the collector
-                should group by topic type
+            parts:
+                The number of leading parts of the topic path to group by.
+                Set to 0 to disable grouping by path.
 
         Returns:
             this builder
         """
-        self._target.groups_by_topic_type = group_by_topic_type
+        self._target = self._target.copy(update=dict(group_by_path_prefix_parts=parts))
         return self
 
     @validate_member_arguments
-    def maximum_groups(
-            self: Self, limit: pydantic.PositiveInt
-    ) -> Self:
+    def export_to_prometheus(self: Self, export: bool) -> Self:
         """
-        Specify the maximum number of groups maintained by the metric collector.
+        Specifies whether the metric collector should export metrics to
+        Prometheus or not.
 
-        By default, the number of groups is not limited.
+        The default is that metrics are not exported to Prometheus.
 
         Args:
-            limit:
-                The maximum number of groups maintained by the metric collector.
+            export:
+                True to export metrics to Prometheus
 
         Returns:
             this builder
         """
-        self._target.maximum_groups = limit
+        self._target = self._target.copy(update=dict(exports_to_prometheus=export))
         return self
 
     @validate_member_arguments
-    def group_by_path_prefix_parts(self: Self, parts: pydantic.NonNegativeInt) -> Self:
+    def maximum_groups(self: Self, limit: pydantic.PositiveInt) -> Self:
         """
-        Specifies the number of leading parts of the topic path the
-        metric collector should use to group results.
-        Since 6.8.
+        Specify the maximum number of groups maintained by the metric collector.
 
-        By default a topic metric collector does not group by the topic
-        path prefix. If a positive number of parts is specified, it
-        will enable grouping.
+        By default, the number of groups is not limited.
 
         Args:
-            parts:
-                The number of leading parts of the topic path to group by.
-                Set to 0 to disable grouping by path.
+            limit:
+                The maximum number of groups maintained by the metric collector.
 
         Returns:
             this builder
         """
-        self._target.group_by_path_prefix_parts = parts
+        self._target = self._target.copy(update=dict(maximum_groups=limit))
         return self
 
-    def reset(self) -> 'TopicMetricCollectorBuilder':
+    def reset(self) -> "TopicMetricCollectorBuilder":
         """
         Reset the builder.
 
         Returns:
             this Builder
         """
         return super().reset()
 
     @validate_member_arguments
     def _create_delegate(
         self, name: pydantic.StrictStr, topic_selector: pydantic.StrictStr
     ) -> TopicMetricCollector:
         return super()._create(name=name, topic_selector=topic_selector)
 
-    def create(
-            self, name: str, topic_selector: str
-    ) -> TopicMetricCollector:
+    def create(self, name: str, topic_selector: str) -> TopicMetricCollector:
         """
         Create a new `TopicMetricCollector` using the values
         currently known to this builder.
 
         Args:
             name:
                 the name of the TopicMetricCollector
```

## diffusion/features/control/session_trees/branch_mapping_table.py

```diff
@@ -86,16 +86,16 @@
             return BranchMappingTable(session_tree_branch, copy.deepcopy(self._mappings))
 
     @classmethod
     def from_fields(cls, *, branch_mappings, **kwargs):
         result = cls(branch_mappings=[BranchMapping(*x) for x in branch_mappings], **kwargs)
         return result
 
-    @classmethod
-    def attr_mappings(cls) -> typing.Dict[str, typing.Any]:
-        return {
-            "branch-mapping-table.path": cls.session_tree_branch,
-            "branch-mapping-table": cls.branch_mappings,
-        }
-
     class Config(MarshalledModel.Config):
-        alias = "branch-mapping-table"
+        @classmethod
+        def attr_mappings_all(cls, modelcls: typing.Type[BranchMappingTable]):
+            return {
+                "branch-mapping-table": {
+                    "branch-mapping-table.path": modelcls.session_tree_branch,
+                    "branch-mapping-table": modelcls.branch_mappings,
+                }
+            }
```

## diffusion/features/timeseries/__init__.py

```diff
@@ -1,22 +1,24 @@
-#  Copyright (c) 2022 Push Technology Ltd., All Rights Reserved.
+#  Copyright (c) 2022-2023 Push Technology Ltd., All Rights Reserved.
 #
 #  Use is subject to license terms.
 #
 #  NOTICE: All information contained herein is, and remains the
 #  property of Push Technology. The intellectual and technical
 #  concepts contained herein are proprietary to Push Technology and
 #  may be covered by U.S. and Foreign Patents, patents in process, and
 #  are protected by trade secret or copyright law.
 
 from __future__ import annotations
 
 import datetime
+import traceback
 import typing
 import typing_extensions
+from pydantic import StrictInt
 
 from diffusion.datatypes.timeseries import (
     EventMetadata,
     TimeSeriesEventDataType,
     TimeSeriesDataType,
 )
 from diffusion.datatypes.timeseries.types import (
@@ -31,15 +33,16 @@
     TimeSeriesAppendRequest,
     TimeSeriesTimestampAppendRequest,
     TimeSeriesEditRequest,
 )
 from diffusion.internal.utils import (
     validate_member_arguments,
 )
-from diffusion.features.timeseries.query.range_query import RangeQueryMode, RangeQuery
+if typing.TYPE_CHECKING:
+    from diffusion.features.timeseries.query.range_query import RangeQuery
 import diffusion.datatypes
 from diffusion.internal.validation import StrictNonNegativeInt
 
 
 @validate_member_arguments
 def get_val(
     value: TimeSeriesValueTypeOrRaw,
@@ -296,22 +299,24 @@
         value_final = get_val(value, value_type)
         request = TimeSeriesEditRequest(
             topic_path=topic_path,
             value_type=str(value_type),
             original_sequence=original_sequence,
             value=bytes(value_final),
         )
-        return await self.session.services.TIME_SERIES_EDIT.invoke(self.session, request)
+        return await self.session.services.TIME_SERIES_EDIT.invoke(
+            self.session, request, response_type=EventMetadata
+        )
 
     async def append(
         self,
         topic_path: str,
         value: TimeSeriesValueTypeOrRaw,
         value_type: typing.Type[TimeSeriesValueType],
-        timestamp: typing.Union[datetime.datetime, StrictNonNegativeInt] = None,
+        timestamp: typing.Union[datetime.datetime, StrictInt] = None,
     ) -> EventMetadata:
         """
         Update a time series topic by appending a new value.
 
         The server will add an event to the end of the time series based on the
         supplied value, with a new sequence number, timestamp, and the author set
         to the authenticated principal of the session.
@@ -323,39 +328,49 @@
                 This must match the value type of the
                 [DataType][diffusion.datatypes.foundation.datatype.DataType]
                 configured as the time series topic's
                 [TIME_SERIES_EVENT_VALUE_TYPE]
                 [diffusion.datatypes.timeseries.TopicSpecification.TIME_SERIES_EVENT_VALUE_TYPE]
                 event value type.
             timestamp: an optional timestamp. The timestamp must be greater or
-                equal to that of the most recent event appended to the topic
+                equal to that of the most recent event appended to the topic.
+                If specifying this as a `datetime.datetime` it should be timezone-aware,
+                otherwise UTC will be assumed.
         Returns:
             a result that completes when a response is received from the server.
         """
         value_final = get_val(value, value_type)
 
         request: TimeSeriesAppendRequest
         args = dict(
             path=topic_path,
             value_type=str(value_type),
             value=value_final,
         )
-        if timestamp:
+        if timestamp is not None:
             if isinstance(timestamp, datetime.datetime):
-                timestamp = int(timestamp.timestamp() * 1000)
+                if not timestamp.tzinfo:
+                    # Naive datetime, we can only assume UTC.
+                    # We may be able to type-annotate this in future:
+                    # https://github.com/pydantic/pydantic/discussions/3477
+                    LOG.warning(
+                        f"Timestamp {timestamp} without timezone provided, assuming UTC"
+                    )
+                timestamp = int(timestamp.astimezone(datetime.timezone.utc).timestamp() * 1000)
+
             service = self.session.services.TIME_SERIES_TIMESTAMP_APPEND
             request = TimeSeriesTimestampAppendRequest(
                 **args,
                 timestamp=timestamp,
             )
         else:
             request = TimeSeriesAppendRequest(**args)
             service = self.session.services.TIME_SERIES_APPEND
 
-        return await service.invoke(self.session, request)
+        return await service.invoke(self.session, request, response_type=EventMetadata)
 
     @classmethod
     def of(cls, val_type: typing.Type[VT]) -> typing.Type[TimeSeriesEventDataType[VT]]:
         """
         Provide a Time Series datatype with the given Event[VT] value type.
 
         Args:
@@ -384,8 +399,9 @@
 
         Args:
             tp: the type of the query
 
         Returns:
             The default range query for the given type.
         """
-        return RangeQuery.create_default(self.session, tp=tp)
+        from diffusion.features.timeseries.query.range_query import RangeQuery
+        return RangeQuery.create_default(self.session, tp=typing.cast(typing.Type[VT], tp))
```

## diffusion/features/timeseries/query/range_query.py

```diff
@@ -8,115 +8,51 @@
 #  may be covered by U.S. and Foreign Patents, patents in process, and
 #  are protected by trade secret or copyright law.
 
 from __future__ import annotations
 
 import functools
 
-import enum
-
 import stringcase
 import typing
-
+try:
+    from typing_extensions import TypeAlias
+except ImportError:
+    pass
 import attr
 import pydantic
 
-try:
-    from typing import TypeAlias  # type: ignore
-except ImportError:
-    from typing_extensions import TypeAlias
+from diffusion.internal.timeseries.query.range_query import RangeQueryMode, RangeQueryBase
 
 from diffusion.exceptions import InvalidOperationError
-from diffusion.features.timeseries.query.range_query_parameters import (
+from diffusion.internal.timeseries.query.range_query_parameters import (
     RangeQueryParameters,
     Range,
     QueryType,
 )
-from diffusion.features.timeseries.query.range_query_request import (
+from diffusion.internal.timeseries.query.range_query_request import (
     RangeQueryRequest,
 )
 from diffusion.internal.session import InternalSession
-from diffusion.datatypes.timeseries.types import VT
-from diffusion.internal.utils import validate_member_arguments, \
-    validate_member_arguments_configured
+from diffusion.datatypes.timeseries.types import VT, VT_other
+from diffusion.internal.utils import validate_member_arguments
 from diffusion.internal.validation import (
     StrictNonNegativeInt,
     StrictNonNegativeTimedelta,
     StrictTimedelta,
 )
 from diffusion.features.timeseries.query.query_result import QueryResult
 
-
-class RangeQueryMode(enum.IntEnum):
-    """
-    The range query mode.
-
-    Since:
-        6.9
-    """
-
-    VIEW_RANGE = 0x00
-    """
-    The range query is in view range mode.
-    """
-    EDIT_RANGE = 0x01
-    """
-    The range query is in edit range mode.
-    """
-
-    def type_name(self):
-        return "value" if self == RangeQueryMode.VIEW_RANGE else "edit"
-
-    def change_current_range(
-        self,
-        original: RangeQueryParameters,
-        range_selector: typing.Callable[[Range], Range],
-    ) -> RangeQueryParameters:
-        """
-        Changes the given
-        [RangeQueryParameters][diffusion.features.timeseries.query.range_query.RangeQueryParameters]
-        into this
-        [RangeQueryMode][diffusion.features.timeseries.query.range_query.RangeQueryMode]
-
-        Args:
-            original: The range query parameters to change the mode of.
-            range_selector: The range selector function.
-        Returns:
-
-            The new RangeQueryParameters
-        Raises:
-            ArgumentError: this mode is invalid for the RangeQuery.
-        """
-
-        if self == RangeQueryMode.VIEW_RANGE:
-            return original.with_view_range(range_selector(original.view_range))
-        elif self == RangeQueryMode.EDIT_RANGE:
-            return original.with_edit_range(range_selector(original.edit_range))
-        raise NotImplementedError()
-
-
-@attr.s(auto_attribs=True, eq=True, hash=True, slots=True, frozen=True)
-class RangeQueryBase(typing.Generic[VT]):
-    session: InternalSession
-    parameters: RangeQueryParameters
-    mode: RangeQueryMode
-    tp: typing.Type[VT]
-
-
 QuerySelf = typing.TypeVar("QuerySelf", bound="RangeQuery")
 """
 A [RangeQuery][diffusion.features.timeseries.query.range_query.RangeQuery]
 or instance of a subclass thereof (used when passing the same type back).
 """
 
 RangeQueryType: TypeAlias = "RangeQuery"
-"""
-A parameterizable [RangeQuery][diffusion.features.timeseries.query.range_query.RangeQuery]
-or instance of a subclass thereof (used when changing the value type).
-"""
 
 
 @attr.s(auto_attribs=True, eq=True, hash=True, slots=True, frozen=True)
 class RangeQuery(typing.Generic[VT], RangeQueryBase[VT]):
     """
     The builder for queries that select a range of events from a time series.
 
@@ -289,50 +225,59 @@
 
     See Also:
         [timeseries.TimeSeries][diffusion.features.timeseries.TimeSeries]
         [timeseries.RangeQuery][diffusion.features.timeseries.query.range_query.RangeQuery]
     """  # noqa: E501, W291
 
     @classmethod
-    @validate_member_arguments
     def create_default(
-        cls: typing.Type["RangeQueryType"],
+        cls,
         session: InternalSession,
         tp: typing.Type[VT],
-    ) -> "RangeQueryType[VT]":
+    ) -> RangeQuery[VT]:
         """
         Create the default Range Query for the given type
         Args:
             session: session from which this query will invoke select operations.
             tp: initial value type of query
 
         Returns:
             The according default Range Query object.
         """
-        return cls(
-            session,
-            RangeQueryParameters.DEFAULT_RANGE_QUERY(),
-            RangeQueryMode.VIEW_RANGE,
-            tp,
-        )
+
+        @validate_member_arguments
+        def checked_result(session: InternalSession, tp: typing.Type[VT]):
+            return typing.cast(
+                RangeQuery[VT],
+                cls(
+                    session,
+                    RangeQueryParameters.DEFAULT_RANGE_QUERY(),
+                    RangeQueryMode.VIEW_RANGE,
+                    tp
+                )
+            )
+
+        return checked_result(session, tp)
 
     @classmethod
     @functools.lru_cache(maxsize=None)
-    @validate_member_arguments
     def of(
-        cls: typing.Type["RangeQueryType"], item: typing.Type[VT]
-    ) -> typing.Type["RangeQueryType[VT]"]:
-        return typing.cast(
-            "typing.Type[RangeQueryType[VT]]",
-            type(
-                stringcase.pascalcase(f"{item}{cls.__name__}"),
-                (cls,),
-                dict(value_type=item),
-            ),
-        )
+        cls, item: typing.Type[VT]
+    ) -> typing.Type[RangeQuery[VT]]:
+        @validate_member_arguments
+        def raw_class(item: typing.Type[VT]) -> typing.Type[RangeQuery[VT]]:
+            return typing.cast(
+                "typing.Type[RangeQuery[VT]]",
+                type(
+                    stringcase.pascalcase(f"{item}{cls.__name__}"),
+                    (cls,),
+                    dict(value_type=item),
+                ),
+            )
+        return raw_class(item)
 
     def for_values(self: QuerySelf) -> QuerySelf:
         """
         Returns a copy of this
         [RangeQuery][diffusion.features.timeseries.query.range_query.RangeQuery]
         configured to perform a value range query with the view range set to
         the entire time series.
@@ -824,18 +769,15 @@
             count: The maximum number of events to return.
 
         Returns:
             The copy of this range query with a new limit.
         """   # noqa: E501, W291
         return attr.evolve(self, parameters=self.parameters.with_limit(count))
 
-    @validate_member_arguments_configured(
-        deferred=lambda: dict(RangeQuery=RangeQuery, RangeQueryType=RangeQueryType)
-    )
-    def as_(self: RangeQueryType, tp: typing.Type[VT]) -> "RangeQueryType[VT]":
+    def as_(self, tp: typing.Type[VT_other]) -> RangeQuery[VT_other]:
         """
         Returns a copy of this
         [RangeQuery][diffusion.features.timeseries.query.range_query.RangeQuery]
         with a different query value type.
 
         Notes:
             A query can only be evaluated successfully against time series topics with a compatible
@@ -853,15 +795,19 @@
 
         Args:
             tp: The new value type.
 
         Returns:
             The copy of this range query with a new query value type.
         """  # noqa: E501, W291
-        return typing.cast("RangeQueryType[VT]", attr.evolve(self, tp=tp))
+        @validate_member_arguments
+        def raw_class(tp: typing.Type[VT_other]) -> RangeQuery[VT_other]:
+            return typing.cast("RangeQuery[VT_other]", attr.evolve(self, tp=tp))
+
+        return raw_class(tp)
 
     def __str__(self):
         return f"range_query({repr(self.tp)}){self.parameters.__str__()}"
 
     @validate_member_arguments
     async def select_from(self, topic_path: pydantic.StrictStr) -> QueryResult[VT]:
         """
@@ -896,15 +842,15 @@
                 [RangeQuery.for_edits][diffusion.features.timeseries.query.range_query.RangeQuery.for_edits]
                 range query, or a
                 [RangeQuery.for_values][diffusion.features.timeseries.query.range_query.RangeQuery.for_values]
                 range query with an
                 [RangeQuery.edit_range][diffusion.features.timeseries.query.range_query.RangeQuery.edit_range].
             SessionClosedError: The calling session is closed.
         """  # noqa: E501, W291
-        from diffusion.features.timeseries.query.range_query_result import RangeQueryResult
+        from diffusion.internal.timeseries.query.range_query_result import RangeQueryResult
 
         request = RangeQueryRequest(topic_path=topic_path, parameters=self.parameters)
 
         result = await self.session.services.RANGE_QUERY.invoke(
             self.session, request, RangeQueryResult
         )
         return result.to_query_result(
```

## diffusion/features/timeseries/query/range_query_parameters.py

```diff
@@ -1,38 +1,17 @@
-#   Copyright (c) 2022 Push Technology Ltd., All Rights Reserved.
+#   Copyright (c) 2023 Push Technology Ltd., All Rights Reserved.
 #
 #   Use is subject to license terms.
 #
 #  NOTICE: All information contained herein is, and remains the
 #  property of Push Technology. The intellectual and technical
 #  concepts contained herein are proprietary to Push Technology and
 #  may be covered by U.S. and Foreign Patents, patents in process, and
 #  are protected by trade secret or copyright law.
-
-from __future__ import annotations
-
-import dataclasses
-import datetime
 import enum
-import functools
-import math
-import typing
-
-import attr
-
-from diffusion.exceptions import ArgumentNoneError, ArgumentOutOfRangeError
-from diffusion.internal.encoded_data import Int64
-from diffusion.internal.utils import validate_member_arguments
-from diffusion.internal.validation import (
-    StrictNonNegativeInt,
-    StrictNonNegativeTimedelta,
-    StrictTimedelta,
-)
-
-from diffusion.internal.serialisers.pydantic import MarshalledModel
 
 
 class StreamStructure(enum.IntEnum):
     """
     The structure of the event stream.
     """
 
@@ -41,847 +20,7 @@
     The stream contains edit events
     """
 
     VALUE_EVENT_STREAM = enum.auto()
     """
     The stream contains value events
     """
-
-
-@dataclasses.dataclass
-class Representation(object):
-    main: str
-    primary: str
-    stream_structure: StreamStructure
-
-    def __str__(self):
-        return f".{self.main}()"
-
-    @property
-    def primary_operator(self):
-        return f".{self.primary}()"
-
-
-class QueryType(enum.IntEnum):
-    """
-    The range query type.
-
-    Since:
-        6.1
-    """
-
-    @property
-    def __mapping__(self) -> typing.Mapping[QueryType, Representation]:
-        return {
-            QueryType.VALUES: Representation(
-                "edit_range", "for_values", StreamStructure.VALUE_EVENT_STREAM
-            ),
-            QueryType.ALL_EDITS: Representation(
-                "all_edits", "for_edits", StreamStructure.EDIT_EVENT_STREAM
-            ),
-            QueryType.LATEST_EDITS: Representation(
-                "latest_edits", "for_edits", StreamStructure.EDIT_EVENT_STREAM
-            ),
-        }
-
-    def __str__(self):
-        return str(self.__mapping__.get(self))
-
-    VALUES = 0x00
-    """
-    Original events in view range merged with latest edits in edit range.
-    """
-
-    ALL_EDITS = 0x01
-    """
-    Original events in view range plus all edits in edit range.
-    """
-    LATEST_EDITS = 0x02
-    """
-    Original events in view range plus latest event in edit range.
-    """
-
-    @property
-    def primary_operator(self) -> str:
-        """
-        Returns the primary operator of a given <see cref="QueryType"/>.
-        """
-        return self.__mapping__[self].primary_operator
-
-    @property
-    def edit_range_operator(self) -> str:
-        """
-        Returns:
-            The edit range operator of the given <paramref name="type"/>.</returns>
-        """
-        return str(self)
-
-    @property
-    def stream_structure(self) -> StreamStructure:
-        """
-        Returns the stream structure of a given <see cref="QueryType"/>.
-
-        Returns:
-            The stream structure of the given `type`
-        """
-        return self.__mapping__[self].stream_structure
-
-
-class SpanPair(typing.NamedTuple):
-    anchor: typing.Optional[str]
-    span: str
-
-
-class PointType(enum.IntEnum):
-    """
-    The point type.
-
-    Since:
-        6.9
-    """
-
-    ABSOLUTE_START = 0x00
-    """
-    The value is ignored.
-    """
-
-    ABSOLUTE_SEQUENCE = 0x01
-    """
-    The value is a absolute sequence number.
-    """
-
-    ABSOLUTE_TIME = 0x02
-    """
-    The value is a <see cref="DateTimeOffset"/>.
-    """
-
-    OFFSET_SEQUENCE = 0x03
-    """
-    The value is the number of terminal events of the series to skip.
-    """
-
-    OFFSET_TIME = 0x04
-    """
-    The value is the terminal duration in milliseconds of the series to skip.
-    """
-
-    NEXT_COUNT = 0x05
-    """
-    The value is a relative number of events after another point.
-    """
-
-    NEXT_TIME = 0x06
-    """
-    The value is a duration in milliseconds after another point.
-    """
-
-    PREVIOUS_COUNT = 0x07
-    """
-    The value is a relative number of events before another point.
-    """
-
-    PREVIOUS_TIME = 0x08
-    """
-    The value is a duration in milliseconds before another point.
-    """
-
-    @property
-    def __mapping__(self) -> typing.Dict[PointType, SpanPair]:
-        return {
-            PointType.ABSOLUTE_START: SpanPair("from_start", "to_start"),
-            PointType.ABSOLUTE_SEQUENCE: SpanPair("from", "to"),
-            PointType.ABSOLUTE_TIME: SpanPair("from", "to"),
-            PointType.OFFSET_SEQUENCE: SpanPair("from_last", "until_last"),
-            PointType.OFFSET_TIME: SpanPair("from_last", "until_last"),
-            PointType.NEXT_COUNT: SpanPair(None, "next"),
-            PointType.NEXT_TIME: SpanPair(None, "next"),
-            PointType.PREVIOUS_COUNT: SpanPair(None, "previous"),
-            PointType.PREVIOUS_TIME: SpanPair(None, "previous"),
-        }
-
-    @property
-    def anchor_operator(self) -> typing.Optional[str]:
-        """
-        Returns the anchor operator for a given <see cref="PointType"/>.
-
-        Returns:
-            The anchor operator for the given <paramref name="type"/>.
-        """
-        try:
-            return self.__mapping__[self].anchor
-        except KeyError:
-            raise ValueError(f"No anchor operator for {type}.")
-
-    @property
-    def span_operator(self) -> str:
-        """
-        Returns the span operator for this `PointType`
-
-        Returns:
-            The span operator.
-        """
-        try:
-            return self.__mapping__[self].span
-        except KeyError:
-            raise ValueError(f"No anchor operator for {type}.")
-
-    def format_unit(self, value: int) -> str:
-        """
-        Returns the unit suffix for a given <see cref="PointType"/>.
-
-        Returns:
-            The unit suffix.
-        """
-        if self in {
-            PointType.ABSOLUTE_TIME,
-            PointType.OFFSET_TIME,
-            PointType.NEXT_TIME,
-            PointType.PREVIOUS_TIME,
-        }:
-            return f"datetime.timedelta(milliseconds={value})"
-        return f"{value}"
-
-    def validate(self, value: StrictNonNegativeInt) -> bool:
-        """
-        Validates a given <paramref name="value"/> based on the rules
-        of this PointType.
-
-        Args:
-            value: The value to validate.
-
-        Returns:
-            `True` if the value is valid for this type
-            Otherwise `False`.
-        """
-        return (
-            self in {PointType.ABSOLUTE_START, PointType.ABSOLUTE_TIME}
-            or value >= 0
-        )
-
-
-PointSelf = typing.TypeVar("PointSelf", bound="Point")
-
-
-class Point(typing.NamedTuple):
-    """
-    The query point for a range.
-
-    Since:
-        6.9
-    """
-
-    @classmethod
-    @functools.lru_cache(maxsize=None)
-    def at_start(cls):
-        """
-        Returns a point representing an absolute sequence.
-        """
-        return Point(0, PointType.ABSOLUTE_START)
-
-    @classmethod
-    @validate_member_arguments
-    def at(
-        cls: typing.Type[PointSelf],
-        time: typing.Union[StrictNonNegativeInt, StrictTimedelta],
-    ) -> PointSelf:
-        """
-        Returns a point representing an absolute time or sequence number.
-
-        Args:
-            time: The absolute time (as a `datetime.timedelta`)
-                or the sequence offset (as a non-negative `int`)
-
-        Returns:
-            The point representing an absolute time.
-        """
-        if isinstance(time, datetime.timedelta):
-            return cls(
-                int(math.ceil(time.total_seconds() * 1000)),
-                PointType.ABSOLUTE_TIME,
-            )
-        return cls(time, PointType.ABSOLUTE_SEQUENCE)
-
-    @classmethod
-    @validate_member_arguments
-    def offset(
-        cls: typing.Type[PointSelf],
-        offset: typing.Union[StrictNonNegativeInt, StrictNonNegativeTimedelta],
-    ) -> PointSelf:
-        """
-        Returns a point representing a sequence offset from the end of the time series.
-        Args:
-            offset: The sequence offset (as a non-negative `int`)
-                or the time span (as a `datetime.timedelta`)
-
-        Returns:
-            The point representing the offset from the end of the time series.
-        """
-
-        if isinstance(offset, datetime.timedelta):
-            return cls.offset_milliseconds(
-                int(math.ceil(offset.total_seconds() * 1000))
-            )
-        return cls(offset, PointType.OFFSET_SEQUENCE)
-
-    @classmethod
-    @validate_member_arguments
-    def offset_milliseconds(
-        cls: typing.Type[PointSelf], milliseconds: StrictNonNegativeInt
-    ) -> PointSelf:
-        """
-        Returns a point representing a duration from the end of the time series.
-        Args:
-            milliseconds: The time span in milliseconds.
-
-        Returns:
-            The point representing a duration from the end of the time series.
-        """
-        return cls(milliseconds, PointType.OFFSET_TIME)
-
-    @classmethod
-    @validate_member_arguments
-    def next(
-        cls: typing.Type[PointSelf],
-        offset: typing.Union[StrictNonNegativeInt, StrictNonNegativeTimedelta],
-    ) -> PointSelf:
-        """
-        Returns a relative point at <paramref name="count"/> events after the anchor.
-
-        Args:
-            offset: either the time span of events following the anchor to select (as a
-                [StrictNonNegativeTimedelta][diffusion.internal.validation.StrictNonNegativeTimedelta])
-                or the end of the range of events to select following the anchor (as a
-                [StrictNonNegativeInt][diffusion.internal.validation.StrictNonNegativeInt])
-
-        Returns:
-            The relative point at `offset` events or `offset` after the anchor.
-        """
-        if isinstance(offset, datetime.timedelta):
-            return cls.next_milliseconds(
-                int(math.ceil(offset.total_seconds() * 1000))
-            )
-        return cls(offset, PointType.NEXT_COUNT)
-
-    @classmethod
-    @validate_member_arguments
-    def next_milliseconds(
-        cls: typing.Type[PointSelf], milliseconds: StrictNonNegativeInt
-    ) -> PointSelf:
-        """
-        Returns a relative point at <paramref name="milliseconds"/> after the anchor.
-
-        Args:
-            milliseconds: The time span in milliseconds.
-        Returns:
-            The relative point at <paramref name="milliseconds"/> after the anchor.
-        """
-        return cls(milliseconds, PointType.NEXT_TIME)
-
-    @classmethod
-    @validate_member_arguments
-    def previous(
-        cls: typing.Type[PointSelf],
-        offset: typing.Union[StrictNonNegativeInt, StrictNonNegativeTimedelta],
-    ) -> PointSelf:
-        """
-        Returns a relative point at <paramref name="count"/> events before the anchor.
-
-        Args:
-            offset:
-                - The end of the range of events to select preceding the anchor (as a
-                [StrictNonNegativeInt][diffusion.internal.validation.StrictNonNegativeInt]) or
-                - The time span of events preceding the anchor to select (as a
-                [StrictNonNegativeTimedelta][diffusion.internal.validation.StrictNonNegativeTimedelta])
-        Returns:
-            The relative point at <paramref name="count"/> events before the anchor.
-        """
-        if isinstance(offset, datetime.timedelta):
-            return cls.previous_milliseconds(
-                int(math.ceil(offset.total_seconds() * 1000))
-            )
-
-        return cls(offset, PointType.PREVIOUS_COUNT)
-
-    @classmethod
-    @validate_member_arguments
-    def previous_milliseconds(
-        cls: typing.Type[PointSelf], milliseconds: StrictNonNegativeInt
-    ) -> PointSelf:
-        """
-        Returns the relative point at <paramref name="milliseconds"/> before the anchor.
-
-        Args:
-            milliseconds: The time span in milliseconds.
-        Returns:
-            The relative point at <paramref name="milliseconds"/> before the anchor.
-        """
-        return cls(milliseconds, PointType.PREVIOUS_TIME)
-
-    value: StrictNonNegativeInt
-    """
-    The value.
-    """
-
-    tp: PointType
-    """
-    The point type.
-    """
-
-    @property
-    def is_absolute(self) -> bool:
-        """
-        Gets whether the current point is absolute or not.
-        Returns:
-            Whether the current point is absolute.
-        """
-        return self.tp.anchor_operator is not None
-
-    def operator_description(self, op: typing.Optional[str] = "") -> str:
-        sb = ""
-        sb += f".{op}("
-
-        if self.tp != PointType.ABSOLUTE_START:
-            quantity = self.tp.format_unit(value=self.value)
-            sb += quantity
-
-        sb += ")"
-        return sb
-
-    def anchor_description(self) -> str:
-        """
-        Returns:
-             the anchor description for the current <see cref="Point"/>.
-        """
-        return self.operator_description(self.tp.anchor_operator)
-
-    def span_description(self) -> str:
-        """
-        Returns the span description for the current <see cref="Point"/>.
-        Returns:
-            The span description.
-        """
-        return self.operator_description(self.tp.span_operator)
-
-    def __str__(self):
-        return f"{self.tp} {self.value}"
-
-
-RangeSelf = typing.TypeVar("RangeSelf", bound="Range")
-
-
-@attr.s(auto_attribs=True, eq=True, hash=True, frozen=True, slots=True)
-class Range(object):
-    """
-    The query range.
-
-    Since:
-        6.9
-    """
-
-    # noinspection PyPep8Naming
-    @classmethod
-    @functools.lru_cache(maxsize=None)
-    def DEFAULT_RANGE(cls: typing.Type[RangeSelf]) -> RangeSelf:
-        """
-        The default range with Point.at_start() as
-        anchor and Point.offset(0) as span.
-        """
-        return cls()
-
-    def __copy__(self):
-        return self
-
-    def __deepcopy__(self, memodict=None):
-        return self.__copy__()
-
-    anchor: Point = Point.at_start()
-    """
-    The anchor point.
-    """
-
-    span: Point = Point.offset(0)
-    """
-    The span point.
-    """
-
-    @classmethod
-    @validate_member_arguments
-    def create(
-        cls: typing.Type[RangeSelf], anchor: Point, span: Point
-    ) -> RangeSelf:
-        """
-        Creates a new
-        [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-        instance.
-
-        Args:
-            anchor: The anchor point.
-            span: The span point.
-
-        Returns:
-            New range
-        """
-
-        if not anchor.is_absolute:
-            raise ValueError("Anchor point is not absolute.")
-        return cls(anchor=anchor, span=span)
-
-    def __attrs_post_init__(self):
-        """
-        Initialises a new
-        [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-        instance.
-        """
-
-        if self.anchor is None:
-            raise ArgumentNoneError(f"Anchor is {self.anchor}")
-
-        if not self.anchor.is_absolute:
-            raise ArgumentOutOfRangeError("Anchor point is not absolute.")
-
-        if not self.span:
-            raise ArgumentNoneError(f"Span is {self.span}")
-
-    def from_start(self) -> Range:
-        """
-        Copies the current
-        [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-        with a new anchor point.
-
-        Returns:
-            The copy of the current
-                [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-                with a new anchor point.
-        """
-        return attr.evolve(self, anchor=Point.at_start())
-
-    @validate_member_arguments
-    def from_(
-        self: RangeSelf,
-        time: typing.Union[StrictNonNegativeInt, StrictTimedelta],
-    ) -> RangeSelf:
-        """
-        Copies the current
-        [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-        with a new anchor point.
-
-        Args:
-            time: The sequence number (as a non-negative `int`) or
-                the absolute time (as a `datetime.timedelta`)
-
-        Returns:
-            The copy of the current
-                [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-                with a new anchor point.
-        """
-        return attr.evolve(self, anchor=Point.at(time))
-
-    @validate_member_arguments
-    def from_last(
-        self: RangeSelf,
-        offset: typing.Union[StrictNonNegativeInt, StrictNonNegativeTimedelta],
-    ) -> RangeSelf:
-        """
-        Copies the current
-        [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-        with a new anchor point.
-        Args:
-            offset: The offset (as a
-                [StrictNonNegativeInt][diffusion.internal.validation.StrictNonNegativeInt]) or
-                a time (as a
-                [StrictNonNegativeTimedelta][diffusion.internal.validation.StrictNonNegativeTimedelta])
-
-        Returns:
-            The copy of the current
-                [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-                with a new anchor point.
-        """
-        return attr.evolve(self, anchor=Point.offset(offset))
-
-    @validate_member_arguments
-    def from_last_milliseconds(
-        self: RangeSelf, milliseconds: StrictNonNegativeInt
-    ) -> RangeSelf:
-        """
-        Copies the current
-        [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-        with a new anchor point.
-
-        Args:
-            milliseconds: The time offset in milliseconds.
-
-        Returns:
-            The copy of the current
-                [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-                with a new anchor point.
-        """
-        return attr.evolve(self, anchor=Point.offset_milliseconds(milliseconds))
-
-    def to_start(self) -> Range:
-        """
-        Copies the current
-        [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-        with a new span point.
-
-        Returns:
-            The copy of the current
-                [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-                with a new span point.
-        """
-        return attr.evolve(self, span=Point.at_start())
-
-    @validate_member_arguments
-    def to(
-        self: RangeSelf,
-        time: typing.Union[StrictNonNegativeInt, StrictTimedelta],
-    ) -> RangeSelf:
-        """
-        Create a copy of the current
-        [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-        with a new span point.
-
-        Args:
-            time: The absolute time (as a `datetime.timedelta`) or
-                the sequence offset (as a non-negative `int`)
-
-        Returns:
-            The copy of the current
-                [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-                with a new span point.
-        """
-        return attr.evolve(self, span=Point.at(time))
-
-    @validate_member_arguments
-    def until_last(
-        self: RangeSelf,
-        offset: typing.Union[StrictNonNegativeInt, StrictNonNegativeTimedelta],
-    ) -> RangeSelf:
-        """
-        Copies the current
-        [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-        with a new span point.
-
-        Args:
-            offset: The offset from the end of the time series as:
-                - time span (as a `datetime.timedelta`) or
-                 - sequence count (as a non-negative `int`)
-
-        Returns:
-            The copy of the current
-                [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-                with a new span point.
-        """
-        return attr.evolve(self, span=Point.offset(offset))
-
-    @validate_member_arguments
-    def until_last_milliseconds(
-        self: RangeSelf, milliseconds: StrictNonNegativeInt
-    ) -> RangeSelf:
-        """
-        Copies the current
-        [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-        with a new span point.
-
-        Args:
-            milliseconds: The time span offset in milliseconds.
-
-        Returns:
-            The copy of the current
-                [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-                with a new span point.
-        """
-        return attr.evolve(self, span=Point.offset_milliseconds(milliseconds))
-
-    @validate_member_arguments
-    def next(
-        self: RangeSelf,
-        offset: typing.Union[StrictNonNegativeInt, StrictNonNegativeTimedelta],
-    ) -> "Range":
-        """
-        Copies the current
-        [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-        with a new span point.
-
-        Args:
-            offset: either the time span of events following the anchor to select (as a
-                [StrictNonNegativeTimedelta][diffusion.internal.validation.StrictNonNegativeTimedelta])
-                or the end of the range of events to select following the anchor (as a
-                [StrictNonNegativeInt][diffusion.internal.validation.StrictNonNegativeInt])
-        Returns:
-            The copy of the current
-                [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-                with a new span point.
-        """  # noqa: E501, W291
-        return attr.evolve(self, span=Point.next(offset))
-
-    @validate_member_arguments
-    def next_milliseconds(
-        self: RangeSelf, milliseconds: StrictNonNegativeInt
-    ) -> RangeSelf:
-        """
-        Copies the current
-        [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-        with a new span point.
-        Args:
-            milliseconds: The next time span in milliseconds.
-
-        Returns:
-            The copy of the current
-                [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-                with a new span point.
-        """
-        return attr.evolve(self, span=Point.next_milliseconds(milliseconds))
-
-    @validate_member_arguments
-    def previous(
-        self: RangeSelf,
-        offset: typing.Union[StrictNonNegativeInt, StrictNonNegativeTimedelta],
-    ) -> RangeSelf:
-        """
-        Copies the current
-        [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-        with a new span point.
-
-        Args:
-            offset:
-                - The end of the range of events to select preceding the anchor (as a
-                [StrictNonNegativeInt][diffusion.internal.validation.StrictNonNegativeInt]) or
-                - The time span of events preceding the anchor to select (as a
-                [StrictNonNegativeTimedelta][diffusion.internal.validation.StrictNonNegativeTimedelta])
-        Returns:
-            The copy of the current
-                [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-                with a new span point.
-        """
-        return attr.evolve(self, span=Point.previous(offset))
-
-    @validate_member_arguments
-    def previous_milliseconds(
-        self: RangeSelf, milliseconds: StrictNonNegativeInt
-    ) -> RangeSelf:
-        """
-        Copies the current
-        [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-        with a new span point.
-
-        Args:
-            milliseconds: The previous time span in milliseconds.
-
-        Returns:
-            The copy of the current
-                [Range][diffusion.features.timeseries.query.range_query_parameters.Range]
-                with a new span point.
-        """
-
-        return attr.evolve(self, span=Point.previous_milliseconds(milliseconds))
-
-    def __str__(self):
-        sb = ""
-
-        if self.anchor != self.DEFAULT_RANGE().anchor:
-            sb += self.anchor.anchor_description()
-
-        if self.span != self.DEFAULT_RANGE().span:
-            sb += self.span.span_description()
-
-        return sb
-
-
-RQPSelf = typing.TypeVar("RQPSelf", bound="RangeQueryParameters")
-
-
-class RangeQueryParameters(MarshalledModel):
-    """
-    The range query parameters.
-
-    Since:
-        6.9
-    """
-    class Config(MarshalledModel.Config):
-        alias = "range-query-parameters"
-        frozen = True
-
-    # noinspection PyPep8Naming
-    @classmethod
-    @functools.lru_cache(maxsize=None)
-    def DEFAULT_RANGE_QUERY(cls) -> RangeQueryParameters:
-        return cls()
-
-    query_type: QueryType = QueryType.VALUES
-    """ The query type """
-
-    view_range: Range = Range.DEFAULT_RANGE()
-    """ The view range """
-
-    edit_range: Range = Range.DEFAULT_RANGE()
-    """ The edit range """
-
-    limit: StrictNonNegativeInt = Int64.max_signed_int()
-
-    @property
-    def is_historic_query(self):
-        """
-        Gets whether the current query parameters are a historic query or not.
-        """
-        return (
-            self.query_type != QueryType.VALUES
-            or self.edit_range != Range.DEFAULT_RANGE()
-        )
-
-    @validate_member_arguments
-    def with_view_range(self: RQPSelf, range: Range) -> RQPSelf:
-        """
-        Creates a copy of the current <see cref="RangeQueryParameters"/>
-        with a new view range.
-
-        Args:
-            range: The new view range.
-
-        Returns:
-            The copy of the current
-                [RangeQueryParameters][diffusion.features.timeseries.query.range_query_parameters.RangeQueryParameters]
-                with a new view `range`.
-        """  # noqa: E501, W291
-        return self.copy(update=dict(view_range=range))
-
-    @validate_member_arguments
-    def with_edit_range(self: RQPSelf, range: Range) -> RQPSelf:
-        return self.copy(update=dict(edit_range=range))
-
-    @validate_member_arguments
-    def with_limit(self: RQPSelf, count: StrictNonNegativeInt) -> RQPSelf:
-        return self.copy(update=dict(limit=count))
-
-    @validate_member_arguments
-    def with_query_type(self: RQPSelf, type: QueryType) -> RQPSelf:
-        """
-        Creates a copy of the current <see cref="RangeQueryParameters"/>
-        with a new query type.
-
-        Args:
-            type: The new query type.
-
-        Returns:
-            The copy of the current
-                [RangeQueryParameters][diffusion.features.timeseries.query.range_query_parameters.RangeQueryParameters]
-                with a new `type`.
-        """  # noqa: E501, W291
-        return self.copy(update=dict(query_type=type))
-
-    def __str__(self):
-        sb = ""
-
-        if self.query_type != QueryType.VALUES:
-            sb += self.query_type.primary_operator
-
-        if self.view_range != self.DEFAULT_RANGE_QUERY().view_range:
-            sb += str(self.view_range)
-
-        if self.edit_range != self.DEFAULT_RANGE_QUERY().edit_range:
-            sb += f"{self.query_type.edit_range_operator}{self.edit_range}"
-        elif self.query_type == QueryType.LATEST_EDITS:
-            sb += QueryType.LATEST_EDITS.edit_range_operator
-
-        if self.limit != self.DEFAULT_RANGE_QUERY().limit:
-            sb += f".limit({self.limit})"
-
-        return sb
```

## diffusion/features/topics/__init__.py

```diff
@@ -9,15 +9,15 @@
 import attr
 import structlog
 
 import diffusion.datatypes as dt
 from diffusion.handlers import HandlerSet
 from diffusion.internal.components import Component
 from diffusion.features.topics.selectors import get_selector
-from diffusion.internal.topics import Topic, spec_conv
+from diffusion.internal.topics import spec_conv, Topic
 from diffusion.internal.topics.constraints import UpdateConstraintType
 from diffusion.features.topics.details.topic_specification import TopicSpecification
 from diffusion.internal.serialisers.attrs import MarshalledModel
 from diffusion.internal.utils import decode
 
 if TYPE_CHECKING:  # pragma: no cover
     from diffusion.session import Session
@@ -112,47 +112,50 @@
     def topic_type(self):
         return self.specification.topic_type.type_code
 
     @property
     def properties(self):
         return self.specification.properties_as_json()
 
-    @classmethod
-    def attr_mappings(cls) -> typing.Dict[str, typing.Any]:
-        return {
-            "protocol14-topic-specification.protocol14-topic-type": "topic_type",
-            "protocol14-topic-specification.topic-properties": "properties",
-        }
+    class Config(MarshalledModel.Config):
+        @classmethod
+        def attr_mappings_all(cls, modelcls):
+            return {
+                cls.alias: {
+                    "protocol14-topic-specification.protocol14-topic-type": "topic_type",
+                    "protocol14-topic-specification.topic-properties": "properties",
+                }
+            }
 
 
 @attr.s(auto_attribs=True, slots=True)
 class TopicBaseNum(MarshalledModel):
     topic_path: str = attr.ib(metadata={"alias": "topic-path"})
 
     specification: DataTypeArgument = attr.ib(
         converter=dt_get,
         metadata={"alias": "protocol14-topic-type"},
     )
 
 
 @attr.s(auto_attribs=True, slots=True)
 class AddTopic(TopicBase):
-    class Config(MarshalledModel.Config):
+    class Config(TopicBase.Config):
         alias = "protocol14-topic-add-request"
 
 
 def unconstrained() -> Unconstrained:
     from diffusion.features.topics.update.constraints import Unconstrained
 
     return Unconstrained.Instance
 
 
 @attr.s(auto_attribs=True, slots=True)
 class SetTopic(TopicBaseNum):
-    class Config(MarshalledModel.Config):
+    class Config(TopicBaseNum.Config):
         alias = "set-topic-request"
 
     value: typing.Union[bytes, AbstractDataType] = attr.ib(metadata={"alias": "bytes"})
 
     def __attrs_post_init__(self):
         if not isinstance(self.value, bytes):
             self.value = get_val(self.value, dt.get(self.specification)).to_bytes()
@@ -162,15 +165,15 @@
         converter=convert_constraints,
         metadata={"alias": "set-topic-request.update-constraint"},
     )
 
 
 @attr.s(auto_attribs=True, slots=True)
 class AddAndSetTopic(TopicBase):
-    class Config(MarshalledModel.Config):
+    class Config(TopicBase.Config):
         alias = "add-and-set-topic-request"
 
     value: typing.Union[bytes, AbstractDataType] = attr.ib(metadata={"alias": "bytes"})
 
     def __attrs_post_init__(self):
         if not isinstance(self.value, bytes):
             self.value = get_val(self.value, dt.get(self.specification)).to_bytes()
```

## diffusion/features/topics/streams.py

```diff
@@ -62,15 +62,15 @@
         super().__init__(public_type)
 
     async def handle(self, event: str, **kwargs) -> typing.Any:
         converted_kwargs = {**kwargs}
         for k in {"topic_value", "old_value"} & kwargs.keys():
             try:
                 converted = self.converter(kwargs[k])
-                LOG.error(f"Converted {k}:{kwargs[k]}->{self.converter}->{converted}")
+                LOG.debug(f"Converted {k}:{kwargs[k]}->{self.converter}->{converted}")
                 converted_kwargs.update({k: converted})
             except Exception as e:
                 LOG.error(e)
                 raise
         try:
             return await self.delegate.handle(event, **converted_kwargs)
         except Exception as e:
```

## diffusion/features/topics/details/topic_specification.py

```diff
@@ -661,16 +661,19 @@
     instead of double quotes and special characters can be escaped.
     The purpose of this property is to allow a client to create topics on
     behalf of other users. This can be used in conjunction with the
     [REMOVAL][diffusion.features.topics.details.topic_specification.TopicSpecification.REMOVAL]
     property so that such topics are removed when there are
     no longer any sessions for the named principal.
     For example:
-    ```
-    specification.with_properties(OWNER="$Principal is 'myPrincipal'"), REMOVAL="when no session has '$Principal is \"myPrincipal\"' for 5s")
+
+    ```pycon
+    >>> import diffusion.datatypes
+    >>> specification = diffusion.datatypes.JSON
+    >>> specification.with_properties(OWNER="$Principal is 'myPrincipal'", REMOVAL="when no session has '$Principal is \"myPrincipal\"' for 5s")
     ```
 
     Since 6.8.3
     """  # NOQA: E501
     COMPRESSION: typing.Optional[typing.Union[CompressionPolicy, bool]] = None
     """
     Key of the topic property that allows the compression policy to be set
```

## diffusion/features/topics/update/__init__.py

```diff
@@ -1,15 +1,20 @@
 from __future__ import annotations
 
 import abc
 import functools
 import typing
-from inspect import isclass
+
+from diffusion.internal.serialisers.base import ChoiceProvider, ChoiceEncoder
 from diffusion.internal.serialisers.generic_model import GenericConfig, GenericModel, \
     GenericModel_T
+from diffusion.internal.topics.constraints import UpdateConstraintType
+
+if typing.TYPE_CHECKING:
+    from diffusion.internal.serialisers import Serialiser
 
 
 class TopicCreationResult:
     CREATED = 0
     EXISTS = 1
 
 
@@ -37,16 +42,14 @@
         Constraints can only be composed if the resulting constraint is satisfiable. Multiple session locks can be held
         but a topic can only have a single value. Constraints specifying multiple topic values can't be constructed.
 
         Constraints can be created using a [ConstraintFactory][diffusion.features.topics.update.constraint_factory.ConstraintFactory].
 
     """  # NOQA
 
-    ID: typing.ClassVar[int]
-
     @property
     def values(self):
         return self.Config.as_tuple(self)[1:]
 
     @classmethod
     def __get_validators__(cls):
         def validator(instance):
@@ -85,47 +88,39 @@
 
     IsTopicConstraint: typing.ClassVar[bool] = False
 
     def get_topic_constraints(self):
         return filter(lambda x: x.IsTopicConstraint is True, self)
 
     def to_bytes(self):
-        return self.Config.to_bytes(self, "update-constraint")
+        return self.Config.to_bytes(self, self.Config.serialiser("update-constraint"))
 
-    class Config(typing.Generic[GenericModel_T], GenericConfig[GenericModel_T]):
-        @classmethod
-        @functools.lru_cache(maxsize=None)
-        def field_names(
-            cls, modelcls: typing.Type[GenericModel_T], serialiser=None
-        ) -> typing.List[str]:
-            raise NotImplementedError()
+    class Config(typing.Generic[GenericModel_T], GenericConfig[GenericModel_T],
+                 ChoiceProvider[UpdateConstraintType]):
+        alias = "update-constraint"
 
         @classmethod
-        def attr_mappings_all(cls, modelcls):
-            return {"update-constraint": cls}
+        def attr_mappings_all(cls, modelcls: typing.Type[GenericModel_T]):
+            return {
+                "update-constraint": {
+                    cls.serialiser("update-constraint")
+                    .to_encoder(ChoiceEncoder)
+                    .get_serialiser_by_provider(
+                        typing.cast(UpdateConstraint.Config, modelcls.Config)
+                    ): modelcls
+                }
+            }
 
         @classmethod
         def as_tuple(
-            cls, item: GenericModel_T, serialiser=None
+            cls, item: GenericModel_T, serialiser: Serialiser = None
         ) -> typing.Tuple[typing.Any, ...]:
 
-            serialiser = cls.get_serialiser(item, serialiser)
-            return (typing.cast(UpdateConstraint, item).ID,) + super().as_tuple(
+            return (typing.cast(UpdateConstraint, item).Config.id(),) + super().as_tuple(
                 item, serialiser
             )
 
         @classmethod
-        def to_bytes(cls, item: GenericModel_T, serialiser=None) -> bytes:
-            as_tuple = cls.as_tuple(item, serialiser=serialiser)
-            return cls.serialiser(serialiser).to_bytes(as_tuple)
-
-        @classmethod
-        def get_serialiser(cls, item: GenericModel_T, serialiser: str = None):
-            from diffusion.internal.serialisers.base import ChoiceEncoder
-
-            serialiser = serialiser or "update-constraint"
-            choice_encoder = cls.serialiser(serialiser).spec[serialiser]
-            assert isclass(choice_encoder) and issubclass(choice_encoder, ChoiceEncoder)
-            serialiser = choice_encoder.serialiser_names.get(
-                typing.cast(UpdateConstraint, item).ID
-            )
-            return serialiser
+        def to_bytes(cls, item: GenericModel_T, serialiser: Serialiser = None) -> bytes:
+            serialiser = cls.check_serialiser(serialiser)
+            as_tuple = serialiser.to_encoder(ChoiceEncoder).as_tuple(item)
+            return serialiser.to_bytes(as_tuple)
```

## diffusion/features/topics/update/constraints.py

```diff
@@ -1,8 +1,8 @@
-#   Copyright (c) 2022 Push Technology Ltd., All Rights Reserved.
+#   Copyright (c) 2022-2023 Push Technology Ltd., All Rights Reserved.
 #
 #   Use is subject to license terms.
 #
 #  NOTICE: All information contained herein is, and remains the
 #  property of Push Technology. The intellectual and technical
 #  concepts contained herein are proprietary to Push Technology and
 #  may be covered by U.S. and Foreign Patents, patents in process, and
@@ -13,30 +13,32 @@
 import collections
 import collections.abc
 import functools
 import itertools
 import typing
 
 import pydantic.dataclasses
-from typing_extensions import overload
+from typing_extensions import overload, Literal
 
 from diffusion.datatypes import AbstractDataType
 from diffusion.features.topics.update import UpdateConstraint, UpdateConstraint_T
-from diffusion.internal.serialisers.dataclass_model import DataclassConfigMixin
 from diffusion.internal.serialisers.generic_model import (
     GenericConfig
 )
 from diffusion.internal.services import ServiceValue
+from diffusion.internal.topics.constraints import UpdateConstraintType
 from diffusion.internal.utils import (
-    validate_member_arguments,
     validate_member_arguments_configured,
     BaseConfig,
 )
 from diffusion.internal.validation import StrictNonNegativeInt
 from diffusion.session.locks.session_locks import SessionLock
+if typing.TYPE_CHECKING:
+    from diffusion.internal.serialisers import Serialiser
+
 
 TypeGetter = typing.Callable[[typing.Any], typing.Type["AbstractDataType"]]
 
 
 class ConstraintSingleton(typing.Generic[UpdateConstraint_T]):
     @functools.lru_cache(maxsize=None)
     def __get__(self, instance, owner) -> UpdateConstraint_T:
@@ -45,41 +47,36 @@
 
 class Unconstrained(UpdateConstraint):
     """
     The unconstrained update constraint.
     """
 
     Instance = typing.cast(typing.ClassVar[ConstraintSingleton], ConstraintSingleton())
-    ID: typing.ClassVar[int] = 0
 
     def __str__(self):
         return "Unconstrained"
 
     class Config(UpdateConstraint.Config["Unconstrained"]):
         @classmethod
-        @functools.lru_cache(maxsize=None)
-        def field_names(
-            cls, modelcls: typing.Type[Unconstrained], serialiser=None
-        ) -> typing.List[str]:
-            return []
+        def id(cls) -> Literal[UpdateConstraintType.UNCONSTRAINED_CONSTRAINT]:
+            return UpdateConstraintType.UNCONSTRAINED_CONSTRAINT
 
         @classmethod
         def attr_mappings_all(cls, modelcls):
             return {"unconstrained-constraint": {}}
 
 
 ConjunctionConstraint_T = typing.TypeVar(
     "ConjunctionConstraint_T", bound="ConjunctionConstraint"
 )
 
 
 @pydantic.dataclasses.dataclass(config=BaseConfig, eq=True, frozen=True)
 class ConjunctionConstraint(UpdateConstraint):
     constraints: typing.Tuple[UpdateConstraint, ...]
-    ID: typing.ClassVar[int] = 1
 
     def __init__(
         self,
         constraints_begin: typing.Union[
             UpdateConstraint, typing.Tuple[UpdateConstraint, ...]
         ] = tuple(),
         second_term: typing.Optional[
@@ -118,93 +115,103 @@
 
     def __str__(self):
         return f"Constraints=({', '.join(str(x) for x in self.constraints)})"
 
     def __iter__(self):
         return iter(self.constraints)
 
-    class Config(
-        DataclassConfigMixin["ConjunctionConstraint"], UpdateConstraint.Config
-    ):
+    class Config(UpdateConstraint.Config):
+        @classmethod
+        def id(cls) -> Literal[UpdateConstraintType.CONJUNCTION_CONSTRAINT]:
+            return UpdateConstraintType.CONJUNCTION_CONSTRAINT
+
         @classmethod
         def as_service_value(
             cls: typing.Type[GenericConfig[ConjunctionConstraint_T]],
             item: ConjunctionConstraint_T,
-            serialiser=None,
+            serialiser: Serialiser = None,
         ) -> ServiceValue:
+            serialiser = cls.check_serialiser(serialiser)
             result = (
                 typing.cast(GenericConfig[ConjunctionConstraint_T], super())
             ).as_service_value(item, serialiser)
             if len(item.constraints):
                 constraint_tuples: typing.Tuple[typing.Any, ...] = sum(
-                    [(x.Config.as_tuple(x),) for x in item.constraints],
+                    (
+                        (cls.entry_from_list_of_choices_as_tuple(x, serialiser),)
+                        for x in item.constraints
+                    ),
                     typing.cast(typing.Tuple[typing.Any, ...], tuple()),
                 )
                 result = result.evolve(**{"conjunction-constraint": constraint_tuples})
             return result
 
 
 @pydantic.dataclasses.dataclass(frozen=True, eq=True)
 class BinaryValueConstraint(UpdateConstraint):
     """
     The update constraint that requires the exact binary value.
     """
 
     bytes: pydantic.StrictBytes
-    ID: typing.ClassVar[int] = 2
     IsTopicConstraint: typing.ClassVar[bool] = True
 
     def __iter__(self):
         return iter((self,))
 
     def __str__(self):
         return f"Bytes={self.bytes}"
 
     class Config(
-        DataclassConfigMixin["BinaryValueConstraint"], UpdateConstraint.Config
+         UpdateConstraint.Config
     ):
+        @classmethod
+        def id(cls) -> Literal[UpdateConstraintType.BINARY_VALUE_CONSTRAINT]:
+            return UpdateConstraintType.BINARY_VALUE_CONSTRAINT
         alias = "binary-value-constraint"
 
         @classmethod
         def attr_mappings_all(cls, modelcls: typing.Type[BinaryValueConstraint]):
-            return {"binary-value-constraint": {"binary-value-constraint": "bytes"}}
+            return {"binary-value-constraint": {"bytes": "bytes"}}
 
 
 class NoValueConstraint(UpdateConstraint):
     """
     The update constraint that requires a topic to have no value.
     """
 
     Instance = typing.cast(typing.ClassVar["NoValueConstraint"], ConstraintSingleton())
-    ID: typing.ClassVar[int] = 3
     IsTopicConstraint: typing.ClassVar[bool] = True
 
     def __str__(self):
         return "NoValue"
 
     class Config(UpdateConstraint.Config["NoValueConstraint"]):
         @classmethod
+        def id(cls) -> Literal[UpdateConstraintType.NO_VALUE_CONSTRAINT]:
+            return UpdateConstraintType.NO_VALUE_CONSTRAINT
+
+        @classmethod
         @functools.lru_cache(maxsize=None)
         def field_names(
-            cls, modelcls: typing.Type[NoValueConstraint], serialiser=None
+            cls, modelcls: typing.Type[NoValueConstraint], serialiser: Serialiser = None
         ) -> typing.List[str]:
             return []
 
         @classmethod
         def attr_mappings_all(cls, modelcls: typing.Type[NoValueConstraint]):
             return {"no-value-constraint": {}}
 
 
 @pydantic.dataclasses.dataclass(frozen=True)
 class LockConstraint(UpdateConstraint):
     """
     The constraint on a [SessionLock][diffusion.session.locks.session_locks.SessionLock]
     """
 
-    ID: typing.ClassVar[int] = 4
     name: pydantic.StrictStr
     sequence: StrictNonNegativeInt
 
     def _frozen_init(self, name: pydantic.StrictStr, sequence: StrictNonNegativeInt):
         object.__setattr__(self, "name", name)
         object.__setattr__(self, "sequence", sequence)
 
@@ -223,15 +230,19 @@
         **kwargs: typing.Union[pydantic.StrictStr, StrictNonNegativeInt, SessionLock],
     ):
         pass
 
     def __str__(self):
         return f"{type(self).__name__}(name='{self.name}', sequence={self.sequence})"
 
-    class Config(DataclassConfigMixin["LockConstraint"], UpdateConstraint.Config):
+    class Config(UpdateConstraint.Config):
+        @classmethod
+        def id(cls) -> Literal[UpdateConstraintType.LOCKED_CONSTRAINT]:
+            return UpdateConstraintType.LOCKED_CONSTRAINT
+
         @classmethod
         def attr_mappings_all(cls, modelcls: typing.Type[LockConstraint]):
             return {
                 "locked-constraint": {
                     "session-lock-name": "name",
                     "session-lock-sequence": "sequence",
                 }
@@ -240,61 +251,71 @@
 
 class NoTopicConstraint(UpdateConstraint):
     """
     The update constraint that requires the path to have no topic.
     """
 
     Instance = typing.cast(typing.ClassVar["NoTopicConstraint"], ConstraintSingleton())
-    ID: typing.ClassVar[int] = 5
     IsTopicConstraint: typing.ClassVar[bool] = True
 
     def __str__(self):
         return "NoTopic"
 
-    class Config(DataclassConfigMixin["NoTopicConstraint"], UpdateConstraint.Config):
+    class Config(UpdateConstraint.Config):
+        @classmethod
+        def id(cls) -> Literal[UpdateConstraintType.NO_TOPIC_CONSTRAINT]:
+            return UpdateConstraintType.NO_TOPIC_CONSTRAINT
+
         @classmethod
         def attr_mappings_all(cls, modelcls: typing.Type[NoTopicConstraint]):
             return {"no-topic-constraint": {}}
 
 
 WithValuesType = typing.Tuple[typing.Tuple[str, bytes], ...]
 
 
+PartialJSONType = typing.TypeVar("PartialJSONType")
+"""
+Instance of PartialJSON or any subclasses
+"""
+
+
 @pydantic.dataclasses.dataclass(config=BaseConfig, frozen=True, eq=True)
 class PartialJSON(UpdateConstraint):
     """
     The constraint requiring the current value of the
     [JSON][diffusion.datatypes.JSON] topic to match the
     partially described value.
     """
 
-    ID: typing.ClassVar[int] = 6
     IsTopicConstraint: typing.ClassVar[bool] = True
 
     with_values: WithValuesType
     without_values: typing.FrozenSet[str]
 
     @property
-    def with_values_dict(self) -> collections.abc.Mapping:
+    def with_values_dict(self) -> typing.Mapping[str, typing.Any]:
         return dict(self.with_values)
 
     @validate_member_arguments_configured(config=BaseConfig)
     def __init__(
         self, with_values, without_values: typing.FrozenSet[str] = frozenset()
     ):
         object.__setattr__(self, "with_values", with_values)
         object.__setattr__(self, "without_values", without_values)
         self.__pydantic_validate_values__()  # type: ignore
         object.__setattr__(self, "with_values", with_values)
         object.__setattr__(self, "without_values", without_values)
 
-    @validate_member_arguments
+    @validate_member_arguments_configured(
+        deferred=lambda: dict(PartialJSONType=PartialJSONType)
+    )
     def with_(
-        self, pointer: pydantic.StrictStr, value: AbstractDataType
-    ) -> "PartialJSON":
+        self: PartialJSONType, pointer: pydantic.StrictStr, value: AbstractDataType
+    ) -> "PartialJSONType":
         """
         Requires a value at a specific position in the JSON object.
 
         Notes:
             The `pointer` is a JSON Pointer (https://tools.ietf.org/html/rfc6901) syntax reference
             locating the `value` in the JSON object.
 
@@ -303,48 +324,59 @@
         Args:
             pointer: The pointer expression.
             value: The value.
         Returns:
             The constraint including the specified `pointer`.
 
         """  # NOQA
+        assert isinstance(self, PartialJSON)
+        return typing.cast(PartialJSONType, self._with_impl(pointer, value))
+
+    def _with_impl(self, pointer: pydantic.StrictStr, value: AbstractDataType):
         new_with_values: typing.Dict[str, bytes] = {**dict(self.with_values)}
         new_without_values = frozenset(self.without_values)
         for k, v in self.with_values:
             new_with_values[k] = v
         new_with_values[pointer] = value.to_bytes()
         final_without_values = new_without_values - frozenset({pointer})
         return type(self)(tuple(new_with_values.items()), final_without_values)
 
-    @validate_member_arguments
-    def without(self, pointer: pydantic.StrictStr):
+    @validate_member_arguments_configured(
+        deferred=lambda: dict(PartialJSON=PartialJSON, PartialJSONType=PartialJSONType)
+    )
+    def without(self: PartialJSONType, pointer: pydantic.StrictStr) -> "PartialJSONType":
         """
         Requires a specific position in the JSON object to be empty.
 
         Notes:
             The `pointer` is a JSON Pointer (https://tools.ietf.org/html/rfc6901) syntax reference
             that should have no value in the JSON object.
 
             The `pointer` syntax is not being verified for correctness.
 
         Args:
             pointer: The pointer expression.
         Returns:
             The constraint including the specified `pointer`.
         """  # NOQA
+        assert isinstance(self, PartialJSON)
         new_with_values = {k: v for k, v in self.with_values if k is not pointer}
-        return type(self)(
+        return typing.cast(PartialJSONType, type(self)(
             tuple(new_with_values.items()),
             self.without_values.union(frozenset({pointer})),
-        )
+        ))
 
     def __str__(self):
         return f"with_values={self.with_values}, without_values={self.without_values}"
 
-    class Config(DataclassConfigMixin["PartialJSON"], UpdateConstraint.Config):
+    class Config(UpdateConstraint.Config):
+        @classmethod
+        def id(cls) -> Literal[UpdateConstraintType.PARTIAL_JSON_CONSTRAINT]:
+            return UpdateConstraintType.PARTIAL_JSON_CONSTRAINT
+
         @classmethod
         def attr_mappings_all(cls, modelcls: typing.Type[PartialJSON]):
             return {
                 "partial-json-constraint": {
                     "partial-json-constraint-with": "with_values",
                     "partial-json-constraint-without": "without_values",
                 }
```

## diffusion/internal/utils.py

```diff
@@ -1,8 +1,9 @@
 """ Various utilities that don't fit into any particular module. """
+from __future__ import annotations
 import enum
 import functools
 import typing
 from collections import defaultdict
 from functools import reduce, wraps
 from inspect import iscoroutinefunction, ismethod
 from itertools import chain
@@ -194,18 +195,14 @@
     arbitrary_types_allowed = True
     TC_ERROR = ValidationError
     allow_population_by_field_name = True
     copy_on_model_validation = "shallow"
     frozen = False
     underscore_attrs_are_private = True
 
-    @classmethod
-    def decode(cls, item):
-        return decode(item)
-
 
 def gen_overload_validator(validated_main_func, overloads, validator, **fwd_refs):
     validated_funcs = []
     for overload in overloads:
         validated_func = validator(overload)
         validated_func.model.update_forward_refs(**fwd_refs)  # type: ignore
         validated_funcs.append(validated_func)
@@ -292,16 +289,18 @@
         def first_time(self, *args, **kwargs):
             nonlocal wrapped
             nonlocal deferred
             if deferred:
                 deferred_run = deferred()
             else:
                 deferred_run = {}
+            updated = {type(self).__name__: type(self)}
+            updated.update(deferred_run)
             validated_main_func.model.update_forward_refs(
-                **{type(self).__name__: type(self)}, **deferred_run
+                **updated
             )
             wrapped = result
             return result(self, *args, **kwargs)
 
         wrapped = first_time
 
         if config.TC_ERROR == ValidationError:
```

## diffusion/internal/encoded_data/abstract.py

```diff
@@ -1,20 +1,29 @@
 """ Abstract definition for encoded data. """
 
 from __future__ import annotations
 
+import inspect
 import io
+import typing
 from abc import ABCMeta, abstractmethod
 from typing import Any, Type, TypeVar, Union
 
 from typing_extensions import Protocol, runtime_checkable
 
+if typing.TYPE_CHECKING:
+    from diffusion.internal.serialisers import Serialiser, Resolver
+
+
+SpecType = typing.TypeVar("SpecType", contravariant=True)
+EncodingProtocolVar = typing.TypeVar("EncodingProtocolVar", bound="EncodingProtocol")
+
 
 @runtime_checkable
-class EncodingProtocol(Protocol):
+class EncodingProtocol(Protocol[SpecType]):
     """General protocol for encoded data.
 
     Must be implemented for all classes which can be used to serialise
     and deserialise the data over the wire, even if they don't extend
     `EncodingType` directly. In other words, it allows for duck-typing
     serialisation/deserialisation.
     """
@@ -28,24 +37,33 @@
         """
 
     def write(self, stream: io.BytesIO) -> io.BytesIO:
         """ Write the bytes representation of a value into a binary stream. """
 
     def to_bytes(self) -> bytes:
         """ Convert the value into its bytes representation. """
+    @classmethod
+    def create(
+        cls: typing.Type[EncodingProtocolVar],
+        spec: "SpecType",
+        name: str,
+        parents: typing.List[str] = None,
+        resolver: "Resolver" = None,
+    ) -> typing.Type[EncodingProtocolVar]:
+        raise NotImplementedError()
 
 
 class EncodingTypeMeta(ABCMeta):
     """ Metaclass for `EncodingType`, implementing functionalities on its subclasses. """
 
     def __repr__(cls):
         return f"encoded_data.{cls.__name__}"
 
 
-class EncodingType(metaclass=EncodingTypeMeta):
+class EncodingType(typing.Generic[SpecType], metaclass=EncodingTypeMeta):
     """ Base class for low-level encoding types. """
 
     value: Any
 
     def __init__(self, value: Any):
         self.value = value
         self.validate()
@@ -75,13 +93,42 @@
             DataValidationError: If a value is considered invalid.
                                  By default there is no validation.
         """
 
     def __repr__(self):
         return f"{type(self).__name__}({repr(self.value)})"
 
+    @classmethod
+    def extract_from(
+        cls: typing.Type[EncodingTypeVar],
+        encoder_or_serialiser: typing.Union[typing.Type[EncodingTypeVar], Serialiser],
+    ) -> typing.Type[EncodingTypeVar]:
+        from diffusion.internal.serialisers.base import Serialiser
+
+        if inspect.isclass(encoder_or_serialiser) and issubclass(
+            typing.cast(typing.Type[EncodingTypeVar], encoder_or_serialiser),
+            cls,
+        ):
+            return typing.cast(typing.Type[EncodingTypeVar], encoder_or_serialiser)
+        assert isinstance(encoder_or_serialiser, Serialiser)
+        return encoder_or_serialiser.to_encoder(cls)
+
+    @classmethod
+    def as_tuple(cls, item):
+        raise NotImplementedError()
+
+    @classmethod
+    def create(
+        cls: typing.Type[EncodingProtocolVar],
+        spec: "SpecType",
+        name: str,
+        parents: typing.List[str] = None,
+        resolver: "Resolver" = None,
+    ) -> typing.Type[EncodingProtocolVar]:
+        raise NotImplementedError()
+
 
 Enc_MetaType = Type[EncodingType]
 Enc_MetaType_Str = Union[str, Enc_MetaType]
-EncodingTypeVar = TypeVar('EncodingTypeVar', bound=EncodingType)
+EncodingTypeVar = TypeVar('EncodingTypeVar', bound=EncodingProtocol)
 Enc_K = TypeVar('Enc_K', bound=EncodingType)
 Enc_V = TypeVar('Enc_V', bound=EncodingType)
```

## diffusion/internal/generated/services.py

```diff
@@ -1,53 +1,65 @@
-from diffusion.internal.services.abstract import OutboundService
+import attr
 from diffusion.internal.serialisers import get_serialiser
-from diffusion.internal.services.topics import (
-    NotifySubscription,
-    AddAndSetTopic,
-    TopicAdd,
-    NotifyUnsubscription,
-    Unsubscribe,
-    Subscribe,
-    TopicRemoval,
-)
-from diffusion.internal.services.session import UserPing, ChangePrincipal, SystemPing
+from diffusion.internal.services.abstract import OutboundService
 from diffusion.internal.services.messaging import (
+    FilterResponse,
     MessagingFilterSender,
-    MessagingReceiverServer,
     MessagingReceiverClient,
     MessagingReceiverControlRegistration,
+    MessagingReceiverServer,
     MessagingSend,
-    FilterResponse,
 )
-import attr
+from diffusion.internal.services.session import ChangePrincipal, SystemPing, UserPing
+from diffusion.internal.services.topics import (
+    AddAndSetTopic,
+    NotifySubscription,
+    NotifyUnsubscription,
+    Subscribe,
+    TopicAdd,
+    TopicRemoval,
+    Unsubscribe,
+)
 
 
 class RangeQuery(OutboundService):
     service_id = 84
     name = "RANGE_QUERY"
-    request_serialiser_map = {24: "range-query-request"}
-    response_serialiser_map = {24: "range-query-result"}
+    request_serialiser_map = {12: "range-query-request", 24: "range-query-request"}
+    response_serialiser_map = {12: "range-query-result", 24: "range-query-result"}
     request_serialiser = get_serialiser("range-query-request")
     response_serialiser = get_serialiser("range-query-result")
 
 
 class TimeSeriesAppend(OutboundService):
     service_id = 99
     name = "TIME_SERIES_APPEND"
-    request_serialiser_map = {24: "time-series-append-request"}
-    response_serialiser_map = {24: "time-series-update-response"}
+    request_serialiser_map = {
+        12: "time-series-append-request",
+        24: "time-series-append-request",
+    }
+    response_serialiser_map = {
+        12: "time-series-update-response",
+        24: "time-series-update-response",
+    }
     request_serialiser = get_serialiser("time-series-append-request")
     response_serialiser = get_serialiser("time-series-update-response")
 
 
 class TimeSeriesEdit(OutboundService):
     service_id = 100
     name = "TIME_SERIES_EDIT"
-    request_serialiser_map = {24: "time-series-edit-request"}
-    response_serialiser_map = {24: "time-series-update-response"}
+    request_serialiser_map = {
+        12: "time-series-edit-request",
+        24: "time-series-edit-request",
+    }
+    response_serialiser_map = {
+        12: "time-series-update-response",
+        24: "time-series-update-response",
+    }
     request_serialiser = get_serialiser("time-series-edit-request")
     response_serialiser = get_serialiser("time-series-update-response")
 
 
 class AcquireSessionLock(OutboundService):
     service_id = 114
     name = "ACQUIRE_SESSION_LOCK"
@@ -154,18 +166,18 @@
 
 class PutTopicMetricCollector(OutboundService):
     service_id = 146
     name = "PUT_TOPIC_METRIC_COLLECTOR"
     request_serialiser_map = {
         16: "protocol16-topic-metric-collector",
         22: "protocol16-topic-metric-collector",
-        24: "topic-metric-collector",
+        24: "protocol24-topic-metric-collector",
     }
-    response_serialiser_map = {16: "void", 22: "void", 24: "void"}
-    request_serialiser = get_serialiser("topic-metric-collector")
+    response_serialiser_map = {16: "void", 22: "void", 24: "void", 25: "void"}
+    request_serialiser = get_serialiser("protocol24-topic-metric-collector")
     response_serialiser = get_serialiser("void")
 
 
 class RemoveTopicMetricCollector(OutboundService):
     service_id = 147
     name = "REMOVE_TOPIC_METRIC_COLLECTOR"
     request_serialiser_map = {16: "string", 22: "string"}
@@ -177,25 +189,31 @@
 class ListTopicMetricCollectors(OutboundService):
     service_id = 148
     name = "LIST_TOPIC_METRIC_COLLECTORS"
     request_serialiser_map = {16: "void", 22: "void", 24: "void"}
     response_serialiser_map = {
         16: "protocol16-topic-metric-collectors",
         22: "protocol16-topic-metric-collectors",
-        24: "topic-metric-collectors",
+        24: "protocol24-topic-metric-collectors",
     }
     request_serialiser = get_serialiser("void")
-    response_serialiser = get_serialiser("topic-metric-collectors")
+    response_serialiser = get_serialiser("protocol24-topic-metric-collectors")
 
 
 class TimeSeriesTimestampAppend(OutboundService):
     service_id = 166
     name = "TIME_SERIES_TIMESTAMP_APPEND"
-    request_serialiser_map = {24: "time-series-timestamp-append-request"}
-    response_serialiser_map = {24: "time-series-update-response"}
+    request_serialiser_map = {
+        19: "time-series-timestamp-append-request",
+        24: "time-series-timestamp-append-request",
+    }
+    response_serialiser_map = {
+        19: "time-series-update-response",
+        24: "time-series-update-response",
+    }
     request_serialiser = get_serialiser("time-series-timestamp-append-request")
     response_serialiser = get_serialiser("time-series-update-response")
 
 
 class PutBranchMappingTable(OutboundService):
     service_id = 176
     name = "PUT_BRANCH_MAPPING_TABLE"
```

## diffusion/internal/serialisers/__init__.py

```diff
@@ -1,48 +1,54 @@
+#  Copyright (c) 2020-2023 Push Technology Ltd., All Rights Reserved.
+#
+#  Use is subject to license terms.
+#
+#  NOTICE: All information contained herein is, and remains the
+#  property of Push Technology. The intellectual and technical
+#  concepts contained herein are proprietary to Push Technology and
+#  may be covered by U.S. and Foreign Patents, patents in process, and
+#  are protected by trade secret or copyright law.
+
 """ Module for defining serialisers.
 
     The key component is the `SERIALISER_SPECS` mapping, which is based on
     the specification in `spec.clj`.
 """
 from __future__ import annotations
 
 from typing import TypeVar
 
 from typing_extensions import Protocol
 
 import typing
 
 if typing.TYPE_CHECKING:
-    from .base import Serialiser
+    from .base import Serialiser, Resolver
     from ..services import ServiceValue
 
 T = TypeVar("T")
 
 
-def get_serialiser(name: str = None) -> Serialiser:
+def get_serialiser(name: str = None, resolver: Resolver = None) -> Serialiser:
     from .spec import NULL_VALUE_KEY
 
     """ Retrieve a serialiser instance based on the spec name. """
     from .base import Serialiser
 
     return Serialiser.by_name(
-        NULL_VALUE_KEY if name is None else name
+        NULL_VALUE_KEY if name is None else name, resolver=resolver
     )
 
 
 class Serialisable(Protocol):
     @classmethod
     def from_fields(cls: typing.Type[T], **kwargs) -> T:
         pass  # pragma: no cover
 
     @classmethod
-    def attr_mappings(cls) -> typing.Dict[str, typing.Any]:
-        pass  # pragma: no cover
-
-    @classmethod
     def from_service_value(
         cls: typing.Type[T], item: ServiceValue
     ) -> T:
         pass  # pragma: no cover
 
 
 Serialisable_T = TypeVar(
```

## diffusion/internal/serialisers/attrs.py

```diff
@@ -16,48 +16,45 @@
 import attr
 
 from diffusion.handlers import LOG
 from diffusion.internal.serialisers.generic_model import (
     GenericModel,
     GenericMetaModel,
     GenericConfig,
-    GenericModel_T,
 )
+
 if typing.TYPE_CHECKING:
     from diffusion.internal.services import ServiceValue
+    from diffusion.internal.serialisers import Serialiser
 
 AttrsModel_T = typing.TypeVar("AttrsModel_T", bound="MarshalledModel")
 AttrsModel_T_Other = typing.TypeVar("AttrsModel_T_Other", bound="MarshalledModel")
 
 
 @attr.s
 class MarshalledModel(GenericModel, metaclass=GenericMetaModel):
     class Config(GenericConfig["MarshalledModel"]):
         _modelcls: typing.Type[MarshalledModel]
 
         @classmethod
         @functools.lru_cache(maxsize=None)
         def find_aliases(
-            cls, modelcls: typing.Type[MarshalledModel], serialiser: typing.Optional[str]
+            cls, modelcls: typing.Type[MarshalledModel], serialiser: Serialiser
         ) -> typing.Mapping[str, str]:
+            serialiser = cls.check_serialiser(serialiser)
             updates = {}
             for x in attr.fields(modelcls):
                 if x.metadata:
-                    target = x.metadata.get(serialiser or cls.alias, x.metadata.get("alias"))
+                    target = x.metadata.get(
+                        getattr(serialiser, "name") or cls.alias, x.metadata.get("alias")
+                    )
                     updates[target] = x.name
             return updates
 
         @classmethod
-        @functools.lru_cache(maxsize=None)
-        def field_names(
-            cls, modelcls: typing.Type[GenericModel_T], serialiser=None
-        ) -> typing.List[str]:
-            return [x.name for x in attr.fields(modelcls)]
-
-        @classmethod
         def from_service_value(
             cls,
             modelcls: typing.Type[MarshalledModel],
             item: ServiceValue,
         ) -> MarshalledModel:
             fields = cls.get_fields(item, modelcls)
             for field_name, field_value in fields.items():
```

## diffusion/internal/serialisers/base.py

```diff
@@ -1,42 +1,83 @@
+#  Copyright (c) 2020-2023 Push Technology Ltd., All Rights Reserved.
+#
+#  Use is subject to license terms.
+#
+#  NOTICE: All information contained herein is, and remains the
+#  property of Push Technology. The intellectual and technical
+#  concepts contained herein are proprietary to Push Technology and
+#  may be covered by U.S. and Foreign Patents, patents in process, and
+#  are protected by trade secret or copyright law.
+
 """ Base classes for implementation of serialisers. """
 
 from __future__ import annotations
 
+import collections
+import functools
 import inspect
 import io
+import os
+import textwrap
 import typing
-from typing import Any, cast, Iterable, List, Mapping, MutableMapping, Sequence, Dict, Type
+from typing import Any, cast, Iterable, List, Mapping, MutableMapping, Sequence, Type
 
 import structlog
 from stringcase import pascalcase, snakecase
+from typing_extensions import runtime_checkable, Protocol
 
 from diffusion.internal.encoded_data import Byte, EncodingType, is_encoder
 from diffusion.internal.utils import flatten_mapping
-import diffusion.internal.serialisers.generic_model as generic_model
-from .compound import MapSerialiser, ScalarSetSerialiser
+from .compound import (
+    GenericMapSerialiser,
+    GenericScalarSetSerialiser, KeyValue,
+)
+from .generic_model import GenericModel_T, GenericModel
 from .spec import (
-    SERIALISER_SPECS, SerialiserMap, NULL_VALUE_KEY, Compound, CompoundSpec
+    SERIALISER_SPECS,
+    SerialiserMap,
+    NULL_VALUE_KEY,
+    Compound,
+    CompoundSpec,
+    SerialiserMapValue, MutableSerialiserMap,
 )
-from diffusion.internal.encoded_data.abstract import Enc_MetaType_Str, Enc_MetaType
+from diffusion.internal.encoded_data.abstract import Enc_MetaType_Str, Enc_MetaType, \
+    EncodingTypeVar, EncodingProtocol
 from diffusion.internal.protocol.exceptions import ErrorReport, ReportsError
 from diffusion.internal.encoded_data.exceptions import StreamExhausted
 
-
 LOG = structlog.get_logger()
 
+ID_Type = typing.TypeVar("ID_Type", bound=int, covariant=True)
+
+
+def log(x: str):
+    stack_length = len(inspect.stack(0))-30
+    to_log = textwrap.indent(x, "    "*stack_length)
+    if os.getenv("DEBUG_RESOLVER"):
+        LOG.debug(to_log)
+
+
+@runtime_checkable
+class ChoiceProvider(Protocol[ID_Type]):
+    @classmethod
+    def id(cls) -> ID_Type:
+        raise NotImplementedError()
+
 
 class Serialiser:
     """ Class for individual serialisers. """
 
     spec: SerialiserMap
+    resolver: Resolver
 
-    def __init__(self, name: str, spec: SerialiserMap):
+    def __init__(self, name: str, spec: SerialiserMap, resolver: Resolver = None):
         self.name = name
         self.spec = spec
+        self.resolver = resolver or resolve
 
     def from_bytes(self, value: bytes):
         """ Deserialise a bytes value. """
         yield from self.read(io.BytesIO(value))
 
     def read(self, stream: io.BytesIO):
         """ Read the value from a binary stream. """
@@ -83,17 +124,18 @@
         """ Returns a list of all the field names. """
         return list(self.spec)
 
     def __repr__(self):
         return f"<{type(self).__name__} name={self.name}>"
 
     @classmethod
-    def by_name(cls, name: str = NULL_VALUE_KEY) -> Serialiser:
+    def by_name(cls, name: str = NULL_VALUE_KEY, resolver: Resolver = None) -> Serialiser:
         """ Retrieve a serialiser instance based on the spec name. """
-        return Serialiser(name, resolve(name))
+        resolver = resolver or resolve
+        return Serialiser(name, resolver(name), resolver=resolver)
 
     def __bool__(self):
         return self.name != NULL_VALUE_KEY
 
     async def error_from(self,
                          value: Mapping[typing.Union[str, int], Any],
                          tp: Type[ReportsError]):
@@ -103,66 +145,49 @@
             if next_next_err:
                 reports = [
                     ErrorReport(*x) for x in
                     typing.cast(typing.Iterable[Any], next_next_err)
                 ]
                 raise tp(reports)
 
-
-class ChoiceEncodingType(type):
-    """ Metaclass for choice encoding types. """
-
-    _choice_encoding_types: Dict[str, ChoiceEncodingType] = {}
-
-    def __new__(mcs, name: str, specs: SerialiserMap) -> ChoiceEncodingType:
-        """ Construct a new choice encoder based on the serialiser specs. """
-        if name not in mcs._choice_encoding_types:
-            serialisers: MutableMapping[int, Serialiser] = {}
-            serialiser_names: MutableMapping[typing.Hashable, str] = {}
-            for key, value in specs.items():
-                if not (isinstance(key, int) and isinstance(value, Sequence)):
-                    raise ValueError(
-                        "Keys have to be integers and values have to be sequences."
-                    )
-                serialiser_name = f"{name}.{key}"
-                if all(map(is_encoder, value)):
-                    spec = value
-                elif isinstance(value, CompoundSpec):
-                    spec = _resolve_compound(key, value)
-                else:
-                    spec = []
-                    for num, val in enumerate(value):
-                        if isinstance(val, CompoundSpec):
-                            spec.append(_resolve_compound(str(num), val))
-                        else:
-                            spec.append(resolve(val))
-                    spec = tuple(spec)
-                    if isinstance(value, str):
-                        serialiser_names[key] = value
-                    elif (
-                        isinstance(value, tuple) and
-                        len(value) == 1 and isinstance(value[0], str)
-                    ):
-                        serialiser_names[key] = value[0]
-                serialisers[key] = Serialiser(serialiser_name, {serialiser_name: spec})
-            class_name = f"{pascalcase(snakecase(name))}ChoiceEncoder"
-            new_type = cast(
-                ChoiceEncodingType,
-                type(class_name, (ChoiceEncoder,),
-                     {"serialisers": serialisers, "serialiser_names": serialiser_names}),
-            )
-            mcs._choice_encoding_types[name] = new_type
-        return mcs._choice_encoding_types[name]
+    @functools.lru_cache(maxsize=None)
+    def get_choice_encoder_from_list(self) -> typing.Type[ChoiceEncoder]:
+        list_encoder = self.to_encoder(ListEncoder)
+        return ChoiceEncoder.extract_from(list_encoder.serialiser)
+
+    def get_encoder(
+        self, *cls: typing.Type[EncodingTypeVar]
+    ) -> typing.Optional[typing.Type[EncodingTypeVar]]:
+        if not len(self.spec.values()) == 1:
+            return None
+        encoder_candidate = typing.cast(
+            typing.Type[EncodingTypeVar],
+            next(iter(self.spec.values())),
+        )
+        # noinspection PyTypeHints
+        if inspect.isclass(encoder_candidate) and issubclass(
+            encoder_candidate, cls
+        ):
+            return encoder_candidate
+        return None
+
+    def to_encoder(
+            self, cls: typing.Type[EncodingTypeVar]
+    ) -> typing.Type[EncodingTypeVar]:
+        result = self.get_encoder(cls)
+        assert result
+        return result
 
 
-class ChoiceEncoder(EncodingType):
+class ChoiceEncoder(EncodingType[SerialiserMap]):
     """ Special "encoding type" for choice-based values (i.e. `one-of'). """
 
     serialisers: Mapping[int, Serialiser]
     serialiser_names: Mapping[typing.Hashable, str]
+    resolver: Resolver
 
     def __init__(self, value: Sequence):
         super().__init__(value)
 
     @classmethod
     def read(cls, stream: io.BytesIO) -> EncodingType:
         """Read the encoded value from a binary stream.
@@ -198,17 +223,101 @@
 
     @property
     def serialiser(self):
         """ Return the serialises spec for the current choice. """
         return self.serialisers[self.choice]
 
     @classmethod
-    def from_name(cls, serialiser_name: str) -> ChoiceEncodingType:
-        """ Instantiate the class by resolving the serialiser name. """
-        return ChoiceEncodingType(serialiser_name, resolve(serialiser_name))
+    def from_name(
+        cls, serialiser_name: str, resolver: Resolver = None
+    ) -> typing.Type[ChoiceEncoder]:
+        """Instantiate the class by resolving the serialiser name."""
+        resolver = resolver or resolve
+        return resolver.resolve_generic(ChoiceEncoder, resolver(serialiser_name),
+                                        serialiser_name)
+
+    @classmethod
+    def get_serialiser_by_id(cls, id: int, resolver: Resolver = None):
+        serialiser_name = cls.serialiser_names.get(id)
+        assert serialiser_name is not None
+        return Serialiser.by_name(serialiser_name, resolver=resolver)
+
+    @classmethod
+    def get_serialiser_by_provider(
+        cls, provider: typing.Union[ChoiceProvider, typing.Type[ChoiceProvider]]
+    ):
+        assert isinstance(provider, ChoiceProvider) or (
+            inspect.isclass(provider)
+            and issubclass(
+                typing.cast(typing.Type[ChoiceProvider], provider), ChoiceProvider
+            )
+        )
+        return cls.get_serialiser_by_id(provider.id(), resolver=cls.resolver)
+
+    @classmethod
+    def as_tuple(cls, item: GenericModel):
+        return item.Config.as_tuple(
+            item, cls.get_serialiser_by_provider(typing.cast(ChoiceProvider, item.Config))
+        )
+
+    @classmethod
+    def create(
+        cls: typing.Type[EncodingTypeVar],
+        spec: SerialiserMap,
+        name: str,
+        parents: typing.List[str] = None,
+        resolver: Resolver = None,
+    ) -> typing.Type[EncodingTypeVar]:
+        """Construct a new choice encoder based on the serialiser specs."""
+        resolver = resolver or resolve
+        serialisers: MutableMapping[int, Serialiser] = {}
+        serialiser_names: MutableMapping[typing.Hashable, str] = {}
+        for key, value in spec.items():
+            if not (isinstance(key, int) and isinstance(value, Sequence)):
+                raise ValueError(
+                    "Keys have to be integers and values have to be sequences."
+                )
+            serialiser_name = f"{name}.{key}"
+            if all(map(is_encoder, value)):
+                sub_spec = value
+            elif isinstance(value, CompoundSpec):
+                sub_spec = resolver.resolve_compound(key, value)
+            else:
+                sub_spec = []
+                for num, val in enumerate(value):
+                    if isinstance(val, CompoundSpec):
+                        sub_spec.append(resolver.resolve_compound(str(num), val))
+                    else:
+                        sub_spec.append(resolver(val))
+                sub_spec = tuple(sub_spec)
+                if isinstance(value, str):
+                    serialiser_names[key] = value
+                elif (
+                    isinstance(value, tuple)
+                    and len(value) == 1
+                    and isinstance(value[0], str)
+                ):
+                    serialiser_names[key] = value[0]
+            serialisers[key] = Serialiser(
+                serialiser_name, {serialiser_name: sub_spec}, resolver=resolver
+            )
+        class_name = f"{pascalcase(snakecase(name))}ChoiceEncoder"
+
+        return typing.cast(
+            typing.Type[EncodingTypeVar],
+            type(
+                class_name,
+                (ChoiceEncoder,),
+                {
+                    "serialisers": serialisers,
+                    "serialiser_names": serialiser_names,
+                    "resolver": resolver,
+                },
+            ),
+        )
 
 
 class ListEncoder(EncodingType):
     """ Special "encoding type" for choice-based values (i.e. `n-of'). """
 
     serialiser: Serialiser
 
@@ -245,107 +354,150 @@
 
     @property
     def values(self) -> Sequence[Any]:
         """ Return the current collection of values. """
         return self.value
 
     @classmethod
-    def from_name(cls, serialiser_name: str) -> ListEncodingType:
-        """ Instantiate the class by resolving the serialiser name. """
-        return ListEncodingType(serialiser_name, resolve(serialiser_name))
+    def from_tuple(
+        cls,
+        item: typing.Iterable[typing.Tuple[typing.Any, ...]],
+        item_type: typing.Type[GenericModel_T],
+    ) -> typing.List[GenericModel_T]:
+        assert isinstance(item, collections.Iterable)
+        return [item_type.Config.from_tuple(item_type, x, cls.serialiser) for x in item]
 
+    @classmethod
+    def as_tuple(
+        cls, item: typing.Iterable[GenericModel]
+    ) -> typing.Tuple[typing.Tuple[typing.Any, ...], ...]:
+        assert isinstance(item, collections.Iterable)
+        return tuple(x.Config.as_tuple(x, cls.serialiser) for x in item)
 
-class ListEncodingType(type):
-    """ Metaclass for list encoding types. """
+    @classmethod
+    def create(cls, spec: SerialiserMap, name: str, parents: List[str] = None,
+               resolver: Resolver = None) -> typing.Type[ListEncoder]:
+        """Construct a new list encoder based on the serialiser specs."""
+        resolver = resolver or resolve
+        hashed_name = f"{id(resolver)}{name}"
+        if "conjunction" in name and resolver.name != "Default":
+            log("Initialising conjunction")
+        log(
+            f"Constructing {cls.__name__}({name}, {spec}, {parents}, {resolver})="
+            f"{hashed_name}"
+        )
+        if is_encoder(spec):
+            serialiser = spec
+        elif isinstance(spec, CompoundSpec):
+            serialiser = resolver.resolve_compound(f"{name}.{spec.type.name}", spec)
+        elif isinstance(spec, str):
+            serialiser = Serialiser.by_name(spec, resolver=resolver)
+        else:
+            raise Exception(f"can't handle ListEncoder of {spec}")
+        class_name = f"{pascalcase(snakecase(name))}ListSerialiser"
+        if not isinstance(serialiser, Serialiser):
+            log(f"{cls}: {serialiser} is not a Serialiser")
+        else:
+            log(f"{cls}: {serialiser} *is* a Serialiser")
+        new_type = cast(
+            typing.Type[ListEncoder],
+            type(class_name, (ListEncoder,), {"serialiser": serialiser}),
+        )
+        return new_type
 
-    _list_encoding_types: Dict[str, ListEncodingType] = {}
 
-    def __new__(
-        mcs, name: str, spec: SerialiserMap, parents: List[str] = None
-    ) -> ListEncodingType:
-        """Construct a new list encoder based on the serialiser specs."""
-        if name not in mcs._list_encoding_types:
-            if is_encoder(spec):
-                serialiser = spec
-            elif isinstance(spec, CompoundSpec):
-                serialiser = _resolve_compound(f"{name}.{spec.type.name}", spec)
-            elif isinstance(spec, str):
-                serialiser = Serialiser.by_name(spec)
-            else:
-                raise Exception(f"can't handle ListEncodingType of {spec}")
-            class_name = f"{pascalcase(snakecase(name))}ListSerialiser"
-            new_type = cast(
-                ListEncodingType,
-                type(class_name, (ListEncoder,), {"serialiser": serialiser}),
-            )
-            mcs._list_encoding_types[name] = new_type
-        return mcs._list_encoding_types[name]
+class Resolver(object):
+    def __init__(self, name: str, specs: typing.Mapping[str, typing.Any], cached: bool = True):
+        self.name = name
+        self.specs = specs
+        self.cached = cached
+        self.cached_items: typing.Dict[str, typing.Type[EncodingProtocol]] = {}
+
+    def __repr__(self):
+        return f"{type(self).__name__}({(self.name, id(self.specs))}) at {id(self)}"
 
+    def __call__(
+        self, serialiser_name: str, parents: List[str] = None
+    ) -> SerialiserMap:
+        """Extract the serialiser types for any serialiser key in the spec.
 
-def resolve(serialiser_name: str, parents: List[str] = None) -> SerialiserMap:
-    """Extract the serialiser types for any serialiser key in the spec.
+        The `parents` argument is used internally to carry the list of all
+        recursive parents, which is eventually concatenated to an internal key.
 
-    The `parents` argument is used internally to carry the list of all
-    recursive parents, which is eventually concatenated to an internal key.
-
-    The name must be a key in the serialiser spec. The value for a key is
-    recursively expanded into a mapping of encoding type classes.
-    """
-    result: SerialiserMap = {}
-    if parents is None:
-        parents = []
-    parents.append(serialiser_name)
-    try:
-        spec: Any = None
-        found = False
-        elements = serialiser_name.split(".")
-        ser_name = ""
-        while elements:
-            ser_name = ".".join(elements)
-
-            if ser_name in SERIALISER_SPECS:
-                spec = SERIALISER_SPECS.get(ser_name)
-                found = True
-                break
-            elements.pop(0)
-        if not found:
-            raise IndexError(f"No such serialiser {ser_name}, {serialiser_name}")
-    except Exception as e:  # pragma: no cover
-        LOG.error(f"Got exception {e}")
-        raise
-    if not (spec is None or is_encoder(spec)):
-        if spec and inspect.isclass(spec) and issubclass(spec, generic_model.model_variants()):
-            spec = spec.Config.get_spec(spec, serialiser_name)
-        if isinstance(spec, str) or not isinstance(spec, Sequence):
-            spec = [spec]
-        if isinstance(spec, CompoundSpec):
-            spec = _resolve_compound(serialiser_name, spec)
-        elif not all(map(is_encoder, spec)):
-            for value in spec:
-                name = ".".join(parents)
-                if isinstance(value, CompoundSpec):
-                    result[name] = _resolve_compound(name, value)
-                elif is_encoder(value):
-                    result[name] = value
-                else:
-                    result.update(resolve(value, parents.copy()))
-            return result
-    return {".".join(parents): spec}
-
-
-def _resolve_compound(name, spec: CompoundSpec):
-    # this is where proper pattern matching would come in handy :)
-    if spec.type is Compound.MAP_OF:
-        key, value = typing.cast(
-            typing.Tuple[Enc_MetaType_Str, Enc_MetaType_Str],
-            tuple(SERIALISER_SPECS.get(sp, sp) for sp in spec.args),
-        )
-        return MapSerialiser(key, value)
-    if spec.type is Compound.SET_OF:
-        set_spec = spec.args[0]
-        return ScalarSetSerialiser(
-            typing.cast(Enc_MetaType, SERIALISER_SPECS.get(set_spec, set_spec))
-        )
-    if spec.type is Compound.ONE_OF:
-        return ChoiceEncodingType(name, spec.args[0])
-    if spec.type is Compound.N_OF:
-        return ListEncodingType(name, spec.args[0])
+        The name must be a key in the serialiser spec. The value for a key is
+        recursively expanded into a mapping of encoding type classes.
+        """
+        log(f"{self}: Resolving {serialiser_name}, parents {parents}")
+
+        result: MutableSerialiserMap = {}
+        if parents is None:
+            parents = []
+        parents.append(serialiser_name)
+        try:
+            spec: Any = None
+            found = False
+            elements = serialiser_name.split(".")
+            ser_name = ""
+            while elements:
+                ser_name = ".".join(elements)
+
+                if ser_name in self.specs:
+                    spec = self.specs.get(ser_name)
+                    found = True
+                    break
+                elements.pop(0)
+            if not found:
+                raise IndexError(f"No such serialiser {ser_name}, {serialiser_name}")
+        except Exception as e:  # pragma: no cover
+            LOG.error(f"Got exception {e}")
+            raise
+        if not (spec is None or is_encoder(spec)):
+            if isinstance(spec, str) or not isinstance(spec, Sequence):
+                spec = [spec]
+            if isinstance(spec, CompoundSpec):
+                spec = self.resolve_compound(serialiser_name, spec)
+            elif not all(map(is_encoder, spec)):
+                for value in spec:
+                    name = ".".join(parents)
+                    if isinstance(value, CompoundSpec):
+                        result[name] = self.resolve_compound(name, value)
+                    elif is_encoder(value):
+                        result[name] = value
+                    else:
+                        result.update(self(value, parents.copy()))
+                return result
+        return {".".join(parents): spec}
+
+    def resolve_compound(self, name: str, spec: CompoundSpec) -> SerialiserMapValue:
+        log(f"{self}: Resolving complex {name} and {spec}")
+        if name == "conjunction-constraint" and self.name != "Default":
+            log(f"{self}: Resolving complex {name} and {spec}")
+        # this is where proper pattern matching would come in handy :)
+        if spec.type is Compound.MAP_OF:
+            key, value = typing.cast(
+                typing.Tuple[Enc_MetaType_Str, Enc_MetaType_Str],
+                tuple(self.specs.get(sp, sp) for sp in spec.args),
+            )
+            return self.resolve_generic(GenericMapSerialiser, KeyValue(key, value))
+        if spec.type is Compound.SET_OF:
+            set_spec = spec.args[0]
+            serialiser = typing.cast(Enc_MetaType, self.specs.get(set_spec, set_spec))
+            return self.resolve_generic(GenericScalarSetSerialiser, serialiser,
+                                        serialiser.__name__)
+        if spec.type is Compound.ONE_OF:
+            return self.resolve_generic(ChoiceEncoder, spec.args[0], name)
+        if spec.type is Compound.N_OF:
+            return self.resolve_generic(ListEncoder, spec.args[0], name)
+        raise NotImplementedError()
+
+    def resolve_generic(
+        self, encoding_type: typing.Type[EncodingTypeVar], spec, name: str = ""
+    ) -> typing.Type[EncodingTypeVar]:
+        if name == "":
+            name = f"{spec}{encoding_type}"
+        if name not in self.cached_items:
+            result = encoding_type.create(spec, name, resolver=self)
+            self.cached_items[name] = result
+        return typing.cast(typing.Type[EncodingTypeVar], self.cached_items[name])
+
+
+resolve = Resolver("Default", SERIALISER_SPECS)
```

## diffusion/internal/serialisers/compound.py

```diff
@@ -1,28 +1,45 @@
+#  Copyright (c) 2020-2023 Push Technology Ltd., All Rights Reserved.
+#
+#  Use is subject to license terms.
+#
+#  NOTICE: All information contained herein is, and remains the
+#  property of Push Technology. The intellectual and technical
+#  concepts contained herein are proprietary to Push Technology and
+#  may be covered by U.S. and Foreign Patents, patents in process, and
+#  are protected by trade secret or copyright law.
+
 """ Serialisers for values consisting of multiple individual values. """
 
 from __future__ import annotations
 
+import dataclasses
 import io
+import typing
 from typing import cast, Collection, Dict, Generic, Iterable, Sequence, Type, TypeVar, Union
 
 from stringcase import pascalcase
 
 from diffusion.internal.encoded_data import EncodingProtocol, EncodingType, Int32
 from diffusion.internal.encoded_data.exceptions import (
     DataValidationError,
     StreamExhausted,
 )
-from .spec import SERIALISER_SPECS
-from ..encoded_data.abstract import EncodingTypeVar, Enc_K, Enc_V
+
+if typing.TYPE_CHECKING:
+    from .base import Resolver, resolve
+
+from ..encoded_data.abstract import EncodingTypeVar, Enc_K, Enc_V, EncodingProtocolVar
 
 T = TypeVar("T", bound=EncodingType)
 
 
-class GenericScalarSetSerialiser(EncodingProtocol, Generic[T]):
+class GenericScalarSetSerialiser(
+    Generic[T, EncodingTypeVar], EncodingProtocol[typing.Type[EncodingTypeVar]]
+):
     """Generic set for multiple scalar values.
 
     Not technically a set, more of a collection.
     """
 
     scalar_type: Type[T]
 
@@ -74,39 +91,41 @@
                     f"{type(self)} requires a collection of {self.scalar_type.__name__} objects"
                 )
             value.validate()  # type: ignore
 
     def __repr__(self):
         return f"<{type(self).__name__} length={len(self.values)}>"
 
+    @classmethod
+    def create(
+        cls: typing.Type[EncodingProtocolVar],
+        serialiser: Type[EncodingTypeVar],
+        name,
+        parents: typing.List[str] = None,
+        resolver: Resolver = None,
+    ) -> typing.Type[EncodingProtocolVar]:
+        """Class constructor."""
+        resolver = resolver or resolve
+        name = pascalcase(f"{resolver.name}{serialiser.__name__}SetSerialiser")
+        return cast(
+            typing.Type[EncodingProtocolVar],
+            type(name, (GenericScalarSetSerialiser,), {"scalar_type": serialiser}),
+        )
 
-class SetSerialiser(type):
-    """ Metaclass for set serialisers. """
-
-
-class ScalarSetSerialiser(Generic[EncodingTypeVar], SetSerialiser):
-    """ Serialiser for a set of scalar values. """
-
-    _serialisers: Dict[str, ScalarSetSerialiser] = {}
 
-    def __new__(
-        mcs, serialiser: Type[EncodingTypeVar]
-    ) -> ScalarSetSerialiser[EncodingTypeVar]:
-        """Class constructor."""
-        name = pascalcase(f"{serialiser.__name__}SetSerialiser")
-        if name not in mcs._serialisers:
-            mcs._serialisers[name] = cast(
-                ScalarSetSerialiser,
-                type(name, (GenericScalarSetSerialiser,), {"scalar_type": serialiser}),
-            )
-        return cast(ScalarSetSerialiser[EncodingTypeVar], mcs._serialisers[name])
+@dataclasses.dataclass
+class KeyValue(typing.Generic[Enc_K, Enc_V]):
+    enc_k: typing.Union[str, typing.Type[Enc_K]]
+    enc_v: typing.Union[str, typing.Type[Enc_V]]
 
 
-class GenericMapSerialiser(Generic[Enc_K, Enc_V], Dict[Enc_K, Enc_V], EncodingProtocol):
-    """ Serialiser for a mapping value. """
+class GenericMapSerialiser(
+    Generic[Enc_K, Enc_V], Dict[Enc_K, Enc_V], EncodingProtocol[KeyValue[Enc_K, Enc_V]]
+):
+    """Serialiser for a mapping value."""
 
     key_type: Type[Enc_K]
     value_type: Type[Enc_V]
 
     def __init__(self, values: Union[dict, Iterable[tuple]]):
         cast_values = {}
         if isinstance(values, dict):
@@ -165,42 +184,43 @@
     def value(self):
         """ All the values; needed for compatibility with `EncodingType`. """
         return self
 
     def __repr__(self):
         return f"<{type(self).__name__} length={len(self)}>"
 
+    @classmethod
+    def create(
+        cls: typing.Type[EncodingProtocolVar],
+        spec: KeyValue,
+        name,
+        parents: typing.List[str] = None,
+        resolver: Resolver = None,
+    ) -> typing.Type[EncodingProtocolVar]:
+        """Class constructor."""
+        from .base import resolve
 
-class MapSerialiser(Generic[Enc_K, Enc_V]):
-    """ Metaclass for mapping serialisers. """
-
-    _serialisers: Dict[str, MapSerialiser] = {}
-
-    def __new__(
-        mcs,
-        key_serialiser: Union[str, Type[Enc_K]],
-        value_serialiser: Union[str, Type[Enc_V]],
-    ) -> MapSerialiser[Enc_K, Enc_V]:
-        """ Class constructor. """
         ks_resolved: Type[Enc_K]
         vs_resolved: Type[Enc_V]
+        resolver = resolver or resolve
+        key_serialiser = spec.enc_k
+        value_serialiser = spec.enc_v
         if isinstance(key_serialiser, str):
-            ks_resolved = cast(Type[Enc_K], SERIALISER_SPECS[key_serialiser])
+            ks_resolved = cast(Type[Enc_K], resolver.specs[key_serialiser])
         else:
             ks_resolved = key_serialiser
         if isinstance(value_serialiser, str):
-            vs_resolved = cast(Type[Enc_V], SERIALISER_SPECS[value_serialiser])
+            vs_resolved = cast(Type[Enc_V], resolver.specs[value_serialiser])
         else:
             vs_resolved = value_serialiser
         name = pascalcase(
             f"{ks_resolved.__name__}{vs_resolved.__name__}MapSerialiser"  # type: ignore
         )
-        if name not in mcs._serialisers:
-            mcs._serialisers[name] = cast(
-                MapSerialiser,
-                type(
-                    name,
-                    (GenericMapSerialiser,),
-                    {"key_type": ks_resolved, "value_type": vs_resolved},
-                ),
-            )
-        return cast(MapSerialiser[Enc_K, Enc_V], mcs._serialisers[name])
+        hashed_name = f"{resolver.name}{name}"
+        return cast(
+            typing.Type[EncodingProtocolVar],
+            type(
+                hashed_name,
+                (GenericMapSerialiser,),
+                {"key_type": ks_resolved, "value_type": vs_resolved},
+            ),
+        )
```

## diffusion/internal/serialisers/generic_model.py

```diff
@@ -1,87 +1,91 @@
-#  Copyright (c) 2022 Push Technology Ltd., All Rights Reserved.
+#  Copyright (c) 2022-2023 Push Technology Ltd., All Rights Reserved.
 #
 #  Use is subject to license terms.
 #
 #  NOTICE: All information contained herein is, and remains the
 #  property of Push Technology. The intellectual and technical
 #  concepts contained herein are proprietary to Push Technology and
 #  may be covered by U.S. and Foreign Patents, patents in process, and
 #  are protected by trade secret or copyright law.
 
 from __future__ import annotations
 
 import functools
+import inspect
 import io
 import typing
 
+import typing_extensions
+
 import stringcase
 
 import diffusion.datatypes
 from diffusion.handlers import LOG
-from diffusion.internal.utils import BaseConfig
+from diffusion.internal.utils import BaseConfig, decode
 
 if typing.TYPE_CHECKING:  # pragma: no cover
     from diffusion.internal.services.abstract import (
         ServiceValue,
     )
-    from diffusion.internal.serialisers.base import Serialiser
+    from diffusion.internal.serialisers.base import Serialiser, Resolver
     from .attrs import MarshalledModel as AttrsModel
     from .pydantic import MarshalledModel as PydanticModel
 
     Model_Variants = typing.Union[AttrsModel, PydanticModel]
     Model_Variants_T = typing.TypeVar("Model_Variants_T", bound=Model_Variants)
 
-from diffusion.internal.serialisers import T
-
 GenericModel_T = typing.TypeVar("GenericModel_T", bound="GenericModel")
 GenericModel_T_Other = typing.TypeVar("GenericModel_T_Other", bound="GenericModel")
 
 
-def model_variants() -> typing.Tuple[typing.Type[Model_Variants], ...]:
-    from .attrs import MarshalledModel as AttrsModel
-    from .pydantic import MarshalledModel as PydanticModel
-
-    return AttrsModel, PydanticModel
-
-
 class GenericConfig(
     typing.Generic[GenericModel_T],
     BaseConfig,
 ):
     """
     Adds Serialiser support to Model.Config
     'alias' defines the name of the serialiser to map to
     """
 
     alias: typing.ClassVar[str]
     allow_population_by_field_name = True
     alias_generator = stringcase.spinalcase
 
     @classmethod
-    def verify_item(cls, item, modelcls):
+    def verify_item(cls, item: ServiceValue, modelcls: typing.Type[GenericModel_T]):
         try:
             assert item._serialiser.name in cls.attr_mappings_all(modelcls)
         except Exception as e:  # pragma: no cover
             LOG.error(f"Got exception {e}")
             raise
 
     @classmethod
     @functools.lru_cache(maxsize=None)
-    def serialiser(cls, name=None) -> "Serialiser":
+    def serialiser(cls, name=None, resolver: Resolver = None) -> "Serialiser":
         from diffusion.internal.serialisers.base import Serialiser
 
         if not name:
-            assert isinstance(cls.alias, str)
-        return Serialiser.by_name(name or cls.alias)
+            if not isinstance(getattr(cls, "alias", None), str):
+                raise RuntimeError(f"{cls} has no 'alias'")
+        return Serialiser.by_name(name or cls.alias, resolver=resolver)
 
     @classmethod
-    def to_bytes(cls, item: GenericModel_T, serialiser=None) -> bytes:
+    def to_bytes(cls, item: GenericModel_T, serialiser: Serialiser = None) -> bytes:
+        serialiser = cls.check_serialiser(serialiser)
         as_tuple = cls.as_tuple(item, serialiser=serialiser)
-        return cls.serialiser(serialiser).to_bytes(*as_tuple)
+        return serialiser.to_bytes(*as_tuple)
+
+    @classmethod
+    def check_serialiser(cls, serialiser: typing.Optional[Serialiser]) -> Serialiser:
+        from diffusion.internal.serialisers.base import Serialiser
+        if serialiser is None:
+            return cls.serialiser()
+        assert isinstance(serialiser, Serialiser)
+        return serialiser
 
     @classmethod
     def from_service_value(
         cls,
         modelcls: typing.Type[GenericModel_T],
         item: ServiceValue,
     ) -> GenericModel_T:
@@ -92,15 +96,15 @@
             LOG.error(f"Got exception {e}")
             raise
 
     @classmethod
     def get_fields(cls, item, modelcls):
         cls.verify_item(item, modelcls)
         mapping = cls.get_model_to_serialiser_mapping(
-            modelcls, serialiser=item._serialiser.name
+            modelcls, serialiser=item._serialiser
         )
         fields = cls.gen_fields(
             item,
             mapping,
             modelcls,
         )
         try:
@@ -111,226 +115,273 @@
             raise
         return fields
 
     @classmethod
     def gen_fields(cls, item, model_to_serialiser_mapping, modelcls):
         try:
             result = {
-                model_key: modelcls.Config.decode(item[serialiser_key])
-                for model_key, serialiser_key in model_to_serialiser_mapping.items()
-                if serialiser_key
+                model_key: modelcls.Config.decode(
+                    item[serialiser.name],
+                    modelcls,
+                    model_key=model_key,
+                    serialiser=serialiser,
+                )
+                for model_key, serialiser in model_to_serialiser_mapping.items()
+                if serialiser
             }
             assert all(x is not None for x in result.keys())
             return result
         except Exception as e:  # pragma: no cover
             LOG.error(f"Got exception {e}")
             raise
 
     @classmethod
     def from_tuple(
         cls,
         modelcls: typing.Type[GenericModel_T],
         tp: typing.Tuple[typing.Any, ...],
-        serialiser=None,
+        serialiser: Serialiser = None
     ) -> GenericModel_T:
+        serialiser = cls.check_serialiser(serialiser)
         sv = cls.service_value(serialiser).evolve(*tp)
         result = cls.from_service_value(modelcls, sv)
         return result
 
     @classmethod
     def fields_from_tuple(
         cls,
         modelcls: typing.Type[GenericModel_T_Other],
         tp: typing.Tuple[typing.Any, ...],
-        serialiser=None,
+        serialiser: Serialiser = None,
     ) -> typing.Mapping[str, typing.Any]:
         sv = cls.service_value(serialiser).evolve(*tp)
         result = cls.get_fields(sv, modelcls)
         return result
 
     @classmethod
     def read(
         cls,
         modelcls: typing.Type[GenericModel_T],
         stream: io.BytesIO,
-        serialiser=None,
+        serialiser: Serialiser = None,
     ) -> GenericModel_T:
+        serialiser = cls.check_serialiser(serialiser)
         return cls.from_tuple(
-            modelcls, tuple(cls.serialiser(serialiser).read(stream)), serialiser
+            modelcls, tuple(serialiser.read(stream)), serialiser
         )
 
     @classmethod
     @functools.lru_cache(maxsize=None)
     def find_aliases(
-        cls, modelcls: typing.Type[GenericModel_T], serialiser: typing.Optional[str]
+        cls, modelcls: typing.Type[GenericModel_T], serialiser: Serialiser
     ) -> typing.Mapping[str, str]:
         return {}
 
     @classmethod
     @functools.lru_cache(maxsize=None)
     def get_model_to_serialiser_mapping(
-        cls, modelcls: typing.Type[Model_Variants], serialiser=None
-    ):
+        cls, modelcls: typing.Type[Model_Variants], serialiser: Serialiser = None
+    ) -> typing.Mapping[str, Serialiser]:
         try:
+            serialiser = cls.check_serialiser(serialiser)
             final_mapping = modelcls.Config.attr_mappings_final(
                 modelcls, serialiser=serialiser
             )
             result = {}
             for serialiser_key, model_key in final_mapping.items():
                 final_model_key = getattr(model_key, "__name__", model_key)
                 final_serialiser_key = cls.sanitize_key(serialiser_key, serialiser)
                 if not (final_serialiser_key and final_model_key):
                     continue
-                result.update({final_model_key: final_serialiser_key})
+                result.update(
+                    {
+                        final_model_key: cls.serialiser(
+                            final_serialiser_key, resolver=serialiser.resolver
+                        )
+                    }
+                )
 
             assert all(x is not None for x in result.keys())
             assert all(x is not None for x in result.values())
             return result
         except Exception as e:  # pragma: no cover
             raise e
 
     @classmethod
-    def sanitize_key(cls, name: str, serialiser=None):
+    def sanitize_key(cls, name: str, serialiser: Serialiser = None):
         sv = cls.service_value(serialiser)
         result = sv.sanitize_key(name)
         if result:
             return result
         if cls.alias_generator:
             result = sv.sanitize_key(cls.alias_generator(name))
         if not result:  # pragma: no cover
             LOG.error(f"Couldn't find {name} in {sv.spec}")
         return result
 
     @classmethod
-    @functools.lru_cache(maxsize=None)
-    def field_names(
-        cls, modelcls: typing.Type[GenericModel_T], serialiser=None
-    ) -> typing.List[str]:
-        raise NotImplementedError()  # pragma: no cover
-
-    @classmethod
     def get_service_value_args(cls, item: Model_Variants, serialiser=None):
         model_to_serialiser_mapping = cls.get_model_to_serialiser_mapping(
             type(item), serialiser=serialiser
         )
         try:
             mappings = {
-                v: cls.as_service_value_field(getattr(item, k), serialiser=v)
+                v.name: cls.as_service_value_field(getattr(item, k), serialiser=v)
                 for k, v in model_to_serialiser_mapping.items()
             }  # NOQA
         except Exception as e:  # pragma: no cover
             raise e
         return mappings
 
     @classmethod
-    def as_service_value_field(cls, item: GenericModel_T, serialiser: str = None):
+    def decode(
+        cls,
+        item,
+        modelcls: typing.Type[GenericModel_T],
+        model_key: str,
+        serialiser: Serialiser = None,
+    ):
+        return decode(item)
+
+    @classmethod
+    def get_field_type(cls, modelcls: typing.Type[Model_Variants], model_key: str):
+        result = typing_extensions.get_type_hints(modelcls).get(model_key)
+        return result
+
+    @classmethod
+    def decode_complex(
+        cls,
+        item,
+        modelcls: typing.Type[Model_Variants],
+        model_key: str,
+        serialiser: Serialiser,
+    ) -> typing.Optional[typing.List]:
+        from diffusion.internal.serialisers.base import ListEncoder
+
+        if len(serialiser.spec.values()) == 1:
+            sub_encoder = next(iter(serialiser.spec.values()), None)
+
+            if inspect.isclass(sub_encoder):
+                if issubclass(sub_encoder, ListEncoder):
+                    item_type = cls.get_field_type(modelcls, model_key).__args__[0]
+
+                    return sub_encoder.from_tuple(item, item_type)
+        return None
+
+    @classmethod
+    def as_service_value_field(cls, item: GenericModel_T, serialiser: Serialiser):
+        from diffusion.internal.serialisers.base import (
+            ListEncoder,
+            ChoiceEncoder,
+        )
+
+        sub_encoder = serialiser.get_encoder(ListEncoder, ChoiceEncoder)
+        if sub_encoder:
+            return sub_encoder.as_tuple(item)
+
         if isinstance(item, diffusion.datatypes.AbstractDataType):
             return item.encode(item.value)
-        elif isinstance(item, GenericModel):
+        if isinstance(item, GenericModel):
             return item.Config.as_tuple(item, serialiser)
         return item
 
     @classmethod
     def as_service_value(
         cls: typing.Type[GenericConfig[GenericModel_T]],
         item: GenericModel_T,
-        serialiser=None,
+        serialiser: Serialiser = None,
     ) -> ServiceValue:
         sv = cls.service_value(serialiser)
         mappings = cls.get_service_value_args(
             typing.cast("Model_Variants", item), serialiser=serialiser
         )
         try:
             return sv.evolve(**mappings)
         except Exception as e:  # pragma: no cover
             LOG.error(f"Caught exception {e}")
             raise
 
     @classmethod
     def as_tuple(
-        cls, item: GenericModel_T, serialiser=None
+        cls, item: GenericModel_T, serialiser: Serialiser = None
     ) -> typing.Tuple[typing.Any, ...]:
-        return tuple(cls.as_service_value(item, serialiser=serialiser).values())
-
-    @classmethod
-    @functools.lru_cache(maxsize=None)
-    def get_spec(cls, modelcls: typing.Type["Model_Variants"], serialiser=None):
-        rev_mapping = {
-            getattr(v, "__name__", v): k
-            for k, v in cls.attr_mappings_final(modelcls, serialiser).items()
-        }
-        spec = [
-            rev_mapping.get(
-                x,
-                rev_mapping.get(cls.alias_generator(x), x),
-            )
-            for x in cls.field_names(modelcls)
-        ]
-        return list(filter(bool, spec))
+        return tuple(item.Config.as_service_value(item, serialiser=serialiser).values())
 
     @classmethod
     @functools.lru_cache(maxsize=None)
     def attr_mappings_final(
-        cls, modelcls: typing.Type[Model_Variants], serialiser=None
+        cls, modelcls: typing.Type[Model_Variants], serialiser: Serialiser = None
     ) -> typing.Dict[str, typing.Any]:
         try:
-            attr_mapping = cls.attr_mappings_all(modelcls).get(serialiser or cls.alias)
+            serialiser = cls.check_serialiser(serialiser)
+            attr_mapping = cls.attr_mappings_all(modelcls).get(serialiser.name)
             result = {**(attr_mapping or {})}
             updates = cls.find_aliases(modelcls, serialiser)
             result.update({k: v for k, v in updates.items() if k and v})
             assert all([x for x in result.keys()])
             assert all([x for x in result.values()])
             return result
         except Exception as e:  # pragma: no cover
             raise e
 
     @classmethod
     @functools.lru_cache(maxsize=None)
-    def service_value(cls, serialiser=None):
+    def service_value(cls, serialiser: Serialiser = None):
         from diffusion.internal.services.abstract import ServiceValue
 
-        return ServiceValue(cls.serialiser(serialiser))
+        return ServiceValue(cls.check_serialiser(serialiser))
 
     @classmethod
     def attr_mappings_all(cls, modelcls):
-        return {cls.alias: modelcls.attr_mappings()}
+        return {cls.alias: {}}
+
+    @classmethod
+    def entry_from_list_of_choices_as_tuple(
+        cls, event: GenericModel, serialiser: Serialiser
+    ):
+        from diffusion.internal.serialisers.base import (
+            ListEncoder,
+            ChoiceEncoder,
+        )
+
+        choice_encoder = ChoiceEncoder.extract_from(
+            serialiser.to_encoder(ListEncoder).serialiser
+        )
+        return choice_encoder.as_tuple(event)
 
 
 class GenericModel(object):
     class Config(GenericConfig):
         pass
 
     def to_bytes(self) -> bytes:
         return self.Config.to_bytes(self)
 
     @classmethod
-    def from_fields(cls: typing.Type[T], **kwargs) -> T:
+    def from_fields(cls: typing.Type[GenericModel_T], **kwargs) -> GenericModel_T:
         # noinspection PyArgumentList
         try:
             return cls(**kwargs)
         except Exception as e:  # pragma: no cover
             LOG.error(f"Got exception {e}")
             raise
 
     @classmethod
-    def attr_mappings(cls) -> typing.Dict[str, typing.Any]:
-        return {}
-
-    @classmethod
     def from_service_value(
         cls: typing.Type[GenericModel_T], item: ServiceValue
     ) -> GenericModel_T:
         return cls.Config.from_service_value(cls, item)
 
     @classmethod
     def from_tuple(
         cls: typing.Type[GenericModel],
         tp: typing.Tuple[typing.Any, ...],
+        serialiser: Serialiser = None
     ):
-        result = cls.Config.from_tuple(cls, tp)
+        result = cls.Config.from_tuple(cls, tp, serialiser=serialiser)
         return result
 
 
 class GenericMetaModel(type):
     Config: typing.Type[GenericConfig]
 
     # noinspection PyAbstractClass
```

## diffusion/internal/serialisers/pydantic.py

```diff
@@ -10,41 +10,40 @@
 from __future__ import annotations
 
 import functools
 import typing
 
 import pydantic
 
+if typing.TYPE_CHECKING:
+    from diffusion.internal.serialisers import Serialiser
+
 from diffusion.internal.serialisers.generic_model import GenericConfig, GenericModel
 MarshalledModel_T = typing.TypeVar("MarshalledModel_T", bound="MarshalledModel")
 
 
 class MarshalledModel(pydantic.BaseModel, GenericModel):
     class Config(GenericConfig["MarshalledModel_T"]):
         allow_population_by_field_name = True
 
         @classmethod
         @functools.lru_cache(maxsize=None)
-        def field_names(
-            cls, modelcls: typing.Type[MarshalledModel_T], serialiser=None
-        ) -> typing.List[str]:
-            return list(v.alias for v in modelcls.__fields__.values())
-
-        @classmethod
-        @functools.lru_cache(maxsize=None)
         def find_aliases(
             cls, modelcls: typing.Type[MarshalledModel_T], serialiser: typing.Optional[str]
         ) -> typing.Mapping[str, str]:
             return {
                 cls.lookup_alias(modelcls, key, serialiser): key
                 for key, field in modelcls.__fields__.items()
             }
 
         @classmethod
         @functools.lru_cache(maxsize=None)
         def lookup_alias(
-            cls, modelcls: typing.Type[MarshalledModel_T], name: str, serialiser=None
+            cls,
+            modelcls: typing.Type[MarshalledModel_T],
+            name: str,
+            serialiser: Serialiser = None,
         ):
             field = modelcls.__fields__.get(name, None)
             if field and field.has_alias and field.alias:
                 return field.alias
             return None
```

## diffusion/internal/serialisers/spec.py

```diff
@@ -1,26 +1,30 @@
+#  Copyright (c) 2020-2023 Push Technology Ltd., All Rights Reserved.
+#
+#  Use is subject to license terms.
+#
+#  NOTICE: All information contained herein is, and remains the
+#  property of Push Technology. The intellectual and technical
+#  concepts contained herein are proprietary to Push Technology and
+#  may be covered by U.S. and Foreign Patents, patents in process, and
+#  are protected by trade secret or copyright law.
+
 """ Specifications for serialisers, based on `spec.clj`. """
 
 from __future__ import annotations
 
 import typing
 from enum import Enum
-from typing import Iterator, MutableMapping, Optional, Sequence, Type, Union
+from typing import Iterator, Optional, Sequence, Type, Union, Mapping, MutableMapping
 
 try:
-    from typing_extensions import Final, TypedDict  # type: ignore  # pragma: no cover
+    from typing_extensions import Final  # type: ignore  # pragma: no cover
 except ImportError:
-    from typing import Final, TypedDict  # type: ignore  # pragma: no cover
+    from typing import Final  # type: ignore  # pragma: no cover
 
-from diffusion.datatypes.timeseries import EventMetadata
-from diffusion.internal.serialisers.timeseries import (
-    TimeSeriesAppendRequest,
-    TimeSeriesTimestampAppendRequest,
-    TimeSeriesEditRequest,
-)
 import structlog
 
 from diffusion.internal.encoded_data import (
     Byte,
     Bytes,
     EncodingProtocol,
     Int32,
@@ -30,15 +34,16 @@
 import diffusion.internal.encoded_data as encoded_data
 
 LOG = structlog.get_logger()
 
 EncodingClass = Type[EncodingProtocol]
 SerialiserChain = Sequence[Optional[EncodingClass]]
 SerialiserMapValue = Union[EncodingClass, SerialiserChain]
-SerialiserMap = MutableMapping[str, SerialiserMapValue]
+SerialiserMap = Mapping[str, SerialiserMapValue]
+MutableSerialiserMap = MutableMapping[str, SerialiserMapValue]
 SerialiserOutput = Iterator[Optional[Type[EncodingProtocol]]]
 
 NULL_VALUE_KEY = "void"
 ENCODING_TYPE_KEYS = {
     NULL_VALUE_KEY: [],
     "BYTE": Byte,
     "BYTES": Bytes,
@@ -78,53 +83,125 @@
         return f"Compound.{self._name_}"
 
 
 SpecItem = Union[str, CompoundSpec]
 SerialiserSpecItem = Optional[Union[EncodingClass, Sequence[SpecItem], SerialiserChain]]
 
 
-SPECS: Final = {
+SERIALISER_SPECS: Final = {
     "add-and-set-topic-request": (
         "topic-path",
         "protocol14-topic-specification",
         "bytes",
         "update-constraint",
     ),
+    "add-serialised": ("generation-id", "update-id", "serialised-object"),
+    "add-topic-persistence-record": (
+        "persistence-origin",
+        "persistence-topic-key",
+        "persistence-specification-key",
+        "path",
+    ),
     "add-topic-result": encoded_data.Byte,
+    "anonymous-connection-action": encoded_data.Byte,
+    "append-record": ("generation-id", "update-id", "persistence-record"),
+    "append-record-pair": (
+        "generation-id",
+        "update-id",
+        "persistence-record",
+        "persistence-record",
+    ),
+    "append-records": (
+        "generation-id",
+        "update-id",
+        Compound.N_OF("persistence-record"),
+    ),
+    "append-result": encoded_data.Byte,
+    "apply-json-patch-request": ("string", "string", "update-constraint"),
+    "apply-selection-event": "topic-selection-event",
+    "authenticated-principal": (encoded_data.String, "role-set"),
     "authenticator-registration-parameters": (
         "service-id",
         "control-group",
         "handler-name",
     ),
+    "authenticator-registration-request": (
+        "authenticator-registration-parameters",
+        "conversation-id",
+    ),
+    "authenticator-request": (
+        "principal",
+        "credentials",
+        "session-properties",
+        "session-properties",
+        "conversation-id",
+    ),
+    "authenticator-response": Compound.ONE_OF(
+        {0: (), 1: (), 2: ("session-properties",)}
+    ),
+    "backup-claim-partition": encoded_data.Int32,
     "backup-claim-session-lock": "cluster-lock-allocation",
-    "binary-value-constraint": encoded_data.Bytes,
+    "binary-value-constraint": "bytes",
     "boolean": encoded_data.Byte,
     "branch-mapping": ("session-filter", "path"),
     "branch-mapping-table": ("path", Compound.N_OF("branch-mapping")),
     "byte": encoded_data.Byte,
     "bytes": encoded_data.Bytes,
+    "change-authorisation-roles-filter-request": (
+        "session-filter",
+        "role-set",
+        "role-set",
+    ),
+    "change-authorisation-roles-filter-result": "count-or-parser-errors",
+    "change-authorisation-roles-request": ("session-id", "role-set", "role-set"),
     "change-principal-request": ("principal", "credentials"),
+    "check-remote-server-result": (
+        "remote-server-connection-state",
+        encoded_data.String,
+    ),
+    "claim-partition": (encoded_data.String, encoded_data.Int32),
+    "claim-partition-result": (encoded_data.Int32, "file-restore-complete"),
+    "claim-session-lock": ("session-lock-name", "session-lock-owner"),
+    "client-info": ("session-token", "connection-info", "session-properties"),
+    "client-type": encoded_data.Byte,
+    "close-client-request": "protocol5-close-client-request",
+    "close-reason": encoded_data.Byte,
     "cluster-lock-allocation": (
         "server-uuid",
         "session-lock-owner",
         "session-lock-sequence",
     ),
+    "command-header": ("service-id", encoded_data.Byte, "conversation-id"),
     "conjunction-constraint": Compound.N_OF(
         Compound.ONE_OF(
             {
                 0: ("unconstrained-constraint",),
                 2: ("binary-value-constraint",),
                 3: ("no-value-constraint",),
                 4: ("locked-constraint",),
                 5: ("no-topic-constraint",),
             }
         )
     ),
+    "connection-capabilities": encoded_data.Byte,
+    "connection-info": (
+        "protocol-version",
+        encoded_data.Int32,
+        "connection-capabilities",
+        encoded_data.Int32,
+    ),
+    "content": ("encoding", encoded_data.Bytes),
     "control-group": encoded_data.String,
+    "control-registration-parameters": ("service-id", "control-group"),
+    "control-registration-request-impl": (
+        "control-registration-parameters",
+        "conversation-id",
+    ),
     "conversation-id": encoded_data.Int64,
+    "count-or-parser-errors": (encoded_data.Int32, "error-report-list"),
     "count-or-parser-errors2": Compound.ONE_OF(
         {0: (encoded_data.Int32,), 1: ("error-report",)}
     ),
     "create-topic-view-result": Compound.ONE_OF(
         {
             0: ("topic-view",),
             1: ("error-report",),
@@ -297,14 +374,15 @@
     "generation-id": encoded_data.Int32,
     "get-session-properties-request": ("session-id", "session-property-keys"),
     "get-session-properties-result": {0: (), 1: "session-properties"},
     "get-topic-view-result": {0: (), 1: "topic-view"},
     "global-handler-backup-processor": Compound.SET_OF(encoded_data.String),
     "group-by-path-prefix-parts": encoded_data.Int32,
     "groups-by-topic-type": "boolean",
+    "groups-by-topic-view": "boolean",
     "handler-name": encoded_data.String,
     "hazelcast-address": (Compound.N_OF(encoded_data.Byte), "port"),
     "i-bytes": encoded_data.Bytes,
     "integer": encoded_data.Int32,
     "internal-session-id": "session-id",
     "is-session-lock-for-unknown-server": (),
     "json-pointer": encoded_data.String,
@@ -370,14 +448,17 @@
     "mqtt-publish-request": ("mqtt-topic-name", "mqtt-payload-format", "mqtt-payload"),
     "mqtt-session-notification": ("internal-session-id", "mqtt-client-id", "principal"),
     "mqtt-session-takeover-result": Compound.N_OF("internal-session-id"),
     "mqtt-topic-name": encoded_data.String,
     "named-topic-view-specification": ("topic-view-name", "topic-view-specification"),
     "no-topic-constraint": (),
     "no-value-constraint": (),
+    "null-count-or-parser-errors": [],
+    "null-integer": [],
+    "owned-topic-removal-result": ("integer", "integer"),
     "partial-json-constraint-with": Compound.MAP_OF("json-pointer", encoded_data.Bytes),
     "partial-json-constraint-without": Compound.SET_OF("json-pointer"),
     "partial-json-constraint": (
         "partial-json-constraint-with",
         "partial-json-constraint-without",
     ),
     "partition-event": (encoded_data.Byte, "partition-generation"),
@@ -703,19 +784,19 @@
         "gateway-service-type-name",
         "gateway-service-type-description",
         "gateway-service-type-schema",
         "boolean",
     ),
     "protocol24-topic-metric-collector": (
         "metric-collector-name",
-        "boolean",
+        "exports-to-prometheus",
         "maximum-groups",
         "topic-selector",
-        "boolean",
-        encoded_data.Int32,
+        "groups-by-topic-type",
+        "group-by-path-prefix-parts"
     ),
     "protocol24-topic-metric-collectors": Compound.N_OF(
         "protocol24-topic-metric-collector"
     ),
     "protocol25-create-remote-server-result": Compound.ONE_OF(
         {
             0: ("protocol25-remote-server",),
@@ -730,26 +811,14 @@
         Compound.N_OF("remote-server-url"),
         "principal",
         "remote-server-connection-options",
         "topic-selector",
         "remote-server-connector",
     ),
     "protocol25-remote-server-definition": ("protocol25-remote-server", "credentials"),
-    "protocol26-topic-metric-collector": (
-        "metric-collector-name",
-        "boolean",
-        "maximum-groups",
-        "topic-selector",
-        "boolean",
-        "boolean",
-        encoded_data.Int32,
-    ),
-    "protocol26-topic-metric-collectors": Compound.N_OF(
-        "protocol26-topic-metric-collector"
-    ),
     "protocol4-system-authentication-configuration": (
         Compound.N_OF("protocol4-system-principal"),
         "anonymous-connection-action",
         "role-set",
     ),
     "protocol4-system-principal": ("string", "role-set"),
     "protocol5-close-client-request": ("session-id", encoded_data.String),
@@ -772,19 +841,19 @@
         {
             0: ("range-query-original-event",),
             1: ("range-query-edit-event",),
             2: ("range-query-metadata-offsets",),
             3: ("range-query-author-encoding",),
         }
     ),
-    "range-query-metadata-offsets": ("sequence", "timestamp"),
+    "range-query-metadata-offsets": ("time-series-sequence", "timestamp"),
     "author-code": "bytes",
     "range-query-author-encoding": ("author-code", "author"),
     "rq-time-series-event-metadata": (
-        "sequence",
+        "time-series-sequence",
         "timestamp",
         "author-code",
     ),
     "range-query-original-event": ("rq-time-series-event-metadata", "value"),
     "edit-event": (
         "time-series-event-metadata",
         "original-event",
@@ -828,14 +897,15 @@
     "routing-subscription-control-request": (
         "conversation-id",
         "conversation-id",
         "session-id",
         encoded_data.String,
     ),
     "routing-subscription-response": ("conversation-id", encoded_data.String),
+    "secondary-acceptor-registration": (encoded_data.String, encoded_data.String),
     "security-command-script": encoded_data.String,
     "security-command-script-result": "error-report-list",
     "serialised-key": ("serialised-key-type", encoded_data.String),
     "serialised-key-type": encoded_data.Byte,
     "serialised-object": ("serialised-key", encoded_data.String, "bytes"),
     "serialised-objects": Compound.N_OF("serialised-object"),
     "serialised-value": ("data-type-name", "bytes"),
@@ -898,15 +968,15 @@
         "exports-to-prometheus",
         "maximum-groups",
         "removes-metrics-with-no-matches",
         "session-filter",
         "session-property-keys",
     ),
     "session-metric-collectors": Compound.N_OF("session-metric-collector"),
-    "session-properties": Compound.SET_OF(encoded_data.String),
+    "session-properties": Compound.MAP_OF(encoded_data.String, encoded_data.String),
     "session-properties-change": (
         encoded_data.String,
         Compound.ONE_OF(
             {
                 1: (encoded_data.String,),
                 2: (encoded_data.String, encoded_data.String),
                 3: (encoded_data.String,),
@@ -953,35 +1023,50 @@
     "set-topic-request": (
         "topic-path",
         "protocol14-topic-type",
         "bytes",
         "update-constraint",
     ),
     "string": encoded_data.String,
+    "string-set-hierarchy-index-wrapper": Compound.MAP_OF(
+        encoded_data.String, Compound.SET_OF(encoded_data.String)
+    ),
+    "subscription-request": ("session-id", "topic-selector"),
+    "throttler-type": encoded_data.Byte,
+    "throttling-limit": encoded_data.Int32,
     "time-millis": encoded_data.Int64,
+    "time-series-append-request": ("path", "data-type-name", "value"),
     "time-series-edit-request": (
         "path",
         "data-type-name",
-        "sequence",
-        "bytes",
+        "time-series-sequence",
+        "value",
+    ),
+    "time-series-event-metadata": (
+        "time-series-sequence",
+        "timestamp",
+        "author"
     ),
     "timestamp": encoded_data.Int64,
     "author": encoded_data.String,
-    "sequence": encoded_data.Int64,
+    "time-series-sequence": encoded_data.Int64,
+    "time-series-timestamp-append-request": (
+        "time-series-append-request",
+        "timestamp"
+    ),
+    "time-series-update-response": "time-series-event-metadata",
+    "topic-control-registration-parameters": ("service-id", "control-group", "path"),
+    "topic-control-registration-request": (
+        "topic-control-registration-parameters",
+        "conversation-id",
+    ),
+    "topic-descendant-event": ("conversation-id", "path", encoded_data.Byte),
     "topic-id": encoded_data.Int32,
+    "topic-notification-selection": ("conversation-id", "topic-selector"),
     "topic-path": encoded_data.String,
-    "topic-metric-collector": (
-        "metric-collector-name",
-        "exports-to-prometheus",
-        "maximum-groups",
-        "topic-selector",
-        "groups-by-topic-type",
-        "group-by-path-prefix-parts",
-    ),
-    "topic-metric-collectors": Compound.N_OF("topic-metric-collector"),
     "topic-properties": Compound.MAP_OF("topic-property-key", encoded_data.String),
     "topic-property-key": encoded_data.String,
     "topic-removal-cluster-state-request": "path",
     "topic-removal-criteria-satisfied": "boolean",
     "topic-removal-state-change-event": (
         "topic-id",
         "topic-removal-criteria-satisfied",
@@ -1045,27 +1130,7 @@
         encoded_data.Byte,
         encoded_data.Bytes,
     ),
     "update-type": encoded_data.Byte,
     "value": encoded_data.Bytes,
     "void": None,
 }
-
-TypedSpecs = TypedDict(
-    "TypedSpecs",
-    {
-        "time-series-append-request": TimeSeriesAppendRequest,
-        "time-series-event-metadata": EventMetadata,
-        "time-series-timestamp-append-request": TimeSeriesTimestampAppendRequest,
-        "time-series-update-response": EventMetadata,
-        "time-series-edit-request": TimeSeriesEditRequest,
-    },
-    total=False,
-)
-
-
-def get_specs() -> typing.Dict[str, typing.Any]:
-    TypedSpecs.__annotations__.update(**SPECS)
-    return TypedSpecs.__annotations__
-
-
-SERIALISER_SPECS = get_specs()
```

## diffusion/internal/serialisers/timeseries.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright (c) 2022 Push Technology Ltd., All Rights Reserved.
+#  Copyright (c) 2022-2023 Push Technology Ltd., All Rights Reserved.
 #
 #  Use is subject to license terms.
 #
 #  NOTICE: All information contained herein is, and remains the
 #  property of Push Technology. The intellectual and technical
 #  concepts contained herein are proprietary to Push Technology and
 #  may be covered by U.S. and Foreign Patents, patents in process, and
@@ -50,24 +50,43 @@
         field,
         config,
     ) -> bytes:
         return bytes(field_value)
 
     class Config(MarshalledModel.Config):
         alias = "time-series-append-request"
+        allow_population_by_field_name = True
 
+        @classmethod
+        def attr_mappings_all(cls, modelcls):
+            return {
+                "time-series-append-request": {
+                    "time-series-append-request.path": "topic_path",
+                    "time-series-append-request.data-type-name": "value_type",
+                    "time-series-append-request.value": "value",
+                }
+            }
 
-class TimeSeriesTimestampAppendRequest(
-    TimeSeriesAppendRequest
-):
+
+class TimeSeriesTimestampAppendRequest(TimeSeriesAppendRequest):
     timestamp: int
 
     class Config(MarshalledModel.Config):
         alias = "time-series-timestamp-append-request"
 
+        @classmethod
+        def attr_mappings_all(cls, modelcls):
+            return {
+                "time-series-timestamp-append-request": {
+                    "time-series-append-request.path": "topic_path",
+                    "time-series-append-request.data-type-name": "value_type",
+                    "time-series-append-request.value": "value",
+                }
+            }
+
 
 class TimeSeriesEditRequest(MarshalledModel):
     """
     The time series edit request.
     Added in version 6.8.3
     """
 
@@ -94,21 +113,21 @@
     def type(self):
         return diffusion.datatypes.get(self.value_type)
 
     """
     The corresponding data type name of the value type.
     """
     original_sequence: int = pydantic.Field(
-        alias="sequence"
+        alias="time-series-sequence"
     )
     """
     The original sequence number.
     """
 
-    value: bytes = pydantic.Field(alias="bytes")
+    value: bytes = pydantic.Field(alias="value")
     """
     The value in serialised form.
     """
     # noinspection PyUnusedLocal,PyNestedDecorators
     @pydantic.validator("value", pre=True)
     @classmethod
     def validate_value(
```

## diffusion/internal/services/abstract.py

```diff
@@ -26,15 +26,14 @@
 from .exceptions import UnknownServiceError
 from diffusion.internal.protocol.exceptions import (
     ReportsError
 )
 # noinspection DuplicatedCode
 from ..serialisers.generic_model import GenericModel, GenericModel_T
 from ..serialisers.spec import (
-    SERIALISER_SPECS,
     NULL_VALUE_KEY,
 )
 
 if TYPE_CHECKING:  # pragma: no cover
     from diffusion.internal.session import InternalSession
     from diffusion.internal.protocol.message_types import (
         ServiceMessage,
@@ -135,17 +134,15 @@
             or self.response_serialiser.name
             == NULL_VALUE_KEY
         ):
             return response
         if not response_type:
             response_type = typing.cast(
                 typing.Type[GenericModel_T],
-                SERIALISER_SPECS.get(
-                    self.response_serialiser.name
-                ),
+                self.response_serialiser
             )
 
         if response_type:
             if inspect.isclass(
                 response_type
             ) and issubclass(response_type, GenericModel):
                 response_type_real = typing.cast(
@@ -175,41 +172,27 @@
             item = copy.copy(self)
         except Exception as e:  # pragma: no cover
             LOG.error(f"Got exception {e}")
             raise
         if request:
             if isinstance(request, GenericModel):
                 item.request = request.Config.as_service_value(
-                    request, serialiser=self.request_serialiser.name
+                    request, serialiser=self.request_serialiser
                 )
             else:
                 item.request = request
         if response:
             if isinstance(response, GenericModel):
                 item.response = response.Config.as_service_value(
-                    response, serialiser=self.response_serialiser.name
+                    response, serialiser=self.response_serialiser
                 )
             else:
                 item.response = response
         return item
 
-    async def __call__(
-        self, session: InternalSession, *args, **kwargs
-    ):
-        try:
-            request_type = SERIALISER_SPECS[
-                self.request_serialiser.name
-            ]
-            return await self.invoke(
-                session, request_type(*args, **kwargs)
-            )
-        except Exception as e:  # pragma: no cover
-            LOG.error(f"Got exception {e}")
-            raise
-
     @classmethod
     def __get_validators__(cls: typing.Type[Service]):
         def validate(val) -> Service:
             if isinstance(val, Service):
                 return val
             raise TypeError(f"{val} is not a {cls}")
         yield validate
```

## diffusion/internal/topics/__init__.py

```diff
@@ -191,18 +191,20 @@
 
     @classmethod
     def from_fields(cls: typing.Type[T], **kwargs) -> T:
         tp: typing.Type[AbstractDataType] = diffusion.datatypes.get(kwargs.pop("topic_type"))
         properties: dict = kwargs.pop("properties", {})
         return cls(kwargs.pop("path"), spec=tp.with_properties(**properties), **kwargs)
 
-    @classmethod
-    def attr_mappings(cls) -> typing.Dict[str, typing.Any]:
-        return {
-            "protocol14-topic-specification.protocol14-topic-type": "topic_type",
-            "protocol14-topic-specification.topic-properties": "properties",
-            "topic-path": cls.path,
-            "protocol14-topic-specification-info.topic-id": cls.id,
-        }
-
     class Config(MarshalledModel.Config):
         alias = "protocol14-topic-specification-info"
+
+        @classmethod
+        def attr_mappings_all(cls, modelcls: typing.Type[Topic]):
+            return {
+                "protocol14-topic-specification-info": {
+                    "protocol14-topic-specification.protocol14-topic-type": "topic_type",
+                    "protocol14-topic-specification.topic-properties": "properties",
+                    "topic-path": modelcls.path,
+                    "protocol14-topic-specification-info.topic-id": modelcls.id,
+                }
+            }
```

## diffusion/session/__init__.py

```diff
@@ -65,26 +65,32 @@
         url: WebSockets URL of the Diffusion server to connect to.
         principal: The name of the security principal associated with the session.
         credentials: Security information required to authenticate the connection.
 
     The recommended method is to instantiate this class as an async context manager.
     Here is a minimal example:
 
-        async with diffusion.Session("ws://diffusion.server:8080") as session:
-            # do some work with the session
+    ```pycon
+    >>> async with diffusion.Session("ws://diffusion.server:8080") as session:
+    ...     # do some work with the session
+    ...     pass
+    ```
 
     The context manager will make sure that the connection is properly closed at
     the end of the program. Alternatively, it is possible to open the connection
     explicitly, which can be useful if the session needs to be passed around, in
     this case the connection needs to be explicitly closed as well:
 
-        session = diffusion.Session("ws://diffusion.server:8080")
-        await session.connect()
-        # do some work with the session
-        await session.close()
+    ```pycon
+    >>> session = diffusion.Session("ws://diffusion.server:8080")
+    >>> await session.connect()
+    >>> # do some work with the session
+    >>> await session.close()
+
+    ```
     """
 
     def __init__(
         self,
         url: str,
         principal: str = None,
         credentials: Optional[Credentials] = None,
```

## diffusion/session/locks/session_lock_acquisition.py

```diff
@@ -1,21 +1,18 @@
-#   Copyright (c) 2022 Push Technology Ltd., All Rights Reserved.
+#   Copyright (c) 2023 Push Technology Ltd., All Rights Reserved.
 #
 #   Use is subject to license terms.
 #
 #  NOTICE: All information contained herein is, and remains the
 #  property of Push Technology. The intellectual and technical
 #  concepts contained herein are proprietary to Push Technology and
 #  may be covered by U.S. and Foreign Patents, patents in process, and
 #  are protected by trade secret or copyright law.
-
 import enum
 
-from diffusion.internal.serialisers.pydantic import MarshalledModel
-
 
 class SessionLockScope(enum.IntEnum):
     """
     Values for the `scope` parameter of
     [Session.lock][diffusion.session.Session.lock]
 
     Since:
@@ -31,51 +28,7 @@
     UNLOCK_ON_CONNECTION_LOSS = 1
     """
     The lock will be released when the acquiring session is closed.
     """
 
     def __str__(self):
         return self.name
-
-
-class Bool(MarshalledModel):
-    value: bool
-
-    def __bool__(self):
-        return self.value
-
-    class Config(MarshalledModel.Config):
-        alias_generator = None
-
-        @classmethod
-        def attr_mappings_all(cls, modelcls):
-            return {"boolean": {"boolean": "value"}}
-
-
-class SessionLockAcquisition(MarshalledModel):
-    """
-    The successful response of a
-    [SessionLockRequest][diffusion.session.locks.session_lock_request.SessionLockRequest]
-    """
-
-    lock_name: str
-    sequence: int
-    scope: SessionLockScope
-
-    class Config(MarshalledModel.Config):
-        frozen = True
-        alias_generator = None
-
-        @classmethod
-        def attr_mappings_all(cls, modelcls):
-            return {
-                "session-lock-acquisition": {
-                    "session-lock-name": "lock_name",
-                    "session-lock-sequence": "sequence",
-                    "session-lock-scope": "scope",
-                }
-            }
-
-    def __str__(self):
-        return (
-            f"""SessionLockAcquisition[{self.lock_name}, {self.sequence}, {self.scope}"""
-        )
```

## diffusion/session/locks/session_locks.py

```diff
@@ -9,31 +9,189 @@
 import pydantic
 
 from diffusion.handlers import LOG
 from diffusion.internal.protocol.conversations import ResponseHandler, ConversationID
 from diffusion.internal.services import ServiceValue
 from diffusion.internal.utils import validate_member_arguments, BaseConfig
 from diffusion.internal.validation import StrictNonNegativeInt
-from diffusion.session.locks.session_lock_acquisition import (
+from diffusion.internal.session.locks.session_lock_acquisition import (
     SessionLockAcquisition,
     SessionLockScope,
-    Bool,
 )
-from diffusion.session.locks.session_lock_request import SessionLockRequest
-from diffusion.session.locks.session_lock_request_cancellation import (
+from diffusion.internal.serialisers.primitives import Bool
+from diffusion.internal.session.locks.session_lock_request import SessionLockRequest
+from diffusion.internal.session.locks.session_lock_request_cancellation import (
     SessionLockRequestCancellation,
 )
 
 if typing.TYPE_CHECKING:
     from diffusion.internal.session import InternalSession, State
 
 
 T = typing.TypeVar("T")
 
 
+@pydantic.dataclasses.dataclass(frozen=True, config=BaseConfig)
+class SessionLock(object):
+    """
+    A [Session][diffusion.session.Session] lock.
+
+    Notes:
+        A session lock is a server-managed resource
+        that can be used to coordinate exclusive access
+        to shared resources across sessions.
+        For example,
+        to ensure a single session has the right to update a topic;
+        to ensure at most one session responds to an event;
+        or to select a single session to perform a housekeeping task.
+        Session locks support general collaborative locking schemes.
+        The application architect is responsible for
+        designing a suitable locking scheme
+        and for ensuring each application component
+        follows the scheme appropriately.
+
+        Session locks are identified by a lock name.
+        Lock names are arbitrary
+        and chosen at will to suit the application.
+        Each lock is owned by at most one session.
+        Locks are established on demand;
+        there is no separate operation to create or destroy a lock.
+
+        A session lock is acquired using the
+        [Session.lock][diffusion.session.Session.lock] method.
+        If no other session owns the lock,
+        the server will assign the lock to the calling session immediately.
+        Otherwise,
+        the server will record that the session is waiting to acquire the lock.
+        A session can call
+        [Session.lock][diffusion.session.Session.lock]
+        more than once for a given session lock
+        – if the lock is acquired,
+        all calls will complete successfully with equal
+        [SessionLock][diffusion.session.locks.session_locks.SessionLock] values.
+
+        If a session closes,
+        the session locks it owns are automatically released.
+        A session can also release a lock by calling
+        [SessionLock.unlock][diffusion.session.locks.session_locks.SessionLock.unlock].
+        When a session lock is released
+        and other sessions are waiting to acquire the lock,
+        the server will arbitrarily select one of the waiting sessions
+        and notify it that it has acquired the lock.
+        All of the newly selected session's pending
+        [Session.lock][diffusion.session.Session.lock]
+        calls will complete normally.
+        Other sessions will continue to wait.
+
+        The [Session.lock][diffusion.session.Session.lock]
+        variant of this method takes a scope parameter
+        that provides the further option of automatically releasing the lock
+        when the session loses its connection to the server.
+
+        # Race conditions
+
+        This session lock API has inherent race conditions.
+        Even if an application is coded correctly
+        to protect a shared resource using session locks,
+        there may be a period where two
+        or more sessions concurrently access the resource.
+        The races arise for several reasons including
+
+        - Due to the <i>check-then-act</i>
+        approach of polling <see cref="IsOwned"/>,
+        the lock can be lost after the check has succeeded
+        but before the resource is accessed;
+
+        - The server can detect a session is disconnected
+        and assign the lock to another session
+        before the original session has detected the disconnection.
+
+        Despite this imprecision,
+        session locks provide a useful way to coordinate session actions.
+
+        > NOTE
+        > This interface does not require user implementation
+        > and is only used to hide implementation details.
+
+        Since:
+            6.10
+    """
+
+    acquisition: SessionLockAcquisition
+    parent: typing.Optional[weakref.ReferenceType] = dataclasses.field(default=None)
+    owned: bool = pydantic.dataclasses.Field(init=False)
+    lock: asyncio.Lock = pydantic.dataclasses.Field(init=False)
+
+    @property
+    def name(self: SessionLock) -> pydantic.StrictStr:
+        return self.acquisition.lock_name
+
+    @property
+    def sequence(self: SessionLock) -> StrictNonNegativeInt:
+        return self.acquisition.sequence
+
+    @property
+    def is_owned(self: SessionLock) -> bool:
+        return self.owned
+
+    @property
+    def scope(self: SessionLock) -> SessionLockScope:
+        return self.acquisition.scope
+
+    def __init__(
+            self: SessionLock,
+            parent: typing.Union[InternalSession, SessionLocks],
+            acquisition: SessionLockAcquisition,
+    ):
+        from diffusion.internal.session import InternalSession
+
+        super().__init__()
+        if isinstance(parent, (InternalSession, SessionLocks)):
+            object.__setattr__(self, "parent", weakref.ref(parent))
+            object.__setattr__(self, "owned", True)
+        else:
+            object.__setattr__(self, "owned", False)
+        object.__setattr__(self, "lock", asyncio.Lock())
+        object.__setattr__(self, "acquisition", acquisition)
+
+    async def unlock(self: SessionLock) -> bool:
+        """
+        Releases this session lock if it is owned by the session.
+
+        Since:
+            6.10.
+
+        Returns:
+            `True` if unlocking is successful, `False` if not
+
+        """
+        async with self.lock:
+            if self.owned:
+                object.__setattr__(self, "owned", False)
+                target = typing.cast(
+                    SessionLocks, typing.cast(weakref.ReferenceType, self.parent)()
+                )
+                return await target.unlock(self)
+
+        return False
+
+    async def set_released(self: SessionLock):
+        """
+        Marks this lock as released.
+        """
+        async with self.lock:
+            object.__setattr__(self, "owned", False)
+
+    def __str__(self):
+        return (
+            f"{type(self).__name__}[Name={self.name}, Sequence={self.sequence},"
+            f" Scope={self.scope.name}, Owned={self.is_owned}]"
+        )
+
+
 class SessionLocks(object):
 
     failover_detection_id: typing.Optional[ConversationID]
 
     async def on_session_event(
         self: SessionLocks,
         *,
@@ -241,165 +399,7 @@
             )
         finally:
             async with self.locker:
                 current_lock = self.locks.get(session_lock.name)
                 if current_lock == session_lock:
                     del self.locks[session_lock.name]
         return result
-
-
-@pydantic.dataclasses.dataclass(frozen=True, config=BaseConfig)
-class SessionLock(object):
-    """
-    A [Session][diffusion.session.Session] lock.
-
-    Notes:
-        A session lock is a server-managed resource
-        that can be used to coordinate exclusive access
-        to shared resources across sessions.
-        For example,
-        to ensure a single session has the right to update a topic;
-        to ensure at most one session responds to an event;
-        or to select a single session to perform a housekeeping task.
-        Session locks support general collaborative locking schemes.
-        The application architect is responsible for
-        designing a suitable locking scheme
-        and for ensuring each application component
-        follows the scheme appropriately.
-
-        Session locks are identified by a lock name.
-        Lock names are arbitrary
-        and chosen at will to suit the application.
-        Each lock is owned by at most one session.
-        Locks are established on demand;
-        there is no separate operation to create or destroy a lock.
-
-        A session lock is acquired using the
-        [Session.lock][diffusion.session.Session.lock] method.
-        If no other session owns the lock,
-        the server will assign the lock to the calling session immediately.
-        Otherwise,
-        the server will record that the session is waiting to acquire the lock.
-        A session can call
-        [Session.lock][diffusion.session.Session.lock]
-        more than once for a given session lock
-        – if the lock is acquired,
-        all calls will complete successfully with equal
-        [SessionLock][diffusion.session.locks.session_locks.SessionLock] values.
-
-        If a session closes,
-        the session locks it owns are automatically released.
-        A session can also release a lock by calling
-        [SessionLock.unlock][diffusion.session.locks.session_locks.SessionLock.unlock].
-        When a session lock is released
-        and other sessions are waiting to acquire the lock,
-        the server will arbitrarily select one of the waiting sessions
-        and notify it that it has acquired the lock.
-        All of the newly selected session's pending
-        [Session.lock][diffusion.session.Session.lock]
-        calls will complete normally.
-        Other sessions will continue to wait.
-
-        The [Session.lock][diffusion.session.Session.lock]
-        variant of this method takes a scope parameter
-        that provides the further option of automatically releasing the lock
-        when the session loses its connection to the server.
-
-        # Race conditions
-
-        This session lock API has inherent race conditions.
-        Even if an application is coded correctly
-        to protect a shared resource using session locks,
-        there may be a period where two
-        or more sessions concurrently access the resource.
-        The races arise for several reasons including
-
-        - Due to the <i>check-then-act</i>
-        approach of polling <see cref="IsOwned"/>,
-        the lock can be lost after the check has succeeded
-        but before the resource is accessed;
-
-        - The server can detect a session is disconnected
-        and assign the lock to another session
-        before the original session has detected the disconnection.
-
-        Despite this imprecision,
-        session locks provide a useful way to coordinate session actions.
-
-        > NOTE
-        > This interface does not require user implementation
-        > and is only used to hide implementation details.
-
-        Since:
-            6.10
-    """
-
-    acquisition: SessionLockAcquisition
-    parent: typing.Optional[weakref.ReferenceType] = dataclasses.field(default=None)
-    _owned: bool = dataclasses.field(init=False)
-    _lock: asyncio.Lock = dataclasses.field(init=False)
-
-    @property
-    def name(self: SessionLock) -> pydantic.StrictStr:
-        return self.acquisition.lock_name
-
-    @property
-    def sequence(self: SessionLock) -> StrictNonNegativeInt:
-        return self.acquisition.sequence
-
-    @property
-    def is_owned(self: SessionLock) -> bool:
-        return self._owned
-
-    @property
-    def scope(self: SessionLock) -> SessionLockScope:
-        return self.acquisition.scope
-
-    def __init__(
-        self: SessionLock,
-        parent: typing.Union[InternalSession, SessionLocks],
-        acquisition: SessionLockAcquisition,
-    ):
-        from diffusion.internal.session import InternalSession
-
-        super().__init__()
-        if isinstance(parent, (InternalSession, SessionLocks)):
-            object.__setattr__(self, "parent", weakref.ref(parent))
-            object.__setattr__(self, "_owned", True)
-        else:
-            object.__setattr__(self, "_owned", False)
-        object.__setattr__(self, "_lock", asyncio.Lock())
-        object.__setattr__(self, "acquisition", acquisition)
-
-    async def unlock(self: SessionLock) -> bool:
-        """
-        Releases this session lock if it is owned by the session.
-
-        Since:
-            6.10.
-
-        Returns:
-            `True` if unlocking is successful, `False` if not
-
-        """
-        async with self._lock:
-            if self._owned:
-                object.__setattr__(self, "_owned", False)
-                target = typing.cast(
-                    SessionLocks, typing.cast(weakref.ReferenceType, self.parent)()
-                )
-                return await target.unlock(self)
-
-        return False
-
-    async def set_released(self: SessionLock):
-        """
-        Marks this lock as released.
-        """
-        async with self._lock:
-            object.__setattr__(self, "_owned", False)
-
-    def __str__(self):
-        return (
-            f"{type(self).__name__}[Name={self.name}, Sequence={self.sequence},"
-            f" Scope={self.scope.name}, Owned={self.is_owned}]"
-        )
```

## Comparing `diffusion/features/timeseries/query/range_query_request.py` & `diffusion/internal/timeseries/query/range_query_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,17 @@
 #  property of Push Technology. The intellectual and technical
 #  concepts contained herein are proprietary to Push Technology and
 #  may be covered by U.S. and Foreign Patents, patents in process, and
 #  are protected by trade secret or copyright law.
 
 from __future__ import annotations
 
-import typing
-
 import pydantic
 
-from diffusion.features.timeseries.query.range_query_parameters import (
+from diffusion.internal.timeseries.query.range_query_parameters import (
     RangeQueryParameters,
     QueryType,
     Range,
     Point,
 )
 from diffusion.internal.serialisers.pydantic import MarshalledModel
 
@@ -64,34 +62,35 @@
     def __str__(self):
         return (
             f"{type(self.parameters).__name__}.DEFAULT_RANGE_QUERY()"
             f'{self.parameters}.select_from("{self.topic_path}")'
         )
 
     class Config(MarshalledModel.Config):
-        alias = "range-query-request"
         frozen = True
 
-    @classmethod
-    def attr_mappings(cls) -> typing.Dict[str, typing.Any]:
-        # fmt: off
-        return {
-            "path": "topic_path",
-            "range-query-parameters.range-query-type": "type",
-            "range-query-parameters.view-range.range-query-range.range-query-anchor":
-                "view_range_anchor",
-            "range-query-parameters.view-range.range-query-range.range-query-span":
-                "view_range_span",
-            "range-query-parameters.edit-range.range-query-range.range-query-anchor":
-                "edit_range_anchor",
-            "range-query-parameters.edit-range.range-query-range.range-query-span":
-                "edit_range_span",
-            "range-query-parameters.limit": "limit",
-        }
-        # fmt: on
+        @classmethod
+        def attr_mappings_all(cls, modelcls):
+            # fmt: off
+            return {
+                "range-query-request": {
+                    "path": "topic_path",
+                    "range-query-parameters.range-query-type": "type",
+                    "range-query-parameters.view-range.range-query-range.range-query-anchor":
+                        "view_range_anchor",
+                    "range-query-parameters.view-range.range-query-range.range-query-span":
+                        "view_range_span",
+                    "range-query-parameters.edit-range.range-query-range.range-query-anchor":
+                        "edit_range_anchor",
+                    "range-query-parameters.edit-range.range-query-range.range-query-span":
+                        "edit_range_span",
+                    "range-query-parameters.limit": "limit",
+                }
+            }
+            # fmt: on
 
     @property
     def limit(self):
         return self.parameters.limit
 
     @classmethod
     def from_fields(
```

## Comparing `diffusion/features/timeseries/query/range_query_result.py` & `diffusion/internal/timeseries/query/range_query_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,19 @@
+#   Copyright (c) 2023 Push Technology Ltd., All Rights Reserved.
+#
+#   Use is subject to license terms.
+#
+#  NOTICE: All information contained herein is, and remains the
+#  property of Push Technology. The intellectual and technical
+#  concepts contained herein are proprietary to Push Technology and
+#  may be covered by U.S. and Foreign Patents, patents in process, and
+#  are protected by trade secret or copyright law.
+
 from __future__ import annotations
 
-import functools
 import typing
 
 import attr
 from pydantic import StrictInt
 
 import diffusion.datatypes
 from diffusion.datatypes.primitives import StringDataType, Int64DataType
@@ -17,15 +26,15 @@
     OriginalEvent,
     EditEvent,
 )
 from diffusion.features.timeseries.query.range_query import QueryResult
 from diffusion.features.timeseries.query.range_query_parameters import StreamStructure
 from diffusion.handlers import LOG
 from diffusion.internal.serialisers.attrs import MarshalledModel
-from diffusion.internal.serialisers.base import ListEncoder, ChoiceEncoder
+from diffusion.internal.serialisers.base import Serialiser
 from diffusion.internal.serialisers.generic_model import GenericConfig
 from diffusion.internal.services import ServiceValue
 from diffusion.internal.utils import validate_member_arguments
 from diffusion.internal.validation import StrictNonNegativeInt
 from diffusion.session.exceptions import IncompatibleTopicError
 
 
@@ -139,23 +148,23 @@
                     "range-query-result.selected-count": "selected_count",
                     "range-query-result.selected-events": "events",
                 }
             }
 
         @classmethod
         def _as_service_value(
-            cls, item: RangeQueryResult, serialiser=None
+            cls, item: RangeQueryResult, serialiser: Serialiser = None
         ) -> ServiceValue:
             return super().as_service_value(item, serialiser)
 
         @classmethod
         def as_service_value(
             cls: typing.Type[GenericConfig[RangeQueryResult_T]],
             item: RangeQueryResult_T,
-            serialiser=None,
+            serialiser: Serialiser = None,
         ) -> ServiceValue:
             # noinspection PyProtectedMember
             result = RangeQueryResult.Config._as_service_value(item, serialiser)
             offsets: EncodingType = [
                 (
                     EventType.METADATA_OFFSETS,
                     *item.offsets.Config.as_tuple(item.offsets),
@@ -199,22 +208,17 @@
 
         @classmethod
         def as_range_query_tuple(
             cls,
             modelcls: typing.Type[RangeQueryResult],
             event: typing.Union[OriginalEvent, EditEvent],
             author_encodings: AuthorCodeMapping,
-            serialiser: str = None,
+            serialiser: Serialiser = None,
         ):
-            selected_events_serialisers: typing.Mapping[
-                int, str
-            ] = cls.get_selected_events_serialiser(modelcls, serialiser)
-            ev_serialiser = cls.serialiser(
-                selected_events_serialisers[EventType.from_type(type(event))]
-            )
+            serialiser = cls.check_serialiser(serialiser)
             if event.metadata:
                 author: bytes = author_encodings.encode(event.metadata.author)
                 event = event.copy(
                     update={"metadata": event.metadata.copy(update={"author": author})}
                 )
             if event.original_event:
                 orig_author: bytes = author_encodings.encode(
@@ -224,37 +228,20 @@
                     update={
                         "original_event": event.original_event.copy(
                             update={"author": orig_author}
                         )
                     }
                 )
 
-            result = event.Config.as_tuple(event, ev_serialiser.name)
-            return result
-
-        @classmethod
-        @functools.lru_cache(maxsize=None)
-        def get_selected_events_serialiser(
-            cls, modelcls, serialiser
-        ) -> typing.Mapping[int, str]:
-            selected_events_spec_key = cls.get_model_to_serialiser_mapping(
+            selected_events_serialiser = cls.get_model_to_serialiser_mapping(
                 modelcls, serialiser
             ).get("events")
-            selected_events_serialiser = typing.cast(
-                ListEncoder, cls.serialiser(serialiser).spec[selected_events_spec_key]
-            )
-
-            range_query_event_data_serialiser = typing.cast(
-                ChoiceEncoder,
-                next(iter(selected_events_serialiser.serialiser.spec.values())),
-            )
-            return typing.cast(
-                typing.Mapping[int, str],
-                range_query_event_data_serialiser.serialiser_names,
-            )
+            assert selected_events_serialiser is not None
+            result = cls.entry_from_list_of_choices_as_tuple(event, selected_events_serialiser)
+            return result
 
     @classmethod
     def from_fields(
         cls,
         *,
         events,
         value_data_type,
```

## Comparing `diffusion/session/locks/session_lock_request.py` & `diffusion/internal/session/locks/session_lock_request.py`

 * *Files identical despite different names*

## Comparing `diffusion/session/locks/session_lock_request_cancellation.py` & `diffusion/internal/session/locks/session_lock_request_cancellation.py`

 * *Files identical despite different names*

## Comparing `diffusion-6.9.0.dist-info/METADATA` & `diffusion-6.9.1.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-Metadata-Version: 2.1
-Name: diffusion
-Version: 6.9.0
-Summary: Python SDK for Diffusion.
-Home-page: 
-https: //www.pushtechnology.com/
-License: Proprietary
-Keywords: diffusion,cloud,websockets,data
-Classifier: License :: Other/Proprietary License
-Classifier: Environment :: Other Environment
-Classifier: Development Status :: 4 - Beta
-Description-Content-Type: text/markdown
-Requires-Dist: aiohttp (==3.*,>=3.6.2)
-Requires-Dist: attrs (==21.*,>=21.4.0)
-Requires-Dist: cbor2 (==5.*,>=5.1.2)
-Requires-Dist: stringcase (==1.*,>=1.2.0)
-Requires-Dist: structlog (==21.*,>=-21.5.0)
-Requires-Dist: typing-extensions (==4.*,>=4.0.1)
-Requires-Dist: pydantic (==1.*,>=1.9.0)
-Requires-Dist: diffusion-core (==0.0.28)
-
-# Python SDK for Diffusion
-
-**Pre-release version; not ready for production.**
-
-The Diffusion Python library allows Python applications to interact with a Diffusion server.
-
-## Supported Python Versions
-
-The Diffusion Python SDK officially supports the following:
-
-Supported Interpreters:
-
-* CPython 3.7.9 or later
-* CPython 3.8.6 or later
-* CPython 3.9.0 or later
-
-Supported Platforms:
-
-* MacOS 10.13-11.5
-* Windows Intel 64-bit
-* Any Linux supported by the [ManyLinux 2010/2014](https://github.com/pypa/manylinux) binary wheel standard.
-
-## Current Capabilities
-
-- Session:
-  - Establish a session
-  - Send user ping
-  - Receive system ping
-- Messaging:
-  - Register request handler
-  - Send request to path
-  - Send request to session
-  - Send request to filter
-  - Register filter message stream
-- Topics:
-  - Topic subscriptions
-  - Topic creation
-  - Topic creation with initial topic value
-  - Topic removal
-  - Topic stream handlers
+Metadata-Version: 2.1
+Name: diffusion
+Version: 6.9.1
+Summary: Python SDK for Diffusion.
+Home-page: 
+https: //www.pushtechnology.com/
+License: Proprietary
+Keywords: diffusion,cloud,websockets,data
+Classifier: License :: Other/Proprietary License
+Classifier: Environment :: Other Environment
+Classifier: Development Status :: 4 - Beta
+Description-Content-Type: text/markdown
+Requires-Dist: aiohttp (==3.*,>=3.6.2)
+Requires-Dist: attrs (==21.*,>=21.4.0)
+Requires-Dist: cbor2 (==5.*,>=5.1.2)
+Requires-Dist: stringcase (==1.*,>=1.2.0)
+Requires-Dist: structlog (==21.*,>=21.5.0)
+Requires-Dist: typing-extensions (==4.*,>=4.0.1)
+Requires-Dist: pydantic (==1.*,>=1.9.0)
+Requires-Dist: diffusion-core (==0.0.28)
+
+# Python SDK for Diffusion
+
+**Pre-release version; not ready for production.**
+
+The Diffusion Python library allows Python applications to interact with a Diffusion server.
+
+## Supported Python Versions
+
+The Diffusion Python SDK officially supports the following:
+
+Supported Interpreters:
+
+* CPython 3.7.9 or later
+* CPython 3.8.6 or later
+* CPython 3.9.0 or later
+
+Supported Platforms:
+
+* MacOS 10.13-11.5
+* Windows Intel 64-bit
+* Any Linux supported by the [ManyLinux 2010/2014](https://github.com/pypa/manylinux) binary wheel standard.
+
+## Current Capabilities
+
+- Session:
+  - Establish a session
+  - Send user ping
+  - Receive system ping
+- Messaging:
+  - Register request handler
+  - Send request to path
+  - Send request to session
+  - Send request to filter
+  - Register filter message stream
+- Topics:
+  - Topic subscriptions
+  - Topic creation
+  - Topic creation with initial topic value
+  - Topic removal
+  - Topic stream handlers
```

## Comparing `diffusion-6.9.0.dist-info/RECORD` & `diffusion-6.9.1.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 diffusion/__init__.py,sha256=OjWoUbuUSxRY59e9v_-CfcyN9ibP-tZiN3SDMBym_Lg,248
 diffusion/exceptions.py,sha256=cpMFnSqTY5UGrYpIIqq34OiM7iai23bGZaIfz9m7BjM,739
-diffusion/datatypes/__init__.py,sha256=O8Mxe7vPxOs4VMpAjJ6F-d-Nvm6TlLe4nF5N5PynhiQ,3731
+diffusion/datatypes/__init__.py,sha256=wYNiKHQ4AzK3dvmlv_6eDh4K3P66eoHOEID6N67LF1Y,3781
 diffusion/datatypes/exceptions.py,sha256=mSCYJvyJBjMmnm8a84u7j91AdpII_WN3_n5UeRcbRs4,494
 diffusion/datatypes/complex/__init__.py,sha256=pXOGDVy6xljKdaYiWpLb1r0ewkWGSdKgokHrvOwO8Ro,652
 diffusion/datatypes/complex/jsondatatype.py,sha256=Kiw6uDTdBt0j04V3nyW-tPhy8KZn3GxuYgrvaSK_DoM,2053
 diffusion/datatypes/complex/recorddatatype.py,sha256=LkefL6Nzh72jXF2uVDU4gIivAeoyX0P8Sh9xEb005bo,214
 diffusion/datatypes/complex/routingdatatype.py,sha256=Ujj5cU_ZN8xb1bY8Qtfsq7izIxmYSyGEb1EFRI4ye9k,204
 diffusion/datatypes/complex/unknowndatatype.py,sha256=-Rm5rKNBEP7C7xd6qQZ6o5-DzH5qMvrdHO0owF0Yhjk,204
 diffusion/datatypes/foundation/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -13,93 +13,99 @@
 diffusion/datatypes/primitives/__init__.py,sha256=XfFA_P-hHDh7hASPATP4BeQGLaLddb4pVkTfoXSz3_g,1088
 diffusion/datatypes/primitives/binarydatatype.py,sha256=gkgAWLQH-_XU6DzJ3TXuPk18jGKGHMxCYjvEsNI5RXc,2095
 diffusion/datatypes/primitives/doubledatatype.py,sha256=CKNyYmuDVerP1NIj1ud56rtF8yeBpU1G7oNvykn-91A,366
 diffusion/datatypes/primitives/int64datatype.py,sha256=rIAKWZ2g7IEk_uDfCPYkiKFVNJYAnsP967xHh9KE7I0,988
 diffusion/datatypes/primitives/primitivedatatype.py,sha256=2kZTJpmZR9YaTDCC-WLCXHQkX_ZW3GvZjoBJkPJ2zWY,1602
 diffusion/datatypes/primitives/stringdatatype.py,sha256=58qgf7iWj41ZHPqf_NJHoA7o9F00-TJNtRO5cXkuyzM,234
 diffusion/datatypes/timeseries/__init__.py,sha256=D3Faq8sVMclZDpO3xGRE71tEEc1mSt1mUYcMF_EDhv4,11467
-diffusion/datatypes/timeseries/time_series_event.py,sha256=Ryd6kby7Z9spdh9eDrBa2XLb13QpAud05e_JB3zj670,18779
-diffusion/datatypes/timeseries/time_series_event_metadata.py,sha256=Ht4Im--J1Amy5s0N9c8YYBObQiWOFzcVMX9jeMvlG5Y,2089
+diffusion/datatypes/timeseries/time_series_event.py,sha256=LWViLWEvqOUCs5VqpTcZaadqplD3XXB7QkMFyT4DmfU,19412
+diffusion/datatypes/timeseries/time_series_event_metadata.py,sha256=vigjpc4vGASyZpQsnaxRqzheQdNnmhEA6d3bVItoSME,2997
 diffusion/datatypes/timeseries/types.py,sha256=KvBKm2zCzhUTsS9TPlUyQzhbfFWxUbTWGsRCbxFvQxo,1645
 diffusion/features/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 diffusion/features/control/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-diffusion/features/control/metrics/__init__.py,sha256=hcVPJt2liKmnD6kL7hPR0Ix-BrV6_b8e19poB6IMXSU,7734
+diffusion/features/control/metrics/__init__.py,sha256=AZm85DGcXn-R3TYwruTP1UtZLxD3YABUKSIEdCy2tGA,8750
 diffusion/features/control/metrics/collector.py,sha256=KEGSiF9BMTnCSz2SBLCR2bgNEv9ML5xHA4yKijGIoCY,1138
 diffusion/features/control/metrics/session_metrics.py,sha256=0Ar2yO_0pn-YW-Kv_4xGHOzd1wBrZMf28onNyq_ZnlU,5218
-diffusion/features/control/metrics/topic_metrics.py,sha256=HmPDAiSld0MOKl6Ege-gICLY7w5FG-GtCMsoXPxVn5U,5046
+diffusion/features/control/metrics/topic_metrics.py,sha256=Jd-ZBr7Xz0HJeUZp14AIDNlJ0N-0-Y46Ip-cFulUhDU,5158
 diffusion/features/control/session_trees/__init__.py,sha256=7cl4C3h20i10MgmbyG3jS3nnNcrfVs2UB2zOHO_KG5c,9508
 diffusion/features/control/session_trees/branch_mapping.py,sha256=2eQBOc7QWDsTca-xH_QRYxttCRptu6tLTcC-1fjgaX0,1334
-diffusion/features/control/session_trees/branch_mapping_table.py,sha256=SRCxX1J2BdEkdP9QB2rMaVUAMF6cHoyD1yOhkBcJ8gE,3332
+diffusion/features/control/session_trees/branch_mapping_table.py,sha256=9vW18y6U-wjRmejMlxQZ5uG-TVPP_qnRfkOunhChEyI,3409
 diffusion/features/control/session_trees/invalid_branch_mapping_exception.py,sha256=NOG1kSY7jEuWtwZN-loIs2gSjQhwnaz85Wg68FE5fFM,1031
-diffusion/features/timeseries/__init__.py,sha256=zoxFd1Tc8T7cJIXAJAd7gsTzCE3EaGp8cnQSs0vkCqs,16865
+diffusion/features/timeseries/__init__.py,sha256=d2Rn2xZTzJTvhQbi02dcF8qPduPTpqqta-E03ew62hY,17686
 diffusion/features/timeseries/query/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 diffusion/features/timeseries/query/query_result.py,sha256=oJo3SWFFt6v2IMkhK1nz9pBGljQ12KltIKgvMdXi1yg,6760
-diffusion/features/timeseries/query/range_query.py,sha256=vQw6V7Q0dgEW8teR8Ilq2Vs2RyEMqHw8EcbV1NHP8f0,51194
-diffusion/features/timeseries/query/range_query_parameters.py,sha256=8doNFAuH-1Lad5TXwkQftTct8Dv08XY9U_KO072l56U,27026
-diffusion/features/timeseries/query/range_query_request.py,sha256=mgdKciGsuYbbcyPkOlQXQxsXNWgUcODHOR7oM6DfQTA,3456
-diffusion/features/timeseries/query/range_query_result.py,sha256=avtERznZBuHTUsac3V8I1S4lnJLsfbJasTmWqbrrj5U,11170
-diffusion/features/topics/__init__.py,sha256=Q-mUjh4HzJK4PT7k2s5MBdbD79oR7vnd6Z7JGs2GcO8,12427
+diffusion/features/timeseries/query/range_query.py,sha256=lPUbYJRSLW2CKNuczlqvISB7GMrLNn519IveQjDG9l4,49729
+diffusion/features/timeseries/query/range_query_parameters.py,sha256=07hqKH7oq1zIAdiKIRCrmF_viLlnXNvlpLYnOjZWar4,710
+diffusion/features/topics/__init__.py,sha256=SL1Vt-K5RRi9x3D-7fHuUhGu-xi97EjzTEdZTb5ist4,12515
 diffusion/features/topics/selectors.py,sha256=KsPEuQrEab8kBijn55RisuNH7BlpLfR5HddZjUTLC6E,8127
-diffusion/features/topics/streams.py,sha256=F5q-JNQ37qt0J76viYTb9XMIFZdJgvp2jO9O8yTTKiQ,2731
+diffusion/features/topics/streams.py,sha256=WZYeamgr5GGHWEvAz3QK-BeHUVVAk7YBr92AuZRZMQA,2731
 diffusion/features/topics/details/__init__.py,sha256=-uW_l93bOAVnG1-KXw2utpQAhK6Gvss9cOCdJtFAyRs,424
-diffusion/features/topics/details/topic_specification.py,sha256=G7dmtfmNQgfhYyCqbCs2fLfG53VcnLq51sCZcEpRa-k,43714
-diffusion/features/topics/update/__init__.py,sha256=o_c-MZaKmcBc6gNEz2z5lsdAowS1njI4gRSWkUYL4kU,4692
+diffusion/features/topics/details/topic_specification.py,sha256=V-TA140oObenIxEF5IUqJnn6GxwDrBElC5pO1igaYuU,43807
+diffusion/features/topics/update/__init__.py,sha256=nYIFxcuE4_-wcyVjWczHAnKL0-wBvYU4vRyLW4H4V3I,4557
 diffusion/features/topics/update/constraint_factory.py,sha256=H9N_GUW9mzK9U4fGW7VI79ZF2239cajWDbLMENA0bOA,4573
-diffusion/features/topics/update/constraints.py,sha256=vzo_558RaFDtvlgNHZzoitazK3P6k0B1l-ACS50AxCM,12226
+diffusion/features/topics/update/constraints.py,sha256=z7v_rXxcOhRjehIl0rO57WFptx5sHX22BbAh63w6dhg,13539
 diffusion/handlers/__init__.py,sha256=gID2EUPLjx_E0LQc5P2gxzhaeLW3atM-6pooYro_RKo,4096
 diffusion/internal/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 diffusion/internal/components.py,sha256=AL-0UOYgbSS3wARdqpsjSLEPJ-6mnF8ZbmUAWzc_YZ0,677
 diffusion/internal/encoder.py,sha256=iyvFLrgzIkWKqsEjqQ6kPcxTUl_O9Wp10ZDwcWbB5Vc,1246
 diffusion/internal/exceptions.py,sha256=up0eC7zVw7bS1uZjZQ1OSqKSqExDuLvFh85_KBJNtTY,507
-diffusion/internal/utils.py,sha256=UnInY7d3B3Ot81IxVg5_gGJ_fZWHjcIKyjTh0iNXmyc,12047
+diffusion/internal/utils.py,sha256=JTgoC-KNIxUUjdWBQehJTDw-9xm3vmnhpEZKO33TvZI,12064
 diffusion/internal/encoded_data/__init__.py,sha256=2s6imf0rMOsTSU023DPRaHi8hhoPEE03RCdedT7wV8k,452
-diffusion/internal/encoded_data/abstract.py,sha256=-8v5Wee1oTyE2WZQb-9dkQOk1rkE2XhV0zlyMRfhDEY,2628
+diffusion/internal/encoded_data/abstract.py,sha256=iO_iJN1oXOSm5FqRZUFmXmte7OxWC4XtiU59xg8gP10,4234
 diffusion/internal/encoded_data/exceptions.py,sha256=MlSaj6Fq6lonpb3bsVkmKKIBAfz6UrRkhVBCK3AyZ4Q,494
 diffusion/internal/encoded_data/generics.py,sha256=1O9KU-3f2bjH-TCU3rS67k4AGyz3fBglIxsY1FgscaY,1928
 diffusion/internal/encoded_data/scalars.py,sha256=-WsECA6bGPNIBvHzkmXfng4OYEYm47vjnxf-ADC0lGg,4912
 diffusion/internal/generated/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-diffusion/internal/generated/services.py,sha256=gFm1ecJIp6wBkDeu_aDWJuBf__1X6-Ikqx14F7_WkUU,10365
+diffusion/internal/generated/services.py,sha256=C5POHzqI-GYB3gFBtJJKRg0ZNIKd0PYkHLpwAvZtA_0,10827
 diffusion/internal/protocol/__init__.py,sha256=PBJY5t93TZ7nDV534E0Cl3jhirX58NS1i-GRX1-Ftxc,6965
 diffusion/internal/protocol/conversations.py,sha256=4a_8fg55enoekZ48OvcITH4li1CBsD8U4erUlKtP8iM,9658
 diffusion/internal/protocol/exceptions.py,sha256=w7i5QHzgQmjfjlo5jHaec826Auc9U9UGZggzuVtRYfk,2518
 diffusion/internal/protocol/message_types.py,sha256=GB79-wevnjfzQAFJutgt6OY8iF6zFNXXRdcQBT573KE,8325
 diffusion/internal/protocol/properties.py,sha256=HTSXFr7tLiCHFcjRbEAKVfoaqA3PMM2Ikmx23Xk_1FQ,11585
-diffusion/internal/serialisers/__init__.py,sha256=aLsceIKAw2nSI7PtGl_EzK07QjSYGEiDm9kwj1rHVgg,1128
-diffusion/internal/serialisers/attrs.py,sha256=w5tNeyJ-lqDGHKwFiL7-mGin0t5J8SX7gkoRQChoVE4,2721
-diffusion/internal/serialisers/base.py,sha256=ZydqYfGFZ3ePYJJ84RZ6YCDP6Xx2jnWDypHDlafRwFE,13067
-diffusion/internal/serialisers/compound.py,sha256=GqyA3UdB6PTCg0RdZ5jLDkuBNjFX875nLlIqAyMWVFE,6990
-diffusion/internal/serialisers/dataclass_model.py,sha256=gceg-08Tqnxa1JBM867ztrnw2SpUe0EI9rHdgWcXZrA,901
-diffusion/internal/serialisers/generic_model.py,sha256=jTprCTmklpb4LAOCQsgZRUE4Rr7IgIPKqf4yUK-2tH8,11433
-diffusion/internal/serialisers/pydantic.py,sha256=cZkgy_NRg5zXXA2pgiAdHlkkfKtz9P01FTRnaB3KNvc,1844
-diffusion/internal/serialisers/spec.py,sha256=v1a6-9EQ9AZHiUK16py-AUPhVwPrEfPv_hEMOeG8aH4,39211
-diffusion/internal/serialisers/timeseries.py,sha256=3k93VXm504Exwr6muBs29eAa-ipsPkh_uDFSrOVsv5Y,3240
+diffusion/internal/serialisers/__init__.py,sha256=A7Z38BPpowpCoimnrStDxmU-ACKxHguIFXZthT2TJkY,1501
+diffusion/internal/serialisers/attrs.py,sha256=z6Nvxu53zcMhDI2fmIijWiDFtf_kPfiHwLF4AV2AhkY,2619
+diffusion/internal/serialisers/base.py,sha256=rQm0oY6be1jW1y0ve_mCMFQGg5Ee3-qPT_QbvfH5sc0,18544
+diffusion/internal/serialisers/compound.py,sha256=HRg8MhuzwujyQCWPBivtU20wCKTK6SMP2YK783ef_tM,7541
+diffusion/internal/serialisers/generic_model.py,sha256=7KUAF-6JsGOAOAABb_xgvLQ9rTxNDnJJbXPxATM9uJ8,13422
+diffusion/internal/serialisers/primitives.py,sha256=Uq2dkxdPbJV7rH5GbWVY8CNAtZvC74GSt3BtdGqP4Po,786
+diffusion/internal/serialisers/pydantic.py,sha256=SleiMFtSBKquOQPwfCqCcEFW1s3lDTMqNcCx8UsL4pM,1712
+diffusion/internal/serialisers/spec.py,sha256=flsLdoT0UQePfo9-oPigYCwvTZdR1q7egXM4F1cG9vY,42379
+diffusion/internal/serialisers/timeseries.py,sha256=oXhnXeryuIy5G4qvXsNbE39mMeV6KggTtU5kAO7pZro,4071
 diffusion/internal/services/__init__.py,sha256=s8C37BUccWHoE9MeQk3uOBAiCgXgaJ7FAxWItWKSYpY,688
-diffusion/internal/services/abstract.py,sha256=PF65AtWyDZ20cpnT6X_eR5DQooOclyzzK8pQZzwR_Mg,14200
+diffusion/internal/services/abstract.py,sha256=mcVCaN98hfcp5YLfHGb0DC_8hSZLMYD4d9uLcJNGK8k,13677
 diffusion/internal/services/exceptions.py,sha256=vvVIvSaK-vby_KSVY9Yp3uDqz3wEcz4ckZ6mgSpnTsk,406
 diffusion/internal/services/locator.py,sha256=WVWyI8muKTkYBfwyKOXr3PRnGY68zKC0JHtDX-FZYkQ,2001
 diffusion/internal/services/messaging.py,sha256=E3USc1DLJPttWelPS07QwjhtjG-DeqSsoxM8SxxVnuU,6822
 diffusion/internal/services/session.py,sha256=crXmTsNVdi5IZbPqMtJ6J6cGSQni5Y4D5aFZkAF04X8,1769
 diffusion/internal/services/topics.py,sha256=T1zfkPGIUpF138c-EYqAgha0ARgtLhOt1HrIZReJDhg,5667
 diffusion/internal/session/__init__.py,sha256=_x0v13SEjiK0auOLp1GG3FYKPLN9WTE8Egv-i3roYIs,6646
 diffusion/internal/session/connection.py,sha256=twoJkOewCzMVrFeq5APkY25_wiAW7RhDuupPqeSAfsk,8506
 diffusion/internal/session/credentials.py,sha256=7RAd86M1fXNqoT3qWq3yvFaIyMbD-I_uLMBjjUeKQUg,1678
 diffusion/internal/session/error_reason.py,sha256=JBOb7OYz7Q_CYusdSAH0M6HcSvXtVI6hcIe0i1hUMwc,4292
 diffusion/internal/session/exception_handler.py,sha256=K3c0M8Mju1W9a_xsr11eLgj_j3UHpidPWshvmSVWNkE,8161
-diffusion/internal/topics/__init__.py,sha256=qjhosVlYjxdD0GO9u3YJQ9zeG0BQkT39i7rkWEMVt6w,7483
+diffusion/internal/session/locks/__init__.py,sha256=yxAnQzNfpIxYSj_XSPK5SYPCT8_mKyMgTZT-ffRaH6g,424
+diffusion/internal/session/locks/session_lock_acquisition.py,sha256=4JXFjZWyPmStN8rj-rr9jGH9CNmudVNTbcyBjA0HxCc,1360
+diffusion/internal/session/locks/session_lock_request.py,sha256=Y2ucymU5E107EcwS6uEy1lWDSfsPKRiY_HGl7zKCBr4,805
+diffusion/internal/session/locks/session_lock_request_cancellation.py,sha256=rZsd6oJy396z9UkiUZPaDK4V2kAO-TRZ1SZpAsCBgo4,710
+diffusion/internal/timeseries/__init__.py,sha256=yxAnQzNfpIxYSj_XSPK5SYPCT8_mKyMgTZT-ffRaH6g,424
+diffusion/internal/timeseries/query/__init__.py,sha256=yxAnQzNfpIxYSj_XSPK5SYPCT8_mKyMgTZT-ffRaH6g,424
+diffusion/internal/timeseries/query/range_query.py,sha256=oGLkFTkltGgSZMnS5btn_wu-qLrAI7KYGSfk5chdzJM,2363
+diffusion/internal/timeseries/query/range_query_parameters.py,sha256=GEJGTLldHFX1EScQuv04BG7-Xdcagk18ntMlYKS3yfY,27383
+diffusion/internal/timeseries/query/range_query_request.py,sha256=95tBAUw-x0Ykh9OXgW75qCC4pVY3NPneraSTDaqa4eo,3556
+diffusion/internal/timeseries/query/range_query_result.py,sha256=lnNE5PyrnmVJRDYnj8EmEqUbW-kOPdjfbOLKgiIK6H4,10765
+diffusion/internal/topics/__init__.py,sha256=ieRGrrTwclmftbD7U0QYmf6Gd-dtu6PUAg6BWURV070,7618
 diffusion/internal/topics/constraints.py,sha256=X3t0Vd36lFFk0VduyIREdg5PGJaY0F323sHfOFddvsY,311
 diffusion/internal/validation/__init__.py,sha256=Db6cEZ0KJCXlp-SciakEqQj20p4GJdthWVE4ETEfgt4,2192
 diffusion/internal/validation/pydantic.py,sha256=wLEek-9k4uBSwPSmNqap2Bd_n6dSKUDi5ouJdve2TVQ,1923
 diffusion/messaging/__init__.py,sha256=fjVIiV0pzwL3ufhMwoYo_4gzVgaEFxPiXIow9I9TNPs,10373
-diffusion/session/__init__.py,sha256=eS7dD4gUR-XraPb34lMph8dWmu1zO9aAHRt0ZSm2-yc,13206
+diffusion/session/__init__.py,sha256=C2tiUAlLX4012zn4e4UspMS9Vz4spISMMfcyhy2wrPo,13266
 diffusion/session/exceptions.py,sha256=3yIucpyScgEz3xSrj-SXz_YNKxb2pJRAjOJ5DwuU5cM,5509
 diffusion/session/retry_strategy.py,sha256=ksor0KPILAkMJBf9tI31IAd5LMHvcSN7MxRaIsu1noE,2166
 diffusion/session/session_container_factory.py,sha256=1a2x2F8FdxZuYCsL9uzzApAKmzfLuDH35i0nPbB972U,1223
 diffusion/session/session_factory.py,sha256=SIVItr2UCN7_4e4-awYLX_g9Wd6GiFlbWsDOXOGPjEs,12135
 diffusion/session/locks/__init__.py,sha256=-uW_l93bOAVnG1-KXw2utpQAhK6Gvss9cOCdJtFAyRs,424
-diffusion/session/locks/session_lock_acquisition.py,sha256=k0ZV3BrGmp4uqCaPEHPK0X0Zr1FfvEp5X5Yuoe6NxsM,2112
-diffusion/session/locks/session_lock_request.py,sha256=Y2ucymU5E107EcwS6uEy1lWDSfsPKRiY_HGl7zKCBr4,805
-diffusion/session/locks/session_lock_request_cancellation.py,sha256=rZsd6oJy396z9UkiUZPaDK4V2kAO-TRZ1SZpAsCBgo4,710
-diffusion/session/locks/session_locks.py,sha256=Pe74elZYV3NoFg4KPZrLkMQtkAR5JBVT4Z6PrFD4uiw,14842
-diffusion-6.9.0.dist-info/METADATA,sha256=RfSszWjyQuy4pC_d4HLln53YxjjZHygRC7vzVckDwKI,1646
-diffusion-6.9.0.dist-info/WHEEL,sha256=KQAdL1r0nkelHXuyWjrA7sdAbDAr-4M34W5cdYiYym0,102
-diffusion-6.9.0.dist-info/top_level.txt,sha256=7Q6zKfH0egqajYyKZcvu9BaNkgK3lP6IuD3_eQzyME0,10
-diffusion-6.9.0.dist-info/RECORD,,
+diffusion/session/locks/session_lock_acquisition.py,sha256=TjOz21iosDckTJH1AhZ5IOYuONKDBiks57qRJhae9hQ,929
+diffusion/session/locks/session_locks.py,sha256=gu8NtcHWRkditfTrZ5ESLF0z2ZPqYAgo5J1toER795U,14937
+diffusion-6.9.1.dist-info/METADATA,sha256=VVKZfUYXKfrxilmGZY2W8sD7dqiGM339dlO1hXmI_9M,1706
+diffusion-6.9.1.dist-info/WHEEL,sha256=Bm0lU0eE5rfO4o-JCrdtDvmsDdxyxI3a6Hi0DzV3SNc,102
+diffusion-6.9.1.dist-info/top_level.txt,sha256=7Q6zKfH0egqajYyKZcvu9BaNkgK3lP6IuD3_eQzyME0,10
+diffusion-6.9.1.dist-info/RECORD,,
```

