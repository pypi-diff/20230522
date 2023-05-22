# Comparing `tmp/moe-2.1.0.tar.gz` & `tmp/moe-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moe-2.1.0.tar", max compression
+gzip compressed data, was "moe-2.1.1.tar", max compression
```

## Comparing `moe-2.1.0.tar` & `moe-2.1.1.tar`

### file list

```diff
@@ -1,61 +1,60 @@
--rw-r--r--   0        0        0     1066 2022-12-21 04:24:17.456883 moe-2.1.0/LICENSE
--rw-r--r--   0        0        0     2907 2022-12-21 04:24:17.456883 moe-2.1.0/README.rst
--rw-r--r--   0        0        0       38 2022-12-21 04:24:17.456883 moe-2.1.0/alembic/README
--rw-r--r--   0        0        0     2008 2022-12-21 04:24:17.456883 moe-2.1.0/alembic/alembic.ini
--rw-r--r--   0        0        0     2517 2022-12-21 04:24:17.460883 moe-2.1.0/alembic/env.py
--rw-r--r--   0        0        0      495 2022-12-21 04:24:17.460883 moe-2.1.0/alembic/script.py.mako
--rw-r--r--   0        0        0      744 2022-12-21 04:24:17.460883 moe-2.1.0/alembic/versions/0ce5960a081e_new_field_catalog_nums.py
--rw-r--r--   0        0        0      587 2022-12-21 04:24:17.460883 moe-2.1.0/alembic/versions/30668259fcd6_new_field_country.py
--rw-r--r--   0        0        0      599 2022-12-21 04:24:17.460883 moe-2.1.0/alembic/versions/32e9fea590b7_new_field_track_total.py
--rw-r--r--   0        0        0      581 2022-12-21 04:24:17.460883 moe-2.1.0/alembic/versions/60608d9d2908_new_field_media.py
--rw-r--r--   0        0        0     3185 2022-12-21 04:24:17.460883 moe-2.1.0/alembic/versions/6d4e785df5cb_initial_generation.py
--rw-r--r--   0        0        0      581 2022-12-21 04:24:17.460883 moe-2.1.0/alembic/versions/817440447857_new_field_label.py
--rw-r--r--   0        0        0      605 2022-12-21 04:24:17.460883 moe-2.1.0/alembic/versions/880c5a2d80ed_remove_audio_format_field.py
--rw-r--r--   0        0        0      601 2022-12-21 04:24:17.460883 moe-2.1.0/alembic/versions/ab11c34c1d0b_new_field_audio_format.py
--rw-r--r--   0        0        0     1154 2022-12-21 04:24:17.460883 moe-2.1.0/alembic/versions/ab5db9861d30_rename_custom_fields.py
--rw-r--r--   0        0        0     5698 2022-12-21 04:24:17.460883 moe-2.1.0/alembic/versions/bf49ac6805f7_json_multi_value_fields.py
--rw-r--r--   0        0        0      597 2022-12-21 04:24:17.460883 moe-2.1.0/alembic/versions/db3a470892c6_new_field_og_date.py
--rw-r--r--   0        0        0      586 2022-12-21 04:24:17.460883 moe-2.1.0/alembic/versions/eb8c7e20a080_new_field_barcode.py
--rw-r--r--   0        0        0      723 2022-12-21 04:24:17.460883 moe-2.1.0/alembic/versions/fe0956c93730_new_field_artists.py
--rw-r--r--   0        0        0      443 2022-12-21 04:24:17.460883 moe-2.1.0/moe/__init__.py
--rw-r--r--   0        0        0      430 2022-12-21 04:24:17.460883 moe-2.1.0/moe/add/__init__.py
--rw-r--r--   0        0        0     3732 2022-12-21 04:24:17.460883 moe-2.1.0/moe/add/add_cli.py
--rw-r--r--   0        0        0     2155 2022-12-21 04:24:17.460883 moe-2.1.0/moe/add/add_core.py
--rwxr-xr-x   0        0        0     4871 2022-12-21 04:24:17.460883 moe-2.1.0/moe/cli.py
--rw-r--r--   0        0        0    15332 2022-12-21 04:24:17.460883 moe-2.1.0/moe/config.py
--rw-r--r--   0        0        0      514 2022-12-21 04:24:17.460883 moe-2.1.0/moe/duplicate/__init__.py
--rw-r--r--   0        0        0     7141 2022-12-21 04:24:17.460883 moe-2.1.0/moe/duplicate/dup_cli.py
--rw-r--r--   0        0        0     5909 2022-12-21 04:24:17.460883 moe-2.1.0/moe/duplicate/dup_core.py
--rw-r--r--   0        0        0      454 2022-12-21 04:24:17.460883 moe-2.1.0/moe/edit/__init__.py
--rw-r--r--   0        0        0     2137 2022-12-21 04:24:17.460883 moe-2.1.0/moe/edit/edit_cli.py
--rw-r--r--   0        0        0     1815 2022-12-21 04:24:17.460883 moe-2.1.0/moe/edit/edit_core.py
--rw-r--r--   0        0        0      311 2022-12-21 04:24:17.460883 moe-2.1.0/moe/library/__init__.py
--rw-r--r--   0        0        0    19614 2022-12-21 04:24:17.460883 moe-2.1.0/moe/library/album.py
--rw-r--r--   0        0        0     6284 2022-12-21 04:24:17.460883 moe-2.1.0/moe/library/extra.py
--rw-r--r--   0        0        0    10049 2022-12-21 04:24:17.460883 moe-2.1.0/moe/library/lib_item.py
--rw-r--r--   0        0        0    18057 2022-12-21 04:24:17.460883 moe-2.1.0/moe/library/track.py
--rw-r--r--   0        0        0     4407 2022-12-21 04:24:17.460883 moe-2.1.0/moe/list.py
--rw-r--r--   0        0        0      544 2022-12-21 04:24:17.460883 moe-2.1.0/moe/moe_import/__init__.py
--rw-r--r--   0        0        0    12253 2022-12-21 04:24:17.460883 moe-2.1.0/moe/moe_import/import_cli.py
--rw-r--r--   0        0        0     3855 2022-12-21 04:24:17.460883 moe-2.1.0/moe/moe_import/import_core.py
--rw-r--r--   0        0        0      472 2022-12-21 04:24:17.460883 moe-2.1.0/moe/move/__init__.py
--rw-r--r--   0        0        0     2506 2022-12-21 04:24:17.460883 moe-2.1.0/moe/move/move_cli.py
--rw-r--r--   0        0        0    10363 2022-12-21 04:24:17.460883 moe-2.1.0/moe/move/move_core.py
--rw-r--r--   0        0        0        0 2022-12-21 04:24:17.460883 moe-2.1.0/moe/py.typed
--rw-r--r--   0        0        0     6972 2022-12-21 04:24:17.460883 moe-2.1.0/moe/query.py
--rw-r--r--   0        0        0      462 2022-12-21 04:24:17.460883 moe-2.1.0/moe/read/__init__.py
--rw-r--r--   0        0        0     1621 2022-12-21 04:24:17.460883 moe-2.1.0/moe/read/read_cli.py
--rw-r--r--   0        0        0      820 2022-12-21 04:24:17.464884 moe-2.1.0/moe/read/read_core.py
--rw-r--r--   0        0        0      450 2022-12-21 04:24:17.464884 moe-2.1.0/moe/remove/__init__.py
--rw-r--r--   0        0        0     1475 2022-12-21 04:24:17.464884 moe-2.1.0/moe/remove/rm_cli.py
--rw-r--r--   0        0        0     1139 2022-12-21 04:24:17.464884 moe-2.1.0/moe/remove/rm_core.py
--rw-r--r--   0        0        0       62 2022-12-21 04:24:17.464884 moe-2.1.0/moe/util/__init__.py
--rw-r--r--   0        0        0      209 2022-12-21 04:24:17.464884 moe-2.1.0/moe/util/cli/__init__.py
--rw-r--r--   0        0        0     2133 2022-12-21 04:24:17.464884 moe-2.1.0/moe/util/cli/prompt.py
--rw-r--r--   0        0        0     2535 2022-12-21 04:24:17.464884 moe-2.1.0/moe/util/cli/query.py
--rw-r--r--   0        0        0      153 2022-12-21 04:24:17.464884 moe-2.1.0/moe/util/core/__init__.py
--rw-r--r--   0        0        0     5616 2022-12-21 04:24:17.464884 moe-2.1.0/moe/util/core/match.py
--rw-r--r--   0        0        0     3034 2022-12-21 04:24:17.464884 moe-2.1.0/moe/write.py
--rw-r--r--   0        0        0     2120 2022-12-21 04:24:17.464884 moe-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4118 1970-01-01 00:00:00.000000 moe-2.1.0/setup.py
--rw-r--r--   0        0        0     4076 1970-01-01 00:00:00.000000 moe-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-22 16:39:36.033294 moe-2.1.1/LICENSE
+-rw-r--r--   0        0        0     3256 2023-05-22 16:39:36.033294 moe-2.1.1/README.rst
+-rw-r--r--   0        0        0       38 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/README
+-rw-r--r--   0        0        0     2008 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/alembic.ini
+-rw-r--r--   0        0        0     2704 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/env.py
+-rw-r--r--   0        0        0      495 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/script.py.mako
+-rw-r--r--   0        0        0      744 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/0ce5960a081e_new_field_catalog_nums.py
+-rw-r--r--   0        0        0      587 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/30668259fcd6_new_field_country.py
+-rw-r--r--   0        0        0      599 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/32e9fea590b7_new_field_track_total.py
+-rw-r--r--   0        0        0      581 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/60608d9d2908_new_field_media.py
+-rw-r--r--   0        0        0     3185 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/6d4e785df5cb_initial_generation.py
+-rw-r--r--   0        0        0      581 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/817440447857_new_field_label.py
+-rw-r--r--   0        0        0      605 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/880c5a2d80ed_remove_audio_format_field.py
+-rw-r--r--   0        0        0      601 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/ab11c34c1d0b_new_field_audio_format.py
+-rw-r--r--   0        0        0     1154 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/ab5db9861d30_rename_custom_fields.py
+-rw-r--r--   0        0        0     5698 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/bf49ac6805f7_json_multi_value_fields.py
+-rw-r--r--   0        0        0      597 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/db3a470892c6_new_field_og_date.py
+-rw-r--r--   0        0        0      586 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/eb8c7e20a080_new_field_barcode.py
+-rw-r--r--   0        0        0      723 2023-05-22 16:39:36.037294 moe-2.1.1/alembic/versions/fe0956c93730_new_field_artists.py
+-rw-r--r--   0        0        0      443 2023-05-22 16:39:36.037294 moe-2.1.1/moe/__init__.py
+-rw-r--r--   0        0        0      430 2023-05-22 16:39:36.037294 moe-2.1.1/moe/add/__init__.py
+-rw-r--r--   0        0        0     3736 2023-05-22 16:39:36.037294 moe-2.1.1/moe/add/add_cli.py
+-rw-r--r--   0        0        0     2154 2023-05-22 16:39:36.037294 moe-2.1.1/moe/add/add_core.py
+-rwxr-xr-x   0        0        0     4870 2023-05-22 16:39:36.037294 moe-2.1.1/moe/cli.py
+-rw-r--r--   0        0        0    15584 2023-05-22 16:39:36.037294 moe-2.1.1/moe/config.py
+-rw-r--r--   0        0        0      514 2023-05-22 16:39:36.037294 moe-2.1.1/moe/duplicate/__init__.py
+-rw-r--r--   0        0        0     7141 2023-05-22 16:39:36.037294 moe-2.1.1/moe/duplicate/dup_cli.py
+-rw-r--r--   0        0        0     5827 2023-05-22 16:39:36.037294 moe-2.1.1/moe/duplicate/dup_core.py
+-rw-r--r--   0        0        0      454 2023-05-22 16:39:36.037294 moe-2.1.1/moe/edit/__init__.py
+-rw-r--r--   0        0        0     2135 2023-05-22 16:39:36.037294 moe-2.1.1/moe/edit/edit_cli.py
+-rw-r--r--   0        0        0     1801 2023-05-22 16:39:36.037294 moe-2.1.1/moe/edit/edit_core.py
+-rw-r--r--   0        0        0      311 2023-05-22 16:39:36.037294 moe-2.1.1/moe/library/__init__.py
+-rw-r--r--   0        0        0    19001 2023-05-22 16:39:36.037294 moe-2.1.1/moe/library/album.py
+-rw-r--r--   0        0        0     5497 2023-05-22 16:39:36.037294 moe-2.1.1/moe/library/extra.py
+-rw-r--r--   0        0        0    10090 2023-05-22 16:39:36.037294 moe-2.1.1/moe/library/lib_item.py
+-rw-r--r--   0        0        0    16982 2023-05-22 16:39:36.037294 moe-2.1.1/moe/library/track.py
+-rw-r--r--   0        0        0     4421 2023-05-22 16:39:36.037294 moe-2.1.1/moe/list.py
+-rw-r--r--   0        0        0      544 2023-05-22 16:39:36.037294 moe-2.1.1/moe/moe_import/__init__.py
+-rw-r--r--   0        0        0    12282 2023-05-22 16:39:36.037294 moe-2.1.1/moe/moe_import/import_cli.py
+-rw-r--r--   0        0        0     3852 2023-05-22 16:39:36.037294 moe-2.1.1/moe/moe_import/import_core.py
+-rw-r--r--   0        0        0      472 2023-05-22 16:39:36.037294 moe-2.1.1/moe/move/__init__.py
+-rw-r--r--   0        0        0     2506 2023-05-22 16:39:36.037294 moe-2.1.1/moe/move/move_cli.py
+-rw-r--r--   0        0        0    10415 2023-05-22 16:39:36.037294 moe-2.1.1/moe/move/move_core.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:39:36.037294 moe-2.1.1/moe/py.typed
+-rw-r--r--   0        0        0     7053 2023-05-22 16:39:36.037294 moe-2.1.1/moe/query.py
+-rw-r--r--   0        0        0      462 2023-05-22 16:39:36.037294 moe-2.1.1/moe/read/__init__.py
+-rw-r--r--   0        0        0     1619 2023-05-22 16:39:36.037294 moe-2.1.1/moe/read/read_cli.py
+-rw-r--r--   0        0        0      818 2023-05-22 16:39:36.037294 moe-2.1.1/moe/read/read_core.py
+-rw-r--r--   0        0        0      450 2023-05-22 16:39:36.037294 moe-2.1.1/moe/remove/__init__.py
+-rw-r--r--   0        0        0     1475 2023-05-22 16:39:36.037294 moe-2.1.1/moe/remove/rm_cli.py
+-rw-r--r--   0        0        0     1228 2023-05-22 16:39:36.037294 moe-2.1.1/moe/remove/rm_core.py
+-rw-r--r--   0        0        0       62 2023-05-22 16:39:36.037294 moe-2.1.1/moe/util/__init__.py
+-rw-r--r--   0        0        0      209 2023-05-22 16:39:36.037294 moe-2.1.1/moe/util/cli/__init__.py
+-rw-r--r--   0        0        0     2131 2023-05-22 16:39:36.037294 moe-2.1.1/moe/util/cli/prompt.py
+-rw-r--r--   0        0        0     2609 2023-05-22 16:39:36.037294 moe-2.1.1/moe/util/cli/query.py
+-rw-r--r--   0        0        0      153 2023-05-22 16:39:36.037294 moe-2.1.1/moe/util/core/__init__.py
+-rw-r--r--   0        0        0     5651 2023-05-22 16:39:36.037294 moe-2.1.1/moe/util/core/match.py
+-rw-r--r--   0        0        0     3033 2023-05-22 16:39:36.037294 moe-2.1.1/moe/write.py
+-rw-r--r--   0        0        0     2114 2023-05-22 16:39:36.041294 moe-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4422 1970-01-01 00:00:00.000000 moe-2.1.1/PKG-INFO
```

### Comparing `moe-2.1.0/LICENSE` & `moe-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/README.rst` & `moe-2.1.1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 ###############
 Welcome to Moe!
 ###############
 Moe is our resident Music-Organizer-Extraordinaire who's sole purpose is to give you full control over your music library by streamlining the process between downloading/ripping music to your filesystem and listening to it with your favorite music player.
 
 In short, Moe maintains a database of your music library that can be updated with various metadata sources, queried, edited, etc. through either an API or command-line interface. All of these features, and more, are made available by a highly extensible plugin ecosystem.
 
