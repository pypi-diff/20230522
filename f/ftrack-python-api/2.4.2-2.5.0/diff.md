# Comparing `tmp/ftrack-python-api-2.4.2.tar.gz` & `tmp/ftrack-python-api-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftrack-python-api-2.4.2.tar", last modified: Tue Mar 28 16:18:40 2023, max compression
+gzip compressed data, was "ftrack-python-api-2.5.0.tar", last modified: Fri May 19 09:04:55 2023, max compression
```

## Comparing `ftrack-python-api-2.4.2.tar` & `ftrack-python-api-2.5.0.tar`

### file list

```diff
@@ -1,250 +1,251 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.457820 ftrack-python-api-2.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.437820 ftrack-python-api-2.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.441820 ftrack-python-api-2.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/LICENSE.python
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-03-28 16:18:40.457820 ftrack-python-api-2.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.441820 ftrack-python-api-2.4.2/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.441820 ftrack-python-api-2.4.2/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/_static/ftrack.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.445820 ftrack-python-api-2.4.2/doc/api_reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.445820 ftrack-python-api-2.4.2/doc/api_reference/accessor/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/accessor/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/accessor/disk.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/accessor/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/accessor/server.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/attribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/cache.rst
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/collection.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.445820 ftrack-python-api-2.4.2/doc/api_reference/entity/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/entity/asset_version.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/entity/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/entity/component.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/entity/factory.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/entity/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/entity/job.rst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/entity/location.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/entity/note.rst
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/entity/project_schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/entity/user.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.445820 ftrack-python-api-2.4.2/doc/api_reference/event/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/event/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/event/expression.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/event/hub.rst
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/event/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/event/subscriber.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/event/subscription.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/exception.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/formatter.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/inspection.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/operation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/plugin.rst
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/query.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.445820 ftrack-python-api-2.4.2/doc/api_reference/resource_identifier_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/resource_identifier_transformer/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/resource_identifier_transformer/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/session.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.445820 ftrack-python-api-2.4.2/doc/api_reference/structure/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/structure/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/structure/id.rst
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/structure/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/structure/origin.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/structure/standard.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/api_reference/symbol.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/caching.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/docutils.conf
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/environment_variables.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/event_list.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.449820 ftrack-python-api-2.4.2/doc/example/
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/assignments_and_allocations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/component.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/custom_attribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/custom_attribute_link.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/encode_media.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/entity_links.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/invite_user.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/job.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/link_attribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/list.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/manage_custom_attribute_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/note.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/project.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/publishing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/review_session.rst
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/scope.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/security_roles.rst
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/sync_ldap_users.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/task_template.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/thumbnail.rst
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/timer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/web_review.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/example/workflow_schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/handling_events.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.449820 ftrack-python-api-2.4.2/doc/image/
--rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/image/configuring_plugins_directory.png
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/introduction.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.449820 ftrack-python-api-2.4.2/doc/locations/
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/locations/configuring.rst
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/locations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/locations/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/locations/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10783 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/querying.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.449820 ftrack-python-api-2.4.2/doc/release/
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/release/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18973 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/release/migrating_from_old_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/release/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    49794 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/release/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.449820 ftrack-python-api-2.4.2/doc/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/resource/example_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/resource/example_plugin_safe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/resource/example_plugin_using_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/security_and_authentication.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/understanding_sessions.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/doc/working_with_entities.rst
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.441820 ftrack-python-api-2.4.2/resource/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.449820 ftrack-python-api-2.4.2/resource/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/resource/plugin/configure_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/resource/plugin/construct_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-28 16:18:40.457820 ftrack-python-api-2.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.449820 ftrack-python-api-2.4.2/source/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.449820 ftrack-python-api-2.4.2/source/ftrack_api/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24335 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/_centralized_storage_scenario.py
--rw-r--r--   0 runner    (1001) docker     (123)    18552 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/_python_ntpath.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-28 16:18:40.000000 ftrack-python-api-2.4.2/source/ftrack_api/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/_weakref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.449820 ftrack-python-api-2.4.2/source/ftrack_api/accessor/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/accessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/accessor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/accessor/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/accessor/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    24242 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.453820 ftrack-python-api-2.4.2/source/ftrack_api/entity/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/entity/asset_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    14718 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/entity/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/entity/component.py
--rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/entity/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/entity/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    27770 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/entity/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/entity/note.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/entity/project_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/entity/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.453820 ftrack-python-api-2.4.2/source/ftrack_api/event/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/event/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/event/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    41173 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/event/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/event/subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/event/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.453820 ftrack-python-api-2.4.2/source/ftrack_api/resource_identifier_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/resource_identifier_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/resource_identifier_transformer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    91354 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.453820 ftrack-python-api-2.4.2/source/ftrack_api/structure/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/structure/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/structure/entity_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/structure/id.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/structure/origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/structure/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/source/ftrack_api/symbol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.453820 ftrack-python-api-2.4.2/source/ftrack_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-03-28 16:18:40.000000 ftrack-python-api-2.4.2/source/ftrack_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-03-28 16:18:40.000000 ftrack-python-api-2.4.2/source/ftrack_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 16:18:40.000000 ftrack-python-api-2.4.2/source/ftrack_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 16:18:40.000000 ftrack-python-api-2.4.2/source/ftrack_python_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-28 16:18:40.000000 ftrack-python-api-2.4.2/source/ftrack_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-28 16:18:40.000000 ftrack-python-api-2.4.2/source/ftrack_python_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.441820 ftrack-python-api-2.4.2/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.441820 ftrack-python-api-2.4.2/test/fixture/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.453820 ftrack-python-api-2.4.2/test/fixture/media/
--rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/fixture/media/colour_wheel.mov
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/fixture/media/image-resized-10.png
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/fixture/media/image.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.453820 ftrack-python-api-2.4.2/test/fixture/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/fixture/plugin/configure_locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/fixture/plugin/construct_entity_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/fixture/plugin/count_session_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/fixture/plugin/get_file_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.453820 ftrack-python-api-2.4.2/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.457820 ftrack-python-api-2.4.2/test/unit/accessor/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/accessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/accessor/test_disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/accessor/test_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.457820 ftrack-python-api-2.4.2/test/unit/entity/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/entity/test_asset_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/entity/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/entity/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/entity/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/entity/test_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/entity/test_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/entity/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/entity/test_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/entity/test_project_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/entity/test_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/entity/test_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.457820 ftrack-python-api-2.4.2/test/unit/event/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/event/event_hub_server_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/event/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/event/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    22869 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/event/test_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/event/test_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/event/test_subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.457820 ftrack-python-api-2.4.2/test/unit/resource_identifier_transformer/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/resource_identifier_transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/resource_identifier_transformer/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 16:18:40.457820 ftrack-python-api-2.4.2/test/unit/structure/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/structure/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/structure/test_entity_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/structure/test_get_file_from_string_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/structure/test_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/structure/test_origin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/structure/test_standard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/test_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16722 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/test_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/test_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/test_inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/test_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    47839 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-03-28 16:18:16.000000 ftrack-python-api-2.4.2/test/unit/test_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.616794 ftrack-python-api-2.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.584794 ftrack-python-api-2.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.588794 ftrack-python-api-2.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/.github/workflows/pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/LICENSE.python
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-19 09:04:55.616794 ftrack-python-api-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.592794 ftrack-python-api-2.5.0/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.592794 ftrack-python-api-2.5.0/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/_static/ftrack.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.592794 ftrack-python-api-2.5.0/doc/api_reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.592794 ftrack-python-api-2.5.0/doc/api_reference/accessor/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/accessor/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/accessor/disk.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/accessor/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/accessor/server.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/cache.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/collection.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.592794 ftrack-python-api-2.5.0/doc/api_reference/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/entity/asset_version.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/entity/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/entity/component.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/entity/factory.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/entity/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/entity/job.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/entity/location.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/entity/note.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/entity/project_schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/entity/user.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.596794 ftrack-python-api-2.5.0/doc/api_reference/event/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/event/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/event/expression.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/event/hub.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/event/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/event/subscriber.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/event/subscription.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/formatter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/inspection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/operation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/query.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.596794 ftrack-python-api-2.5.0/doc/api_reference/resource_identifier_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/resource_identifier_transformer/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/resource_identifier_transformer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/session.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.596794 ftrack-python-api-2.5.0/doc/api_reference/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/structure/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/structure/id.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/structure/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/structure/origin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/structure/standard.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/api_reference/symbol.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/caching.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/docutils.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/environment_variables.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/event_list.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.600794 ftrack-python-api-2.5.0/doc/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/assignments_and_allocations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/component.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/custom_attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/custom_attribute_link.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/encode_media.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/entity_links.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/invite_user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/job.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/link_attribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/list.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/manage_custom_attribute_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/note.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/publishing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/review_session.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/scope.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/security_roles.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/sync_ldap_users.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/task_template.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/thumbnail.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/timer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/web_review.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/example/workflow_schema.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/handling_events.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.600794 ftrack-python-api-2.5.0/doc/image/
+-rw-r--r--   0 runner    (1001) docker     (123)     7313 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/image/configuring_plugins_directory.png
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/introduction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.600794 ftrack-python-api-2.5.0/doc/locations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/locations/configuring.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/locations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/locations/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/locations/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10783 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/querying.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.600794 ftrack-python-api-2.5.0/doc/release/
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/release/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18973 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/release/migrating_from_old_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/release/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    49794 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/release/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.600794 ftrack-python-api-2.5.0/doc/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/resource/example_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/resource/example_plugin_safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/resource/example_plugin_using_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/security_and_authentication.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/understanding_sessions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15639 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/doc/working_with_entities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.584794 ftrack-python-api-2.5.0/resource/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.600794 ftrack-python-api-2.5.0/resource/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/resource/plugin/configure_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/resource/plugin/construct_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-19 09:04:55.616794 ftrack-python-api-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.600794 ftrack-python-api-2.5.0/source/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.604794 ftrack-python-api-2.5.0/source/ftrack_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24335 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/_centralized_storage_scenario.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18552 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/_python_ntpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-19 09:04:55.000000 ftrack-python-api-2.5.0/source/ftrack_api/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/_weakref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.604794 ftrack-python-api-2.5.0/source/ftrack_api/accessor/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/accessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/accessor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/accessor/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/accessor/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24242 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16162 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.604794 ftrack-python-api-2.5.0/source/ftrack_api/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/entity/asset_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14718 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/entity/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/entity/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15526 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/entity/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/entity/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27770 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/entity/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/entity/note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/entity/project_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/entity/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.604794 ftrack-python-api-2.5.0/source/ftrack_api/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/event/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/event/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41173 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/event/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/event/subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/event/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.604794 ftrack-python-api-2.5.0/source/ftrack_api/resource_identifier_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/resource_identifier_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/resource_identifier_transformer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91692 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.608794 ftrack-python-api-2.5.0/source/ftrack_api/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/structure/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/structure/entity_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/structure/id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/structure/origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/structure/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/source/ftrack_api/symbol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.608794 ftrack-python-api-2.5.0/source/ftrack_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-19 09:04:55.000000 ftrack-python-api-2.5.0/source/ftrack_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-19 09:04:55.000000 ftrack-python-api-2.5.0/source/ftrack_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:04:55.000000 ftrack-python-api-2.5.0/source/ftrack_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:04:55.000000 ftrack-python-api-2.5.0/source/ftrack_python_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-19 09:04:55.000000 ftrack-python-api-2.5.0/source/ftrack_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-19 09:04:55.000000 ftrack-python-api-2.5.0/source/ftrack_python_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.588794 ftrack-python-api-2.5.0/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.588794 ftrack-python-api-2.5.0/test/fixture/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.608794 ftrack-python-api-2.5.0/test/fixture/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    17627 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/fixture/media/colour_wheel.mov
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/fixture/media/image-resized-10.png
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/fixture/media/image.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.608794 ftrack-python-api-2.5.0/test/fixture/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/fixture/plugin/configure_locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/fixture/plugin/construct_entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/fixture/plugin/count_session_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/fixture/plugin/get_file_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.612794 ftrack-python-api-2.5.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.612794 ftrack-python-api-2.5.0/test/unit/accessor/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/accessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8097 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/accessor/test_disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/accessor/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.612794 ftrack-python-api-2.5.0/test/unit/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/entity/test_asset_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/entity/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/entity/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/entity/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/entity/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/entity/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/entity/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/entity/test_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/entity/test_project_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/entity/test_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/entity/test_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.612794 ftrack-python-api-2.5.0/test/unit/event/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/event/event_hub_server_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/event/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/event/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22869 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/event/test_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/event/test_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/event/test_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.616794 ftrack-python-api-2.5.0/test/unit/resource_identifier_transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/resource_identifier_transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/resource_identifier_transformer/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:04:55.616794 ftrack-python-api-2.5.0/test/unit/structure/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/structure/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/structure/test_entity_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/structure/test_get_file_from_string_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/structure/test_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/structure/test_origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9313 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/structure/test_standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/test_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16722 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/test_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6836 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/test_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/test_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/test_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5908 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4787 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47839 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-19 09:04:29.000000 ftrack-python-api-2.5.0/test/unit/test_timer.py
```

### Comparing `ftrack-python-api-2.4.2/.github/workflows/cicd.yml` & `ftrack-python-api-2.5.0/.github/workflows/cicd.yml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
       - uses: actions/checkout@v3
       - name: Run pytest
         run: |
           python setup.py test
         env:
           FTRACK_SERVER: http://ftrack:80
           FTRACK_API_USER: ${{ secrets.FTRACK_API_USER }}
