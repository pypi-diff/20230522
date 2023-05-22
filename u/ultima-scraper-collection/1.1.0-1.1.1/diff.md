# Comparing `tmp/ultima_scraper_collection-1.1.0.tar.gz` & `tmp/ultima_scraper_collection-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultima_scraper_collection-1.1.0.tar", max compression
+gzip compressed data, was "ultima_scraper_collection-1.1.1.tar", max compression
```

## Comparing `ultima_scraper_collection-1.1.0.tar` & `ultima_scraper_collection-1.1.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0      788 2023-05-14 20:46:02.767921 ultima_scraper_collection-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      293 2023-02-26 12:00:14.727199 ultima_scraper_collection-1.1.0/ultima_scraper_collection/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/__init__.py
--rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/__init__.py
--rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
--rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
--rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
--rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
--rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
--rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
--rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
--rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
--rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
--rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
--rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
--rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
--rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
--rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
--rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
--rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
--rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
--rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
--rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
--rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
--rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
--rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
--rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
--rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
--rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
--rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
--rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
--rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
--rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
--rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
--rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
--rw-r--r--   0        0        0     1611 2023-04-20 22:10:05.846209 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
--rw-r--r--   0        0        0     2764 2023-05-08 21:50:28.707049 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
--rw-r--r--   0        0        0     2073 2023-04-20 22:22:10.068827 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
--rw-r--r--   0        0        0     9499 2023-05-14 03:29:16.005497 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
--rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/database_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/datascraper_manager/__init__.py
--rw-r--r--   0        0        0     1558 2023-03-12 13:14:10.302489 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
--rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
--rw-r--r--   0        0        0     5390 2023-05-14 03:41:06.309010 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
--rw-r--r--   0        0        0     5640 2023-05-14 03:41:28.928194 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
--rw-r--r--   0        0        0    10135 2023-05-14 18:59:18.593115 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/download_manager.py
--rw-r--r--   0        0        0    13669 2023-05-14 19:55:15.091076 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/filesystem_manager.py
--rw-r--r--   0        0        0     6102 2023-03-05 04:29:30.964171 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/legacy_code.py
--rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/metadata_manager/__init__.py
--rw-r--r--   0        0        0    27818 2023-05-14 17:11:10.534764 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
--rw-r--r--   0        0        0     6837 2023-05-14 02:04:39.528451 ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/option_manager.py
--rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-1.1.0/ultima_scraper_collection/modules/__init__.py
--rw-r--r--   0        0        0    17809 2023-05-14 04:28:12.046662 ultima_scraper_collection-1.1.0/ultima_scraper_collection/modules/module_streamliner.py
--rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-1.1.0/ultima_scraper_collection/py.typed
--rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 ultima_scraper_collection-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      788 2023-05-22 11:06:28.657966 ultima_scraper_collection-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-02-26 12:00:14.727199 ultima_scraper_collection-1.1.1/ultima_scraper_collection/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:41.007744 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.441267 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-06 01:27:30.462039 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-04 04:03:12.661102 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-26 11:42:54.461267 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/__init__.py
+-rw-r--r--   0        0        0       38 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/README
+-rw-r--r--   0        0        0     2150 2023-03-05 04:16:43.534861 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      662 2023-03-05 04:20:42.303797 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py
+-rw-r--r--   0        0        0      941 2023-03-05 04:20:47.520466 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py
+-rw-r--r--   0        0        0      861 2022-04-25 23:29:43.807242 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py
+-rw-r--r--   0        0        0     3182 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py
+-rw-r--r--   0        0        0     1651 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py
+-rw-r--r--   0        0        0     1415 2023-03-05 04:20:57.727140 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py
+-rw-r--r--   0        0        0     2201 2023-03-03 17:13:51.407142 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini
+-rw-r--r--   0        0        0    77824 2023-02-14 03:46:10.695467 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:15.033139 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:28:22.753355 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-10 12:27:11.408006 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/__init__.py
+-rw-r--r--   0        0        0     2296 2023-03-10 12:28:05.882882 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1769 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py
+-rw-r--r--   0        0        0     1649 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini
+-rw-r--r--   0        0        0      493 2023-03-10 12:30:45.700616 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/messages.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db
+-rw-r--r--   0        0        0     2288 2023-03-10 12:32:59.654189 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0     1762 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py
+-rw-r--r--   0        0        0     1643 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini
+-rw-r--r--   0        0        0      488 2023-03-10 12:32:58.467491 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/posts.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db
+-rw-r--r--   0        0        0     2294 2023-03-10 12:32:46.997189 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py
+-rw-r--r--   0        0        0      494 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/script.py.mako
+-rw-r--r--   0        0        0      797 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py
+-rw-r--r--   0        0        0     1647 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py
+-rw-r--r--   0        0        0     1766 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py
+-rw-r--r--   0        0        0      798 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py
+-rw-r--r--   0        0        0      794 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py
+-rw-r--r--   0        0        0     2011 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini
+-rw-r--r--   0        0        0      490 2023-03-10 12:32:57.520800 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/stories.py
+-rw-r--r--   0        0        0    36864 2022-01-17 19:20:07.000000 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db
+-rw-r--r--   0        0        0        0 2022-12-05 14:27:20.696663 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/__init__.py
+-rw-r--r--   0        0        0     1611 2023-04-20 22:10:05.846209 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py
+-rw-r--r--   0        0        0     2764 2023-05-08 21:50:28.707049 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py
+-rw-r--r--   0        0        0     2073 2023-04-20 22:22:10.068827 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py
+-rw-r--r--   0        0        0     9499 2023-05-14 03:29:16.005497 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py
+-rw-r--r--   0        0        0      442 2023-03-12 15:01:42.766490 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/database_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:06:18.482305 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/__init__.py
+-rw-r--r--   0        0        0     1576 2023-05-22 07:47:32.668760 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:04:46.426896 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/datascrapers/__init__.py
+-rw-r--r--   0        0        0     5390 2023-05-14 03:41:06.309010 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py
+-rw-r--r--   0        0        0     5640 2023-05-14 03:41:28.928194 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py
+-rw-r--r--   0        0        0    10564 2023-05-22 04:57:37.439982 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/download_manager.py
+-rw-r--r--   0        0        0    13669 2023-05-14 19:55:15.091076 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/filesystem_manager.py
+-rw-r--r--   0        0        0     6102 2023-03-05 04:29:30.964171 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/legacy_code.py
+-rw-r--r--   0        0        0        0 2023-01-26 08:21:03.864558 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/metadata_manager/__init__.py
+-rw-r--r--   0        0        0    27937 2023-05-22 04:54:03.366424 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py
+-rw-r--r--   0        0        0     7080 2023-05-22 08:09:26.097930 ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/option_manager.py
+-rw-r--r--   0        0        0        0 2023-03-14 06:55:35.872202 ultima_scraper_collection-1.1.1/ultima_scraper_collection/modules/__init__.py
+-rw-r--r--   0        0        0    17837 2023-05-22 07:44:05.266486 ultima_scraper_collection-1.1.1/ultima_scraper_collection/modules/module_streamliner.py
+-rw-r--r--   0        0        0        0 2023-02-26 16:07:35.717380 ultima_scraper_collection-1.1.1/ultima_scraper_collection/py.typed
+-rw-r--r--   0        0        0      663 1970-01-01 00:00:00.000000 ultima_scraper_collection-1.1.1/PKG-INFO
```

### Comparing `ultima_scraper_collection-1.1.0/pyproject.toml` & `ultima_scraper_collection-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "ultima-scraper-collection"
-version = "1.1.0"
+version = "1.1.1"
 description = ""
 authors = [
     "DIGITALCRIMINALS <89371864+digitalcriminals@users.noreply.github.com>",
 ]
 packages = [{include = "ultima_scraper_collection"}]
 include = ["ultima_scraper_collection/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 
 sqlalchemy = "^2.0.1"
 psycopg2 = "^2.9.5"
 alembic = "^1.9.2"
 tqdm = "^4.65.0"
-ultima-scraper-api = "^1.1.0"
+ultima-scraper-api = "^1.1.1"
 ultima-scraper-renamer = "^1.1.0"
 ffmpeg-python = "^0.2.0"
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.2"
 black = {version = "^23.3.0", allow-prereleases = true}
 
 [tool.semantic_release]
```

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/0d4d92c0498e_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/1454e4d1c6b8_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/37c4f2719d65_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/5493253cc03c_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/b791cf213df9_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic/versions/d2f2002f3c36_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/databases/user_data/migration/base_user_database.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/2c36fcc0b921_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/7c1c6e101059_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/aeb9fe314556_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/bf20242a238f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic/versions/d0118d8ec0b4_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/messages/migration/test_messages.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/194e05269f09_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/5b4bea08c27f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/6b1b10eb67de_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/990fc1108317_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic/versions/a918b6b05d2f_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/posts/migration/test_posts.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/29f675c35eee_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/2e4f8364f7e2_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/3076beb33c1b_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/e0c73f066547_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic/versions/ebc3f4bb0782_content.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/legacy_databases/stories/migration/test_stories.db`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/api_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/media_model.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/models/user_database.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/database_manager/connections/sqlite/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/datascraper_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import ultima_scraper_api
 from ultima_scraper_api.apis.onlyfans import onlyfans
-
 from ultima_scraper_collection import datascraper_types
 from ultima_scraper_collection.managers.datascraper_manager.datascrapers.fansly import (
     FanslyDataScraper,
 )
 from ultima_scraper_collection.managers.datascraper_manager.datascrapers.onlyfans import (
     OnlyFansDataScraper,
 )
@@ -13,15 +12,17 @@
 
 class DataScraperManager:
     def __init__(self) -> None:
         self.active_datascraper = None
         self.datascrapers: list[datascraper_types] = []
 
     def select_datascraper(
-        self, api: ultima_scraper_api.api_types, option_manager: OptionManager=OptionManager()
+        self,
+        api: ultima_scraper_api.api_types,
+        option_manager: OptionManager = OptionManager(),
     ):
         self.active_datascraper = self.get_datascraper(api)
         if not self.active_datascraper:
             self.active_datascraper = self.add_datascraper(api, option_manager)
         return self.active_datascraper
 
     def add_datascraper(
```

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/datascrapers/fansly.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/datascraper_manager/datascrapers/onlyfans.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/download_manager.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/download_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,14 +121,18 @@
                         raise Exception(
                             f"{download_item.id} has no directory\n {download_item}"
                         )
                     decrypted_media_paths: list[Path] = []
                     final_size = 0
                     error = None
                     for response in responses:
+                        if download_item.drm and await self.drm_check_downloaded(
+                            download_item
+                        ):
+                            continue
                         download_path, error = await self.writer(
                             response, download_item, encrypted=bool(download_item.key)
                         )
                         if error:
                             attempt += 1
                             break
                         if authed_drm and download_item.drm and download_path:
@@ -156,17 +160,15 @@
                             decrypted_media_paths,
                         )
                         if not formatted:
                             pass
                         final_size = download_path.stat().st_size
                     timestamp = db_media.created_at.timestamp()
                     await main_helper.format_file(
-                        download_path,
-                        timestamp,
-                        self.reformat,
+                        download_path, timestamp, self.reformat
                     )
                     db_media.size = final_size
                     db_media.downloaded = True
                     break
                 except asyncio.TimeoutError as e:
                     pass
                 except Exception as e:
@@ -192,14 +194,21 @@
             db_media.filename = download_item.filename
             download = await self.check(db_media, response)
             if not download:
                 return download_path, None
             failed = await self.filesystem_manager.write_data(response, download_path)
             return download_path, failed
 
+    async def drm_check_downloaded(self, download_item: MediaMetadata):
+        download_path = download_item.get_filepath()
+        if download_path.exists():
+            if download_path.stat().st_size and download_item.__db_item__.size:
+                return True
+        return False
+
     async def check(self, download_item: TemplateMediaModel, response: ClientResponse):
         filepath = Path(download_item.directory, download_item.filename)
         response_status = False
         if response.status == 200:
             response_status = True
             if response.content_length:
                 download_item.size = response.content_length
```

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/filesystem_manager.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/filesystem_manager.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/legacy_code.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/legacy_code.py`

 * *Files identical despite different names*

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/metadata_manager/metadata_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.sqlite_database import (
     DBCollection,
     SqliteDatabase,
 )
 from ultima_scraper_collection.managers.database_manager.database_manager import (
     DatabaseManager,
 )
-from ultima_scraper_collection.managers.filesystem_manager import (
-    FilesystemManager,
-)
+from ultima_scraper_collection.managers.filesystem_manager import FilesystemManager
 
 api_types = ultima_scraper_api.api_types
 user_types = ultima_scraper_api.user_types
 content_types = ultima_scraper_api.content_types
 from ultima_scraper_api.classes.prepare_metadata import format_content
 from ultima_scraper_api.helpers import main_helper
 
@@ -279,14 +277,18 @@
             url_path = url.path
             if "Protected" in url.path:
                 index = url.path.index("/files")
                 url_path = url.path[index:]
             if media_url.path == url_path:
                 return self
 
+    def get_filepath(self):
+        assert self.directory and self.filename
+        return Path(self.directory, self.filename)
+
 
 class MetadataManager:
     def __init__(
         self,
         subscription: user_types,
         filesystem_manager: FilesystemManager,
         db_manager: SqliteDatabase | None = None,
```

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/managers/option_manager.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/managers/option_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,19 @@
                 final_list = await self.choose_option()
                 self.final_choices = [
                     key
                     for choice in final_list
                     for key in self.items
                     if choice.lower() == key.auth_details.username.lower()
                 ]
+                set1 = set(self.final_choices)
+                set2 = set(self.items)
+                difference = list(set2 - set1)
+                for auth in difference:
+                    await auth.session_manager.active_session.close()
             case "subscriptions":
                 subscription_users = [x for x in self.items]
                 self.item_keys = [x.username for x in subscription_users]
                 my_string = " | ".join(
                     map(
                         lambda x: f"{subscription_users.index(x)+1} = {x.username}",
                         subscription_users,
```

### Comparing `ultima_scraper_collection-1.1.0/ultima_scraper_collection/modules/module_streamliner.py` & `ultima_scraper_collection-1.1.1/ultima_scraper_collection/modules/module_streamliner.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,40 +4,38 @@
 from itertools import product
 from typing import Any, Optional
 
 import ultima_scraper_api
 import ultima_scraper_api.classes.make_settings as make_settings
 from sqlalchemy.exc import OperationalError
 from tqdm.asyncio import tqdm_asyncio
-from ultima_scraper_renamer import renamer
-
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.models.api_model import (
     ApiModel,
 )
 from ultima_scraper_collection.managers.database_manager.connections.sqlite.sqlite_database import (
     DBCollection,
 )
 from ultima_scraper_collection.managers.database_manager.database_manager import (
     DatabaseManager,
 )
 from ultima_scraper_collection.managers.download_manager import DownloadManager
 from ultima_scraper_collection.managers.filesystem_manager import FilesystemManager
 from ultima_scraper_collection.managers.metadata_manager.metadata_manager import (
     MetadataManager,
 )
+from ultima_scraper_renamer import renamer
 
 auth_types = ultima_scraper_api.auth_types
 user_types = ultima_scraper_api.user_types
 message_types = ultima_scraper_api.message_types
 error_types = ultima_scraper_api.error_types
 subscription_types = ultima_scraper_api.subscription_types
 
 from typing import TYPE_CHECKING
 
-
 if TYPE_CHECKING:
     from ultima_scraper_collection.managers.datascraper_manager.datascrapers.fansly import (
         FanslyDataScraper,
     )
     from ultima_scraper_collection.managers.datascraper_manager.datascrapers.onlyfans import (
         OnlyFansDataScraper,
     )
@@ -372,17 +370,18 @@
         auth: auth_types,
         datascraper: datascraper_types,
         site_settings: make_settings.SiteSettings,
         identifiers: list[int | str] | list[str] = [],
     ) -> tuple[bool, list[user_types]]:
         status = False
         subscriptions: list[subscription_types] = []
-        authed = await auth.login()
+        auth = await auth.login()
 
-        if authed.active and site_settings:
+        if auth.check_authed() and site_settings:
+            authed = auth
             # metadata_filepath = (
             #     authed.directory_manager.profile.metadata_directory.joinpath(
             #         "Mass Messages.json"
             #     )
             # )
             # if authed.isPerformer:
             #     imported = main_helper.import_json(metadata_filepath)
```

### Comparing `ultima_scraper_collection-1.1.0/PKG-INFO` & `ultima_scraper_collection-1.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: ultima-scraper-collection
-Version: 1.1.0
+Version: 1.1.1
 Summary: 
 Author: DIGITALCRIMINALS
 Author-email: 89371864+digitalcriminals@users.noreply.github.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: alembic (>=1.9.2,<2.0.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: psycopg2 (>=2.9.5,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.1,<3.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
-Requires-Dist: ultima-scraper-api (>=1.1.0,<2.0.0)
+Requires-Dist: ultima-scraper-api (>=1.1.1,<2.0.0)
 Requires-Dist: ultima-scraper-renamer (>=1.1.0,<2.0.0)
```