+Because all of this functionality is available as a python API which doesn't always require a database of music to operate on, Moe also provides an extensive suite of tools for handling and operating on music files. This can greatly simplify or enhance any other script/program that deals with music.
+
 Usage
 =====
+
+CLI
+---
 Moe comes with a command-line interface which is how most users will take advantage of the library management features. Below is a screenshot of Moe importing an album from the filesystem and adding it to the underlying database all while fixing tags, relocating the files, and anything else you can imagine.
 
 .. image:: _static/import_example.png
 
-Alternatively, because all the core functionality is available via an API, the underlying music management system can be incorporated into any existing program or other user interface.
+Once added to Moe, querying your library or manipulating your music by editing tags, renaming files, etc. is all just a single command away. The ultimate goal is to automate away any tedius and time-consuming steps you have in your workflow without sacrificing the attention to detail. With the help of an *extremely* flexible plugin system, you can easily fine-tune your music library exactly how you like.
 
-Finally, although a lot of Moe's functionality exists around the idea of operating on a library database of your music, the database is entirely optional. In this case, Moe provides a convenient set of tools and functionality for handling music in a general sense. For example, below is a standalone python script that takes an album directory and Musicbrainz release ID from the command-line, and then updates the underlying files' tags with any changes from Musicbrainz (utilizing the ``musicbrainz`` plugin).
+Library
+-------
+As previously mentioned, all of Moe's music management logic and functionality is also available as a python library. As an example, below is a standalone script that takes an album directory and Musicbrainz release ID from the command-line, and then updates the underlying files' tags with any changes from Musicbrainz.
 
 .. code:: python
 
     #!/usr/bin/env python3
 
     import argparse
     import pathlib
@@ -47,10 +54,10 @@
         for track in album.tracks:
             write_tags(track)
 
 
     if __name__ == "__main__":
         main()
 
-This is just a small taste of what Moe is capable of and how it can make your life easier when dealing with music in Python.
+This is just a small taste of what Moe is capable of and how it can make your life easier when dealing with music.
 
 If you want to learn more, check out the `Getting Started <https://mrmoe.readthedocs.io/en/latest/getting_started.html>`_ docs.
```

### Comparing `moe-2.1.0/alembic/alembic.ini` & `moe-2.1.1/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/alembic/env.py` & `moe-2.1.1/alembic/env.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,25 +44,35 @@
 def run_migrations_online():
     """Run migrations in 'online' mode.
 
     In this scenario we need to create an Engine and associate a connection
     with the context.
     """
     connectable = config.attributes.get("connection", None)
+
     if not connectable:
         # only create Engine if we don't have a Connection from the outside
         moe_config = Config(init_db=False)
         moe_config._init_db(create_tables=False)
         connectable = moe_config.engine
 
-    # When connectable is already a Connection object, calling
-    # connect() gives us a *branched connection*.
-    with connectable.connect() as connection:
+        with connectable.connect() as connection:
+            context.configure(
+                connection=connection,
+                target_metadata=target_metadata,
+                render_as_batch=True,
+            )
+
+            with context.begin_transaction():
+                context.run_migrations()
+    else:
         context.configure(
-            connection=connection, target_metadata=target_metadata, render_as_batch=True
+            connection=connectable,
+            target_metadata=target_metadata,
+            render_as_batch=True,
         )
 
         with context.begin_transaction():
             context.run_migrations()
 
 
 run_migrations_online()
```

### Comparing `moe-2.1.0/alembic/versions/0ce5960a081e_new_field_catalog_nums.py` & `moe-2.1.1/alembic/versions/0ce5960a081e_new_field_catalog_nums.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/alembic/versions/30668259fcd6_new_field_country.py` & `moe-2.1.1/alembic/versions/30668259fcd6_new_field_country.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/alembic/versions/32e9fea590b7_new_field_track_total.py` & `moe-2.1.1/alembic/versions/32e9fea590b7_new_field_track_total.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/alembic/versions/60608d9d2908_new_field_media.py` & `moe-2.1.1/alembic/versions/60608d9d2908_new_field_media.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/alembic/versions/6d4e785df5cb_initial_generation.py` & `moe-2.1.1/alembic/versions/6d4e785df5cb_initial_generation.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/alembic/versions/817440447857_new_field_label.py` & `moe-2.1.1/alembic/versions/817440447857_new_field_label.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/alembic/versions/880c5a2d80ed_remove_audio_format_field.py` & `moe-2.1.1/alembic/versions/880c5a2d80ed_remove_audio_format_field.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/alembic/versions/ab11c34c1d0b_new_field_audio_format.py` & `moe-2.1.1/alembic/versions/ab11c34c1d0b_new_field_audio_format.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/alembic/versions/ab5db9861d30_rename_custom_fields.py` & `moe-2.1.1/alembic/versions/ab5db9861d30_rename_custom_fields.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/alembic/versions/bf49ac6805f7_json_multi_value_fields.py` & `moe-2.1.1/alembic/versions/bf49ac6805f7_json_multi_value_fields.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/alembic/versions/db3a470892c6_new_field_og_date.py` & `moe-2.1.1/alembic/versions/db3a470892c6_new_field_og_date.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/alembic/versions/eb8c7e20a080_new_field_barcode.py` & `moe-2.1.1/alembic/versions/eb8c7e20a080_new_field_barcode.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/alembic/versions/fe0956c93730_new_field_artists.py` & `moe-2.1.1/alembic/versions/fe0956c93730_new_field_artists.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/moe/add/add_cli.py` & `moe-2.1.1/moe/add/add_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     Raises:
         SystemExit: Path given does not exist.
     """
     paths = [Path(arg_path) for arg_path in args.paths]
 
     album: Optional[Album] = None
     if args.album_query:
-        albums = cast(Album, cli_query(session, args.album_query, "album"))
+        albums = cast(list[Album], cli_query(session, args.album_query, "album"))
 
         if len(albums) > 1:
             log.error("Query returned more than one album.")
             raise SystemExit(1)
         else:
             album = albums[0]
 
@@ -114,15 +114,15 @@
     """
     if path.is_file():
         try:
             moe.add.add_item(session, Track.from_file(path, album=album))
         except TrackError:
             if not album:
                 raise AddError(
-                    f"An album query is required to add an extra. [{path=!r}]"
+                    f"An album query is required to add an extra. [{path=}]"
                 ) from None
 
             moe.add.add_item(session, Extra(album, path))
     elif path.is_dir():
         moe.add.add_item(session, Album.from_dir(path))
     else:
         raise AddError(f"Path not found. [{path=}]")
```

### Comparing `moe-2.1.0/moe/add/add_core.py` & `moe-2.1.1/moe/add/add_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,15 +43,15 @@
               to the library.
             * `Pluggy hook wrapper documention
               <https://pluggy.readthedocs.io/en/stable/#wrappers>`_
         """
 
 
 @moe.hookimpl
-def add_hooks(pm: pluggy.manager.PluginManager):
+def add_hooks(pm: pluggy._manager.PluginManager):
     """Registers `add` hookspecs to Moe."""
     from moe.add.add_core import Hooks
 
     pm.add_hookspecs(Hooks)
 
 
 class AddError(Exception):
@@ -68,14 +68,14 @@
     Args:
         session: Library db session.
         item: Item to be added.
 
     Raises:
         AddError: Unable to add the item to the library.
     """
-    log.debug(f"Adding item to the library. [{item=!r}]")
+    log.debug(f"Adding item to the library. [{item=}]")
 
     config.CONFIG.pm.hook.pre_add(item=item)
     session.add(item)
     session.flush()
 