-          FTRACK_API_KEY: ${{ secrets.FTRACK_API_KEY }}
+          FTRACK_API_KEY: ${{ secrets.FTRACK_API_KEY_UNITTEST }}
   build:
     runs-on: ubuntu-latest
     name: Build package distribution
     steps:
       - uses: actions/checkout@v1
       - uses: actions/setup-python@v4
         with:
```

### Comparing `ftrack-python-api-2.4.2/LICENSE.python` & `ftrack-python-api-2.5.0/LICENSE.python`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/LICENSE.txt` & `ftrack-python-api-2.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/PKG-INFO` & `ftrack-python-api-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftrack-python-api
-Version: 2.4.2
+Version: 2.5.0
 Summary: Python API for ftrack.
 Home-page: https://github.com/ftrackhq/ftrack-python
 Author: ftrack
 Author-email: support@ftrack.com
 License: Apache License (2.0)
 Project-URL: Documentation, http://ftrack-python-api.rtd.ftrack.com/en/Unknown version/
 Project-URL: Source Code, https://github.com/ftrackhq/ftrack-python/src/Unknown version
```

### Comparing `ftrack-python-api-2.4.2/README.rst` & `ftrack-python-api-2.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/caching.rst` & `ftrack-python-api-2.5.0/doc/caching.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/conf.py` & `ftrack-python-api-2.5.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/environment_variables.rst` & `ftrack-python-api-2.5.0/doc/environment_variables.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/event_list.rst` & `ftrack-python-api-2.5.0/doc/event_list.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/assignments_and_allocations.rst` & `ftrack-python-api-2.5.0/doc/example/assignments_and_allocations.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/component.rst` & `ftrack-python-api-2.5.0/doc/example/component.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/custom_attribute.rst` & `ftrack-python-api-2.5.0/doc/example/custom_attribute.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/custom_attribute_link.rst` & `ftrack-python-api-2.5.0/doc/example/custom_attribute_link.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/encode_media.rst` & `ftrack-python-api-2.5.0/doc/example/encode_media.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/entity_links.rst` & `ftrack-python-api-2.5.0/doc/example/entity_links.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/index.rst` & `ftrack-python-api-2.5.0/doc/example/index.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/job.rst` & `ftrack-python-api-2.5.0/doc/example/job.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/link_attribute.rst` & `ftrack-python-api-2.5.0/doc/example/link_attribute.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/list.rst` & `ftrack-python-api-2.5.0/doc/example/list.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/manage_custom_attribute_configuration.rst` & `ftrack-python-api-2.5.0/doc/example/manage_custom_attribute_configuration.rst`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
         session.create('CustomAttributeConfiguration', {
             'entity_type': 'task',
             'object_type_id': object_type['id'],
             'type': custom_attribute_type,
             'label': 'Foo',
             'key': 'foo',
             'default': 'bar',
+            'config': json.dumps({'markdown': False})
         })
         session.commit()
 
     Can be associated with a `project_id`.
 
 :show:
     Represents Projects custom attribute configurations.
