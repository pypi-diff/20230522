# Comparing `tmp/semantha_sdk-4.8.1.tar.gz` & `tmp/semantha_sdk-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantha_sdk-4.8.1.tar", max compression
+gzip compressed data, was "semantha_sdk-5.2.0.tar", max compression
```

## Comparing `semantha_sdk-4.8.1.tar` & `semantha_sdk-5.2.0.tar`

### file list

```diff
@@ -1,85 +1,142 @@
--rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-4.8.1/LICENSE
--rw-r--r--   0        0        0     1596 2023-03-30 15:56:31.833146 semantha_sdk-4.8.1/pyproject.toml
--rw-r--r--   0        0        0     7831 2023-03-15 04:48:34.896873 semantha_sdk-4.8.1/README.md
--rw-r--r--   0        0        0     1288 2023-03-15 17:19:29.855440 semantha_sdk-4.8.1/semantha_sdk/__init__.py
--rw-r--r--   0        0        0        0 2023-02-28 08:03:18.509414 semantha_sdk-4.8.1/semantha_sdk/api/__init__.py
--rw-r--r--   0        0        0     1154 2023-02-22 09:56:52.493394 semantha_sdk-4.8.1/semantha_sdk/api/current_user.py
--rw-r--r--   0        0        0      824 2023-03-30 09:36:38.140254 semantha_sdk-4.8.1/semantha_sdk/api/diff.py
--rw-r--r--   0        0        0     5221 2023-03-30 09:36:38.143378 semantha_sdk-4.8.1/semantha_sdk/api/domain/__init__.py
--rw-r--r--   0        0        0     2881 2023-03-30 09:36:38.146612 semantha_sdk-4.8.1/semantha_sdk/api/domain/classes.py
--rw-r--r--   0        0        0     2382 2023-03-30 09:36:38.150194 semantha_sdk-4.8.1/semantha_sdk/api/domain/cluster.py
--rw-r--r--   0        0        0     2863 2023-03-30 09:36:38.152207 semantha_sdk-4.8.1/semantha_sdk/api/domain/comparison.py
--rw-r--r--   0        0        0     2020 2023-03-30 09:36:38.154732 semantha_sdk-4.8.1/semantha_sdk/api/domain/document_annotations.py
--rw-r--r--   0        0        0     5137 2023-03-30 09:36:38.157240 semantha_sdk-4.8.1/semantha_sdk/api/domain/document_classes.py
--rw-r--r--   0        0        0     2358 2023-03-30 09:36:38.160813 semantha_sdk-4.8.1/semantha_sdk/api/domain/documents.py
--rw-r--r--   0        0        0     1628 2023-02-22 09:56:52.505911 semantha_sdk-4.8.1/semantha_sdk/api/domain/model.py
--rw-r--r--   0        0        0    14358 2023-03-30 09:36:38.163322 semantha_sdk-4.8.1/semantha_sdk/api/domain/reference_documents.py
--rw-r--r--   0        0        0     5481 2023-03-30 09:36:38.166876 semantha_sdk-4.8.1/semantha_sdk/api/domain/references.py
--rw-r--r--   0        0        0      892 2023-03-30 09:36:38.170401 semantha_sdk-4.8.1/semantha_sdk/api/domain/settings.py
--rw-r--r--   0        0        0     2248 2023-03-30 09:36:38.173496 semantha_sdk-4.8.1/semantha_sdk/api/domain/similarity_matrix.py
--rw-r--r--   0        0        0      411 2023-02-22 09:56:52.512832 semantha_sdk-4.8.1/semantha_sdk/api/domain/statistics.py
--rw-r--r--   0        0        0     1399 2023-03-13 22:03:25.716422 semantha_sdk-4.8.1/semantha_sdk/api/domain/tags.py
--rw-r--r--   0        0        0      520 2023-03-14 07:25:08.827328 semantha_sdk-4.8.1/semantha_sdk/api/info.py
--rw-r--r--   0        0        0      306 2023-03-30 09:36:38.176505 semantha_sdk-4.8.1/semantha_sdk/api/metadata_types.py
--rw-r--r--   0        0        0     1538 2023-03-13 21:57:13.088908 semantha_sdk-4.8.1/semantha_sdk/api/model/__init__.py
--rw-r--r--   0        0        0     3374 2023-03-06 09:15:25.101746 semantha_sdk-4.8.1/semantha_sdk/api/model/boost_words.py
--rw-r--r--   0        0        0      695 2023-03-30 09:36:38.178579 semantha_sdk-4.8.1/semantha_sdk/api/model/data_properties.py
--rw-r--r--   0        0        0      307 2023-03-30 09:36:38.182099 semantha_sdk-4.8.1/semantha_sdk/api/model/extractor_types.py
--rw-r--r--   0        0        0      615 2023-03-30 09:36:38.184629 semantha_sdk-4.8.1/semantha_sdk/api/model/instances.py
--rw-r--r--   0        0        0      816 2023-02-28 08:03:18.535991 semantha_sdk-4.8.1/semantha_sdk/api/model/named_entities.py
--rw-r--r--   0        0        0     4319 2023-02-22 09:56:52.525369 semantha_sdk-4.8.1/semantha_sdk/api/model/synonyms.py
--rw-r--r--   0        0        0     2080 2023-03-14 08:24:57.314881 semantha_sdk-4.8.1/semantha_sdk/api/semantha_api.py
--rw-r--r--   0        0        0      413 2023-02-14 17:17:50.169885 semantha_sdk-4.8.1/semantha_sdk/api/semantha_endpoint.py
--rw-r--r--   0        0        0      450 2023-02-22 09:56:52.527369 semantha_sdk-4.8.1/semantha_sdk/model/__init__.py
--rw-r--r--   0        0        0      416 2023-03-16 17:15:26.621348 semantha_sdk-4.8.1/semantha_sdk/model/area.py
--rw-r--r--   0        0        0      470 2023-02-28 08:03:18.537993 semantha_sdk-4.8.1/semantha_sdk/model/boost_word.py
--rw-r--r--   0        0        0      790 2023-02-28 08:03:18.538993 semantha_sdk-4.8.1/semantha_sdk/model/cls.py
--rw-r--r--   0        0        0     1417 2023-03-30 09:36:38.187132 semantha_sdk-4.8.1/semantha_sdk/model/cluster.py
--rw-r--r--   0        0        0      920 2023-03-06 09:15:25.102744 semantha_sdk-4.8.1/semantha_sdk/model/complex_property.py
--rw-r--r--   0        0        0      301 2023-02-28 08:03:18.550512 semantha_sdk-4.8.1/semantha_sdk/model/data_type.py
--rw-r--r--   0        0        0      372 2023-02-28 08:03:18.551516 semantha_sdk-4.8.1/semantha_sdk/model/diff.py
--rw-r--r--   0        0        0      714 2023-03-30 09:36:38.190373 semantha_sdk-4.8.1/semantha_sdk/model/document.py
--rw-r--r--   0        0        0     1064 2023-02-28 08:03:18.556039 semantha_sdk-4.8.1/semantha_sdk/model/document_class.py
--rw-r--r--   0        0        0      379 2023-02-28 08:03:18.558045 semantha_sdk-4.8.1/semantha_sdk/model/document_metadata.py
--rw-r--r--   0        0        0      390 2023-02-28 08:03:18.559553 semantha_sdk-4.8.1/semantha_sdk/model/domain.py
--rw-r--r--   0        0        0      465 2023-02-28 08:03:18.561563 semantha_sdk-4.8.1/semantha_sdk/model/domain_configuration.py
--rw-r--r--   0        0        0     2557 2023-03-14 12:34:28.927105 semantha_sdk-4.8.1/semantha_sdk/model/domain_settings.py
--rw-r--r--   0        0        0      333 2023-02-28 08:03:18.566090 semantha_sdk-4.8.1/semantha_sdk/model/entity.py
--rw-r--r--   0        0        0      502 2023-03-06 09:15:25.104745 semantha_sdk-4.8.1/semantha_sdk/model/extraction_area.py
--rw-r--r--   0        0        0      547 2023-03-06 09:15:25.106751 semantha_sdk-4.8.1/semantha_sdk/model/extraction_file.py
--rw-r--r--   0        0        0      432 2023-03-06 09:15:25.108755 semantha_sdk-4.8.1/semantha_sdk/model/extraction_reference.py
--rw-r--r--   0        0        0      471 2023-03-06 09:15:25.110755 semantha_sdk-4.8.1/semantha_sdk/model/file_reference.py
--rw-r--r--   0        0        0      303 2023-03-06 09:15:25.113752 semantha_sdk-4.8.1/semantha_sdk/model/finding.py
--rw-r--r--   0        0        0      438 2023-03-14 08:30:58.860283 semantha_sdk-4.8.1/semantha_sdk/model/info.py
--rw-r--r--   0        0        0      333 2023-02-28 08:03:18.568105 semantha_sdk-4.8.1/semantha_sdk/model/label.py
--rw-r--r--   0        0        0      357 2023-03-13 16:50:44.846903 semantha_sdk-4.8.1/semantha_sdk/model/language.py
--rw-r--r--   0        0        0      500 2023-03-06 09:15:25.115748 semantha_sdk-4.8.1/semantha_sdk/model/linked_instance.py
--rw-r--r--   0        0        0      386 2023-03-06 09:15:25.116749 semantha_sdk-4.8.1/semantha_sdk/model/linked_value.py
--rw-r--r--   0        0        0      458 2023-03-06 09:15:25.119749 semantha_sdk-4.8.1/semantha_sdk/model/matrix_row.py
--rw-r--r--   0        0        0      340 2023-02-28 08:03:18.570103 semantha_sdk-4.8.1/semantha_sdk/model/metadata.py
--rw-r--r--   0        0        0      383 2023-03-13 16:50:44.840365 semantha_sdk-4.8.1/semantha_sdk/model/model_class.py
--rw-r--r--   0        0        0     1427 2023-03-14 15:09:28.197027 semantha_sdk-4.8.1/semantha_sdk/model/model_instance.py
--rw-r--r--   0        0        0      350 2023-02-22 09:56:52.548931 semantha_sdk-4.8.1/semantha_sdk/model/named_entity.py
--rw-r--r--   0        0        0      649 2023-02-28 08:03:18.572097 semantha_sdk-4.8.1/semantha_sdk/model/page.py
--rw-r--r--   0        0        0     1195 2023-03-16 17:14:49.745182 semantha_sdk-4.8.1/semantha_sdk/model/paragraph.py
--rw-r--r--   0        0        0      473 2023-03-06 09:15:25.122755 semantha_sdk-4.8.1/semantha_sdk/model/process_information.py
--rw-r--r--   0        0        0      406 2023-03-06 09:15:25.124749 semantha_sdk-4.8.1/semantha_sdk/model/rect.py
--rw-r--r--   0        0        0      748 2023-03-06 09:15:25.127758 semantha_sdk-4.8.1/semantha_sdk/model/reference.py
--rw-r--r--   0        0        0     3429 2023-02-28 08:03:18.577616 semantha_sdk-4.8.1/semantha_sdk/model/reference_document.py
--rw-r--r--   0        0        0      650 2023-03-17 08:43:53.406250 semantha_sdk-4.8.1/semantha_sdk/model/semantha_entity.py
--rw-r--r--   0        0        0      788 2023-03-06 09:15:25.129755 semantha_sdk-4.8.1/semantha_sdk/model/semantic_model.py
--rw-r--r--   0        0        0      722 2023-03-16 17:16:08.719823 semantha_sdk-4.8.1/semantha_sdk/model/sentence.py
--rw-r--r--   0        0        0      411 2023-03-06 09:15:25.131750 semantha_sdk-4.8.1/semantha_sdk/model/simple_property.py
--rw-r--r--   0        0        0      484 2023-02-28 08:03:18.583619 semantha_sdk-4.8.1/semantha_sdk/model/synonym.py
--rw-r--r--   0        0        0      365 2023-03-06 09:15:25.133751 semantha_sdk-4.8.1/semantha_sdk/model/table_instance.py
--rw-r--r--   0        0        0      433 2023-02-28 08:03:18.585132 semantha_sdk-4.8.1/semantha_sdk/model/user_data.py
--rw-r--r--   0        0        0      367 2023-03-06 09:15:25.135751 semantha_sdk-4.8.1/semantha_sdk/model/version.py
--rw-r--r--   0        0        0       47 2023-02-14 17:17:50.231591 semantha_sdk-4.8.1/semantha_sdk/request/__init__.py
--rw-r--r--   0        0        0      552 2023-02-08 14:11:47.954426 semantha_sdk-4.8.1/semantha_sdk/request/semantha_request.py
--rw-r--r--   0        0        0       57 2023-02-14 17:17:50.233837 semantha_sdk-4.8.1/semantha_sdk/response/__init__.py
--rw-r--r--   0        0        0      107 2023-02-08 14:11:47.961667 semantha_sdk-4.8.1/semantha_sdk/response/semantha_error.py
--rw-r--r--   0        0        0     3472 2023-03-14 15:09:28.198027 semantha_sdk-4.8.1/semantha_sdk/response/semantha_response.py
--rw-r--r--   0        0        0       37 2023-02-14 17:17:50.239851 semantha_sdk-4.8.1/semantha_sdk/rest/__init__.py
--rw-r--r--   0        0        0     4131 2023-03-30 15:56:20.772721 semantha_sdk-4.8.1/semantha_sdk/rest/rest_client.py
--rw-r--r--   0        0        0     8805 1970-01-01 00:00:00.000000 semantha_sdk-4.8.1/setup.py
--rw-r--r--   0        0        0     8516 1970-01-01 00:00:00.000000 semantha_sdk-4.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11545 2022-12-09 10:06:55.386837 semantha_sdk-5.2.0/LICENSE
+-rw-r--r--   0        0        0     1631 2023-05-22 16:40:37.048488 semantha_sdk-5.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7644 2023-05-22 17:43:51.933450 semantha_sdk-5.2.0/README.md
+-rw-r--r--   0        0        0     1288 2023-05-11 17:26:57.327736 semantha_sdk-5.2.0/semantha_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 17:26:57.329739 semantha_sdk-5.2.0/semantha_sdk/api/__init__.py
+-rw-r--r--   0        0        0      930 2023-05-22 16:30:13.775000 semantha_sdk-5.2.0/semantha_sdk/api/bulk.py
+-rw-r--r--   0        0        0      729 2023-05-22 16:30:13.778000 semantha_sdk-5.2.0/semantha_sdk/api/bulk_domains.py
+-rw-r--r--   0        0        0      739 2023-05-22 16:30:13.812000 semantha_sdk-5.2.0/semantha_sdk/api/bulk_model.py
+-rw-r--r--   0        0        0     1628 2023-05-22 16:30:13.794000 semantha_sdk-5.2.0/semantha_sdk/api/bulkdomains_documentclasses.py
+-rw-r--r--   0        0        0     1493 2023-05-22 16:30:13.784000 semantha_sdk-5.2.0/semantha_sdk/api/bulkdomains_domain.py
+-rw-r--r--   0        0        0     3671 2023-05-22 16:30:13.807000 semantha_sdk-5.2.0/semantha_sdk/api/bulkdomains_referencedocuments.py
+-rw-r--r--   0        0        0     3423 2023-05-22 16:30:13.811000 semantha_sdk-5.2.0/semantha_sdk/api/bulkdomains_references.py
+-rw-r--r--   0        0        0     1191 2023-05-22 16:30:13.818000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_boostwords.py
+-rw-r--r--   0        0        0      832 2023-05-22 16:30:13.821000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_class.py
+-rw-r--r--   0        0        0     1730 2023-05-22 16:30:13.819000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_classes.py
+-rw-r--r--   0        0        0     1577 2023-05-22 16:30:13.825000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_dataproperties.py
+-rw-r--r--   0        0        0     2722 2023-05-22 16:30:13.816000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_domain.py
+-rw-r--r--   0        0        0      726 2023-05-22 16:30:13.814000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_domains.py
+-rw-r--r--   0        0        0     1509 2023-05-22 16:30:13.827000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_instances.py
+-rw-r--r--   0        0        0     1508 2023-05-22 16:30:13.831000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_metadata.py
+-rw-r--r--   0        0        0     1216 2023-05-22 16:30:13.832000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_namedentities.py
+-rw-r--r--   0        0        0     1111 2023-05-22 16:30:13.834000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_stopwords.py
+-rw-r--r--   0        0        0     1170 2023-05-22 16:30:13.836000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_synonyms.py
+-rw-r--r--   0        0        0      976 2023-05-22 16:30:13.823000 semantha_sdk-5.2.0/semantha_sdk/api/bulkmodelclass_instances.py
+-rw-r--r--   0        0        0     5667 2023-05-22 16:30:13.873000 semantha_sdk-5.2.0/semantha_sdk/api/clusters.py
+-rw-r--r--   0        0        0     1050 2023-05-22 16:30:13.837000 semantha_sdk-5.2.0/semantha_sdk/api/currentuser.py
+-rw-r--r--   0        0        0     1369 2023-05-22 16:30:13.840000 semantha_sdk-5.2.0/semantha_sdk/api/diff.py
+-rw-r--r--   0        0        0     2315 2023-05-22 16:30:13.848000 semantha_sdk-5.2.0/semantha_sdk/api/documentannotations.py
+-rw-r--r--   0        0        0     1387 2023-05-22 16:30:13.854000 semantha_sdk-5.2.0/semantha_sdk/api/documentclass.py
+-rw-r--r--   0        0        0     1823 2023-05-22 16:30:13.850000 semantha_sdk-5.2.0/semantha_sdk/api/documentclasses.py
+-rw-r--r--   0        0        0     3566 2023-05-22 16:30:13.857000 semantha_sdk-5.2.0/semantha_sdk/api/documentcomparisons.py
+-rw-r--r--   0        0        0     3497 2023-05-22 16:30:13.861000 semantha_sdk-5.2.0/semantha_sdk/api/documents.py
+-rw-r--r--   0        0        0     3947 2023-05-22 16:30:13.844000 semantha_sdk-5.2.0/semantha_sdk/api/domain.py
+-rw-r--r--   0        0        0     1013 2023-05-22 16:30:13.841000 semantha_sdk-5.2.0/semantha_sdk/api/domains.py
+-rw-r--r--   0        0        0      791 2023-05-22 16:30:13.906000 semantha_sdk-5.2.0/semantha_sdk/api/info.py
+-rw-r--r--   0        0        0     1648 2023-05-22 16:30:13.907000 semantha_sdk-5.2.0/semantha_sdk/api/languages.py
+-rw-r--r--   0        0        0     1529 2023-05-22 16:30:13.909000 semantha_sdk-5.2.0/semantha_sdk/api/model.py
+-rw-r--r--   0        0        0     1545 2023-05-22 16:30:13.914000 semantha_sdk-5.2.0/semantha_sdk/api/model_boostwords.py
+-rw-r--r--   0        0        0      762 2023-05-22 16:30:13.910000 semantha_sdk-5.2.0/semantha_sdk/api/model_datatypes.py
+-rw-r--r--   0        0        0     1524 2023-05-22 16:30:13.913000 semantha_sdk-5.2.0/semantha_sdk/api/model_domain.py
+-rw-r--r--   0        0        0      706 2023-05-22 16:30:13.911000 semantha_sdk-5.2.0/semantha_sdk/api/model_domains.py
+-rw-r--r--   0        0        0      777 2023-05-22 16:30:13.917000 semantha_sdk-5.2.0/semantha_sdk/api/model_extractortypes.py
+-rw-r--r--   0        0        0      774 2023-05-22 16:30:13.918000 semantha_sdk-5.2.0/semantha_sdk/api/model_metadatatypes.py
+-rw-r--r--   0        0        0     1514 2023-05-22 16:30:13.916000 semantha_sdk-5.2.0/semantha_sdk/api/model_synonyms.py
+-rw-r--r--   0        0        0     1107 2023-05-22 16:30:13.862000 semantha_sdk-5.2.0/semantha_sdk/api/modelclasses.py
+-rw-r--r--   0        0        0     2112 2023-05-22 16:30:13.864000 semantha_sdk-5.2.0/semantha_sdk/api/modelinstances.py
+-rw-r--r--   0        0        0     1546 2023-05-22 16:30:13.874000 semantha_sdk-5.2.0/semantha_sdk/api/namedentities.py
+-rw-r--r--   0        0        0     1494 2023-05-22 16:30:13.881000 semantha_sdk-5.2.0/semantha_sdk/api/paragraph.py
+-rw-r--r--   0        0        0      682 2023-05-22 16:30:13.880000 semantha_sdk-5.2.0/semantha_sdk/api/paragraphs.py
+-rw-r--r--   0        0        0    14477 2023-05-11 17:26:57.378270 semantha_sdk-5.2.0/semantha_sdk/api/reference_documents.py
+-rw-r--r--   0        0        0     2074 2023-05-22 16:30:13.878000 semantha_sdk-5.2.0/semantha_sdk/api/referencedocument.py
+-rw-r--r--   0        0        0     8930 2023-05-22 16:30:13.870000 semantha_sdk-5.2.0/semantha_sdk/api/referencedocuments.py
+-rw-r--r--   0        0        0     6565 2023-05-22 16:30:13.887000 semantha_sdk-5.2.0/semantha_sdk/api/references.py
+-rw-r--r--   0        0        0      789 2023-05-22 16:30:13.838000 semantha_sdk-5.2.0/semantha_sdk/api/roles.py
+-rw-r--r--   0        0        0     2113 2023-05-11 17:26:57.387783 semantha_sdk-5.2.0/semantha_sdk/api/semantha_api.py
+-rw-r--r--   0        0        0      413 2023-05-11 17:26:57.389783 semantha_sdk-5.2.0/semantha_sdk/api/semantha_endpoint.py
+-rw-r--r--   0        0        0      836 2023-05-22 16:30:13.883000 semantha_sdk-5.2.0/semantha_sdk/api/sentence.py
+-rw-r--r--   0        0        0      676 2023-05-22 16:30:13.882000 semantha_sdk-5.2.0/semantha_sdk/api/sentences.py
+-rw-r--r--   0        0        0     1379 2023-05-22 16:30:13.889000 semantha_sdk-5.2.0/semantha_sdk/api/settings.py
+-rw-r--r--   0        0        0     5389 2023-05-22 16:30:13.893000 semantha_sdk-5.2.0/semantha_sdk/api/similaritymatrix.py
+-rw-r--r--   0        0        0     4015 2023-05-22 16:30:13.895000 semantha_sdk-5.2.0/semantha_sdk/api/similaritymatrix_cluster.py
+-rw-r--r--   0        0        0      844 2023-05-22 16:30:13.875000 semantha_sdk-5.2.0/semantha_sdk/api/statistic.py
+-rw-r--r--   0        0        0      840 2023-05-22 16:30:13.899000 semantha_sdk-5.2.0/semantha_sdk/api/tag.py
+-rw-r--r--   0        0        0     1115 2023-05-22 16:30:13.900000 semantha_sdk-5.2.0/semantha_sdk/api/tag_referencedocuments.py
+-rw-r--r--   0        0        0      912 2023-05-22 16:30:13.897000 semantha_sdk-5.2.0/semantha_sdk/api/tags.py
+-rw-r--r--   0        0        0     1310 2023-05-22 16:30:13.905000 semantha_sdk-5.2.0/semantha_sdk/api/validation.py
+-rw-r--r--   0        0        0     4129 2023-05-22 16:30:14.061000 semantha_sdk-5.2.0/semantha_sdk/model/__init__.py
+-rw-r--r--   0        0        0      607 2023-05-22 16:30:14.008000 semantha_sdk-5.2.0/semantha_sdk/model/annotation_cell.py
+-rw-r--r--   0        0        0      654 2023-05-22 16:30:14.026000 semantha_sdk-5.2.0/semantha_sdk/model/annotation_page.py
+-rw-r--r--   0        0        0      546 2023-05-22 16:30:13.977000 semantha_sdk-5.2.0/semantha_sdk/model/boost_word.py
+-rw-r--r--   0        0        0      930 2023-05-22 16:30:13.985000 semantha_sdk-5.2.0/semantha_sdk/model/class_bulk.py
+-rw-r--r--   0        0        0      508 2023-05-22 16:30:14.043000 semantha_sdk-5.2.0/semantha_sdk/model/clustered_document.py
+-rw-r--r--   0        0        0      672 2023-05-22 16:30:14.005000 semantha_sdk-5.2.0/semantha_sdk/model/clustering_response.py
+-rw-r--r--   0        0        0     1139 2023-05-22 16:30:14.045000 semantha_sdk-5.2.0/semantha_sdk/model/complex_property.py
+-rw-r--r--   0        0        0      516 2023-05-22 16:30:14.034000 semantha_sdk-5.2.0/semantha_sdk/model/current_user.py
+-rw-r--r--   0        0        0      604 2023-05-22 16:30:13.967000 semantha_sdk-5.2.0/semantha_sdk/model/data_property.py
+-rw-r--r--   0        0        0      476 2023-05-22 16:30:13.978000 semantha_sdk-5.2.0/semantha_sdk/model/difference.py
+-rw-r--r--   0        0        0      519 2023-05-22 16:30:14.047000 semantha_sdk-5.2.0/semantha_sdk/model/distance.py
+-rw-r--r--   0        0        0     1213 2023-05-22 16:30:14.002000 semantha_sdk-5.2.0/semantha_sdk/model/document.py
+-rw-r--r--   0        0        0      939 2023-05-22 16:30:13.988000 semantha_sdk-5.2.0/semantha_sdk/model/document_class.py
+-rw-r--r--   0        0        0      723 2023-05-22 16:30:13.993000 semantha_sdk-5.2.0/semantha_sdk/model/document_class_bulk.py
+-rw-r--r--   0        0        0      507 2023-05-22 16:30:14.014000 semantha_sdk-5.2.0/semantha_sdk/model/document_class_node.py
+-rw-r--r--   0        0        0      628 2023-05-22 16:30:14.042000 semantha_sdk-5.2.0/semantha_sdk/model/document_cluster.py
+-rw-r--r--   0        0        0     1004 2023-05-22 16:30:14.040000 semantha_sdk-5.2.0/semantha_sdk/model/document_information.py
+-rw-r--r--   0        0        0      503 2023-05-22 16:30:14.007000 semantha_sdk-5.2.0/semantha_sdk/model/document_meta_data.py
+-rw-r--r--   0        0        0      498 2023-05-22 16:30:13.992000 semantha_sdk-5.2.0/semantha_sdk/model/document_named_entity.py
+-rw-r--r--   0        0        0      564 2023-05-22 16:30:13.971000 semantha_sdk-5.2.0/semantha_sdk/model/domain.py
+-rw-r--r--   0        0        0      447 2023-05-22 16:30:13.999000 semantha_sdk-5.2.0/semantha_sdk/model/entity.py
+-rw-r--r--   0        0        0      597 2023-05-22 16:30:14.032000 semantha_sdk-5.2.0/semantha_sdk/model/extraction_area.py
+-rw-r--r--   0        0        0      729 2023-05-22 16:30:14.028000 semantha_sdk-5.2.0/semantha_sdk/model/extraction_file.py
+-rw-r--r--   0        0        0      536 2023-05-22 16:30:14.006000 semantha_sdk-5.2.0/semantha_sdk/model/extraction_reference.py
+-rw-r--r--   0        0        0      842 2023-05-22 16:30:14.038000 semantha_sdk-5.2.0/semantha_sdk/model/features.py
+-rw-r--r--   0        0        0      512 2023-05-22 16:30:14.015000 semantha_sdk-5.2.0/semantha_sdk/model/file_reference.py
+-rw-r--r--   0        0        0      498 2023-05-22 16:30:13.958000 semantha_sdk-5.2.0/semantha_sdk/model/finding.py
+-rw-r--r--   0        0        0      524 2023-05-22 16:30:14.012000 semantha_sdk-5.2.0/semantha_sdk/model/info.py
+-rw-r--r--   0        0        0      839 2023-05-22 16:30:13.962000 semantha_sdk-5.2.0/semantha_sdk/model/instance.py
+-rw-r--r--   0        0        0      531 2023-05-22 16:30:14.013000 semantha_sdk-5.2.0/semantha_sdk/model/instance_child.py
+-rw-r--r--   0        0        0      408 2023-05-22 16:30:13.978000 semantha_sdk-5.2.0/semantha_sdk/model/label.py
+-rw-r--r--   0        0        0      474 2023-05-22 16:30:14.031000 semantha_sdk-5.2.0/semantha_sdk/model/language_detection.py
+-rw-r--r--   0        0        0      576 2023-05-22 16:30:14.035000 semantha_sdk-5.2.0/semantha_sdk/model/linked_instance.py
+-rw-r--r--   0        0        0      483 2023-05-22 16:30:13.997000 semantha_sdk-5.2.0/semantha_sdk/model/linked_value.py
+-rw-r--r--   0        0        0      582 2023-05-22 16:30:14.009000 semantha_sdk-5.2.0/semantha_sdk/model/matrix_row.py
+-rw-r--r--   0        0        0      499 2023-05-22 16:30:13.989000 semantha_sdk-5.2.0/semantha_sdk/model/meta_info_page.py
+-rw-r--r--   0        0        0      493 2023-05-22 16:30:14.048000 semantha_sdk-5.2.0/semantha_sdk/model/metadata.py
+-rw-r--r--   0        0        0      430 2023-05-22 16:30:13.990000 semantha_sdk-5.2.0/semantha_sdk/model/metadata_value.py
+-rw-r--r--   0        0        0      528 2023-05-22 16:30:13.998000 semantha_sdk-5.2.0/semantha_sdk/model/model_class.py
+-rw-r--r--   0        0        0     1482 2023-05-22 16:30:14.018000 semantha_sdk-5.2.0/semantha_sdk/model/model_instance.py
+-rw-r--r--   0        0        0      485 2023-05-22 16:30:13.981000 semantha_sdk-5.2.0/semantha_sdk/model/named_entity.py
+-rw-r--r--   0        0        0      787 2023-05-22 16:30:14.003000 semantha_sdk-5.2.0/semantha_sdk/model/page.py
+-rw-r--r--   0        0        0      528 2023-05-22 16:30:14.024000 semantha_sdk-5.2.0/semantha_sdk/model/page_content.py
+-rw-r--r--   0        0        0      948 2023-05-22 16:30:13.969000 semantha_sdk-5.2.0/semantha_sdk/model/paragraph.py
+-rw-r--r--   0        0        0      486 2023-05-22 16:30:13.965000 semantha_sdk-5.2.0/semantha_sdk/model/paragraph_update.py
+-rw-r--r--   0        0        0      493 2023-05-22 16:30:14.010000 semantha_sdk-5.2.0/semantha_sdk/model/plotly_chart.py
+-rw-r--r--   0        0        0      577 2023-05-22 16:30:13.973000 semantha_sdk-5.2.0/semantha_sdk/model/process_information.py
+-rw-r--r--   0        0        0      445 2023-05-22 16:30:14.036000 semantha_sdk-5.2.0/semantha_sdk/model/rect.py
+-rw-r--r--   0        0        0      775 2023-05-22 16:30:14.030000 semantha_sdk-5.2.0/semantha_sdk/model/reference.py
+-rw-r--r--   0        0        0      728 2023-05-22 16:30:14.046000 semantha_sdk-5.2.0/semantha_sdk/model/reference_documents_response_container.py
+-rw-r--r--   0        0        0      646 2023-05-22 16:30:13.995000 semantha_sdk-5.2.0/semantha_sdk/model/response_meta_info.py
+-rw-r--r--   0        0        0      650 2023-05-11 17:26:57.498002 semantha_sdk-5.2.0/semantha_sdk/model/semantha_entity.py
+-rw-r--r--   0        0        0      873 2023-05-22 16:30:14.023000 semantha_sdk-5.2.0/semantha_sdk/model/semantic_model.py
+-rw-r--r--   0        0        0      518 2023-05-22 16:30:13.996000 semantha_sdk-5.2.0/semantha_sdk/model/semi_super_vised_document.py
+-rw-r--r--   0        0        0      792 2023-05-22 16:30:13.976000 semantha_sdk-5.2.0/semantha_sdk/model/sentence.py
+-rw-r--r--   0        0        0     1669 2023-05-22 16:30:14.022000 semantha_sdk-5.2.0/semantha_sdk/model/settings.py
+-rw-r--r--   0        0        0      454 2023-05-22 16:30:13.979000 semantha_sdk-5.2.0/semantha_sdk/model/simple_property.py
+-rw-r--r--   0        0        0      695 2023-05-22 16:30:13.974000 semantha_sdk-5.2.0/semantha_sdk/model/smart_cluster_response_container.py
+-rw-r--r--   0        0        0      851 2023-05-22 16:30:14.011000 semantha_sdk-5.2.0/semantha_sdk/model/smart_cluster_semi_supervised_request.py
+-rw-r--r--   0        0        0      608 2023-05-22 16:30:13.970000 semantha_sdk-5.2.0/semantha_sdk/model/statistic.py
+-rw-r--r--   0        0        0      480 2023-05-22 16:30:13.991000 semantha_sdk-5.2.0/semantha_sdk/model/stop_word.py
+-rw-r--r--   0        0        0      542 2023-05-22 16:30:13.963000 semantha_sdk-5.2.0/semantha_sdk/model/synonym.py
+-rw-r--r--   0        0        0      466 2023-05-22 16:30:13.997000 semantha_sdk-5.2.0/semantha_sdk/model/table.py
+-rw-r--r--   0        0        0      565 2023-05-22 16:30:13.982000 semantha_sdk-5.2.0/semantha_sdk/model/table_instance.py
+-rw-r--r--   0        0        0      462 2023-05-22 16:30:14.033000 semantha_sdk-5.2.0/semantha_sdk/model/tag_docs.py
+-rw-r--r--   0        0        0      464 2023-05-22 16:30:13.983000 semantha_sdk-5.2.0/semantha_sdk/model/version.py
+-rw-r--r--   0        0        0       47 2023-05-11 17:26:57.519543 semantha_sdk-5.2.0/semantha_sdk/request/__init__.py
+-rw-r--r--   0        0        0      552 2023-05-11 17:26:57.521550 semantha_sdk-5.2.0/semantha_sdk/request/semantha_request.py
+-rw-r--r--   0        0        0       57 2023-05-11 17:26:57.522556 semantha_sdk-5.2.0/semantha_sdk/response/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-11 17:26:57.524555 semantha_sdk-5.2.0/semantha_sdk/response/semantha_error.py
+-rw-r--r--   0        0        0     3472 2023-05-11 17:26:57.525555 semantha_sdk-5.2.0/semantha_sdk/response/semantha_response.py
+-rw-r--r--   0        0        0       37 2023-05-11 17:26:57.527555 semantha_sdk-5.2.0/semantha_sdk/rest/__init__.py
+-rw-r--r--   0        0        0     4354 2023-05-11 17:26:57.528555 semantha_sdk-5.2.0/semantha_sdk/rest/rest_client.py
+-rw-r--r--   0        0        0     8563 1970-01-01 00:00:00.000000 semantha_sdk-5.2.0/setup.py
+-rw-r--r--   0        0        0     8322 1970-01-01 00:00:00.000000 semantha_sdk-5.2.0/PKG-INFO
```

### Comparing `semantha_sdk-4.8.1/LICENSE` & `semantha_sdk-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `semantha_sdk-4.8.1/pyproject.toml` & `semantha_sdk-5.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantha-sdk"
-version = "4.8.1"
+version = "5.2.0"
 description = "This is a python client sdk for accessing semantha (the semantic platform)"
 authors = [
     "Sebastian Weigelt <sebastian.weigelt@semantha.ai>",
     "Georg Müller <georg@semantha.ai>",
     "Tom Kaminski <tom.kaminski@semantha.ai>",
     "Timo Januschke <timo.januschke@semantha.ai>"
 ]
@@ -15,32 +15,33 @@
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "semantha_sdk"}]
 
 [tool.poetry.group.unittest]
 optional = true
 
-[tool.poetry.group.dev]
+[tool.poetry.group.build]
 optional = true
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests = "2.28.2"
+requests = "2.30.0"
 marshmallow = "3.19.0"
-marshmallow-dataclass = "8.5.12"
+marshmallow-dataclass = "8.5.14"
 pyhumps = "3.8.0"
 
 [tool.poetry.group.unittest.dependencies]
-coverage = "7.2.1"
-pytest = "7.2.1"
+coverage = "7.2.5"
+pytest = "7.3.1"
 pytest-cov = "4.0.0"
 toml = "0.10.2"
+parameterized = "^0.9.0"
 
-[tool.poetry.group.dev.dependencies]
-jupyter = "1.0.0"
+[tool.poetry.group.build.dependencies]
+pip-licenses = "4.3.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.source]]
 name = "tt-nexus-pypi-proxy"
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/__init__.py` & `semantha_sdk-5.2.0/semantha_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-4.8.1/semantha_sdk/api/current_user.py` & `semantha_sdk-5.2.0/semantha_sdk/api/tags.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,33 @@
-from __future__ import annotations
-
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.user_data import UserData, UserDataSchema
+from semantha_sdk.api.tag import TagEndpoint
 from semantha_sdk.rest.rest_client import RestClient
+from typing import List
 
 
-class CurrentUserRolesEndpoint(SemanthaAPIEndpoint):
-    """ Access role(s) information about the currently logged-in user. """
+class TagsEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! """
 
     @property
-    def _endpoint(self):
-        return self._parent_endpoint + "/roles"
-
-    def get(self) -> list[str]:
-        return self._session.get(self._endpoint).execute().as_list()
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/tags"
 
+    def get(self
+        ) -> List[str]:
+        """
+        Get tags 
+        Args:
+            
+        """
+        q_params = {}
+        return self._session.get(self._endpoint, q_params=q_params).execute().as_list()
 
-class CurrentUserEndpoint(SemanthaAPIEndpoint):
-    """ Access information about the currently logged-in user. """
 
-    def __init__(self, session: RestClient, parent_endpoint: str):
+    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
         super().__init__(session, parent_endpoint)
-        self.__roles = CurrentUserRolesEndpoint(session, self._endpoint)
 
-    @property
-    def _endpoint(self):
-        return self._parent_endpoint + "/currentuser"
 
-    @property
-    def roles(self):
-        return self.__roles
 
-    def get(self) -> UserData:
-        return self._session.get(self._endpoint).execute().to(UserDataSchema)
+    def __call__(self, tagname: str) -> TagEndpoint:
+        return TagEndpoint(self._session, self._endpoint, tagname)
+
+
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/api/diff.py` & `semantha_sdk-5.2.0/semantha_sdk/api/bulk.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-from __future__ import annotations
-
+from semantha_sdk.api.bulk_domains import BulkDomainsEndpoint
+from semantha_sdk.api.bulk_model import BulkModelEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.diff import Diff as DiffDTO, DiffSchema
+from semantha_sdk.rest.rest_client import RestClient
 
 
-class DiffEndpoint(SemanthaAPIEndpoint):
-    """ Create diffs between two texts. """
+class BulkEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! """
 
     @property
-    def _endpoint(self):
-        return self._parent_endpoint + "/diff"
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/bulk"
+
+
+    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+        super().__init__(session, parent_endpoint)
+
+        self.__domains = BulkDomainsEndpoint(session, self._endpoint)
+        self.__model = BulkModelEndpoint(session, self._endpoint)
+
 
-    def post(self, left: str, right: str) -> list[DiffDTO]:
-        """ Create a diff between two given texts.
+    @property
+    def domains(self) -> BulkDomainsEndpoint:
+        return self.__domains
+
+
+    @property
+    def model(self) -> BulkModelEndpoint:
+        return self.__model
 
-        Args:
-            left (object): One of the two texts for the diff.
-            right (object): The other text for the diff.
-        """
-
-        return self._session.post(
-            url=self._endpoint,
-            body={
-                "left": left,
-                "right": right
-            }
-        ).execute().to(DiffSchema)
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/api/domain/classes.py` & `semantha_sdk-5.2.0/semantha_sdk/api/documentclasses.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,59 @@
-from semantha_sdk import RestClient
+from semantha_sdk.api.documentclass import DocumentclassEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model import Class
-from semantha_sdk.response import SemanthaPlatformResponse
+from semantha_sdk.model.document_class import DocumentClass, DocumentClassSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient
+from typing import List
 
 
-class ClassEndpoint(SemanthaAPIEndpoint):
-    """ Endpoint for a specific class.
-
-        Allows for accessing class instances.
-    """
-
-    def __init__(self, session: RestClient, parent_endpoint: str, classid: str):
-        super().__init__(session, parent_endpoint)
-        self.__classid = classid
+class DocumentclassesEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! """
 
     @property
-    def _endpoint(self):
-        return self._parent_endpoint + f"/{self.__classid}"
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/documentclasses"
 
-    def get_instance(self):
-        """ (Not yet implemented) Get all instances of the class """
-        raise NotImplementedError("Not  yet implemented!")
-        return self.__sesssion.get(self._endpoint).execute()
-
-    def delete_instance(self):
-        """ (Not yet implemented) Delete all instances of the class """
-        raise NotImplementedError("Not  yet implemented!")
-        return self.__sesssion.delete(self._endpoint).execute()
+    def get(self
+        ) -> List[DocumentClass]:
+        """
+        Get all document classes 
+        Args:
+            
+        """
+        q_params = {}
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(DocumentClassSchema)
+
+    def post(self
+        , body: DocumentClass = None
+        ) -> DocumentClass:
+        """
+        Create one or more document classes
+        Args:
+            body (DocumentClass): 
+            
+        """
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            json=DocumentClassSchema().dump(body),
+            headers=RestClient.to_header(MediaType.JSON),
+            q_params=q_params
+        ).execute()
+        return response.to(DocumentClassSchema)
+
+
+    def delete(self) -> None:
+        """
+        Delete all document classes
+        """
+        self._session.delete(self._endpoint).execute()
 
+    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+        super().__init__(session, parent_endpoint)
 
-class ClassesEndpoint(SemanthaAPIEndpoint):
-    """ Endpoint for the classes in a domain.
 
-        References: Specific api for specific classes
 
-    """
+    def __call__(self, id: str) -> DocumentclassEndpoint:
+        return DocumentclassEndpoint(self._session, self._endpoint, id)
 
-    @property
-    def _endpoint(self):
-        return self._parent_endpoint + "/classes"
 
-    def get_classes(self) -> SemanthaPlatformResponse:
-        """ (Not yet implemented) Get all classes """
-        raise NotImplementedError("Not  yet implemented!")
-        return self._session.get(self._endpoint).execute()
-
-    def post_classes(self, classes: list[Class]) -> SemanthaPlatformResponse:
-        """ (Not yet implemented) Create one or more classes """
-        raise NotImplementedError("Not  yet implemented!")
-        body = [_class.data for _class in classes]
-        return self._session.post(self._endpoint, ).execute()
-
-    def delete_classes(self) -> SemanthaPlatformResponse:
-        """ (Not yet implemented) Delete all classes """
-        raise NotImplementedError("Not  yet implemented!")
-        return self._session.delete(self._endpoint).execute()
-
-    def get_class(self, classid: str):
-        """ (Not yet implemented) Get a specific class by id """
-        raise NotImplementedError("Not  yet implemented!")
-        return ClassEndpoint(self._session, self._endpoint, classid)
-
-    def put_class(self, _class: Class):
-        """ (Not yet implemented) Add a given class """
-        raise NotImplementedError("Not  yet implemented!")
-        body = _class.data
-        return self._session.put(self._endpoint, body).execute()
-
-    def delete_class(self, classid: str):
-        """ (Not yet implemented) Delete a class given its class id """
-        raise NotImplementedError("Not  yet implemented!")
-        return self._session.delete(self._endpoint + f"/{classid}").execute()
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/api/domain/document_annotations.py` & `semantha_sdk-5.2.0/semantha_sdk/api/documentannotations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 from io import IOBase
-from typing import Optional
-
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.model.document import Document, DocumentSchema
+from semantha_sdk.rest.rest_client import MediaType
+from semantha_sdk.rest.rest_client import RestClient
+
 
+class DocumentannotationsEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! """
 
-class DocumentAnnotationsEndpoint(SemanthaAPIEndpoint):
     @property
-    def _endpoint(self):
+    def _endpoint(self) -> str:
         return self._parent_endpoint + "/documentannotations"
 
-    def post(
-            self,
-            file: IOBase,
-            document: Optional[Document] = None,
-            similaritythreshold: Optional[float] = None,
-            synonymousthreshold: Optional[float] = None,
-            marknomatch: Optional[bool] = None,
-            withreferencetext: Optional[bool] = None
-    ):
-        """ (Not yet implemented) Download the original input document with the referenced document/library matches as
-        annotated comments.
-
+    def post(self
+        , file: IOBase = None
+        , document: Document = None
+        , similaritythreshold: float = None
+        , synonymousthreshold: float = None
+        , marknomatch: bool = None
+        , withreferencetext: bool = None
+        ) -> IOBase:
+        """
+        Download the original input document with the referenced document/library matches as annotated comments
         Args:
             file (IOBase): Input document (left document).
-            document (Document): ...
-            similaritythreshold (float): Threshold for the similarity score.
-                semantha will not deliver results with a sentence score lower than the threshold.
-                In general, the higher the threshold, the more precise the results.
+            document (Document): 
+            similaritythreshold (float): Threshold for the similarity score. semantha will not deliver results with a sentence score lower than the threshold.
+        In general, the higher the threshold, the more precise the results.
             synonymousthreshold (float): Threshold for good matches.
-            marknomatch (bool): Marks paragraphs that have not matched.
-            withreferencetext (bool): Provide the reference text in the result JSON.
-                If set to false, you have to query the library to resolve the references yourself.
+            marknomatch (bool): Marks the paragraphs that have not matched
+            withreferencetext (bool): Provide the reference text in the result JSON. If set to false, you have to query the library to resolve the references yourself.
+            
         """
-        document = DocumentSchema().dumps(document)
-
-        return self._session.post(
-            self._endpoint,
+        q_params = {}
+        response = self._session.post(
+            url=self._endpoint,
+            
             body={
+            
                 "file": file,
                 "document": document,
                 "similaritythreshold": similaritythreshold,
                 "synonymousthreshold": synonymousthreshold,
                 "marknomatch": marknomatch,
                 "withreferencetext": withreferencetext
-            }
+            },
+            
+            headers=RestClient.to_header(MediaType.XLSX),
+            q_params=q_params
         )
+
+
+    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+        super().__init__(session, parent_endpoint)
+
+
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/api/domain/documents.py` & `semantha_sdk-5.2.0/semantha_sdk/api/paragraph.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,43 @@
-from __future__ import annotations
-
-from io import IOBase
-from typing import Optional
-
-from semantha_sdk import RestClient
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.document import DocumentSchema
+from semantha_sdk.model.paragraph import Paragraph, ParagraphSchema
+from semantha_sdk.model.paragraph_update import ParagraphUpdate, ParagraphUpdateSchema
+from semantha_sdk.rest.rest_client import RestClient
 
 
-class DocumentEndpoint(SemanthaAPIEndpoint):
-
-    def __init__(self, session: RestClient, parent_endpoint: str, id: str):
-        super().__init__(session, parent_endpoint)
-        self._id = id
+class ParagraphEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! """
 
     @property
-    def _endpoint(self):
-        return self._parent_endpoint + "/" + self._id
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + f"/{self._id}"
 
-    def get(self):
-        return self._session.get(self._endpoint).execute().to(DocumentSchema)
-
-
-class DocumentsEndpoint(SemanthaAPIEndpoint):
-    """ /api/{domainname}/documents endpoint. """
+    def get(self
+        ) -> Paragraph:
+        """
+        Get paragraph by ID 
+        Args:
+            
+        """
+        q_params = {}
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(ParagraphSchema)
 
-    @property
-    def _endpoint(self):
-        return self._parent_endpoint + "/documents"
+    def patch(self, paragraphupdate: ParagraphUpdate) -> ParagraphUpdate:
+        """
+        Update a specific paragraph of a specific reference document of the library
+        """
+        return self._session.patch(
+            url=self._endpoint,
+            json=ParagraphUpdateSchema().dump(paragraphupdate)
+        ).execute().to(ParagraphSchema)
 
-    def post(
-            self,
-            file: Optional[IOBase] = None,
-            type: Optional[str] = None,
-            documenttype: Optional[str] = None,
-            withareas: Optional[bool] = None,
-            mode: Optional[str] = None,
-            withparagraphtype: Optional[bool] = None
-    ) -> list[DocumentEndpoint]:
-        """ Create a document model
 
-        Args:
+    def delete(self) -> None:
+        """
+        Delete a specific paragraph of a specific reference document of the library
+        """
+        self._session.delete(self._endpoint).execute()
 
-            file (IOBase): Input document (as file)
-            type (str): Enum: "similarity" "extraction". Choose the structure of a document
-                for similarity or extraction. The type depends on the Use Case you're in.
-            documenttype (str): Specifies the document type that is to be used by semantha
-                when reading the uploaded PDF document.
-            withareas (bool): Gives back the coordinates of referenced area.
-            mode (str): 'paragraph' or 'sentence'
-            withparagraphtype (bool): The type of the paragraph, for example heading, text.
-        """
-        return self._session.post(
-            self._endpoint,
-            body={
-                "file": file,
-                "type": type,
-                "documenttype": documenttype,
-                "withareas": withareas,
-                "mode": mode,
-                "withparagraphtype": withparagraphtype
-            }
-        ).execute().to(DocumentSchema)
+    def __init__(self, session: RestClient, parent_endpoint: str, id: str) -> None:
+        super().__init__(session, parent_endpoint)
+        self._id=id
 
-    def __call__(self, id: str):
-        return DocumentEndpoint(self._session, self._endpoint, id)
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/api/domain/model.py` & `semantha_sdk-5.2.0/semantha_sdk/api/model_domain.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,50 @@
-from semantha_sdk import RestClient
-from semantha_sdk.api.model.boost_words import BoostwordsEndpoint
-from semantha_sdk.api.model.synonyms import SynonymsEndpoint
+from io import IOBase
+from semantha_sdk.api.model_boostwords import ModelBoostwordsEndpoint
+from semantha_sdk.api.model_synonyms import ModelSynonymsEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
+from semantha_sdk.rest.rest_client import RestClient
 
 
-class DomainModelEndpoint(SemanthaAPIEndpoint):
-    """ Endpoint for a specific domain.
+class ModelDomainEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! """
 
-        References: attributes, backups, boostwords, classes, extractors,
-            formatters, instances, metadata, namedentities, regexes, relations,
-            rulefunctions, rules, synonyms
-    """
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + f"/{self._domainname}"
+
+    def get(self
+        ) -> IOBase:
+        """
+        Get a domain by domainname 
+        Args:
+            
+        """
+        q_params = {}
+        return self._session.get(self._endpoint, q_params=q_params)
+
+    def patch(self, iobase: IOBase) -> IOBase:
+        """
+        Update a domain by domainname
+        """
+        return self._session.patch(
+            url=self._endpoint,
+            json=iobase
+        )
 
-    def __init__(self, session: RestClient, parent_endpoint: str, domain_name: str):
+
+    def __init__(self, session: RestClient, parent_endpoint: str, domainname: str) -> None:
         super().__init__(session, parent_endpoint)
-        self._domain_name = domain_name
-        self.__boostwords = BoostwordsEndpoint(session, self._endpoint)
-        self.__synonyms = SynonymsEndpoint(session, self._endpoint)
+        self._domainname=domainname
+        self.__boostwords = ModelBoostwordsEndpoint(session, self._endpoint)
+        self.__synonyms = ModelSynonymsEndpoint(session, self._endpoint)
 
-    @property
-    def _endpoint(self):
-        return self._parent_endpoint + f"/{self._domain_name}"
 
     @property
-    def boostwords(self) -> BoostwordsEndpoint:
+    def boostwords(self) -> ModelBoostwordsEndpoint:
         return self.__boostwords
 
-    @property
-    def synonyms(self) -> SynonymsEndpoint:
-        return self.__synonyms
 
-
-class DomainModelsEndpoint(SemanthaAPIEndpoint):
-    """
-        References:
-            Specific domains by name
-    """
     @property
-    def _endpoint(self):
-        return self._parent_endpoint + "/domains"
+    def synonyms(self) -> ModelSynonymsEndpoint:
+        return self.__synonyms
 
-    def __call__(self, domain_name: str) -> DomainModelEndpoint:
-        # Returns a Domain object for the given domainname, throws error if id doesn't exist
-        return DomainModelEndpoint(self._session, self._endpoint, domain_name)
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/api/domain/reference_documents.py` & `semantha_sdk-5.2.0/semantha_sdk/api/reference_documents.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
 from io import IOBase
 from typing import List, Optional
 
 from semantha_sdk import RestClient
-from semantha_sdk.api.domain.cluster import DocumentClusterEndpoint
-from semantha_sdk.api.model.named_entities import NamedEntitiesEndpoint
-from semantha_sdk.api.domain.statistics import StatisticsEndpoint
+from semantha_sdk.api.clusters import ClustersEndpoint
+from semantha_sdk.api.document_named_entities import DocumentNamedEntitiesEndpoint
+from semantha_sdk.api.statistic import StatisticEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.model import Paragraph
 from semantha_sdk.model.document import DocumentSchema, Document
-from semantha_sdk.model.paragraph import ParagraphSchema, PatchParagraph
-from semantha_sdk.model.reference_document import DocumentInformationSchema, ReferenceDocuments, \
-    ReferenceDocumentsSchema, DocumentInformation
+from semantha_sdk.model.paragraph import Paragraph, ParagraphSchema
+from semantha_sdk.model.document_information import DocumentInformation, DocumentInformationSchema
+from semantha_sdk.model.reference_documents_response_container import ReferenceDocumentsResponseContainer, \
+    ReferenceDocumentsResponseContainerSchema
 from semantha_sdk.model.sentence import Sentence, SentenceSchema
 
 
 class ReferenceDocumentEndpoint(SemanthaAPIEndpoint):
     class ReferenceDocumentParagraphs(SemanthaAPIEndpoint):
 
         @property
@@ -40,15 +41,15 @@
                 """ Get the paragraph of the reference document """
                 return self._session.get(self._endpoint).execute().to(ParagraphSchema)
 
             def delete(self):
                 """ Delete the paragraph of the reference document """
                 self._session.delete(self._endpoint).execute()
 
-            def patch(self, update: PatchParagraph) -> Paragraph:
+            def patch(self, update: Paragraph) -> Paragraph:
                 """Update the paragraph of the reference document
                 Args:
                     update (Paragraph): (partial) paragraph information that should be updated. Please provide an
                                         instance of Paragraph (semantha_sdk.model.Paragraphs.Paragraph). E.g. to alter
                                         (only) the text of the paragraph you can use something like
                                         Paragraph({"text": "updated text"}).
                 """
@@ -124,17 +125,17 @@
         ).execute().to(DocumentInformationSchema)
 
 
 class ReferenceDocumentsEndpoint(SemanthaAPIEndpoint):
 
     def __init__(self, session: RestClient, parent_endpoint: str):
         super().__init__(session, parent_endpoint)
-        self.__statistics = StatisticsEndpoint(session, self._endpoint)
-        self.__named_entities = NamedEntitiesEndpoint(session, self._endpoint)
-        self.__document_clusters = DocumentClusterEndpoint(session, self._endpoint)
+        self.__statistics = StatisticEndpoint(session, self._endpoint)
+        self.__named_entities = DocumentNamedEntitiesEndpoint(session, self._endpoint)
+        self.__document_clusters = ClustersEndpoint(session, self._endpoint)
 
     @property
     def _endpoint(self):
         return self._parent_endpoint + "/referencedocuments"
 
     @property
     def statistic(self):
@@ -157,15 +158,15 @@
             name: Optional[str] = None,
             createdbefore: Optional[int] = None,
             createdafter: Optional[int] = None,
             metadata: Optional[str] = None,
             comment: Optional[str] = None,
             sort: Optional[str] = None,
             fields: Optional[str] = None
-            ) -> ReferenceDocuments:
+            ) -> ReferenceDocumentsResponseContainer:
         """ Get reference documents (library documents)
 
         If no parameters are set all reference documents are returned.
         However, the result set can be filtered (filter_*), sorted (sort_by), sliced (offset AND limit) and the returned
         attributes/fields can be manipulated (return_fields) to reduce the size of the response.
         Note that some filters and sorting can only be used iff slicing is used (offset and limit).
 
@@ -233,15 +234,15 @@
             if metadata is not None:
                 q_params["metadata"] = metadata
             if comment is not None:
                 q_params["comment"] = comment
             if sort is not None:
                 q_params["sort"] = sort
 
-        return self._session.get(self._endpoint, q_params=q_params).execute().to(ReferenceDocumentsSchema)
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(ReferenceDocumentsResponseContainerSchema)
 
     def delete(self):
         """ Delete all reference documents """
         self._session.delete(self._endpoint).execute()
 
     def post(
             self,
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/api/domain/tags.py` & `semantha_sdk-5.2.0/semantha_sdk/api/namedentities.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,38 @@
-from __future__ import annotations
-
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.reference_document import ReferenceDocumentsSchema
-
+from semantha_sdk.model.document_named_entity import DocumentNamedEntity, DocumentNamedEntitySchema
+from semantha_sdk.rest.rest_client import RestClient
+from typing import List
 
-class DomainTagEndpoint(SemanthaAPIEndpoint):
-    def __init__(self, session, endpoint, tag: str):
-        SemanthaAPIEndpoint.__init__(self, session, endpoint)
-        self.tag = tag
 
-    @property
-    def _endpoint(self):
-        return f"{self._parent_endpoint}/{self.tag}"
+class NamedentitiesEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! """
 
     @property
-    def referencedocuments(self):
-        class ReferenceDocumentsForTag(SemanthaAPIEndpoint):
-            @property
-            def _endpoint(self):
-                return f"{self._parent_endpoint}/referencedocuments"
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/namedentities"
 
-            def get(self):
-                return self._session.get(self._endpoint).execute().as_list()
+    def get(self
+        , tags: str = None
+        , documentclassids: str = None
+        ) -> List[DocumentNamedEntity]:
+        """
+        Get all custom entities 
+        Args:
+            tags (str): List of tags to filter the reference library. You can combine the tags using a comma (OR) and using a plus sign (AND).
+            documentclassids (str): List of documentclass IDs for the target. The limit here is 1000 IDs.
+        The IDs are passed as a JSON array.
+        This does not apply on the GET referencedocuments call. Here the ids are separated with a comma.
+            
+        """
+        q_params = {}
+        if tags is not None:
+            q_params["tags"] = tags
+        if documentclassids is not None:
+            q_params["documentclassids"] = documentclassids
+        return self._session.get(self._endpoint, q_params=q_params).execute().to(DocumentNamedEntitySchema)
 
-            def delete(self):
-                return self._session.delete(self._endpoint)
 
-        return ReferenceDocumentsForTag(self._session, self._endpoint)
-
-class DomainTagsEndpoint(SemanthaAPIEndpoint):
-
-    @property
-    def _endpoint(self):
-        return self._parent_endpoint + "/tags"
+    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+        super().__init__(session, parent_endpoint)
 
-    def get(self) -> list[str]:
-        """Get all tags that are defined for the domain"""
-        return self._session.get(self._endpoint).execute().as_list()
 
-    def __call__(self, tag: str):
-        return DomainTagEndpoint(self._session, self._endpoint, tag)
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/api/info.py` & `semantha_sdk-5.2.0/semantha_sdk/api/bulkmodel_domains.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-from __future__ import annotations
-
+from semantha_sdk.api.bulkmodel_domain import BulkmodelDomainEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.info import VersionInfo as VersionInfo, VersionInfoSchema
+from semantha_sdk.rest.rest_client import RestClient
 
 
-class InfoEndpoint(SemanthaAPIEndpoint):
-    """ Returns API version information. """
+class BulkmodelDomainsEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! """
 
     @property
-    def _endpoint(self):
-        return self._parent_endpoint + "/info"
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/domains"
+
+
+    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+
+    def __call__(self, domainname: str) -> BulkmodelDomainEndpoint:
+        return BulkmodelDomainEndpoint(self._session, self._endpoint, domainname)
 
-    def get(self) -> VersionInfo:
-        """ 
-        """
 
-        return self._session.get(self._endpoint).execute().to(VersionInfoSchema)
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/api/model/__init__.py` & `semantha_sdk-5.2.0/semantha_sdk/api/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,44 @@
-from semantha_sdk.api.domain.model import DomainModelsEndpoint, DomainModelEndpoint
-from semantha_sdk.api.model.extractor_types import ExtractorTypesEndpoint
-from semantha_sdk.api.metadata_types import MetadataTypesEndpoint
+from semantha_sdk.api.model_datatypes import ModelDatatypesEndpoint
+from semantha_sdk.api.model_domains import ModelDomainsEndpoint
+from semantha_sdk.api.model_extractortypes import ModelExtractortypesEndpoint
+from semantha_sdk.api.model_metadatatypes import ModelMetadatatypesEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
 from semantha_sdk.rest.rest_client import RestClient
 
-from typing import List
 
 class ModelEndpoint(SemanthaAPIEndpoint):
-    """
-        api/model endpoint
+    """ author semantha, this is a generated class do not change manually! """
+
+    @property
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/model"
 
-        References: datatypes, domains, exctractortypes, metadatatypes
-    """
 
-    def __init__(self, session: RestClient, parent_endpoint: str):
+    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
         super().__init__(session, parent_endpoint)
-        self.__model_domains = DomainModelsEndpoint(session, self._endpoint)
-        self.__extractor_types = ExtractorTypesEndpoint(session, self._endpoint)
-        self.__metadata_types = MetadataTypesEndpoint(session, self._endpoint)
 
-    @property
-    def _endpoint(self):
-        return self._parent_endpoint + "/model"
+        self.__datatypes = ModelDatatypesEndpoint(session, self._endpoint)
+        self.__domains = ModelDomainsEndpoint(session, self._endpoint)
+        self.__extractortypes = ModelExtractortypesEndpoint(session, self._endpoint)
+        self.__metadatatypes = ModelMetadatatypesEndpoint(session, self._endpoint)
+
 
     @property
-    def domains(self):
-        return self.__model_domains
+    def datatypes(self) -> ModelDatatypesEndpoint:
+        return self.__datatypes
+
 
     @property
-    def extractortypes(self):
-        return self.__extractor_types
+    def domains(self) -> ModelDomainsEndpoint:
+        return self.__domains
+
 
     @property
-    def metadatatypes(self):
-        return self.__metadata_types
+    def extractortypes(self) -> ModelExtractortypesEndpoint:
+        return self.__extractortypes
 
-    def datatypes(self) -> List[str]:
-        endpoint = f"{self._endpoint}/datatypes"
-        return self._session.get(endpoint).execute().as_list()
 
-    def __call__(self, domain: str) -> DomainModelEndpoint:
-        return DomainModelEndpoint(self._session, self._endpoint, domain)
+    @property
+    def metadatatypes(self) -> ModelMetadatatypesEndpoint:
+        return self.__metadatatypes
+
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/api/model/named_entities.py` & `semantha_sdk-5.2.0/semantha_sdk/api/paragraphs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from __future__ import annotations
-
-from typing import Optional
-
+from semantha_sdk.api.paragraph import ParagraphEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.named_entity import NamedEntity, NamedEntitySchema
+from semantha_sdk.rest.rest_client import RestClient
 
 
-class NamedEntitiesEndpoint(SemanthaAPIEndpoint):
+class ParagraphsEndpoint(SemanthaAPIEndpoint):
+    """ author semantha, this is a generated class do not change manually! """
 
     @property
-    def _endpoint(self):
-        return self._parent_endpoint + "/namedentities"
+    def _endpoint(self) -> str:
+        return self._parent_endpoint + "/paragraphs"
+
+
+    def __init__(self, session: RestClient, parent_endpoint: str) -> None:
+        super().__init__(session, parent_endpoint)
+
+
+
+    def __call__(self, id: str) -> ParagraphEndpoint:
+        return ParagraphEndpoint(self._session, self._endpoint, id)
+
 
-    def get(self) -> Optional[list[NamedEntity]]:
-        """ Get all named entities (aka custom entities) that were extracted from the reference documents.
-        Note: Might be None iff no named entities have been extracted.
-        """
-        res = self._session.get(self._endpoint).execute()
-        if res.content_is_empty():
-            return None
-        return self._session.get(self._endpoint).execute().to(NamedEntitySchema)
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/api/semantha_api.py` & `semantha_sdk-5.2.0/semantha_sdk/api/semantha_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 from io import IOBase
 
-from semantha_sdk.api.current_user import CurrentUserEndpoint
+from semantha_sdk.api.currentuser import CurrentuserEndpoint
 from semantha_sdk.api.diff import DiffEndpoint
 from semantha_sdk.api.info import InfoEndpoint
-from semantha_sdk.api.domain import DomainsEndpoint
+from semantha_sdk.api.languages import LanguagesEndpoint
+from semantha_sdk.api.domains import DomainsEndpoint
 from semantha_sdk.api.model import ModelEndpoint
 from semantha_sdk.api.semantha_endpoint import SemanthaAPIEndpoint
-from semantha_sdk.model.language import LanguageSchema
+from semantha_sdk.model.language_detection import LanguageDetectionSchema
 from semantha_sdk.rest.rest_client import RestClient
 
 
 class SemanthaAPI(SemanthaAPIEndpoint):
     """ Entry point to the Semantha API.
 
         References the /currentuser, /domains, /info, /model, /languages and /diff endpoints.
@@ -20,26 +21,27 @@
         Note:
             The __init__ method is not meant to be invoked directly
             use `semantha_sdk.login()` with your credentials instead.
     """
 
     def __init__(self, session: RestClient, parent_endpoint: str, endpoint_without_version: str):
         super().__init__(session, parent_endpoint)
-        self.__current_user = CurrentUserEndpoint(session, self._endpoint)
+        self.__current_user = CurrentuserEndpoint(session, self._endpoint)
         self.__diff = DiffEndpoint(session, self._endpoint)
         self.__domains = DomainsEndpoint(session, self._endpoint)
         self.__model = ModelEndpoint(session, self._endpoint)
         self.__info = InfoEndpoint(session, endpoint_without_version)
+        self.__languages = LanguagesEndpoint(session, self._endpoint);
 
     @property
     def _endpoint(self):
         return self._parent_endpoint
 
     @property
-    def currentuser(self) -> CurrentUserEndpoint:
+    def currentuser(self) -> CurrentuserEndpoint:
         return self.__current_user
 
     @property
     def domains(self) -> DomainsEndpoint:
         return self.__domains
 
     @property
@@ -50,12 +52,10 @@
     def model(self) -> ModelEndpoint:
         return self.__model
 
     @property
     def info(self) -> InfoEndpoint:
         return self.__info
 
-    def languages(self, file: IOBase):
-        endpoint = f"{self._endpoint}/languages"
-        return self._session.post(endpoint, body={
-            "file": file
-        }).execute().to(LanguageSchema)
+    @property
+    def languages(self) -> LanguagesEndpoint:
+        return self.__languages
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/model/cls.py` & `semantha_sdk-5.2.0/semantha_sdk/model/model_class.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,18 @@
-from __future__ import annotations
-
 from dataclasses import dataclass
-from typing import List
 
 from marshmallow_dataclass import class_schema
 
-from semantha_sdk.model.data_type import DataType
-from semantha_sdk.model.label import Label
-from semantha_sdk.model.metadata import Metadata
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-
-@dataclass(frozen=True)
-class Class(SemanthaModelEntity):
-    id: str
-    name: str
-    read_only: bool
-    functional: bool
-    labels: List[Label]
-    metadata: List[Metadata]
-    comment: str
-    datatype: DataType
-    attribute_ids: List[str]
-    relevant_for_relation: bool
-    object_property_id: str
-    parent_id: str
+from typing import List, Optional
 
 
-ClassSchema = class_schema(Class, base_schema=SemanthaSchema)
+@dataclass(frozen=True)
+class ModelClass(SemanthaModelEntity):
+	""" author semantha, this is a generated class do not change manually! """
+	name: Optional[str]
+	label: Optional[str]
+	sub_model_classes: Optional[List["ModelClass"]]
+	
+	
+ModelClassSchema = class_schema(ModelClass, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/model/document.py` & `semantha_sdk-5.2.0/semantha_sdk/model/reference_documents_response_container.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-from __future__ import annotations
-
 from dataclasses import dataclass
-from typing import Optional, List
 
 from marshmallow_dataclass import class_schema
 
-from semantha_sdk.model.page import Page
-from semantha_sdk.model.reference import Reference
-from semantha_sdk.model.reference_document import DocumentInformation
-from semantha_sdk.model.semantha_entity import SemanthaSchema
-
+from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-@dataclass(frozen=True)
-class Document(DocumentInformation):
-    pages: Optional[List[Page]] = None
-    references: Optional[List[Reference]] = None
-    image_pages: Optional[str] = None
+from semantha_sdk.model.document_information import DocumentInformation
+from semantha_sdk.model.response_meta_info import ResponseMetaInfo
+from typing import List, Optional
 
-    def __hash__(self):
-        return hash(self.id)
 
-
-DocumentSchema = class_schema(Document, base_schema=SemanthaSchema)
+@dataclass(frozen=True)
+class ReferenceDocumentsResponseContainer(SemanthaModelEntity):
+	""" author semantha, this is a generated class do not change manually! """
+	meta: Optional[ResponseMetaInfo]
+	data: Optional[List[DocumentInformation]]
+	
+	
+ReferenceDocumentsResponseContainerSchema = class_schema(ReferenceDocumentsResponseContainer, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/model/extraction_file.py` & `semantha_sdk-5.2.0/semantha_sdk/model/instance_child.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
 
-from semantha_sdk.model import SemanthaModelEntity
-from semantha_sdk.model.document import Document
-from semantha_sdk.model.semantha_entity import SemanthaSchema
+from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
+from typing import Optional
 
-@dataclass(frozen=True)
-class ExtractionFile(SemanthaModelEntity):
-    id: str
-    external_id: str
-    name: str
-    processed: bool
-    binary: str
-    document_extractor: str
-    document: Document
 
-ExtractionFileSchema = class_schema(ExtractionFile, base_schema=SemanthaSchema)
+@dataclass(frozen=True)
+class InstanceChild(SemanthaModelEntity):
+	""" author semantha, this is a generated class do not change manually! """
+	id: Optional[str]
+	name: str
+	relation_id: str
+	class_name: Optional[str]
+	class_id: str
+	
+	
+InstanceChildSchema = class_schema(InstanceChild, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/model/model_instance.py` & `semantha_sdk-5.2.0/semantha_sdk/model/model_instance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 from dataclasses import dataclass
-from typing import List, Any, Optional
 
 from marshmallow_dataclass import class_schema
 
-from semantha_sdk.model import SemanthaModelEntity, Metadata, Label
+from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
+
 from semantha_sdk.model.complex_property import ComplexProperty
 from semantha_sdk.model.extraction_reference import ExtractionReference
 from semantha_sdk.model.file_reference import FileReference
 from semantha_sdk.model.finding import Finding
+from semantha_sdk.model.label import Label
 from semantha_sdk.model.linked_instance import LinkedInstance
-from semantha_sdk.model.semantha_entity import SemanthaSchema
+from semantha_sdk.model.metadata import Metadata
 from semantha_sdk.model.simple_property import SimpleProperty
+from typing import List, Optional
 
 
 @dataclass(frozen=True)
 class ModelInstance(SemanthaModelEntity):
-    id: Optional[str]
-    name: Optional[str]
-    class_id: Optional[str]
-    relation_id: Optional[str]
-    type: Optional[str]
-    ignore_import: Optional[bool]
-    simple_properties: Optional[List[SimpleProperty]]
-    metadata: Optional[List[Metadata]]
-    qualified_name: Optional[str]
-    extractor_class_ids: Optional[List[str]]
-    label: Optional[str]
-    labels: Optional[List[Label]]
-    file: Optional[FileReference]
-    complex_properties: Optional[List[ComplexProperty]]
-    findings: Optional[List[Finding]]
-    references: Optional[List[ExtractionReference]]
-    linked_instances: Optional[List[LinkedInstance]]
-
-ModelInstanceSchema = class_schema(ModelInstance, base_schema=SemanthaSchema)
+	""" author semantha, this is a generated class do not change manually! """
+	id: Optional[str]
+	name: str
+	class_id: str
+	relation_id: Optional[str]
+	type: Optional[str]
+	ignore_import: Optional[bool]
+	simple_properties: Optional[List[SimpleProperty]]
+	metadata: Optional[List[Metadata]]
+	qualified_name: Optional[str]
+	extractor_class_ids: Optional[List[str]]
+	label: Optional[str]
+	labels: Optional[List[Label]]
+	file: Optional[FileReference]
+	complex_properties: Optional[List[ComplexProperty]]
+	findings: Optional[List[Finding]]
+	references: Optional[List[ExtractionReference]]
+	linked_instances: Optional[List[LinkedInstance]]
+	
+	
+ModelInstanceSchema = class_schema(ModelInstance, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/model/page.py` & `semantha_sdk-5.2.0/semantha_sdk/model/current_user.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,18 @@
-from __future__ import annotations
-
 from dataclasses import dataclass
 
 from marshmallow_dataclass import class_schema
-from typing import Optional, List
 
-from semantha_sdk.model.paragraph import Paragraph
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
-
-@dataclass(frozen=True)
-class PageContent(SemanthaModelEntity):
-    paragraphs: Optional[List[Paragraph]]
-
-
-PageContentSchema = class_schema(PageContent, base_schema=SemanthaSchema)
+from typing import List, Optional
 
 
 @dataclass(frozen=True)
-class Page(SemanthaModelEntity):
-    contents: List[PageContent]
-
-
-PageSchema = class_schema(Page, base_schema=SemanthaSchema)
+class CurrentUser(SemanthaModelEntity):
+	""" author semantha, this is a generated class do not change manually! """
+	name: Optional[str]
+	valid_until: Optional[int]
+	roles: Optional[List[str]]
+	
+	
+CurrentUserSchema = class_schema(CurrentUser, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/model/reference.py` & `semantha_sdk-5.2.0/semantha_sdk/model/reference.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from __future__ import annotations
-
 from dataclasses import dataclass
-from typing import Optional, Dict
 
 from marshmallow_dataclass import class_schema
 
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
 
+from typing import Dict, Optional
+
 
 @dataclass(frozen=True)
 class Reference(SemanthaModelEntity):
-    document_id: str
-    similarity: float
-    color: Optional[str]
-    document_name: Optional[str]
-    page_number: Optional[int]
-    paragraph_id: Optional[str]
-    sentence_id: Optional[str]
-    text: Optional[str]
-    context: Optional[Dict[str, str]]
-    type: Optional[str]
-    comment: Optional[str]
-    has_opposite_meaning: Optional[bool]
-
-
+	""" author semantha, this is a generated class do not change manually! """
+	document_id: Optional[str]
+	document_name: Optional[str]
+	page_number: Optional[int]
+	paragraph_id: Optional[str]
+	sentence_id: Optional[str]
+	similarity: Optional[float]
+	text: Optional[str]
+	context: Optional[Dict[str, str]]
+	type: Optional[str]
+	color: Optional[str]
+	comment: Optional[str]
+	has_opposite_meaning: Optional[bool]
+	
+	
 ReferenceSchema = class_schema(Reference, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/model/semantha_entity.py` & `semantha_sdk-5.2.0/semantha_sdk/model/semantha_entity.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-4.8.1/semantha_sdk/model/semantic_model.py` & `semantha_sdk-5.2.0/semantha_sdk/model/semantic_model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from dataclasses import dataclass
-from typing import Any, List
 
 from marshmallow_dataclass import class_schema
 
-from semantha_sdk.model import SemanthaModelEntity
+from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
+
 from semantha_sdk.model.extraction_file import ExtractionFile
 from semantha_sdk.model.model_instance import ModelInstance
 from semantha_sdk.model.process_information import ProcessInformation
-from semantha_sdk.model.semantha_entity import SemanthaSchema
 from semantha_sdk.model.table_instance import TableInstance
+from typing import List, Optional
 
 
 @dataclass(frozen=True)
 class SemanticModel(SemanthaModelEntity):
-    files: List[ExtractionFile]
-    instances: List[ModelInstance]
-    tables: List[TableInstance]
-    process_information: ProcessInformation
-
-
-SemanticModelSchema = class_schema(SemanticModel, base_schema=SemanthaSchema)
+	""" author semantha, this is a generated class do not change manually! """
+	files: Optional[List[ExtractionFile]]
+	instances: Optional[List[ModelInstance]]
+	tables: Optional[List[TableInstance]]
+	process_information: Optional[ProcessInformation]
+	
+	
+SemanticModelSchema = class_schema(SemanticModel, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/model/sentence.py` & `semantha_sdk-5.2.0/semantha_sdk/model/paragraph.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,30 @@
-from __future__ import annotations
-
 from dataclasses import dataclass
-from typing import Optional, List
 
 from marshmallow_dataclass import class_schema
 
-from semantha_sdk.model.named_entity import NamedEntity
-from semantha_sdk.model.reference import Reference
 from semantha_sdk.model.semantha_entity import SemanthaModelEntity, SemanthaSchema
-from semantha_sdk.model.area import Area
-
 
-@dataclass(frozen=True)
-class Sentence(SemanthaModelEntity):
-    id: str
-    text: str
-    document_name: Optional[str]
-    named_entities: Optional[List[NamedEntity]]
-    references: Optional[List[Reference]]
-    areas: Optional[List[Area]]
+from semantha_sdk.model.rect import Rect
+from semantha_sdk.model.reference import Reference
+from semantha_sdk.model.sentence import Sentence
+from typing import Dict, List, Optional
 
 
-SentenceSchema = class_schema(Sentence, base_schema=SemanthaSchema)
+@dataclass(frozen=True)
+class Paragraph(SemanthaModelEntity):
+	""" author semantha, this is a generated class do not change manually! """
+	text: Optional[str]
+	type: Optional[str]
+	id: Optional[str]
+	document_name: Optional[str]
+	sentences: Optional[List[Sentence]]
+	references: Optional[List[Reference]]
+	context: Optional[Dict[str, str]]
+	areas: Optional[List[Rect]]
+	comment: Optional[str]
+	verified: Optional[bool]
+	data_url_image: Optional[str]
+	references_safe: Optional[List[Reference]]
+	
+	
+ParagraphSchema = class_schema(Paragraph, base_schema=SemanthaSchema)
```