-    log.info(f"Item added to the library. [{item=!r}]")
+    log.info(f"Added item to the library. [{item=!s}]")
```

### Comparing `moe-2.1.0/moe/cli.py` & `moe-2.1.1/moe/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             * `The python documentation for adding sub-parsers.
               <https://docs.python.org/3/library/argparse.html#sub-commands>`_
             * The :meth:`~moe.query.query` function.
         """
 
 
 @moe.hookimpl
-def add_hooks(pm: pluggy.manager.PluginManager):
+def add_hooks(pm: pluggy._manager.PluginManager):
     """Registers `CLI` hookspecs to Moe."""
     from moe.cli import Hooks
 
     pm.add_hookspecs(Hooks)
 
 
 def _parse_args(args: list[str]):
@@ -152,15 +152,15 @@
         moe_log.setLevel(logging.ERROR)
     elif args.quiet == 2:
         moe_log.setLevel(logging.CRITICAL)
 
 
 def main(args: list[str] = sys.argv[1:]):
     """Runs the CLI."""
-    log.debug(f"Commandline arguments received. [{args=!r}]")
+    log.debug(f"Commandline arguments received. [{args=}]")
 
     if not config.CONFIG:
         try:
             Config()
         except ConfigValidationError as err:
             log.error(err)
             raise SystemExit(1) from err
```

### Comparing `moe-2.1.0/moe/config.py` & `moe-2.1.1/moe/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,17 +27,19 @@
 import importlib.util
 import logging
 import os
 import re
 import sys
 from pathlib import Path
 from types import ModuleType
-from typing import NamedTuple, Optional, Union, cast
+from typing import Any, NamedTuple, Optional, Union, cast
 
 import dynaconf
+import dynaconf.base
+import dynaconf.validator
 import pluggy
 import sqlalchemy
 import sqlalchemy.event
 import sqlalchemy.orm
 
 import alembic.command
 import alembic.config
@@ -96,15 +98,15 @@
 
         See Also:
             https://www.dynaconf.com/validation/#validation for more info.
         """
 
     @staticmethod
     @moe.hookspec
-    def add_hooks(pm: pluggy.manager.PluginManager):
+    def add_hooks(pm: pluggy._manager.PluginManager):
         """Add hookspecs to be registered to Moe.
 
         Args:
             pm: PluginManager that registers the hookspec.
 
         Example:
             .. code:: python
@@ -195,15 +197,15 @@
     validators = [
         dynaconf.Validator("DEFAULT_PLUGINS", default=DEFAULT_PLUGINS),
         dynaconf.Validator("DISABLE_PLUGINS", default=set()),
         dynaconf.Validator("ENABLE_PLUGINS", default=set()),
         dynaconf.Validator("LIBRARY_PATH", default="~/Music"),
         dynaconf.Validator("ORIGINAL_DATE", default=False),
     ]
-    settings.validators.register(*validators)
+    settings.validators.register(*validators)  # type: ignore
 
 
 class ExtraPlugin(NamedTuple):
     """Used to specify extra plugins when initializing the config.
 
     Attributes:
         plugin: This is the class or module of the plugin to register.
@@ -218,15 +220,15 @@
     """Initializes moe configuration settings and database.
 
     Attributes:
         config_dir (Path): Filesystem path of the configuration directory.
         config_file (Path): Filesystem path of the configuration settings file.
         enabled_plugins (set[str]): Enabled plugins as specified by the configuration.
         engine (sa.engine.base.Engine): Database engine in use.
-        pm (pluggy.manager.PluginManager): Plugin manager that handles plugin logic.
+        pm (pluggy._manager.PluginManager): Plugin manager that handles plugin logic.
         settings (dynaconf.base.LazySettings): User configuration settings.
     """
 
     def __init__(
         self,
         config_dir: Path = Path.home() / ".config" / "moe",  # noqa: B008
         settings_filename: str = "config.toml",
@@ -270,15 +272,15 @@
 
         Moe uses sqlite by default.
 
         Args:
             create_tables: Whether or not to create and update the db tables.
                 If doing db migrations manually, e.g. in alembic, this should be False.
         """
-        log.debug(f"Initializing database. [{create_tables=!r}]")
+        log.debug(f"Initializing database. [{create_tables=}]")
 
         db_path = self.config_dir / "library.db"
 
         if not self.engine:
             self.engine = sqlalchemy.create_engine("sqlite:///" + str(db_path))
 
         moe_sessionmaker.configure(bind=self.engine)
@@ -326,18 +328,21 @@
         """
         from moe.library.lib_item import PathType
 
         log.debug(f"Reading configuration file. [config_file={self.config_file}]")
 
         self.config_file.touch(exist_ok=True)
 
-        self.settings = dynaconf.Dynaconf(
-            envvar_prefix="MOE",  # export envvars with `export MOE_FOO=bar`
-            settings_file=str(self.config_file.resolve()),
-        )
+        self.settings = cast(
+            Any,
+            dynaconf.Dynaconf(
+                envvar_prefix="MOE",  # export envvars with `export MOE_FOO=bar`
+                settings_file=str(self.config_file.resolve()),
+            ),
+        )  # cast to Any until dynaconf implements proper type stubs
 
         self._setup_plugins()
         self.pm.hook.add_config_validator(settings=self.settings)
         self._validate_settings()
 
         PathType.library_path = Path(self.settings.library_path)
 
@@ -365,15 +370,17 @@
             core_plugins: Optional mapping of core plugin modules to names.
                 These plugins cannot be overwritten by the user configuration.
             default_plugins: Optional mapping of default plugin modules to names.
                 These plugins are enabled by default, but can be disabled by the config.
         """
         log.debug("Setting up plugins.")
 
-        self.pm = pluggy.PluginManager("moe")
+        self.pm = cast(
+            Any, pluggy.PluginManager("moe")
+        )  # avoids pluggy hook type errors
 
         # register core modules that cannot be disabled by the config
         for plugin_name, module in core_plugins.items():
             self.pm.register(importlib.import_module(module), plugin_name)
 
         # need to validate `config` specific settings separately so we have access to
         # the 'default_plugins' setting
```

### Comparing `moe-2.1.0/moe/duplicate/__init__.py` & `moe-2.1.1/moe/duplicate/__init__.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/moe/duplicate/dup_cli.py` & `moe-2.1.1/moe/duplicate/dup_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/moe/duplicate/dup_core.py` & `moe-2.1.1/moe/duplicate/dup_core.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Detect and handle duplicates in the library."""
 
 import logging
-from typing import Optional
+from typing import Optional, Sequence
 
 import sqlalchemy
 from sqlalchemy.orm.session import Session
 
 import moe
 from moe import config
 from moe.library import Album, Extra, LibItem, Track
@@ -66,36 +66,36 @@
     """Check for and resolve duplicates when items are edited."""
     yield  # run all `edit_changed_items` hook implementations
 
     albums = [item for item in items if isinstance(item, Album)]  # resolve albums first
     tracks = [item for item in items if isinstance(item, Track)]
     extras = [item for item in items if isinstance(item, Extra)]
 
-    resolve_duplicates(session, albums)  # type: ignore
-    resolve_duplicates(session, tracks)  # type: ignore
-    resolve_duplicates(session, extras)  # type: ignore
+    resolve_duplicates(session, albums)
+    resolve_duplicates(session, tracks)
+    resolve_duplicates(session, extras)
 
 
 @moe.hookimpl(hookwrapper=True)
 def edit_new_items(session: Session, items: list[LibItem]):
     """Check for and resolve duplicates when items are added to the library."""
     yield  # run all `edit_new_items` hook implementations
 
     albums = [item for item in items if isinstance(item, Album)]  # resolve albums first
     tracks = [item for item in items if isinstance(item, Track)]
     extras = [item for item in items if isinstance(item, Extra)]
 
-    resolve_duplicates(session, albums)  # type: ignore
-    resolve_duplicates(session, tracks)  # type: ignore
-    resolve_duplicates(session, extras)  # type: ignore
+    resolve_duplicates(session, albums)
+    resolve_duplicates(session, tracks)
+    resolve_duplicates(session, extras)
 
 
-def resolve_duplicates(session: Session, items: list[LibItem]):
+def resolve_duplicates(session: Session, items: Sequence[LibItem]):
     """Search for and resolve any duplicates of items in ``items``."""
-    log.debug(f"Checking for duplicate items. [{items=!r}]")
+    log.debug(f"Checking for duplicate items. [{items=}]")
 
     resolved_items = []
     for item in items:
         if _is_removed(item):
             continue
 
         dup_items = get_duplicates(session, item, items)
@@ -121,15 +121,15 @@
                     f"[item_a={item!r}, item_b={dup_item!r}]"
                 )
 
         if dup_items:
             resolved_items.append(item)
 
     if resolved_items:
-        log.debug(f"Resolved duplicate items. [{resolved_items=!r}]")
+        log.debug(f"Resolved duplicate items. [{resolved_items=}]")
     else:
         log.debug("No duplicate items found.")
 
 
 def _is_removed(item):
     """Check whether or not an item is removed from the library."""
     insp = sqlalchemy.inspect(item)
@@ -137,15 +137,15 @@
     if insp.deleted or insp.transient:
         return True
 
     return False
 
 
 def get_duplicates(
-    session: Session, item: LibItem, others: Optional[list[LibItem]] = None
+    session: Session, item: LibItem, others: Optional[Sequence[LibItem]] = None
 ) -> list[LibItem]:
     """Returns items considered duplicates of ``item``.
 
     Args:
         session: Library db session.
         item: Library item to get duplicates of.
         others: Items to compare against. If not given, will query the database
```

### Comparing `moe-2.1.0/moe/edit/edit_cli.py` & `moe-2.1.1/moe/edit/edit_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     items = cli_query(session, args.query, args.query_type)
 
     error_count = 0
     for term in args.fv_terms:
         try:
             field, value = term.split("=")
         except ValueError:
-            log.error(f"Invalid FIELD=VALUE format. [{term=!r}]")
+            log.error(f"Invalid FIELD=VALUE format. [{term=}]")
             error_count += 1
             continue
 
         for item in items:
             try:
                 edit.edit_item(item, field, value)
             except edit.EditError as err:
```

### Comparing `moe-2.1.0/moe/edit/edit_core.py` & `moe-2.1.1/moe/edit/edit_core.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,27 +24,27 @@
         item: Library item to edit.
         field: Item field to edit.
         value: Value to set the item's field to.
 
     Raises:
         EditError: ``field`` is not a valid attribute or is not editable.
     """
-    log.debug(f"Editing item. [{item=!r}, {field=!r}, {value=!r}]")
+    log.debug(f"Editing item. [{item=}, {field=}, {value=}]")
 
     if field == "path":
-        raise EditError(f"Non-editable field given. [{field=!r}]")
+        raise EditError(f"Non-editable field given. [{field=}]")
 
     try:
         attr = getattr(item.__class__, field)
     except AttributeError as a_err:
         if field in item.custom:
             item.custom[field] = value
             return
 
-        raise EditError(f"Invalid field given. [{field=!r}]") from a_err
+        raise EditError(f"Invalid field given. [{field=}]") from a_err
 
     try:
         column_type = attr.property.columns[0].type
     except AttributeError:
         # hybrid_property
         setattr(item, field, value)
         return
@@ -57,8 +57,8 @@
         try:
             setattr(item, field, datetime.date.fromisoformat(value))
         except ValueError as v_err:
             raise EditError("Date must be in format YYYY-MM-DD") from v_err
     else:
         setattr(item, field, value)
 
-    log.info(f"Item edited. [{item=!r}, {field=!r}, {value=!r}]")
+    log.info(f"Item edited. [{item=!s}, {field=}, {value=}]")
```

### Comparing `moe-2.1.0/moe/library/album.py` & `moe-2.1.1/moe/library/album.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """An Album in the database and any related logic."""
 
 import datetime
 import logging
 from pathlib import Path, PurePath
-from typing import TYPE_CHECKING, Any, Optional, TypeVar, Union, cast
+from typing import TYPE_CHECKING, Any, Optional, Union, cast
 
 import pluggy
 import sqlalchemy as sa
-from sqlalchemy import JSON, Column, Date, Integer, String
+from sqlalchemy import JSON, Integer
 from sqlalchemy.ext.hybrid import hybrid_property
 from sqlalchemy.ext.mutable import MutableDict, MutableSet
-from sqlalchemy.orm import relationship
+from sqlalchemy.orm import Mapped, mapped_column, relationship
 
 import moe
 from moe import config
 from moe.library.lib_item import LibItem, LibraryError, MetaLibItem, SABase, SetType
 
 if TYPE_CHECKING:
     from moe.library.extra import Extra