@@ -262,38 +263,39 @@
     asset_version, list, user, group, asset and component.
 
 :object_type_id_to:
     When setting entity_type_to to "task" object_type_id_to must also be specified.
 
 Below is an example of how to create a custom attribute link between a
 TypedContext object such as Shot and AssetVersion::
-
+    security_role = session.query('SecurityRole').first()
+    task_object_id = session.query('ObjectType where name is "task"').one()['id']
     session.create('CustomAttributeLinkConfiguration', {
         'entity_type': 'task',
         'object_type_id': task_object_id,
         'entity_type_to': 'asset_version',
         'label': 'Delivered version',
         'key': 'delivered_version',
         'config': '{}',
         'one_to_one': True,
         'write_security_roles': [security_role],
         'read_security_roles': [security_role]
     })
 
 An other example creating a custom attribute link between a Sequence
 and a Shot specifying object_type for both sides.::
-
+    security_role = session.query('SecurityRole').first()
     shot_object_id = session.query('ObjectType where name is "shot"').one()['id']
     sequence_object_id = session.query('ObjectType where name is "sequence"').one()['id']
 
     session.create('CustomAttributeLinkConfiguration', {
         'entity_type': 'task',
         'object_type_id': sequence_object,
         'entity_type_to': 'task',
-        'object_type_id_to': shot_object_id
+        'object_type_id_to': shot_object_id,
         'label': 'Master shot',
         'key': 'master_shot',
         'config': '{}',
         'one_to_one': True,
         'write_security_roles': [security_role],
         'read_security_roles': [security_role]
     })