### Comparing `semantha_sdk-4.8.1/semantha_sdk/request/semantha_request.py` & `semantha_sdk-5.2.0/semantha_sdk/request/semantha_request.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-4.8.1/semantha_sdk/response/semantha_response.py` & `semantha_sdk-5.2.0/semantha_sdk/response/semantha_response.py`

 * *Files identical despite different names*

### Comparing `semantha_sdk-4.8.1/semantha_sdk/rest/rest_client.py` & `semantha_sdk-5.2.0/semantha_sdk/rest/rest_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,15 +28,18 @@
     return data
 
 
 def _filter_json(data: dict):
     data = {k: v for k, v in data.items() if v is not None}
     return data
 
-
+class MediaType:
+    XLSX = "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet"
+    JSON = "application/json"
+    
 class RestClient:
 
     def __init__(self, server_url: str, api_key: str):
         self.__server_url = server_url
         self.__api_key = api_key
 
     def __build_headers_for_json_request(self) -> dict[str, str]:
@@ -113,7 +116,10 @@
             raise ValueError("Either a body (files/form-data) or a json must be provided!")
         return self.__request("PATCH", url, files=body, json=json, params=q_params)
 
     def put(self, url: str, body: dict = None, json: dict | list = None, q_params: dict[str, str] = None) -> SemanthaRequest:
         if body is None and json is None:
             raise ValueError("Either a body (files/form-data) or a json must be provided!")
         return self.__request("PUT", url, files=body, json=json, params=q_params)