@@ -36,15 +36,15 @@
         "Uniqueness" is meant in terms of whether the two albums should be considered
         duplicates in the library. These additional conditions will be applied inside a
         album's :meth:`is_unique` method.
         """
 
 
 @moe.hookimpl
-def add_hooks(pm: pluggy.manager.PluginManager):
+def add_hooks(pm: pluggy._manager.PluginManager):
     """Registers `album` hookspecs to Moe."""
     from moe.library.album import Hooks
 
     pm.add_hookspecs(Hooks)
 
 
 class AlbumError(LibraryError):
@@ -200,15 +200,15 @@
             other_value = other.custom.get(custom_field)
             if other_value and (
                 overwrite or (not overwrite and not self.custom[custom_field])
             ):
                 self.custom[custom_field] = other_value
 
         log.debug(
-            f"MetaAlbums merged. [album_a={self!r}, album_b={other!r}, {overwrite=!r}]"
+            f"MetaAlbums merged. [album_a={self!r}, album_b={other!r}, {overwrite=}]"
         )
 
     def __eq__(self, other: "MetaAlbum") -> bool:
         """Compares MetaAlbums by their fields."""
         if type(self) != type(other):
             return False
 
@@ -270,18 +270,14 @@
             track_reprs.append(f"{track.disc}.{track.track_num} - {track.title}")
         repr_str += ", tracks=[" + ", ".join(track_reprs) + "]"
 
         repr_str += ")"
         return repr_str
 
 
-# Album generic, used for typing classmethod
-A = TypeVar("A", bound="Album")
-
-
 class Album(LibItem, SABase, MetaAlbum):
     """An album is a collection of tracks and represents a specific album release.
 
     Albums also house any attributes that are shared by tracks e.g. albumartist.
 
     Attributes:
         artist (str): AKA albumartist.
@@ -302,46 +298,38 @@
         track_total (Optional[int]): Number of tracks that *should* be in the album.
             If an album is missing tracks, then ``len(tracks) < track_total``.
         tracks (list[Track]): Album's corresponding tracks.
     """
 
     __tablename__ = "album"
 
-    artist: str = cast(str, Column(String, nullable=False))
-    barcode: Optional[str] = cast(Optional[str], Column(String, nullable=True))
-    catalog_nums: Optional[set[str]] = cast(
-        Optional[set[str]], MutableSet.as_mutable(Column(SetType, nullable=True))
+    artist: Mapped[str]
+    barcode: Mapped[Optional[str]]
+    catalog_nums: Mapped[Optional[set[str]]] = mapped_column(
+        MutableSet.as_mutable(SetType()), nullable=True
     )
-    country: Optional[str] = cast(Optional[str], Column(String, nullable=True))
-    date: datetime.date = cast(datetime.date, Column(Date, nullable=False))
-    disc_total: int = cast(int, Column(Integer, nullable=False, default=1))
-    label: Optional[str] = cast(Optional[str], Column(String, nullable=True))
-    media: Optional[str] = cast(Optional[str], Column(String, nullable=True))
-    original_date: Optional[datetime.date] = cast(
-        Optional[datetime.date], Column(Date, nullable=True)
-    )
-    title: str = cast(str, Column(String, nullable=False))
-    track_total: Optional[int] = cast(Optional[int], Column(Integer, nullable=True))
-    custom: dict[str, Any] = cast(
-        dict[str, Any],
-        Column(
-            MutableDict.as_mutable(JSON(none_as_null=True)),
-            default="{}",
-            nullable=False,
-        ),
+    country: Mapped[Optional[str]]
+    date: Mapped[datetime.date]
+    disc_total: Mapped[int] = mapped_column(Integer, nullable=False, default=1)
+    label: Mapped[Optional[str]]
+    media: Mapped[Optional[str]]
+    original_date: Mapped[Optional[datetime.date]]
+
+    title: Mapped[str]
+    track_total: Mapped[Optional[int]]
+    custom: Mapped[dict[str, Any]] = mapped_column(
+        MutableDict.as_mutable(JSON(none_as_null=True)), default="{}", nullable=False
     )
 
-    tracks: list["Track"] = relationship(
-        "Track",
+    tracks: Mapped[list["Track"]] = relationship(
         back_populates="album",
         cascade="all, delete-orphan",
         collection_class=list,
     )
-    extras: list["Extra"] = relationship(
-        "Extra",
+    extras: Mapped[list["Extra"]] = relationship(
         back_populates="album",
         cascade="all, delete-orphan",
         collection_class=list,
     )
 
     def __init__(
         self,
@@ -377,15 +365,15 @@
 
         if config.CONFIG.settings.original_date and self.original_date:
             self.date = self.original_date
 
         log.debug(f"Album created. [album={self!r}]")
 
     @classmethod
-    def from_dir(cls: type[A], album_path: Path) -> A:
+    def from_dir(cls, album_path: Path) -> "Album":
         """Creates an album from a directory.
 
         Args:
             album_path: Album directory path. The directory will be scanned for any
                 files to be added to the album. Any non-track files will be added as
                 extras.
 
@@ -414,15 +402,15 @@
 
         if not album:
             raise AlbumError(f"No tracks found in album directory. [dir={album_path}]")
 
         for extra_path in extra_paths:
             Extra(album, extra_path)
 
-        log.debug(f"Album created from directory. [dir={album_path}, {album=!r}]")
+        log.debug(f"Album created from directory. [dir={album_path}, {album=}]")
         return album
 
     @property
     def fields(self) -> set[str]:
         """Returns any editable, track-specific fields."""
         return super().fields.union({"path"})
 
@@ -470,17 +458,15 @@
         for custom_field in self.custom:
             other_value = other.custom.get(custom_field)
             if other_value and (
                 overwrite or (not overwrite and not self.custom[custom_field])
             ):
                 self.custom[custom_field] = other_value
 
-        log.debug(
-            f"Albums merged. [album_a={self!r}, album_b={other!r}, {overwrite=!r}]"
-        )
+        log.debug(f"Albums merged. [album_a={self!r}, album_b={other!r}, {overwrite=}]")
 
     def _merge_tracks(
         self, other: Union["Album", MetaAlbum], overwrite: bool = False
     ) -> None:
         """Merges the tracks of another album into this one."""
         new_tracks: list["Track"] = []
         for other_track in other.tracks:
@@ -504,33 +490,35 @@
                 if conflict_extra:
                     conflict_extra.merge(other_extra, overwrite)
                 else:
                     new_extras.append(other_extra)
             self.extras.extend(new_extras)
 
     @hybrid_property
-    def original_year(self) -> Optional[int]:  # type: ignore
+    def original_year(self) -> Optional[int]:
         """Gets an Album's year."""
         if self.original_date is None:
             return None
 
         return self.original_date.year
 
-    @original_year.expression  # type: ignore
-    def original_year(cls):  # noqa: B902
+    @original_year.inplace.expression  # type: ignore
+    @classmethod
+    def _original_year_expression(cls):
         """Returns a year at the sql level."""
         return sa.extract("year", cls.original_date)
 
     @hybrid_property
-    def year(self) -> int:  # type: ignore
+    def year(self) -> int:
         """Gets an Album's year."""
         return self.date.year
 
-    @year.expression  # type: ignore
-    def year(cls):  # noqa: B902
+    @year.inplace.expression
+    @classmethod
+    def _year_expression(cls):
         """Returns a year at the sql level."""
         return sa.extract("year", cls.date)
 
     def __repr__(self):
         """Represents an Album using its fields."""
         field_reprs = []
         for field in self.fields:
```

### Comparing `moe-2.1.0/moe/library/extra.py` & `moe-2.1.1/moe/library/extra.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Any non-music item attached to an album such as log files are considered extras."""
 
 import logging
 from pathlib import Path, PurePath
-from typing import Any, cast
+from typing import Any
 
 import pluggy
-from sqlalchemy import JSON, Column, Integer
+from sqlalchemy import JSON, Integer
 from sqlalchemy.ext.mutable import MutableDict
-from sqlalchemy.orm import relationship
+from sqlalchemy.orm import Mapped, mapped_column, relationship
 from sqlalchemy.schema import ForeignKey
 
 import moe
 from moe import config
 from moe.library.album import Album
 from moe.library.lib_item import LibItem, SABase
 
@@ -21,48 +21,25 @@
 
 
 class Hooks:
     """Extra hook specifications."""
 
     @staticmethod
     @moe.hookspec
-    def create_custom_extra_fields() -> dict[str, Any]:  # type: ignore
-        """Creates new custom fields for an Extra.
-
-        Returns:
-            Dict of the field names to their default values or ``None`` for no default.
-
-        Example:
-            .. code:: python
-
-                return {"my_new_field": "default value", "other_field": None}
-
-            You can then access your new field as if it were a normal field::
-
-                extra.my_new_field = "awesome new value"
-
-        Important:
-            Your custom field should follow the same naming rules as any other python
-            variable i.e. no spaces, starts with a letter, and consists solely of
-            alpha-numeric and underscore characters.
-        """  # noqa: DAR202
-
-    @staticmethod
-    @moe.hookspec
     def is_unique_extra(extra: "Extra", other: "Extra") -> bool:  # type: ignore
         """Add new conditions to determine whether two extras are unique.
 
         "Uniqueness" is meant in terms of whether the two extras should be considered
         duplicates in the library. These additional conditions will be applied inside a
         extra's :meth:`is_unique` method.
         """
 
 
 @moe.hookimpl
-def add_hooks(pm: pluggy.manager.PluginManager):
+def add_hooks(pm: pluggy._manager.PluginManager):
     """Registers `extra` hookspecs to Moe."""
     from moe.library.extra import Hooks
 
     pm.add_hookspecs(Hooks)
 
 
 class Extra(LibItem, SABase):
@@ -72,25 +49,20 @@
         album (Album): Album the extra file belongs to.
         custom (dict[str, Any]): Dictionary of custom fields.
         path (pathlib.Path): Filesystem path of the extra file.
     """
 
     __tablename__ = "extra"
 