```

### Comparing `ftrack-python-api-2.4.2/doc/example/metadata.rst` & `ftrack-python-api-2.5.0/doc/example/metadata.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/note.rst` & `ftrack-python-api-2.5.0/doc/example/note.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/project.rst` & `ftrack-python-api-2.5.0/doc/example/project.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/publishing.rst` & `ftrack-python-api-2.5.0/doc/example/publishing.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/review_session.rst` & `ftrack-python-api-2.5.0/doc/example/review_session.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/scope.rst` & `ftrack-python-api-2.5.0/doc/example/scope.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/security_roles.rst` & `ftrack-python-api-2.5.0/doc/example/security_roles.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/sync_ldap_users.rst` & `ftrack-python-api-2.5.0/doc/example/sync_ldap_users.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/task_template.rst` & `ftrack-python-api-2.5.0/doc/example/task_template.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/thumbnail.rst` & `ftrack-python-api-2.5.0/doc/example/thumbnail.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/timer.rst` & `ftrack-python-api-2.5.0/doc/example/timer.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/web_review.rst` & `ftrack-python-api-2.5.0/doc/example/web_review.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/example/workflow_schema.rst` & `ftrack-python-api-2.5.0/doc/example/workflow_schema.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/glossary.rst` & `ftrack-python-api-2.5.0/doc/glossary.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/handling_events.rst` & `ftrack-python-api-2.5.0/doc/handling_events.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/image/configuring_plugins_directory.png` & `ftrack-python-api-2.5.0/doc/image/configuring_plugins_directory.png`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/index.rst` & `ftrack-python-api-2.5.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/installing.rst` & `ftrack-python-api-2.5.0/doc/installing.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/introduction.rst` & `ftrack-python-api-2.5.0/doc/introduction.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/locations/configuring.rst` & `ftrack-python-api-2.5.0/doc/locations/configuring.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/locations/overview.rst` & `ftrack-python-api-2.5.0/doc/locations/overview.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/locations/tutorial.rst` & `ftrack-python-api-2.5.0/doc/locations/tutorial.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/querying.rst` & `ftrack-python-api-2.5.0/doc/querying.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/release/index.rst` & `ftrack-python-api-2.5.0/doc/release/index.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/release/migrating_from_old_api.rst` & `ftrack-python-api-2.5.0/doc/release/migrating_from_old_api.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/release/migration.rst` & `ftrack-python-api-2.5.0/doc/release/migration.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/release/release_notes.rst` & `ftrack-python-api-2.5.0/doc/release/release_notes.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/resource/example_plugin.py` & `ftrack-python-api-2.5.0/doc/resource/example_plugin.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/resource/example_plugin_using_session.py` & `ftrack-python-api-2.5.0/doc/resource/example_plugin_using_session.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/security_and_authentication.rst` & `ftrack-python-api-2.5.0/doc/security_and_authentication.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/tutorial.rst` & `ftrack-python-api-2.5.0/doc/tutorial.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/understanding_sessions.rst` & `ftrack-python-api-2.5.0/doc/understanding_sessions.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/doc/working_with_entities.rst` & `ftrack-python-api-2.5.0/doc/working_with_entities.rst`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/resource/plugin/configure_locations.py` & `ftrack-python-api-2.5.0/resource/plugin/configure_locations.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/resource/plugin/construct_entity_type.py` & `ftrack-python-api-2.5.0/resource/plugin/construct_entity_type.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/setup.py` & `ftrack-python-api-2.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/__init__.py` & `ftrack-python-api-2.5.0/source/ftrack_api/__init__.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/_centralized_storage_scenario.py` & `ftrack-python-api-2.5.0/source/ftrack_api/_centralized_storage_scenario.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/_python_ntpath.py` & `ftrack-python-api-2.5.0/source/ftrack_api/_python_ntpath.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/_weakref.py` & `ftrack-python-api-2.5.0/source/ftrack_api/_weakref.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/accessor/base.py` & `ftrack-python-api-2.5.0/source/ftrack_api/accessor/base.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/accessor/disk.py` & `ftrack-python-api-2.5.0/source/ftrack_api/accessor/disk.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/accessor/server.py` & `ftrack-python-api-2.5.0/source/ftrack_api/accessor/server.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/attribute.py` & `ftrack-python-api-2.5.0/source/ftrack_api/attribute.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/cache.py` & `ftrack-python-api-2.5.0/source/ftrack_api/cache.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/collection.py` & `ftrack-python-api-2.5.0/source/ftrack_api/collection.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/data.py` & `ftrack-python-api-2.5.0/source/ftrack_api/data.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/entity/asset_version.py` & `ftrack-python-api-2.5.0/source/ftrack_api/entity/asset_version.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/entity/base.py` & `ftrack-python-api-2.5.0/source/ftrack_api/entity/base.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/entity/component.py` & `ftrack-python-api-2.5.0/source/ftrack_api/entity/component.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/entity/factory.py` & `ftrack-python-api-2.5.0/source/ftrack_api/entity/factory.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/entity/job.py` & `ftrack-python-api-2.5.0/source/ftrack_api/entity/job.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/entity/location.py` & `ftrack-python-api-2.5.0/source/ftrack_api/entity/location.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/entity/note.py` & `ftrack-python-api-2.5.0/source/ftrack_api/entity/note.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/entity/project_schema.py` & `ftrack-python-api-2.5.0/source/ftrack_api/entity/project_schema.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/entity/user.py` & `ftrack-python-api-2.5.0/source/ftrack_api/entity/user.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/event/base.py` & `ftrack-python-api-2.5.0/source/ftrack_api/event/base.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/event/expression.py` & `ftrack-python-api-2.5.0/source/ftrack_api/event/expression.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/event/hub.py` & `ftrack-python-api-2.5.0/source/ftrack_api/event/hub.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/event/subscriber.py` & `ftrack-python-api-2.5.0/source/ftrack_api/event/subscriber.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/event/subscription.py` & `ftrack-python-api-2.5.0/source/ftrack_api/event/subscription.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/exception.py` & `ftrack-python-api-2.5.0/source/ftrack_api/exception.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/formatter.py` & `ftrack-python-api-2.5.0/source/ftrack_api/formatter.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/inspection.py` & `ftrack-python-api-2.5.0/source/ftrack_api/inspection.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/logging.py` & `ftrack-python-api-2.5.0/source/ftrack_api/logging.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/operation.py` & `ftrack-python-api-2.5.0/source/ftrack_api/operation.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/plugin.py` & `ftrack-python-api-2.5.0/source/ftrack_api/plugin.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/query.py` & `ftrack-python-api-2.5.0/source/ftrack_api/query.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/resource_identifier_transformer/base.py` & `ftrack-python-api-2.5.0/source/ftrack_api/resource_identifier_transformer/base.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/session.py` & `ftrack-python-api-2.5.0/source/ftrack_api/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1688,46 +1688,55 @@
             'content-type': 'application/json',
             'accept': 'application/json'
         }
         data = self.encode(data, entity_attribute_strategy='modified_only')
 
         self.logger.debug(L('Calling server {0} with {1!r}', url, data))
 