+
+    def to_header(accept_mime_type: str):
+        return {"Accept": accept_mime_type}
```

### Comparing `semantha_sdk-4.8.1/setup.py` & `semantha_sdk-5.2.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['semantha_sdk',
  'semantha_sdk.api',
- 'semantha_sdk.api.domain',
- 'semantha_sdk.api.model',
  'semantha_sdk.model',
  'semantha_sdk.request',
  'semantha_sdk.response',
  'semantha_sdk.rest']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['marshmallow-dataclass==8.5.12',
+['marshmallow-dataclass==8.5.14',
  'marshmallow==3.19.0',
  'pyhumps==3.8.0',
- 'requests==2.28.2']
+ 'requests==2.30.0']
 
 setup_kwargs = {
     'name': 'semantha-sdk',
-    'version': '4.8.1',
+    'version': '5.2.0',
     'description': 'This is a python client sdk for accessing semantha (the semantic platform)',
-    'long_description': '![](https://www.semantha.de/wp-content/uploads/semantha-inverted.svg)\n\n# semantha® SDK\n\nThe semantha SDK is a high-level REST client to access the [semantha](http://semantha.ai) API.\nThe SDK is still under development.\nAn overview of the current progress (i.e. implemented and tested resources and endpoints) may be found at the end of\nthis document (State of Development).\nThe semantha SDK is compatible with python >= 3.8.\n\n### Disclaimer\n\n**IMPORTANT:** The SDK is under development and interfaces may change at any time without notice.\nUse with caution and on own risk.\n\n### Update Note\n\nVersion 4.5.0 comes with a major restructuring of the SDK.\nAll sub-resources are directly accessible (instead of invoking getters).\nThat also means that (except for a few) all functions are plain get/post/delete/put/patch.\nFor example, in Versions < 4.5.0 a domain resource was fetched using `semantha_sdk.domains.get_one("domain_name")`.\nStarting with 4.5.0 it is `semantha_sdk.domains("domain_name")`.\nThat also means that get/post/put/patch functions return semantha model objects (and never resources), which makes usage more consistent.\n\n### Access\n\nTo access semantha\'s API you will need an API and a server url.\nBoth can be requested via [this contact form](https://www.semantha.de/request/).\n\n### Basic Usage\n\n#### Import\n\n```\nimport semantha_sdk\n```\n\n#### Authentication\n\n```\nsemantha = semantha_sdk.login(url="<semantha platform server URL>", key="<your key>")\n# or\nsemantha = semantha_sdk.login(url="<semantha platform server URL>", key_file="<path to your key file (json format)>")\n```\n\n#### End-point (Resource) Access\n\n```\n# end-points (resp. resources) can be used like objects\ncurrent_user = semantha.currentuser\nmy_domain = semantha.domains("my_domain")\n\n# they may have sub-resources, which can be retrieved as objects as well\nreference_documents = my_domain.referencedocuments\n```\n\n#### CRUD on End-points\n\n```\n# CRUD operations are functions\ndomain_settings = my_domain.settings.get()\nmy_domain.referencedocuments.delete() (deletes ALL reference document/library entries)\n```\n\n#### Function Return Types & semantha Data Model\n\n```\n# some functions only return None, e.g.\nmy_domain.referencedocuments.delete() # returns NoneType\n\n# others return built in types, e.g\nroles_list = currentuser.roles.get() # returns list[str]\n\n# but most return objects of the semantha Data Model\n# (all returned objects are instances of frozen dataclasses)\nsettings = my_domain.settings.get() # returns instance of DomainSettings\n# attributes can be accessed as properties, e.g.\nsettings.enable_tagging # returns true or false\n# Data Model objects may be complex\ndocument = my_domain.references.post(file=a, referencedocument=b) # returns instance of Document\n# the following returns the similarity value of the first references of the first sentence of the\n# the first paragraph on the first page of the document (if a reference was found for this sentence)\nsimilarity = pages[0].contents[0].paragraphs[0].references[0].similarity # returns float\n```\n\n### State of Development\n\nThe following resources and end-points are fully functional and (partially) tested:\n\n- [X] login -> API\n    - [X] .currentuser -> CurrentUser\n        - [X] get -> UserData(SemanthaModelEntity)\n        - [X] roles -> CurrentUserRoles\n          - [x] get -> list[str]\n    - [X] .diff -> Diff\n        - [X] post -> list[Diff(SemanthaModelEntity)]\n    - [X] .info -> VersionInfo\n        - [X] get -> VersionInfo\n    - [x] .languages -> list[str]\n    - [X] .domains -> Domains\n        - [X] get -> list[Domain(SemanthaModelEntity)]\n    - [X] .domains("domain_name") -> Domain\n        - [X] .documentannotations -> DocumentAnnotations\n            - [ ] post -> not yet implemented\n        - [X] .documentclasses -> DocumentClasses\n            - [X] get -> list[DocumentClass(SemanthaModelEntity)]\n            - [X] post -> DocumentClass(SemanthaModelEntity)\n            - [X] delete -> None\n        - [X] .documentclasses("id") -> DocumentClass\n            - [X] get -> DocumentClass(SemanthaModelEntity)\n            - [X] delete -> None\n            - [X] put -> DocumentClass(SemanthaModelEntity)\n            - [x] documentclasses -> InnerDocumentClasses\n                - [x] get -> list[DocumentClass(SemanthaModelEntity)]\n                - [x] post -> DocumentClass(SemanthaModelEntity)\n            - [x] referencedocuments -> InnerReferenceDocuments\n                - [x] get -> list[Document(SemanthaModelEntity)]\n                - [x] patch -> None\n                - [x] delete -> None\n        - [X] .documentcomparisons -> DocumentComparisons\n            - [ ] post -> not yet implemented\n          - [X] .documents -> Documents\n              - [X] post -> list[Document(SemanthaModelEntity)]\n        - [x] .modelinstances -> ModelInstance\n        - [x] .modelclasses -> ModelClass\n        - [X] .referencedocuments -> ReferenceDocuments\n            - [X] get -> ReferenceDocuments(SemanthaModelEntity)\n            - [X] delete -> None\n            - [X] post -> list[DocumentInformation(SemanthaModelEntity)]\n            - [x] .clusters -> DocumentCluster\n              - [x] get -> DocumentCluster(SemanthaModelEntity)\n            - [x] .statistic -> Statistics\n              - [x] get -> Statistic(SemanthaModelEntity)\n            - [x] .namedentities -> NamedEntities\n              - [x] get -> Optional[NamedEntities(SemanthaModelEntity)]\n        - [x] .referencedocuments("id") -> ReferenceDocument\n            - [X] get -> Document(SemanthaModelEntity)\n            - [X] delete -> None\n            - [X] patch -> DocumentInformation(SemanthaModelEntity)\n            - [X] .paragraphs("id") -> ReferenceDocumentParagraph\n                - [X] get -> Paragraph(SemanthaModelEntity)\n                - [X] patch -> Paragraph(SemanthaModelEntity)\n                - [X] delete -> None\n            - [X] .sentences("id") -> ReferenceDocumentSentence\n                - [x] get -> Sentence(SemanthaModelEntity)\n        - [X] .references -> References\n            - [X] post -> Document(SemanthaModelEntity)\n        - [x] .settings -> DomainSettings\n            - [X] get -> DomainSettings(SemanthaModelEntity)\n            - [X] patch -> DomainSettings(SemanthaModelEntity)\n        - [x] .similaritymatrix -> List[MatrixRow]\n            - [x] .clusters -> List[MatrixRow]\n        - [ ] .tags -> DomainTags\n            - [X] get -> list[str]\n            - .("tag").referencedocuments\n              - [x] get\n              - [x] delete\n        - [x] .validation -> SemanticModel\n    - [ ] .model\n      - [x] .domains("domain_name")\n        - [x] .boostwords -> Boostwords\n            - [x] get -> list[Boostword(SemanthaModelEntity)]\n            - [X] delete -> None\n            - [X] post_word -> Boostword(SemanthaModelEntity)\n            - [X] post_regex -> Boostword(SemanthaModelEntity)\n        - [x] .boostwords("id") -> Boostword\n            - [X] get -> Boostword(SemanthaModelEntity)\n            - [X] delete -> None\n            - [X] put_word -> Boostword(SemanthaModelEntity)\n            - [X] put_regex -> Boostword(SemanthaModelEntity)\n        - [x] .synonyms -> Synonyms\n            - [X] get -> list[Synonym(SemanthaModelEntity)]\n            - [X] delete -> None\n            - [X] post_word -> Synonym(SemanthaModelEntity)\n            - [X] post_regex -> Synonym(SemanthaModelEntity)\n        - [x] .synonyms("id") -> Synonym\n            - [X] get -> Synonym(SemanthaModelEntity)\n            - [X] delete -> None\n            - [X] put_word -> Synonym(SemanthaModelEntity)\n            - [X] put_regex -> Synonym(SemanthaModelEntity)\n        - [x] .datatypes -> list[str]',
+    'long_description': '![](https://www.semantha.de/wp-content/uploads/semantha-inverted.svg)\n\n# semantha® SDK\n\nThe semantha SDK is a high-level REST client to access the [semantha](http://semantha.ai) API.\nThe SDK is still under development.\nAn overview of the current progress (i.e. implemented and tested resources and endpoints) may be found at the end of\nthis document (State of Development).\nThe semantha SDK is compatible with python >= 3.8.\n\n## Design guideline/idea\nEvery api call can easily be translated into a python sdk call:\n`GET /api/info -> api.info.get()`\nThe SDK offers type hints and doc strings for services, parameters, input types and return types within your IDE.\n\n### Disclaimer\n\n**IMPORTANT:** The SDK is still under development and interfaces may change at any time without notice.\nUse with caution and on own risk.\n\n## Update Notes\n\n### Version 5.2.0\n\nThe SDK is now automatically generated from our openapi.json specification. It covers 71/169 (=42%) of all available services. Many class names and package names have been changed.\n\n### Version 4.5.0\nMajor restructuring of the SDK.\nAll sub-resources are directly accessible (instead of invoking getters).\nThat also means that (except for a few) all functions are plain get/post/delete/put/patch.\nFor example, in Versions < 4.5.0 a domain resource was fetched using `semantha_sdk.domains.get_one("domain_name")`.\nStarting with 4.5.0 it is `semantha_sdk.domains("domain_name")`.\nThat also means that get/post/put/patch functions return semantha model objects (and never resources), which makes usage more consistent.\n\n### Access\n\nTo access semantha\'s API you will need an API and a server url.\nBoth can be requested via [this contact form](https://www.semantha.de/request/).\n\n## Example Usage\n\n### Authentication with key\n\n```\nimport semantha_sdk\napi = semantha_sdk.login(server_url="<semantha platform server URL>", key="<your key>")\nprint("Talking to semantha server: " + api.info.get().version)\n```\n\n### Authentication with key file\n\n```\nimport semantha_sdk\napi = semantha_sdk.login(server_url="<semantha platform server URL>", key_file="<path to your key file (json format)>")\n# end-points (resp. resources) can be used like objects\nmy_domain = api.domains("my_domain")\n# they may have sub-resources, which can be retrieved as objects as well\nreference_documents = my_domain.referencedocuments\n# GET all reference documents\nprint("Library contains "+ len(reference_documents.get()) + " entries")\n```\n\n### CRUD on End-points\n\n```\n# CRUD operations are functions\ndomain_settings = my_domain.settings.get()\n#Warning: this deletes ALL reference documents/library entries\nmy_domain.referencedocuments.delete() \n```\n\n### Function Return Types & semantha Data Model\n\n```\n# some functions only return None, e.g.\nmy_domain.referencedocuments.delete() # returns NoneType\n\n# others return built in types, e.g\nroles_list = currentuser.roles.get() # returns List[str]\n\n# but most return objects of the semantha Data Model\n# (all returned objects are instances of frozen dataclasses)\nsettings = my_domain.settings.get() # returns instance of Settings\n# attributes can be accessed as properties, e.g.\nsettings.enable_tagging # returns true or false\n# Data Model objects may be complex\ndocument = my_domain.references.post(file=a, referencedocument=b) # returns instance of Document\n# the following returns the similarity value of the first references of the first sentence of the\n# the first paragraph on the first page of the document (if a reference was found for this sentence)\nsimilarity = pages[0].contents[0].paragraphs[0].references[0].similarity # returns float\n```\n\n## State of Development\n\nThe following resources and end-points are fully functional and (partially) tested:\n\n- [X] login -> API\n    - [X] .currentuser -> CurrentUser\n        - [X] get -> CurrentUser\n        - [X] roles -> RolesEndpoint\n          - [x] get -> List[str]\n    - [X] .diff -> Diff\n        - [X] post -> List[Difference]\n    - [X] .info -> InfoEndpoint\n        - [X] get -> Info\n    - [x] .languages -> List[str]\n    - [X] .domains -> Domains\n        - [X] get -> List[Domain]\n    - [X] .domains("domain_name") -> Domain\n        - [X] .documentannotations -> DocumentAnnotationsEndpoint\n            - [X] post -> IOBase\n        - [X] .documentclasses -> DocumentclassesEndpoint\n            - [X] get -> List[DocumentClass]\n            - [X] post -> DocumentClass\n            - [X] delete -> None\n        - [X] .documentclasses("id") -> DocumentclassEndpoint\n            - [X] get -> DocumentClass(\n            - [X] delete -> None\n            - [X] put -> DocumentClass\n            - [ ] documentclasses -> \n                - [ ] get -> List[DocumentClass]\n                - [ ] post -> DocumentClass\n            - [x] referencedocuments -> ReferencedocumentsEndpoint\n                - [x] get -> List[Document]\n                - [x] patch -> None\n                - [x] delete -> None\n        - [X] .documentcomparisons -> DocumentcomparisonsEndpoint\n            - [ ] post ->\n          - [X] .documents -> DocumentsEndpoint\n              - [X] post -> List[Document]\n        - [x] .modelinstances -> ModelInstance\n        - [x] .modelclasses -> ModelClass\n        - [X] .referencedocuments -> ReferenceDocuments\n            - [X] get -> ReferenceDocuments\n            - [X] delete -> None\n            - [X] post -> list[DocumentInformation]\n            - [x] .clusters -> DocumentCluster\n              - [x] get -> DocumentCluster\n            - [x] .statistic -> Statistics\n              - [x] get -> Statistic\n            - [x] .namedentities -> NamedEntities\n              - [x] get -> Optional[NamedEntities]\n        - [x] .referencedocuments("id") -> ReferenceDocument\n            - [X] get -> Document\n            - [X] delete -> None\n            - [X] patch -> DocumentInformation\n            - [X] .paragraphs("id") -> ReferenceDocumentParagraph\n                - [X] get -> Paragraph\n                - [X] patch -> Paragraph\n                - [X] delete -> None\n            - [X] .sentences("id") -> ReferenceDocumentSentence\n                - [x] get -> Sentence\n        - [X] .references -> References\n            - [X] post -> Document\n        - [x] .settings -> DomainSettings\n            - [X] get -> DomainSettings\n            - [X] patch -> DomainSettings\n        - [x] .similaritymatrix -> List[MatrixRow]\n            - [x] .clusters -> List[MatrixRow]\n        - [ ] .tags -> DomainTags\n            - [X] get -> list[str]\n            - .("tag").referencedocuments\n              - [x] get\n              - [x] delete\n        - [x] .validation -> SemanticModel\n    - [ ] .model\n      - [x] .domains("domain_name")\n        - [x] .boostwords -> Boostwords\n            - [x] get -> list[Boostword]\n            - [X] delete -> None\n            - [X] post_word -> Boostword\n            - [X] post_regex -> Boostword\n        - [x] .boostwords("id") -> Boostword\n            - [X] get -> Boostword\n            - [X] delete -> None\n            - [X] put_word -> Boostword\n            - [X] put_regex -> Boostword\n        - [x] .synonyms -> Synonyms\n            - [X] get -> list[Synonym]\n            - [X] delete -> None\n            - [X] post_word -> Synonym\n            - [X] post_regex -> Synonym\n        - [x] .synonyms("id") -> Synonym\n            - [X] get -> Synonym\n            - [X] delete -> None\n            - [X] put_word -> Synonym\n            - [X] put_regex -> Synonym\n        - [x] .datatypes -> list[str]',
     'author': 'Sebastian Weigelt',
     'author_email': 'sebastian.weigelt@semantha.ai',
     'maintainer': 'semantha support',
     'maintainer_email': 'support@semantha.de',
     'url': 'https://semantha.de',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `semantha_sdk-4.8.1/PKG-INFO` & `semantha_sdk-5.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantha-sdk
-Version: 4.8.1
+Version: 5.2.0
 Summary: This is a python client sdk for accessing semantha (the semantic platform)
 Home-page: https://semantha.de
 License: Apache-2.0
 Author: Sebastian Weigelt
 Author-email: sebastian.weigelt@semantha.ai
 Maintainer: semantha support
 Maintainer-email: support@semantha.de
@@ -12,193 +12,200 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: marshmallow (==3.19.0)
-Requires-Dist: marshmallow-dataclass (==8.5.12)
+Requires-Dist: marshmallow-dataclass (==8.5.14)
 Requires-Dist: pyhumps (==3.8.0)
-Requires-Dist: requests (==2.28.2)
+Requires-Dist: requests (==2.30.0)
 Description-Content-Type: text/markdown
 
 ![](https://www.semantha.de/wp-content/uploads/semantha-inverted.svg)
 
 # semantha® SDK
 
 The semantha SDK is a high-level REST client to access the [semantha](http://semantha.ai) API.
 The SDK is still under development.
 An overview of the current progress (i.e. implemented and tested resources and endpoints) may be found at the end of
 this document (State of Development).
 The semantha SDK is compatible with python >= 3.8.
 
+## Design guideline/idea
+Every api call can easily be translated into a python sdk call:
+`GET /api/info -> api.info.get()`
+The SDK offers type hints and doc strings for services, parameters, input types and return types within your IDE.
+
 ### Disclaimer
 
-**IMPORTANT:** The SDK is under development and interfaces may change at any time without notice.
+**IMPORTANT:** The SDK is still under development and interfaces may change at any time without notice.
 Use with caution and on own risk.
 
-### Update Note
+## Update Notes
+
+### Version 5.2.0
+
+The SDK is now automatically generated from our openapi.json specification. It covers 71/169 (=42%) of all available services. Many class names and package names have been changed.
 
-Version 4.5.0 comes with a major restructuring of the SDK.
+### Version 4.5.0
+Major restructuring of the SDK.
 All sub-resources are directly accessible (instead of invoking getters).
 That also means that (except for a few) all functions are plain get/post/delete/put/patch.
 For example, in Versions < 4.5.0 a domain resource was fetched using `semantha_sdk.domains.get_one("domain_name")`.
 Starting with 4.5.0 it is `semantha_sdk.domains("domain_name")`.
 That also means that get/post/put/patch functions return semantha model objects (and never resources), which makes usage more consistent.
 
 ### Access
 
 To access semantha's API you will need an API and a server url.
 Both can be requested via [this contact form](https://www.semantha.de/request/).
 
-### Basic Usage
+## Example Usage
 
-#### Import
+### Authentication with key
 
 ```
 import semantha_sdk
+api = semantha_sdk.login(server_url="<semantha platform server URL>", key="<your key>")
+print("Talking to semantha server: " + api.info.get().version)
 ```
 
-#### Authentication
-
-```
-semantha = semantha_sdk.login(url="<semantha platform server URL>", key="<your key>")
-# or
-semantha = semantha_sdk.login(url="<semantha platform server URL>", key_file="<path to your key file (json format)>")
-```
-
-#### End-point (Resource) Access
+### Authentication with key file
 
 ```
+import semantha_sdk
+api = semantha_sdk.login(server_url="<semantha platform server URL>", key_file="<path to your key file (json format)>")
 # end-points (resp. resources) can be used like objects
-current_user = semantha.currentuser
-my_domain = semantha.domains("my_domain")
-
+my_domain = api.domains("my_domain")
 # they may have sub-resources, which can be retrieved as objects as well
 reference_documents = my_domain.referencedocuments
+# GET all reference documents
+print("Library contains "+ len(reference_documents.get()) + " entries")
 ```
 
-#### CRUD on End-points
+### CRUD on End-points
 
 ```
 # CRUD operations are functions
 domain_settings = my_domain.settings.get()
-my_domain.referencedocuments.delete() (deletes ALL reference document/library entries)
+#Warning: this deletes ALL reference documents/library entries
+my_domain.referencedocuments.delete() 
 ```
 
-#### Function Return Types & semantha Data Model
+### Function Return Types & semantha Data Model
 
 ```
 # some functions only return None, e.g.
 my_domain.referencedocuments.delete() # returns NoneType
 
 # others return built in types, e.g
-roles_list = currentuser.roles.get() # returns list[str]
+roles_list = currentuser.roles.get() # returns List[str]
 
 # but most return objects of the semantha Data Model
 # (all returned objects are instances of frozen dataclasses)
-settings = my_domain.settings.get() # returns instance of DomainSettings
+settings = my_domain.settings.get() # returns instance of Settings
 # attributes can be accessed as properties, e.g.
 settings.enable_tagging # returns true or false
 # Data Model objects may be complex
 document = my_domain.references.post(file=a, referencedocument=b) # returns instance of Document
 # the following returns the similarity value of the first references of the first sentence of the
 # the first paragraph on the first page of the document (if a reference was found for this sentence)
 similarity = pages[0].contents[0].paragraphs[0].references[0].similarity # returns float
 ```
 
-### State of Development
+## State of Development
 
 The following resources and end-points are fully functional and (partially) tested:
 
 - [X] login -> API
     - [X] .currentuser -> CurrentUser
-        - [X] get -> UserData(SemanthaModelEntity)
-        - [X] roles -> CurrentUserRoles
-          - [x] get -> list[str]
+        - [X] get -> CurrentUser
+        - [X] roles -> RolesEndpoint
+          - [x] get -> List[str]
     - [X] .diff -> Diff
-        - [X] post -> list[Diff(SemanthaModelEntity)]
-    - [X] .info -> VersionInfo
-        - [X] get -> VersionInfo
-    - [x] .languages -> list[str]
+        - [X] post -> List[Difference]
+    - [X] .info -> InfoEndpoint
+        - [X] get -> Info
+    - [x] .languages -> List[str]
     - [X] .domains -> Domains
-        - [X] get -> list[Domain(SemanthaModelEntity)]
+        - [X] get -> List[Domain]
     - [X] .domains("domain_name") -> Domain
-        - [X] .documentannotations -> DocumentAnnotations
-            - [ ] post -> not yet implemented
-        - [X] .documentclasses -> DocumentClasses
-            - [X] get -> list[DocumentClass(SemanthaModelEntity)]
-            - [X] post -> DocumentClass(SemanthaModelEntity)
-            - [X] delete -> None
-        - [X] .documentclasses("id") -> DocumentClass
-            - [X] get -> DocumentClass(SemanthaModelEntity)
-            - [X] delete -> None
-            - [X] put -> DocumentClass(SemanthaModelEntity)
-            - [x] documentclasses -> InnerDocumentClasses
-                - [x] get -> list[DocumentClass(SemanthaModelEntity)]
-                - [x] post -> DocumentClass(SemanthaModelEntity)
-            - [x] referencedocuments -> InnerReferenceDocuments
-                - [x] get -> list[Document(SemanthaModelEntity)]
+        - [X] .documentannotations -> DocumentAnnotationsEndpoint
+            - [X] post -> IOBase
+        - [X] .documentclasses -> DocumentclassesEndpoint
+            - [X] get -> List[DocumentClass]
+            - [X] post -> DocumentClass
+            - [X] delete -> None
+        - [X] .documentclasses("id") -> DocumentclassEndpoint
+            - [X] get -> DocumentClass(
+            - [X] delete -> None
+            - [X] put -> DocumentClass
+            - [ ] documentclasses -> 
+                - [ ] get -> List[DocumentClass]
+                - [ ] post -> DocumentClass
+            - [x] referencedocuments -> ReferencedocumentsEndpoint
+                - [x] get -> List[Document]
                 - [x] patch -> None
                 - [x] delete -> None
-        - [X] .documentcomparisons -> DocumentComparisons
-            - [ ] post -> not yet implemented
-          - [X] .documents -> Documents
-              - [X] post -> list[Document(SemanthaModelEntity)]
+        - [X] .documentcomparisons -> DocumentcomparisonsEndpoint
+            - [ ] post ->
+          - [X] .documents -> DocumentsEndpoint
+              - [X] post -> List[Document]
         - [x] .modelinstances -> ModelInstance
         - [x] .modelclasses -> ModelClass
         - [X] .referencedocuments -> ReferenceDocuments
-            - [X] get -> ReferenceDocuments(SemanthaModelEntity)
+            - [X] get -> ReferenceDocuments
             - [X] delete -> None
-            - [X] post -> list[DocumentInformation(SemanthaModelEntity)]
+            - [X] post -> list[DocumentInformation]
             - [x] .clusters -> DocumentCluster
-              - [x] get -> DocumentCluster(SemanthaModelEntity)
+              - [x] get -> DocumentCluster
             - [x] .statistic -> Statistics
-              - [x] get -> Statistic(SemanthaModelEntity)
+              - [x] get -> Statistic
             - [x] .namedentities -> NamedEntities
-              - [x] get -> Optional[NamedEntities(SemanthaModelEntity)]
+              - [x] get -> Optional[NamedEntities]
         - [x] .referencedocuments("id") -> ReferenceDocument
-            - [X] get -> Document(SemanthaModelEntity)
+            - [X] get -> Document
             - [X] delete -> None
-            - [X] patch -> DocumentInformation(SemanthaModelEntity)
+            - [X] patch -> DocumentInformation
             - [X] .paragraphs("id") -> ReferenceDocumentParagraph
-                - [X] get -> Paragraph(SemanthaModelEntity)
-                - [X] patch -> Paragraph(SemanthaModelEntity)
+                - [X] get -> Paragraph
+                - [X] patch -> Paragraph
                 - [X] delete -> None
             - [X] .sentences("id") -> ReferenceDocumentSentence
-                - [x] get -> Sentence(SemanthaModelEntity)
+                - [x] get -> Sentence
         - [X] .references -> References
-            - [X] post -> Document(SemanthaModelEntity)
+            - [X] post -> Document
         - [x] .settings -> DomainSettings
-            - [X] get -> DomainSettings(SemanthaModelEntity)
-            - [X] patch -> DomainSettings(SemanthaModelEntity)
+            - [X] get -> DomainSettings
+            - [X] patch -> DomainSettings
         - [x] .similaritymatrix -> List[MatrixRow]
             - [x] .clusters -> List[MatrixRow]
         - [ ] .tags -> DomainTags
             - [X] get -> list[str]
             - .("tag").referencedocuments
               - [x] get
               - [x] delete
         - [x] .validation -> SemanticModel
     - [ ] .model
       - [x] .domains("domain_name")
         - [x] .boostwords -> Boostwords
-            - [x] get -> list[Boostword(SemanthaModelEntity)]
+            - [x] get -> list[Boostword]
             - [X] delete -> None
-            - [X] post_word -> Boostword(SemanthaModelEntity)
-            - [X] post_regex -> Boostword(SemanthaModelEntity)
+            - [X] post_word -> Boostword
+            - [X] post_regex -> Boostword
         - [x] .boostwords("id") -> Boostword
-            - [X] get -> Boostword(SemanthaModelEntity)
+            - [X] get -> Boostword
             - [X] delete -> None
-            - [X] put_word -> Boostword(SemanthaModelEntity)
-            - [X] put_regex -> Boostword(SemanthaModelEntity)
+            - [X] put_word -> Boostword
+            - [X] put_regex -> Boostword
         - [x] .synonyms -> Synonyms
-            - [X] get -> list[Synonym(SemanthaModelEntity)]
+            - [X] get -> list[Synonym]
             - [X] delete -> None
-            - [X] post_word -> Synonym(SemanthaModelEntity)
-            - [X] post_regex -> Synonym(SemanthaModelEntity)
+            - [X] post_word -> Synonym
+            - [X] post_regex -> Synonym
         - [x] .synonyms("id") -> Synonym
-            - [X] get -> Synonym(SemanthaModelEntity)
+            - [X] get -> Synonym
             - [X] delete -> None
-            - [X] put_word -> Synonym(SemanthaModelEntity)
-            - [X] put_regex -> Synonym(SemanthaModelEntity)
+            - [X] put_word -> Synonym
+            - [X] put_regex -> Synonym
         - [x] .datatypes -> list[str]
```