-    custom: dict[str, Any] = cast(
-        dict[str, Any],
-        Column(
-            MutableDict.as_mutable(JSON(none_as_null=True)),
-            default="{}",
-            nullable=False,
-        ),
+    custom: Mapped[dict[str, Any]] = mapped_column(
+        MutableDict.as_mutable(JSON(none_as_null=True)), default="{}", nullable=False
     )
 
-    _album_id: int = cast(int, Column(Integer, ForeignKey("album._id")))
-    album: Album = relationship("Album", back_populates="extras")
+    _album_id: Mapped[int] = mapped_column(Integer, ForeignKey("album._id"))
+    album: Mapped["Album"] = relationship(back_populates="extras")
 
     def __init__(self, album: Album, path: Path, **kwargs):
         """Creates an Extra.
 
         Args:
             album: Album the extra file belongs to.
             path: Filesystem path of the extra file.
@@ -130,15 +102,15 @@
         """Merges another extra into this one.
 
         Args:
             other: Other extra to be merged with the current extra.
             overwrite: Whether or not to overwrite self if a conflict exists.
         """
         log.debug(
-            f"Merging extras. [extra_a={self!r}, extra_b={other!r}, {overwrite=!r}]"
+            f"Merging extras. [extra_a={self!r}, extra_b={other!r}, {overwrite=}]"
         )
 
         omit_fields = {"album"}
         for field in self.fields - omit_fields:
             other_value = getattr(other, field)
             self_value = getattr(self, field)
             if other_value and (overwrite or (not overwrite and not self_value)):
@@ -147,17 +119,15 @@
         for custom_field in self.custom:
             other_value = other.custom.get(custom_field)
             if other_value and (
                 overwrite or (not overwrite and not self.custom[custom_field])
             ):
                 self.custom[custom_field] = other_value
 
-        log.debug(
-            f"Extras merged. [extra_a={self!r}, extra_b={other!r}, {overwrite=!r}]"
-        )
+        log.debug(f"Extras merged. [extra_a={self!r}, extra_b={other!r}, {overwrite=}]")
 
     def __eq__(self, other):
         """Compares Extras by their fields."""
         if not isinstance(other, Extra):
             return False
 
         for field in self.fields:
@@ -178,15 +148,19 @@
     def __repr__(self):
         """Represents an Extra using its path and album."""
         field_reprs = []
         omit_fields = {"album"}
         for field in self.fields - omit_fields:
             if hasattr(self, field):
                 field_reprs.append(f"{field}={getattr(self, field)!r}")
-        repr_str = "Extra(" + ", ".join(field_reprs) + f", album='{self.album}'"
+        repr_str = (
+            "Extra("
+            + ", ".join(field_reprs)
+            + f", album='{self.album}'"  # noqa: B907 album repr is too long
+        )
 
         custom_field_reprs = []
         for custom_field, value in self.custom.items():
             custom_field_reprs.append(f"{custom_field}={value}")
         if custom_field_reprs:
             repr_str += ", custom_fields=[" + ", ".join(custom_field_reprs) + "]"
```

### Comparing `moe-2.1.0/moe/library/lib_item.py` & `moe-2.1.1/moe/library/lib_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """Shared functionality between library albums, extras, and tracks."""
 
 import logging
 from pathlib import Path
-from typing import Any, cast
+from typing import Any
 
 import pluggy
 import sqlalchemy
-import sqlalchemy as sa
 import sqlalchemy.event
 import sqlalchemy.orm
-from sqlalchemy import Column, Integer
-from sqlalchemy.orm import declarative_base
+import sqlalchemy.types
+from sqlalchemy import Integer
+from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column
 from sqlalchemy.orm.session import Session
 
 import moe
 from moe import config
 
 __all__ = ["LibItem", "LibraryError", "MetaLibItem"]
 
 log = logging.getLogger("moe.lib_item")
 
-SABase = declarative_base()
+
+class SABase(DeclarativeBase):
+    pass
 
 
 class LibraryError(Exception):
     """General library error."""
 
 
 class Hooks:
@@ -103,15 +105,15 @@
         See Also:
             The :meth:`edit_new_items` hook for editing items before their values are
             finalized.
         """
 
 
 @moe.hookimpl
-def add_hooks(pm: pluggy.manager.PluginManager):
+def add_hooks(pm: pluggy._manager.PluginManager):
     """Registers `add` hookspecs to Moe."""
     from moe.library.lib_item import Hooks
 
     pm.add_hookspecs(Hooks)
 
 
 @moe.hookimpl
@@ -149,26 +151,26 @@
         `SQLAlchemy docs on state management <https://docs.sqlalchemy.org/en/14/orm/session_state_management.html>`_
     """  # noqa: E501
     changed_items = []
     for dirty_item in session.dirty:
         if session.is_modified(dirty_item) and isinstance(dirty_item, LibItem):
             changed_items.append(dirty_item)
     if changed_items:
-        log.debug(f"Editing changed items. [{changed_items=!r}]")
+        log.debug(f"Editing changed items. [{changed_items=}]")
         config.CONFIG.pm.hook.edit_changed_items(session=session, items=changed_items)
-        log.debug(f"Edited changed items. [{changed_items=!r}]")
+        log.debug(f"Edited changed items. [{changed_items=}]")
 
     new_items = []
     for new_item in session.new:
         if isinstance(new_item, LibItem):
             new_items.append(new_item)
     if new_items:
-        log.debug(f"Editing new items. [{new_items=!r}]")
+        log.debug(f"Editing new items. [{new_items=}]")
         config.CONFIG.pm.hook.edit_new_items(session=session, items=new_items)
-        log.debug(f"Edited new items. [{new_items=!r}]")
+        log.debug(f"Edited new items. [{new_items=}]")
 
 
 def _process_after_flush(
     session: sqlalchemy.orm.Session,
     flush_context: sqlalchemy.orm.UOWTransaction,
 ):
     """Runs the ``process_*_items`` hook specifications after items are flushed.
@@ -185,50 +187,50 @@
         `SQLAlchemy docs on state management <https://docs.sqlalchemy.org/en/14/orm/session_state_management.html>`_
     """  # noqa: E501
     changed_items = []
     for dirty_item in session.dirty:
         if session.is_modified(dirty_item) and isinstance(dirty_item, LibItem):
             changed_items.append(dirty_item)
     if changed_items:
-        log.debug(f"Processing changed items. [{changed_items=!r}]")
+        log.debug(f"Processing changed items. [{changed_items=}]")
         config.CONFIG.pm.hook.process_changed_items(
             session=session, items=changed_items
         )
-        log.debug(f"Processed changed items. [{changed_items=!r}]")
+        log.debug(f"Processed changed items. [{changed_items=}]")
 
     new_items = []
     for new_item in session.new:
         if isinstance(new_item, LibItem):
             new_items.append(new_item)
     if new_items:
-        log.debug(f"Processing new items. [{new_items=!r}]")
+        log.debug(f"Processing new items. [{new_items=}]")
         config.CONFIG.pm.hook.process_new_items(session=session, items=new_items)
-        log.debug(f"Processed new items. [{new_items=!r}]")
+        log.debug(f"Processed new items. [{new_items=}]")
 
     removed_items = []
     for removed_item in session.deleted:
         if isinstance(removed_item, LibItem):
             removed_items.append(removed_item)
     if removed_items:
-        log.debug(f"Processing removed items. [{removed_items=!r}]")
+        log.debug(f"Processing removed items. [{removed_items=}]")
         config.CONFIG.pm.hook.process_removed_items(
             session=session, items=removed_items
         )
-        log.debug(f"Processed removed items. [{removed_items=!r}]")
+        log.debug(f"Processed removed items. [{removed_items=}]")
 
 
-class PathType(sa.types.TypeDecorator):
+class PathType(sqlalchemy.types.TypeDecorator):
     """A custom type for paths for database storage.
 
     Normally, paths are Path type, but we can't store that in the database,
     so we normalize the paths first to strings for database storage. Paths are stored as
     relative paths from ``library_path`` in the config.
     """
 
-    impl = sa.types.String  # sql type
+    impl = sqlalchemy.types.String  # sql type
     cache_ok = True  # expected to produce same bind/result behavior and sql generation
 
     library_path: Path  # will be set on config initialization
 
     def process_bind_param(self, pathlib_path, dialect):
         """Normalize pathlib paths as strings for the database.
 
@@ -249,18 +251,18 @@
         """Convert the path back to a Path object on the way out."""
         if path_str is None:
             return None
 
         return Path(self.library_path / path_str)
 
 
-class SetType(sa.types.TypeDecorator):
+class SetType(sqlalchemy.types.TypeDecorator):
     """A custom type for storing sets as json in a database."""
 
-    impl = sa.types.JSON  # sql type
+    impl = sqlalchemy.types.JSON  # sql type
     cache_ok = True  # expected to produce same bind/result behavior and sql generation
 
     def process_bind_param(self, json_set, dialect):
         """Convert the set to a list so it's valid json."""
         if json_set is not None:
             return list(json_set)
         return None
@@ -297,13 +299,13 @@
         """Library items implement the `lt` magic method to allow sorting."""
         raise NotImplementedError
 
 
 class LibItem(MetaLibItem):
     """Base class for library items i.e. Albums, Extras, and Tracks."""
 
-    _id: int = cast(int, Column(Integer, primary_key=True))
-    path: Path = cast(Path, Column(PathType, nullable=False, unique=True))
+    _id: Mapped[int] = mapped_column(Integer, primary_key=True)
+    path: Mapped[Path] = mapped_column(PathType, nullable=False, unique=True)
 
     def is_unique(self, other: "LibItem") -> bool:
         """Returns whether an item is unique in the library from ``other``."""
         raise NotImplementedError
```

### Comparing `moe-2.1.0/moe/library/track.py` & `moe-2.1.1/moe/library/track.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """A Track in the database and any related logic."""
 
 import logging
 from pathlib import Path
-from typing import Any, Optional, TypeVar, cast
+from typing import Any, Optional
 
 import mediafile
 import pluggy
-from sqlalchemy import JSON, Column, Integer, String
+from sqlalchemy import JSON, Integer
 from sqlalchemy.ext.mutable import MutableDict, MutableSet
-from sqlalchemy.orm import relationship
+from sqlalchemy.orm import Mapped, mapped_column, relationship
 from sqlalchemy.schema import ForeignKey, UniqueConstraint
 
 import moe
 from moe import config
 from moe.library.album import Album, MetaAlbum
 from moe.library.lib_item import LibItem, LibraryError, MetaLibItem, SABase, SetType
 
@@ -22,37 +22,14 @@
 
 
 class Hooks:
     """Track hook specifications."""
 
     @staticmethod
     @moe.hookspec
-    def create_custom_track_fields() -> dict[str, Any]:  # type: ignore
-        """Creates new custom fields for a Track.
-
-        Returns:
-            Dict of the field names to their default values or ``None`` for no default.
-
-        Example:
-            Inside your hook implementation::
-
-                return {"my_new_field": "default value", "other_field": None}
-
-            You can then access your new field as if it were a normal field::
-
-                track.my_new_field = "awesome new value"
-
-        Important:
-            Your custom field should follow the same naming rules as any other python
-            variable i.e. no spaces, starts with a letter, and consists solely of
-            alpha-numeric and underscore characters.
-        """  # noqa: DAR202
-
-    @staticmethod
-    @moe.hookspec
     def is_unique_track(track: "Track", other: "Track") -> bool:  # type: ignore
         """Add new conditions to determine whether two tracks are unique.
 
         "Uniqueness" is meant in terms of whether the two tracks should be considered
         duplicates in the library. These additional conditions will be applied inside a
         track's :meth:`is_unique` method.
         """
@@ -91,15 +68,15 @@
             * `Mediafile docs <https://mediafile.readthedocs.io/en/latest/>`_
             * The :meth:`~moe.write.Hooks.write_custom_tags` hook for writing
               tags.
         """
 
 
 @moe.hookimpl
-def add_hooks(pm: pluggy.manager.PluginManager):
+def add_hooks(pm: pluggy._manager.PluginManager):
     """Registers `track` hookspecs to Moe."""
     from moe.library.track import Hooks
 
     pm.add_hookspecs(Hooks)
 
 
 @moe.hookimpl(tryfirst=True)
@@ -132,18 +109,14 @@
     track_fields["track_num"] = audio_file.track
 
 
 class TrackError(LibraryError):
     """Error performing some operation on a Track."""
 
 
-# Track generic, used for typing classmethod
-T = TypeVar("T", bound="Track")
-
-
 class MetaTrack(MetaLibItem):
     """A track containing only metadata.
 
     It does not exist on the filesystem nor in the library. It can be used
     to represent information about a track to later be merged into a full ``Track``
     instance.
 
@@ -221,15 +194,15 @@
         """Merges another track into this one.
 
         Args:
             other: Other track to be merged with the current track.
             overwrite: Whether or not to overwrite self if a conflict exists.
         """
         log.debug(
-            f"Merging tracks. [track_a={self!r}, track_b={other!r}, {overwrite=!r}]"
+            f"Merging tracks. [track_a={self!r}, track_b={other!r}, {overwrite=}]"
         )
 
         omit_fields = {"album"}
         for field in self.fields - omit_fields:
             other_value = getattr(other, field, None)
             self_value = getattr(self, field, None)
             if other_value and (overwrite or (not overwrite and not self_value)):
@@ -238,17 +211,15 @@
         for custom_field in self.custom:
             other_value = other.custom.get(custom_field)
             if other_value and (
                 overwrite or (not overwrite and not self.custom[custom_field])
             ):
                 self.custom[custom_field] = other_value
 
-        log.debug(
-            f"Tracks merged. [track_a={self!r}, track_b={other!r}, {overwrite=!r}]"
-        )
+        log.debug(f"Tracks merged. [track_a={self!r}, track_b={other!r}, {overwrite=}]")
 
     def __eq__(self, other) -> bool:
         """Compares Tracks by their fields."""
         if type(self) != type(other):
             return False
 
         for field in self.fields:
@@ -275,15 +246,15 @@
         omit_fields = {"album"}
         for field in self.fields - omit_fields:
             if hasattr(self, field):
                 field_reprs.append(f"{field}={getattr(self, field)!r}")
         repr_str = (
             f"{type(self).__name__}("
             + ", ".join(field_reprs)
-            + f", album='{self.album}'"
+            + f", album='{self.album}'"  # noqa: B907 album repr is too long
         )
 
         custom_field_reprs = []
         for custom_field, value in self.custom.items():
             custom_field_reprs.append(f"{custom_field}={value}")
         if custom_field_reprs:
             repr_str += ", custom_fields=[" + ", ".join(custom_field_reprs) + "]"
@@ -313,35 +284,30 @@
     Note:
         Altering any album-related property attributes, will result in changing the
         album field and thus all other tracks in the album as well.
     """
 
     __tablename__ = "track"
 
-    artist: str = cast(str, Column(String, nullable=False))
-    artists: Optional[set[str]] = cast(
-        Optional[set[str]], MutableSet.as_mutable(Column(SetType, nullable=True))
+    artist: Mapped[str]
+    artists: Mapped[Optional[set[str]]] = mapped_column(
+        MutableSet.as_mutable(SetType()), nullable=True
     )
-    disc: int = cast(int, Column(Integer, nullable=False, default=1))
-    genres: Optional[set[str]] = cast(
-        Optional[set[str]], MutableSet.as_mutable(Column(SetType, nullable=True))
+    disc: Mapped[int] = mapped_column(Integer, nullable=False, default=1)
+    genres: Mapped[Optional[set[str]]] = mapped_column(
+        MutableSet.as_mutable(SetType()), nullable=True
     )
-    title: str = cast(str, Column(String, nullable=False))
-    track_num: int = cast(int, Column(Integer, nullable=False))
-    custom: dict[str, Any] = cast(
-        dict[str, Any],
-        Column(
-            MutableDict.as_mutable(JSON(none_as_null=True)),
-            default="{}",
-            nullable=False,
-        ),
+    title: Mapped[str]
+    track_num: Mapped[int]
+    custom: Mapped[dict[str, Any]] = mapped_column(
+        MutableDict.as_mutable(JSON(none_as_null=True)), default="{}", nullable=False
     )
 
-    _album_id: int = cast(int, Column(Integer, ForeignKey("album._id")))
-    album: Album = relationship("Album", back_populates="tracks")
+    _album_id: Mapped[int] = mapped_column(Integer, ForeignKey("album._id"))
+    album: Mapped["Album"] = relationship(back_populates="tracks")
 
     __table_args__ = (UniqueConstraint("disc", "track_num", "_album_id"),)
 
     def __init__(
         self,
         album: Album,
         path: Path,
@@ -406,15 +372,15 @@
         for disc_num, disc_dir in enumerate(sorted(disc_dirs), start=1):
             if self.path.is_relative_to(disc_dir):
                 return disc_num
 
         return 1
 
     @classmethod
-    def from_file(cls: type[T], track_path: Path, album: Optional[Album] = None) -> T:
+    def from_file(cls, track_path: Path, album: Optional[Album] = None) -> "Track":
         """Alternate initializer that creates a Track from a track file.
 
         Will read any tags from the given path and save them to the Track.
 
         Args:
             track_path: Filesystem path of the track.
             album: Corresponding album for the track. If not given, the album will be
@@ -460,15 +426,15 @@
             missing_reqd_fields.append("album_artist")
         if not album_title and not album:
             missing_reqd_fields.append("album_title")
         if not date and not album:
             missing_reqd_fields.append("date")
         if missing_reqd_fields:
             raise ValueError(
-                f"Track is missing required fields. [{missing_reqd_fields=!r}]"
+                f"Track is missing required fields. [{missing_reqd_fields=}]"
             )
 
         if not album:
             album = Album(
                 path=track_path.parent,
                 artist=album_artist,
                 title=album_title,
```

### Comparing `moe-2.1.0/moe/list.py` & `moe-2.1.1/moe/list.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Note:
     This plugin is enabled by default.
 """
 
 import argparse
 import logging
 from collections import OrderedDict
-from typing import Any
+from typing import Any, Sequence
 
 from sqlalchemy.orm.session import Session
 
 import moe
 import moe.cli
 from moe import config
 from moe.library import Album, Extra, LibItem, Track
@@ -74,15 +74,15 @@
         for item in items:
             if args.paths:
                 print(item.path)
             else:
                 print(item)
 
 
-def _fmt_infos(items: list[LibItem]):
+def _fmt_infos(items: Sequence[LibItem]):
     """Formats information for multiple items together."""
     out_str = ""
     for item in items:
         out_str += _fmt_info(item) + "\n"
 
         if item is not items[-1]:
             out_str += "\n"
```

### Comparing `moe-2.1.0/moe/moe_import/__init__.py` & `moe-2.1.1/moe/moe_import/__init__.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/moe/moe_import/import_cli.py` & `moe-2.1.1/moe/moe_import/import_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                         title="Abort", shortcut_key="x", func=_abort_changes
                     )
                 )
         """
 
 
 @moe.hookimpl
-def add_hooks(pm: pluggy.manager.PluginManager):
+def add_hooks(pm: pluggy._manager.PluginManager):
     """Registers `import` cli hookspecs to Moe."""
     from moe.moe_import.import_cli import Hooks
 
     pm.add_hookspecs(Hooks)
 
 
 @moe.hookimpl
@@ -186,15 +186,15 @@
             this album.
         candidate: New candidate album with all metadata changes. Will be compared
             against ``old_album``.
 
     Raises:
         AbortImport: Import prompt was aborted by the user.
     """
-    log.debug(f"Running import prompt. [{new_album=!r}, {candidate=!r}]")
+    log.debug(f"Running import prompt. [{new_album=}, {candidate=}]")
 
     console.print(_fmt_import_updates(new_album, candidate))
 
     prompt_choices: list[PromptChoice] = []
     config.CONFIG.pm.hook.add_import_prompt_choice(prompt_choices=prompt_choices)
 
     prompt_choice = choice_prompt(prompt_choices)
@@ -208,17 +208,17 @@
     """Applies the album changes."""
     log.debug("Applying changes from import prompt.")
 
     for old_track, new_track in get_matching_tracks(new_album, candidate.album):
         if not old_track and new_track:
             candidate.album.tracks.remove(new_track)  # missing track
         elif old_track and not new_track:
-            new_album.tracks.remove(
-                new_album.get_track(old_track.track_num, old_track.disc)
-            )  # unmatched track
+            unmatched_track = new_album.get_track(old_track.track_num, old_track.disc)
+            assert unmatched_track
+            new_album.tracks.remove(unmatched_track)
         elif (
             old_track
             and new_track
             and new_album.get_track(new_track.track_num, new_track.disc) != old_track
         ):
             # matchup track and disc numbers of matches to ensure they merge properly
             old_track.track_num = new_track.track_num
```

### Comparing `moe-2.1.0/moe/moe_import/import_core.py` & `moe-2.1.1/moe/moe_import/import_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             new_album: Album being added to the library.
             candidates: New candidate albums with imported metadata sorted by how well
                  they match ``new_album``.
         """
 
 
 @moe.hookimpl
-def add_hooks(pm: pluggy.manager.PluginManager):
+def add_hooks(pm: pluggy._manager.PluginManager):
     """Registers `import` core hookspecs to Moe."""
     from moe.moe_import.import_core import Hooks
 
     pm.add_hookspecs(Hooks)
 
 
 @moe.hookimpl
@@ -108,19 +108,19 @@
         return
 
     import_album(album)
 
 
 def import_album(album: Album):
     """Imports album metadata for an album."""
-    log.debug(f"Importing album metadata. [{album=!r}]")
+    log.debug(f"Importing album metadata. [{album=}]")
 
     candidates = config.CONFIG.pm.hook.get_candidates(album=album)
     candidates = list(itertools.chain.from_iterable(candidates))
     candidates.sort(key=operator.attrgetter("match_value"), reverse=True)
 
     config.CONFIG.pm.hook.process_candidates(
         new_album=album,
         candidates=candidates,
     )
 
-    log.debug(f"Imported album metadata. [{album=!r}]")
+    log.debug(f"Imported album metadata. [{album=}]")
```

### Comparing `moe-2.1.0/moe/move/move_cli.py` & `moe-2.1.1/moe/move/move_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/moe/move/move_core.py` & `moe-2.1.1/moe/move/move_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import re
 import shutil
 from contextlib import suppress
 from pathlib import Path
 from typing import Callable, Optional, Union
 
 import dynaconf
+import dynaconf.base
 import pluggy
 from unidecode import unidecode
 
 import moe
 from moe import config
 from moe.library import Album, Extra, LibItem, Track
 
@@ -34,15 +35,15 @@
         Returns:
             A list of all custom path functions your plugin creates. The list should
             contain the callable functions themselves.
         """  # noqa: DAR202
 
 
 @moe.hookimpl
-def add_hooks(pm: pluggy.manager.PluginManager):
+def add_hooks(pm: pluggy._manager.PluginManager):
     """Registers `add` hookspecs to Moe."""
     from moe.move.move_core import Hooks
 
     pm.add_hookspecs(Hooks)
 
 
 @moe.hookimpl
@@ -57,15 +58,15 @@
 
     validators = [
         dynaconf.Validator("MOVE.ASCIIFY_PATHS", default=False),
         dynaconf.Validator("MOVE.ALBUM_PATH", default=default_album_path),
         dynaconf.Validator("MOVE.EXTRA_PATH", default=default_extra_path),
         dynaconf.Validator("MOVE.TRACK_PATH", default=default_track_path),
     ]
-    settings.validators.register(*validators)
+    settings.validators.register(*validators)  # type: ignore
 
 
 @moe.hookimpl(trylast=True)
 def edit_new_items(items: list[LibItem]):
     """Copies and formats the path of an item after it has been added to the library."""
     for item in items:
         copy_item(item)
@@ -182,15 +183,15 @@
         raise NotImplementedError
 
     plugin_funcs = config.CONFIG.pm.hook.create_path_template_func()
     for funcs in plugin_funcs:
         for func in funcs:
             globals()[func.__name__] = func
 
-    return eval(f'f"""{template}"""')
+    return eval(f'f"""{template}"""')  # noqa: B907
 
 
 def _sanitize_path_part(path_part: str) -> str:
     """Sanitizes a part of a path to be compatible with most filesystems.
 
     Note:
         Only sub-paths of the library path will be affected.
@@ -230,43 +231,43 @@
         _copy_file_item(item)
 
 
 def _copy_album(album: Album):
     """Copies an album to a destination as determined by the user configuration."""
     dest = fmt_item_path(album)
 
-    log.debug(f"Copying album. [{dest=}, {album=!r}]")
+    log.debug(f"Copying album. [{dest=}, {album=}]")
 
     dest.mkdir(parents=True, exist_ok=True)
     album.path = dest
 
     for track in album.tracks:
         _copy_file_item(track)
 
     for extra in album.extras:
         _copy_file_item(extra)
 
-    log.info(f"Album copied. [{dest=}, {album=!r}]")
+    log.info(f"Copied album. [{dest=!s}, {album=!s}]")
 
 
 def _copy_file_item(item: Union[Extra, Track]):
     """Copies an extra or track to a destination as determined by the user config."""
     dest = fmt_item_path(item)
     if dest.exists() and dest.samefile(item.path):
         item.path = dest
         return
 
-    log.debug(f"Copying item. [{dest=}, {item=!r}]")
+    log.debug(f"Copying item. [{dest=}, {item=}]")
 
     dest.parent.mkdir(parents=True, exist_ok=True)
     shutil.copyfile(item.path, dest)
 
     item.path = dest
 
-    log.info(f"Copied item. [{dest=}, {item=!r}]")
+    log.info(f"Copied item. [{dest=!s}, {item=!s}]")
 
 
 ########################################################################################
 # Move
 ########################################################################################
 def move_item(item: LibItem):
     """Moves an item to a destination as determined by the user configuration.
@@ -285,15 +286,15 @@
 
     Note:
         Empty leftover directories will be removed.
     """
     dest = fmt_item_path(album)
     old_album_dir = album.path
 
-    log.debug(f"Moving album. [{dest=}, {album=!r}]")
+    log.debug(f"Moving album. [{dest=}, {album=}]")
 
     dest.mkdir(parents=True, exist_ok=True)
     album.path = dest
 
     for track in album.tracks:
         _move_file_item(track)
 
@@ -306,25 +307,25 @@
             old_child.rmdir()
     with suppress(OSError):
         old_album_dir.rmdir()
     for old_parent in old_album_dir.parents:
         with suppress(OSError):
             old_parent.rmdir()
 
-    log.info(f"Moved album. [{dest=}, {album=!r}]")
+    log.info(f"Moved album. [{dest=!s}, {album=!s}]")
 
 
 def _move_file_item(item: Union[Extra, Track]):
     """Moves an extra or track to a destination as determined by the user config."""
     dest = fmt_item_path(item)
     if dest.exists() and dest.samefile(item.path):
         item.path = dest
         return
 
-    log.debug(f"Moving item. [{dest=}, {item=!r}]")
+    log.debug(f"Moving item. [{dest=}, {item=}]")
 
     dest.parent.mkdir(parents=True, exist_ok=True)
     item.path.replace(dest)
 
     item.path = dest
 
-    log.info(f"Moved item. [{dest=}, {item=!r}]")
+    log.info(f"Moved item. [{dest=!s}, {item=!s}]")
```

### Comparing `moe-2.1.0/moe/query.py` & `moe-2.1.1/moe/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Provides functionality to query the library for albums, extras, and tracks."""
 
 import logging
 import re
 import shlex
 from pathlib import Path
-from typing import Type
+from typing import Type, Union
 
 import sqlalchemy as sa
 import sqlalchemy.orm
 import sqlalchemy.sql.elements
 from sqlalchemy.orm.session import Session
 
 from moe.library import Album, Extra, LibItem, Track
@@ -26,15 +26,17 @@
 # each query will be split into these groups
 FIELD_TYPE = "field_type"
 FIELD = "field"
 SEPARATOR = "separator"
 VALUE = "value"
 
 
-def query(session: Session, query_str: str, query_type: str) -> list[LibItem]:
+def query(
+    session: Session, query_str: str, query_type: str
+) -> Union[list[Album], list[Extra], list[Track]]:
     """Queries the database for items matching the given query string.
 
     Args:
         session: Library db session.
         query_str: Query string to parse. See the query docs for more info.
         query_type: Type of library item to return: either 'album', 'extra', or 'track'.
 
@@ -43,15 +45,15 @@
 
     Raises:
         QueryError: Invalid query.
 
     See Also:
         `The query docs <https://mrmoe.readthedocs.io/en/latest/query.html>`_
     """
-    log.debug(f"Querying library for items. [{query_str=!r}, {query_type=!r}]")
+    log.debug(f"Querying library for items. [{query_str=}, {query_type=}]")
 
     terms = shlex.split(query_str)
     if not terms:
         raise QueryError("No query given.")
 
     if query_type == "album":
         library_query = session.query(Album)
@@ -63,24 +65,24 @@
         library_query = session.query(Track).join(Album)
     if query_type != "extra" and session.query(Extra).first():
         library_query = library_query.join(Extra)
 
     for term in terms:
         parsed_term = _parse_term(term)
         library_query = library_query.filter(
-            _create_filter_expression(
+            _create_filter_expression(  # type: ignore
                 parsed_term[FIELD_TYPE],
                 parsed_term[FIELD],
                 parsed_term[SEPARATOR],
                 parsed_term[VALUE],
             )
         )
     items = library_query.all()
 
-    log.debug(f"Queried library for items. [{items=!r}]")
+    log.debug(f"Queried library for items. [{items=}]")
     return items
 
 
 def _parse_term(term: str) -> dict[str, str]:
     """Parse the given database query term.
 
     A term is a single field:value declaration.
@@ -118,15 +120,15 @@
         (?P<{VALUE}>.*)
         """,
         re.VERBOSE,
     )
 
     match = re.match(query_re, term)
     if not match:
-        raise QueryError(f"Invalid query term. [{term=!r}]")
+        raise QueryError(f"Invalid query term. [{term=}]")
 
     match_dict = match.groupdict()
     match_dict[FIELD] = match_dict[FIELD].lower()
     if match_dict[FIELD_TYPE] == "a:":
         match_dict[FIELD_TYPE] = "album"
     elif match_dict[FIELD_TYPE] == "e:":
         match_dict[FIELD_TYPE] = "extra"
@@ -153,21 +155,21 @@
 
     Raises:
         QueryError: Invalid query given.
     """
     attr = _get_field_attr(field, field_type)
 
     if separator == ":":
-        if match := re.fullmatch(r"(?P<low>\d*)..(?P<high>\d*)", value):
-            if match["low"] and match["high"]:
-                return sa.and_(attr >= match["low"], attr <= match["high"])
-            if match["low"]:
-                return attr >= match["low"]
-            if match["high"]:
-                return attr <= match["high"]
+        if num_range := re.fullmatch(r"(?P<min>\d*)..(?P<max>\d*)", value):
+            if num_range["min"] and num_range["max"]:
+                return sa.and_(attr >= num_range["min"], attr <= num_range["max"])
+            if num_range["min"]:
+                return attr >= num_range["min"]
+            if num_range["max"]:
+                return attr <= num_range["max"]
 
         if str(attr).endswith(".path"):
             return attr == Path(value)
 
         # normal string match query - should be case insensitive
         return attr.ilike(value, escape="/")
     elif separator == "::":
@@ -176,15 +178,15 @@
         except re.error as re_err:
             raise QueryError(
                 f"Invalid regular expression. [regex={value!r}]"
             ) from re_err
 
         return attr.op("regexp")(sa.sql.expression.literal(value))
 
-    raise QueryError(f"Invalid query type separator. [{separator=!r}]")
+    raise QueryError(f"Invalid query type separator. [{separator=}]")
 
 
 def _get_field_attr(field: str, field_type: str):
     """Gets the corresponding attribute for the given field to use in a query filter."""
     # convert singular multi-value fields to their plural equivalents
     if field == "catalog_num" and field_type == "album":
         field = "catalog_nums"
```

### Comparing `moe-2.1.0/moe/read/read_cli.py` & `moe-2.1.1/moe/read/read_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,12 +51,12 @@
     for item in items:
         try:
             read.read_item(item)
         except FileNotFoundError:
             if args.remove:
                 remove.remove_item(session, item)
             else:
-                log.error(f"Could not find item's path. [{item=!r}]")
+                log.error(f"Could not find item's path. [{item=}]")
                 error_count += 1
 
     if error_count:
         raise SystemExit(1)
```

### Comparing `moe-2.1.0/moe/read/read_core.py` & `moe-2.1.1/moe/read/read_core.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,18 +14,18 @@
 
     Args:
         item: Item to update.
 
     Raises:
         FileNotFoundError: Item's path doesn't exist.
     """
-    log.debug(f"Reading item's file for changes. [{item=!r}]")
+    log.debug(f"Reading item's file for changes. [{item=}]")
 
     if not item.path.exists():
         raise FileNotFoundError(f"Item's path does not exist. [path={item.path!r}]")
 
     if isinstance(item, Track):
         item.merge(Track.from_file(item.path), overwrite=True)
     elif isinstance(item, Album):
         item.merge(Album.from_dir(item.path), overwrite=True)
 
-    log.info(f"Updated item from filesystem. [{item=!r}]")
+    log.info(f"Updated item from filesystem. [{item=!s}]")
```

### Comparing `moe-2.1.0/moe/remove/rm_cli.py` & `moe-2.1.1/moe/remove/rm_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.0/moe/remove/rm_core.py` & `moe-2.1.1/moe/remove/rm_core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """Core api for removing items from the library."""
 
 import logging
 
 import sqlalchemy
 import sqlalchemy.exc
 from sqlalchemy.orm.session import Session
+from sqlalchemy.orm.state import InstanceState
 
 from moe.library import Extra, LibItem, Track
 
 __all__ = ["remove_item"]
 
 log = logging.getLogger("moe.remove")
 
 
 def remove_item(session: Session, item: LibItem):
     """Removes an item from the library."""
-    log.debug(f"Removing item from the library. [{item=!r}]")
+    log.debug(f"Removing item from the library. [{item=}]")
 
     insp = sqlalchemy.inspect(item)
+    assert isinstance(insp, InstanceState)
+
     if insp.persistent:
         session.delete(item)
     elif insp.pending:
         session.expunge(item)
         if isinstance(item, (Track, Extra)):
             item.album = None  # type: ignore
 
@@ -32,8 +35,8 @@
         # occurs before any inserts or updates in the original session
         if insp.persistent:
             session.expunge(item)
             new_session = Session(session.connection())
             new_session.delete(item)
             new_session.flush()
 
-    log.info(f"Removed item from the library. [{item=!r}]")
+    log.info(f"Removed item from the library. [{item=!s}]")
```

### Comparing `moe-2.1.0/moe/util/cli/prompt.py` & `moe-2.1.1/moe/util/cli/prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,9 +66,9 @@
         question, choices=questionary_choices, use_shortcuts=True, use_arrow_keys=True
     ).ask()
 
     for prompt_choice in prompt_choices:
         if prompt_choice.shortcut_key == user_input:
             return prompt_choice
 
-    log.error(f"Invalid option selected. [{user_input=!r}]")
+    log.error(f"Invalid option selected. [{user_input=}]")
     raise SystemExit(1)
```

### Comparing `moe-2.1.0/moe/util/cli/query.py` & `moe-2.1.1/moe/util/cli/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """CLI-specific query help functionality."""
 
 import argparse
 import logging
+from typing import Union
 
 from sqlalchemy.orm.session import Session
 
-from moe.library import LibItem
+from moe.library import Album, Extra, Track
 from moe.query import QueryError, query
 
 __all__ = ["cli_query", "query_parser"]
 
 log = logging.getLogger("moe.cli")
 
 query_parser = argparse.ArgumentParser(
@@ -56,15 +57,17 @@
     const="extra",
     dest="query_type",
     help="query for matching extras",
 )
 query_parser.set_defaults(query_type="track")
 
 
-def cli_query(session: Session, query_str: str, query_type: str) -> list[LibItem]:
+def cli_query(
+    session: Session, query_str: str, query_type: str
+) -> Union[list[Album], list[Extra], list[Track]]:
     """Wrapper around the core query call, with some added cli error handling.
 
     Args:
         session: Library db session.
         query_str: Query string to parse. See the query docs for more info.
         query_type: Type of library item to return: either 'album', 'extra', or 'track'.
```

### Comparing `moe-2.1.0/moe/util/core/match.py` & `moe-2.1.1/moe/util/core/match.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from moe.library import MetaAlbum, MetaTrack
 
 log = logging.getLogger("moe")
 
 __all__ = ["get_match_value", "get_matching_tracks"]
 
+# Custom type declarations used for abbreviated annotations.
 TrackMatch = tuple[Optional[MetaTrack], Optional[MetaTrack]]
 TrackCoord = tuple[
     tuple[int, int], tuple[int, int]
 ]  # ((a.disc, a.track_num), (b.disc, b.track_num))
 
 MATCH_ALBUM_FIELD_WEIGHTS = {
     "artist": 0.8,
@@ -45,15 +46,15 @@
         item_b: Second item to compare. Should be the same type as ``item_a``
             or a subclass i.e. ``MetaAlbums`` and ``Albums`` can be compared.
 
     Returns:
         The match value is a weighted sum according to the defined weights for each
         applicable field.
     """
-    log.debug(f"Determining match value between items. [{item_a=!r}, {item_b=!r}]")
+    log.debug(f"Determining match value between items. [{item_a=}, {item_b=}]")
 
     if issubclass(type(item_a), MetaAlbum):
         field_weights = MATCH_ALBUM_FIELD_WEIGHTS
     else:
         field_weights = MATCH_TRACK_FIELD_WEIGHTS
 
     penalties = []
@@ -74,15 +75,15 @@
                 else:
                     penalty = 0
 
         penalties.append(penalty * weight)
 
     match_value = 1 - sum(penalties) / sum(field_weights.values())
 
-    log.debug(f"Determined match value between items. [{match_value=!r}]")
+    log.debug(f"Determined match value between items. [{match_value=}]")
     return match_value
 
 
 def get_matching_tracks(  # noqa: C901 (I don't see benefit from splitting)
     album_a: MetaAlbum, album_b: MetaAlbum, match_threshold: float = 0.7
 ) -> list[TrackMatch]:
     """Returns a list of tuples of track match pairs.
@@ -95,17 +96,15 @@
 
     Returns:
         A list of tuples of track match pairs. Each track in ``album_a`` and
         ``album_b`` will appear with its respective track match or ``None`` if no match
         was found. Each tuple represents a match and will be in the form
         ``(album_a_track, album_b_track)``.
     """
-    log.debug(
-        f"Finding matching tracks. [{album_a=!r}, {album_b=!r}, {match_threshold=!r}]"
-    )
+    log.debug(f"Finding matching tracks. [{album_a=}, {album_b=}, {match_threshold=}]")
 
     # get all match values for every pair of tracks between both albums
     track_match_values: dict[TrackCoord, float] = {}
     for a_track in album_a.tracks:
         for b_track in album_b.tracks:
             track_match_values[
                 ((a_track.disc, a_track.track_num), (b_track.disc, b_track.track_num))
```

### Comparing `moe-2.1.0/moe/write.py` & `moe-2.1.1/moe/write.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             * `Mediafile docs <https://mediafile.readthedocs.io/en/latest/>`_
             * The :meth:`~moe.library.track.Hooks.read_custom_tags` hook for reading
               tags.
         """
 
 
 @moe.hookimpl
-def add_hooks(pm: pluggy.manager.PluginManager):
+def add_hooks(pm: pluggy._manager.PluginManager):
     """Registers `write` hookspecs to Moe."""
     from moe.write import Hooks
 
     pm.add_hookspecs(Hooks)
 
 
 @moe.hookimpl
@@ -95,12 +95,12 @@
     audio_file.tracktotal = track.album.track_total
 
     audio_file.save()
 
 
 def write_tags(track: Track):
     """Write tags to a track's file."""
-    log.debug(f"Writing tags to track. [{track=!r}]")
+    log.debug(f"Writing tags to track. [{track=}]")
 
     config.CONFIG.pm.hook.write_custom_tags(track=track)
 
-    log.info(f"Wrote tags to track. [{track=!r}]")
+    log.info(f"Wrote tags to track. [{track=!s}]")
```

### Comparing `moe-2.1.0/pyproject.toml` & `moe-2.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "Moe"
 include = ["alembic/*", "alembic/versions/*"]
-version = "2.1.0"
+version = "2.1.1"
 description = "The ultimate tool for managing your music library."
 authors = ["Jacob Pavlock <jtpavlock@gmail.com>"]
 repository = "https://github.com/MoeMusic/Moe"
 documentation = "https://mrmoe.readthedocs.io/en/latest/index.html"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
@@ -19,51 +19,51 @@
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 alembic = "^1.4.2"
 dynaconf = "^3.1.4"
 mediafile = "^0.11.0"
 musicbrainzngs = "^0.7.1"
-pluggy = "^0.13.1"
-rich = "^12.5.1"
-SQLAlchemy = "^1.4.15"
+pluggy = "^1.0.0"
+rich = "^13.0.0"
+SQLAlchemy = "^2.0.0"
 Unidecode = "^1.2.0"
 questionary = "^1.9.0"
 
 [tool.poetry.group.test.dependencies]
 debugpy = "^1.4.1"
-pytest = "^6.0.1"
-pytest-cov = "^2.10.0"
-tox = "^3.26.0"
+pytest = "^7.0.0"
+pytest-cov = "^4.0.0"
+tox = "^4.0.0"
 
 [tool.poetry.group.lint.dependencies]
-black = "^22.6.0"
-commitizen = "^2.17.12"
+black = "^23.0.0"
+commitizen = "^3.0.0"
 darglint = "^1.8.1"
-flake8 = "^5.0.4"
-flake8-alphabetize = "^0.0.17"
-flake8-bugbear = "^22.7.1"
+flake8 = "^6.0.0"
+flake8-alphabetize = "^0.0.19"
+flake8-bugbear = "^23.0.0"
 flake8-comprehensions = "^3.10.0"
 flake8-docstrings = "^1.5.0"
 flake8-pytest-style = "^1.6.0"
 flake8-use-fstring = "^1.1"
 "github3.py" = "^3.2.0"
 isort = "^5.10.1"
 mccabe = "^0.7.0"
-pre-commit = "^2.6.0"
+pre-commit = "^3.0.0"
 pyright = "^1.1.267"
 
 [tool.poetry.group.docs.dependencies]
 furo = "*"
 pypandoc = "^1.9"
-Sphinx = "^5.2.3"
+Sphinx = "^6.0.0"
 
 [tool.commitizen]
 name = "cz_customize"
-version = "2.1.0"
+version = "2.1.1"
 version_files = [
     "pyproject.toml:^version",
 ]
 tag_format = "v$version"
 
 [tool.commitizen.customize]
 schema_pattern = '(build|ci|deprecate|docs|feat|fix|perf|refactor|release|style|test)(\(\w+\))?!?:\s\S.*'
```

### Comparing `moe-2.1.0/setup.py` & `moe-2.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,93 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: moe
+Version: 2.1.1
+Summary: The ultimate tool for managing your music library.
+Home-page: https://github.com/MoeMusic/Moe
+License: MIT
+Author: Jacob Pavlock
+Author-email: jtpavlock@gmail.com
+Requires-Python: >=3.9,<3.12
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Multimedia :: Sound/Audio :: Editors
+Requires-Dist: SQLAlchemy (>=2.0.0,<3.0.0)
+Requires-Dist: Unidecode (>=1.2.0,<2.0.0)
+Requires-Dist: alembic (>=1.4.2,<2.0.0)
+Requires-Dist: dynaconf (>=3.1.4,<4.0.0)
+Requires-Dist: mediafile (>=0.11.0,<0.12.0)
+Requires-Dist: musicbrainzngs (>=0.7.1,<0.8.0)
+Requires-Dist: pluggy (>=1.0.0,<2.0.0)
+Requires-Dist: questionary (>=1.9.0,<2.0.0)
+Requires-Dist: rich (>=13.0.0,<14.0.0)
+Project-URL: Documentation, https://mrmoe.readthedocs.io/en/latest/index.html
+Project-URL: Repository, https://github.com/MoeMusic/Moe
+Description-Content-Type: text/x-rst
+
+###############
+Welcome to Moe!
+###############
+Moe is our resident Music-Organizer-Extraordinaire who's sole purpose is to give you full control over your music library by streamlining the process between downloading/ripping music to your filesystem and listening to it with your favorite music player.
+
+In short, Moe maintains a database of your music library that can be updated with various metadata sources, queried, edited, etc. through either an API or command-line interface. All of these features, and more, are made available by a highly extensible plugin ecosystem.
+
+Because all of this functionality is available as a python API which doesn't always require a database of music to operate on, Moe also provides an extensive suite of tools for handling and operating on music files. This can greatly simplify or enhance any other script/program that deals with music.
+
+Usage
+=====
+
+CLI
+---
+Moe comes with a command-line interface which is how most users will take advantage of the library management features. Below is a screenshot of Moe importing an album from the filesystem and adding it to the underlying database all while fixing tags, relocating the files, and anything else you can imagine.
+
+.. image:: _static/import_example.png
+
+Once added to Moe, querying your library or manipulating your music by editing tags, renaming files, etc. is all just a single command away. The ultimate goal is to automate away any tedius and time-consuming steps you have in your workflow without sacrificing the attention to detail. With the help of an *extremely* flexible plugin system, you can easily fine-tune your music library exactly how you like.
+
+Library
+-------
+As previously mentioned, all of Moe's music management logic and functionality is also available as a python library. As an example, below is a standalone script that takes an album directory and Musicbrainz release ID from the command-line, and then updates the underlying files' tags with any changes from Musicbrainz.
+
+.. code:: python
+
+    #!/usr/bin/env python3
+
+    import argparse
+    import pathlib
+
+    from moe.config import Config, ConfigValidationError
+    from moe.library import Album
+    from moe.write import write_tags
+    import moe_musicbrainz
+
+    def main():
+        try:
+            config.Config(config_dir=Path.home() / ".config" / "my_script", init_db=False)
+        except config.ConfigValidationError as err:
+            raise SystemExit(1) from err
+
+        parser = argparse.ArgumentParser(
+            description="Update an album with musicbrainz tags."
+        )
+        parser.add_argument("path", help="dir of the album to update")
+        parser.add_argument("mb_id", help="musicbrainz id of the album to fetch")
+        args = parser.parse_args()
+
+        album = Album.from_dir(pathlib.Path(args.path))
+
+        album.merge(moe_musicbrainz.get_album_by_id(args.mb_id), overwrite=True)
+
+        for track in album.tracks:
+            write_tags(track)
 
-packages = \
-['moe',
- 'moe.add',
- 'moe.duplicate',
- 'moe.edit',
- 'moe.library',
- 'moe.moe_import',
- 'moe.move',
- 'moe.read',
- 'moe.remove',
- 'moe.util',
- 'moe.util.cli',
- 'moe.util.core']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['SQLAlchemy>=1.4.15,<2.0.0',
- 'Unidecode>=1.2.0,<2.0.0',
- 'alembic>=1.4.2,<2.0.0',
- 'dynaconf>=3.1.4,<4.0.0',
- 'mediafile>=0.11.0,<0.12.0',
- 'musicbrainzngs>=0.7.1,<0.8.0',
- 'pluggy>=0.13.1,<0.14.0',
- 'questionary>=1.9.0,<2.0.0',
- 'rich>=12.5.1,<13.0.0']
-
-entry_points = \
-{'console_scripts': ['moe = moe.cli:main']}
-
-setup_kwargs = {
-    'name': 'moe',
-    'version': '2.1.0',
-    'description': 'The ultimate tool for managing your music library.',
-    'long_description': '###############\nWelcome to Moe!\n###############\nMoe is our resident Music-Organizer-Extraordinaire who\'s sole purpose is to give you full control over your music library by streamlining the process between downloading/ripping music to your filesystem and listening to it with your favorite music player.\n\nIn short, Moe maintains a database of your music library that can be updated with various metadata sources, queried, edited, etc. through either an API or command-line interface. All of these features, and more, are made available by a highly extensible plugin ecosystem.\n\nUsage\n=====\nMoe comes with a command-line interface which is how most users will take advantage of the library management features. Below is a screenshot of Moe importing an album from the filesystem and adding it to the underlying database all while fixing tags, relocating the files, and anything else you can imagine.\n\n.. image:: _static/import_example.png\n\nAlternatively, because all the core functionality is available via an API, the underlying music management system can be incorporated into any existing program or other user interface.\n\nFinally, although a lot of Moe\'s functionality exists around the idea of operating on a library database of your music, the database is entirely optional. In this case, Moe provides a convenient set of tools and functionality for handling music in a general sense. For example, below is a standalone python script that takes an album directory and Musicbrainz release ID from the command-line, and then updates the underlying files\' tags with any changes from Musicbrainz (utilizing the ``musicbrainz`` plugin).\n\n.. code:: python\n\n    #!/usr/bin/env python3\n\n    import argparse\n    import pathlib\n\n    from moe.config import Config, ConfigValidationError\n    from moe.library import Album\n    from moe.write import write_tags\n    import moe_musicbrainz\n\n    def main():\n        try:\n            config.Config(config_dir=Path.home() / ".config" / "my_script", init_db=False)\n        except config.ConfigValidationError as err:\n            raise SystemExit(1) from err\n\n        parser = argparse.ArgumentParser(\n            description="Update an album with musicbrainz tags."\n        )\n        parser.add_argument("path", help="dir of the album to update")\n        parser.add_argument("mb_id", help="musicbrainz id of the album to fetch")\n        args = parser.parse_args()\n\n        album = Album.from_dir(pathlib.Path(args.path))\n\n        album.merge(moe_musicbrainz.get_album_by_id(args.mb_id), overwrite=True)\n\n        for track in album.tracks:\n            write_tags(track)\n\n\n    if __name__ == "__main__":\n        main()\n\nThis is just a small taste of what Moe is capable of and how it can make your life easier when dealing with music in Python.\n\nIf you want to learn more, check out the `Getting Started <https://mrmoe.readthedocs.io/en/latest/getting_started.html>`_ docs.\n',
-    'author': 'Jacob Pavlock',
-    'author_email': 'jtpavlock@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/MoeMusic/Moe',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<3.12',
-}
 
+    if __name__ == "__main__":
+        main()
+
+This is just a small taste of what Moe is capable of and how it can make your life easier when dealing with music.
+
+If you want to learn more, check out the `Getting Started <https://mrmoe.readthedocs.io/en/latest/getting_started.html>`_ docs.
 
-setup(**setup_kwargs)
```