-        response = self._request.post(
-            url,
-            headers=headers,
-            data=data,
-            timeout=self.request_timeout,
-        )
+        try:
+            response = self._request.post(
+                url,
+                headers=headers,
+                data=data,
+                timeout=self.request_timeout,
+            )
+            response.raise_for_status()
 
-        self.logger.debug(L('Call took: {0}', response.elapsed.total_seconds()))
+        except requests.exceptions.HTTPError:
+            error_message = (
+                'Server reported error: {0}'
+                .format(response.text)
+            )
+            self._raise_server_error(error_message)
 
+        self.logger.debug(L('Call took: {0}', response.elapsed.total_seconds()))
         self.logger.debug(L('Response: {0!r}', response.text))
-        try:
-            result = self.decode(response.text)
 
+        try:        
+            result = self.decode(response.text)
         except Exception:
             error_message = (
                 'Server reported error in unexpected format. Raw error was: {0}'
                 .format(response.text)
             )
-            self.logger.exception(error_message)
-            raise ftrack_api.exception.ServerError(error_message)
+            self._raise_server_error(error_message)
 
         else:
             if 'exception' in result:
                 # Handle exceptions.
                 error_message = 'Server reported error: {0}({1})'.format(
                     result['exception'], result['content']
                 )
-                self.logger.exception(error_message)
-                raise ftrack_api.exception.ServerError(error_message)
-
+                self._raise_server_error(error_message)
         return result
 
+    def _raise_server_error(self, error_message):
+        self.logger.exception(error_message)
+        raise ftrack_api.exception.ServerError(error_message)
+
     def encode(self, data, entity_attribute_strategy='set_only'):
         '''Return *data* encoded as JSON formatted string.
 
         *entity_attribute_strategy* specifies how entity attributes should be
         handled. The following strategies are available:
 
         * *all* - Encode all attributes, loading any that are currently NOT_SET.
```

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/structure/base.py` & `ftrack-python-api-2.5.0/source/ftrack_api/structure/base.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/structure/id.py` & `ftrack-python-api-2.5.0/source/ftrack_api/structure/id.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/structure/origin.py` & `ftrack-python-api-2.5.0/source/ftrack_api/structure/origin.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/structure/standard.py` & `ftrack-python-api-2.5.0/source/ftrack_api/structure/standard.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_api/symbol.py` & `ftrack-python-api-2.5.0/source/ftrack_api/symbol.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/source/ftrack_python_api.egg-info/PKG-INFO` & `ftrack-python-api-2.5.0/source/ftrack_python_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftrack-python-api
-Version: 2.4.2
+Version: 2.5.0
 Summary: Python API for ftrack.
 Home-page: https://github.com/ftrackhq/ftrack-python
 Author: ftrack
 Author-email: support@ftrack.com
 License: Apache License (2.0)
 Project-URL: Documentation, http://ftrack-python-api.rtd.ftrack.com/en/Unknown version/
 Project-URL: Source Code, https://github.com/ftrackhq/ftrack-python/src/Unknown version
```

### Comparing `ftrack-python-api-2.4.2/source/ftrack_python_api.egg-info/SOURCES.txt` & `ftrack-python-api-2.5.0/source/ftrack_python_api.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 MANIFEST.in
 README.rst
 pytest.ini
 readthedocs.yaml
 setup.cfg
 setup.py
 .github/workflows/cicd.yml
+.github/workflows/pr.yml
 doc/caching.rst
 doc/conf.py
 doc/docutils.conf
 doc/environment_variables.rst
 doc/event_list.rst
 doc/glossary.rst
 doc/handling_events.rst
```

### Comparing `ftrack-python-api-2.4.2/test/fixture/media/colour_wheel.mov` & `ftrack-python-api-2.5.0/test/fixture/media/colour_wheel.mov`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/fixture/media/image.png` & `ftrack-python-api-2.5.0/test/fixture/media/image.png`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/fixture/plugin/configure_locations.py` & `ftrack-python-api-2.5.0/test/fixture/plugin/configure_locations.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/fixture/plugin/construct_entity_type.py` & `ftrack-python-api-2.5.0/test/fixture/plugin/construct_entity_type.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/fixture/plugin/count_session_event.py` & `ftrack-python-api-2.5.0/test/fixture/plugin/count_session_event.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/fixture/plugin/get_file_type.py` & `ftrack-python-api-2.5.0/test/fixture/plugin/get_file_type.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/accessor/test_disk.py` & `ftrack-python-api-2.5.0/test/unit/accessor/test_disk.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/accessor/test_server.py` & `ftrack-python-api-2.5.0/test/unit/accessor/test_server.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/conftest.py` & `ftrack-python-api-2.5.0/test/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/entity/test_asset_version.py` & `ftrack-python-api-2.5.0/test/unit/entity/test_asset_version.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/entity/test_component.py` & `ftrack-python-api-2.5.0/test/unit/entity/test_component.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/entity/test_factory.py` & `ftrack-python-api-2.5.0/test/unit/entity/test_factory.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/entity/test_job.py` & `ftrack-python-api-2.5.0/test/unit/entity/test_job.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/entity/test_location.py` & `ftrack-python-api-2.5.0/test/unit/entity/test_location.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/entity/test_metadata.py` & `ftrack-python-api-2.5.0/test/unit/entity/test_metadata.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/entity/test_note.py` & `ftrack-python-api-2.5.0/test/unit/entity/test_note.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/entity/test_project_schema.py` & `ftrack-python-api-2.5.0/test/unit/entity/test_project_schema.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/entity/test_scopes.py` & `ftrack-python-api-2.5.0/test/unit/entity/test_scopes.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/entity/test_user.py` & `ftrack-python-api-2.5.0/test/unit/entity/test_user.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/event/event_hub_server_heartbeat.py` & `ftrack-python-api-2.5.0/test/unit/event/event_hub_server_heartbeat.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/event/test_base.py` & `ftrack-python-api-2.5.0/test/unit/event/test_base.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/event/test_expression.py` & `ftrack-python-api-2.5.0/test/unit/event/test_expression.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/event/test_hub.py` & `ftrack-python-api-2.5.0/test/unit/event/test_hub.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/event/test_subscriber.py` & `ftrack-python-api-2.5.0/test/unit/event/test_subscriber.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/event/test_subscription.py` & `ftrack-python-api-2.5.0/test/unit/event/test_subscription.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/resource_identifier_transformer/test_base.py` & `ftrack-python-api-2.5.0/test/unit/resource_identifier_transformer/test_base.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/structure/test_base.py` & `ftrack-python-api-2.5.0/test/unit/structure/test_base.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/structure/test_entity_id.py` & `ftrack-python-api-2.5.0/test/unit/structure/test_entity_id.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/structure/test_get_file_from_string_event.py` & `ftrack-python-api-2.5.0/test/unit/structure/test_get_file_from_string_event.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/structure/test_id.py` & `ftrack-python-api-2.5.0/test/unit/structure/test_id.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/structure/test_origin.py` & `ftrack-python-api-2.5.0/test/unit/structure/test_origin.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/structure/test_standard.py` & `ftrack-python-api-2.5.0/test/unit/structure/test_standard.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/test_attribute.py` & `ftrack-python-api-2.5.0/test/unit/test_attribute.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/test_cache.py` & `ftrack-python-api-2.5.0/test/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/test_collection.py` & `ftrack-python-api-2.5.0/test/unit/test_collection.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/test_custom_attribute.py` & `ftrack-python-api-2.5.0/test/unit/test_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/test_data.py` & `ftrack-python-api-2.5.0/test/unit/test_data.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/test_formatter.py` & `ftrack-python-api-2.5.0/test/unit/test_formatter.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/test_inspection.py` & `ftrack-python-api-2.5.0/test/unit/test_inspection.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/test_operation.py` & `ftrack-python-api-2.5.0/test/unit/test_operation.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/test_package.py` & `ftrack-python-api-2.5.0/test/unit/test_package.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/test_plugin.py` & `ftrack-python-api-2.5.0/test/unit/test_plugin.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/test_query.py` & `ftrack-python-api-2.5.0/test/unit/test_query.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/test_session.py` & `ftrack-python-api-2.5.0/test/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `ftrack-python-api-2.4.2/test/unit/test_timer.py` & `ftrack-python-api-2.5.0/test/unit/test_timer.py`

 * *Files identical despite different names*

