# Comparing `tmp/tutor-15.3.5.tar.gz` & `tmp/tutor-15.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-15.3.5.tar", last modified: Fri Apr 28 07:16:55 2023, max compression
+gzip compressed data, was "dist/tutor-15.3.6.tar", last modified: Mon May 22 16:59:42 2023, max compression
```

## Comparing `tutor-15.3.5.tar` & `tutor-15.3.6.tar`

### file list

```diff
@@ -1,149 +1,159 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/
--rw-r--r--   0 ci        (1000) ci        (1000)      121 2023-04-28 07:15:59.000000 tutor-15.3.5/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     6664 2023-04-28 07:16:55.000000 tutor-15.3.5/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     4745 2023-04-28 07:15:59.000000 tutor-15.3.5/README.rst
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/requirements/
--rw-r--r--   0 ci        (1000) ci        (1000)       98 2023-04-28 07:15:59.000000 tutor-15.3.5/requirements/base.in
--rw-r--r--   0 ci        (1000) ci        (1000)      341 2023-04-28 07:15:59.000000 tutor-15.3.5/requirements/plugins.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-04-28 07:16:55.000000 tutor-15.3.5/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     2505 2023-04-28 07:15:59.000000 tutor-15.3.5/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/
--rw-r--r--   0 ci        (1000) ci        (1000)     1159 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1843 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/bindmounts.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/commands/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/commands/__init__.py
--rwxr-xr-x   0 ci        (1000) ci        (1000)     4349 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/commands/cli.py
--rw-r--r--   0 ci        (1000) ci        (1000)    17488 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/commands/compose.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5647 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/commands/config.py
--rw-r--r--   0 ci        (1000) ci        (1000)      794 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/commands/context.py
--rw-r--r--   0 ci        (1000) ci        (1000)     4880 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/commands/dev.py
--rw-r--r--   0 ci        (1000) ci        (1000)     6304 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/commands/images.py
--rw-r--r--   0 ci        (1000) ci        (1000)    11445 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/commands/jobs.py
--rw-r--r--   0 ci        (1000) ci        (1000)    20161 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/commands/k8s.py
--rw-r--r--   0 ci        (1000) ci        (1000)     7466 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/commands/local.py
--rw-r--r--   0 ci        (1000) ci        (1000)    13436 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/commands/plugins.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/commands/upgrade/
--rw-r--r--   0 ci        (1000) ci        (1000)      146 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/commands/upgrade/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1826 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/commands/upgrade/common.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5853 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/commands/upgrade/k8s.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5574 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/commands/upgrade/local.py
--rw-r--r--   0 ci        (1000) ci        (1000)     9685 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/core/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/core/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/core/hooks/
--rw-r--r--   0 ci        (1000) ci        (1000)      451 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/core/hooks/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     8085 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/core/hooks/actions.py
--rw-r--r--   0 ci        (1000) ci        (1000)     3376 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/core/hooks/contexts.py
--rw-r--r--   0 ci        (1000) ci        (1000)    12849 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/core/hooks/filters.py
--rw-r--r--   0 ci        (1000) ci        (1000)      638 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/core/hooks/priorities.py
--rw-r--r--   0 ci        (1000) ci        (1000)    17511 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/env.py
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/exceptions.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1213 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/fmt.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/hooks/
--rw-r--r--   0 ci        (1000) ci        (1000)      273 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/hooks/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)    25047 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/hooks/catalog.py
--rw-r--r--   0 ci        (1000) ci        (1000)      657 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/images.py
--rw-r--r--   0 ci        (1000) ci        (1000)     5076 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/interactive.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/plugins/
--rw-r--r--   0 ci        (1000) ci        (1000)     3653 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/plugins/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      548 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/plugins/base.py
--rw-r--r--   0 ci        (1000) ci        (1000)     6989 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/plugins/indexes.py
--rw-r--r--   0 ci        (1000) ci        (1000)    15132 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/plugins/v0.py
--rw-r--r--   0 ci        (1000) ci        (1000)     2324 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/plugins/v1.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/py.typed
--rw-r--r--   0 ci        (1000) ci        (1000)     1536 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/serialize.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1385 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/tasks.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/apps/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/apps/caddy/
--rw-r--r--   0 ci        (1000) ci        (1000)     1989 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/caddy/Caddyfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/apps/openedx/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/apps/openedx/config/
--rw-r--r--   0 ci        (1000) ci        (1000)     1542 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/config/cms.env.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1787 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/config/lms.env.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/apps/openedx/config/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)      673 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/config/partials/auth.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/cms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/cms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      591 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/cms/development.py
--rw-r--r--   0 ci        (1000) ci        (1000)      529 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/cms/production.py
--rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/cms/test.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/lms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1132 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/lms/development.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1039 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/lms/production.py
--rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/lms/test.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)     9859 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/partials/common_all.py
--rw-r--r--   0 ci        (1000) ci        (1000)      924 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/partials/common_cms.py
--rw-r--r--   0 ci        (1000) ci        (1000)     1748 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/partials/common_lms.py
--rw-r--r--   0 ci        (1000) ci        (1000)      105 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/settings/partials/common_test.py
--rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/openedx/uwsgi.ini
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/apps/redis/
--rw-r--r--   0 ci        (1000) ci        (1000)      854 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/apps/redis/redis.conf
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/build/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/build/openedx/
--rw-r--r--   0 ci        (1000) ci        (1000)    10443 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/build/openedx/bin/
--rwxr-xr-x   0 ci        (1000) ci        (1000)     7042 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/bin/openedx-assets
--rwxr-xr-x   0 ci        (1000) ci        (1000)      116 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/bin/reload-uwsgi
--rw-r--r--   0 ci        (1000) ci        (1000)     2329 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/bin/site-configuration
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/build/openedx/locale/
--rw-r--r--   0 ci        (1000) ci        (1000)      438 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/locale/customlocales.md
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/build/openedx/requirements/
--rw-r--r--   0 ci        (1000) ci        (1000)      305 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/requirements/private-sample.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       29 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/revisions.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/build/openedx/settings/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/build/openedx/settings/cms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/settings/cms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      317 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/settings/cms/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/settings/cms/i18n.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/build/openedx/settings/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/settings/lms/__init__.py
--rw-r--r--   0 ci        (1000) ci        (1000)      306 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/settings/lms/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/settings/lms/i18n.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/build/openedx/settings/partials/
--rw-r--r--   0 ci        (1000) ci        (1000)      441 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/settings/partials/assets.py
--rw-r--r--   0 ci        (1000) ci        (1000)      420 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/settings/partials/i18n.py
--rw-r--r--   0 ci        (1000) ci        (1000)      262 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/settings/uwsgi.ini
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/build/openedx/themes/
--rw-r--r--   0 ci        (1000) ci        (1000)       75 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/openedx/themes/README
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/build/permissions/
--rw-r--r--   0 ci        (1000) ci        (1000)      189 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/permissions/Dockerfile
--rw-r--r--   0 ci        (1000) ci        (1000)      302 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/build/permissions/setowner.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/config/
--rw-r--r--   0 ci        (1000) ci        (1000)      515 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/config/base.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2627 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/config/defaults.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/dev/
--rw-r--r--   0 ci        (1000) ci        (1000)      885 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/dev/docker-compose.jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1721 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/dev/docker-compose.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/jobs/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/jobs/init/
--rw-r--r--   0 ci        (1000) ci        (1000)      418 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/jobs/init/cms.sh
--rw-r--r--   0 ci        (1000) ci        (1000)     1807 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/jobs/init/lms.sh
--rw-r--r--   0 ci        (1000) ci        (1000)      756 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/jobs/init/mounted-edx-platform.sh
--rw-r--r--   0 ci        (1000) ci        (1000)     1455 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/jobs/init/mysql.sh
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/k8s/
--rw-r--r--   0 ci        (1000) ci        (1000)    13208 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/k8s/deployments.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2090 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/k8s/jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)      125 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/k8s/namespace.yml
--rw-r--r--   0 ci        (1000) ci        (1000)       28 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/k8s/override.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2416 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/k8s/services.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     1428 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/k8s/volumes.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     2142 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/kustomization.yml
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor/templates/local/
--rw-r--r--   0 ci        (1000) ci        (1000)     1216 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/local/docker-compose.jobs.yml
--rw-r--r--   0 ci        (1000) ci        (1000)      950 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/local/docker-compose.prod.yml
--rw-r--r--   0 ci        (1000) ci        (1000)     6701 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/local/docker-compose.yml
--rw-r--r--   0 ci        (1000) ci        (1000)       19 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/templates/version
--rw-r--r--   0 ci        (1000) ci        (1000)     1327 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/types.py
--rw-r--r--   0 ci        (1000) ci        (1000)    11298 2023-04-28 07:15:59.000000 tutor-15.3.5/tutor/utils.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-04-28 07:16:55.000000 tutor-15.3.5/tutor.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     6664 2023-04-28 07:16:54.000000 tutor-15.3.5/tutor.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     3813 2023-04-28 07:16:54.000000 tutor-15.3.5/tutor.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-04-28 07:16:54.000000 tutor-15.3.5/tutor.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       51 2023-04-28 07:16:54.000000 tutor-15.3.5/tutor.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)      397 2023-04-28 07:16:54.000000 tutor-15.3.5/tutor.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        6 2023-04-28 07:16:54.000000 tutor-15.3.5/tutor.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-05-22 16:58:51.000000 tutor-15.3.6/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)      121 2023-05-22 16:58:51.000000 tutor-15.3.6/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     6664 2023-05-22 16:59:42.000000 tutor-15.3.6/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     4745 2023-05-22 16:58:51.000000 tutor-15.3.6/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-05-22 16:58:51.000000 tutor-15.3.6/pyproject.toml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/requirements/
+-rw-r--r--   0 ci        (1000) ci        (1000)       98 2023-05-22 16:58:51.000000 tutor-15.3.6/requirements/base.in
+-rw-r--r--   0 ci        (1000) ci        (1000)      341 2023-05-22 16:58:51.000000 tutor-15.3.6/requirements/plugins.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-05-22 16:59:42.000000 tutor-15.3.6/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     2505 2023-05-22 16:58:51.000000 tutor-15.3.6/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tests/
+-rw-r--r--   0 ci        (1000) ci        (1000)     4172 2023-05-22 16:58:51.000000 tutor-15.3.6/tests/test_config.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    15899 2023-05-22 16:58:51.000000 tutor-15.3.6/tests/test_env.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      472 2023-05-22 16:58:51.000000 tutor-15.3.6/tests/test_images.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     3063 2023-05-22 16:58:51.000000 tutor-15.3.6/tests/test_plugin_indexes.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     8273 2023-05-22 16:58:51.000000 tutor-15.3.6/tests/test_plugins_v0.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1617 2023-05-22 16:58:51.000000 tutor-15.3.6/tests/test_serialize.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    10669 2023-05-22 16:58:51.000000 tutor-15.3.6/tests/test_utils.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1159 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1843 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/bindmounts.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/commands/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/commands/__init__.py
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     4349 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/commands/cli.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    17488 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/commands/compose.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5647 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/commands/config.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      794 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/commands/context.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     4880 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/commands/dev.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     6304 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/commands/images.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    11445 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/commands/jobs.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    20161 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/commands/k8s.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     7466 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/commands/local.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    13436 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/commands/plugins.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/commands/upgrade/
+-rw-r--r--   0 ci        (1000) ci        (1000)      146 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/commands/upgrade/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1826 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/commands/upgrade/common.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5853 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/commands/upgrade/k8s.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5574 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/commands/upgrade/local.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     9685 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/core/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/core/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/core/hooks/
+-rw-r--r--   0 ci        (1000) ci        (1000)      451 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/core/hooks/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     8085 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/core/hooks/actions.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     3376 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/core/hooks/contexts.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    12849 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/core/hooks/filters.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      638 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/core/hooks/priorities.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    17511 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/env.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/exceptions.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1213 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/fmt.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/hooks/
+-rw-r--r--   0 ci        (1000) ci        (1000)      273 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/hooks/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    25047 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/hooks/catalog.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      657 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/images.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     5076 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/interactive.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/plugins/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3653 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/plugins/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      548 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/plugins/base.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     6989 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/plugins/indexes.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    15132 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/plugins/v0.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     2324 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/plugins/v1.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/py.typed
+-rw-r--r--   0 ci        (1000) ci        (1000)     1536 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/serialize.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1385 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/tasks.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/apps/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/apps/caddy/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1989 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/caddy/Caddyfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/apps/openedx/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/apps/openedx/config/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1542 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/config/cms.env.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1787 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/config/lms.env.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/apps/openedx/config/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)      673 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/config/partials/auth.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/cms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/cms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      591 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/cms/development.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      529 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/cms/production.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/cms/test.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/lms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1132 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/lms/development.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1039 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/lms/production.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       91 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/lms/test.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)     9859 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/partials/common_all.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      924 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/partials/common_cms.py
+-rw-r--r--   0 ci        (1000) ci        (1000)     1748 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/partials/common_lms.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      105 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/settings/partials/common_test.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/openedx/uwsgi.ini
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/apps/redis/
+-rw-r--r--   0 ci        (1000) ci        (1000)      854 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/apps/redis/redis.conf
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/build/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/build/openedx/
+-rw-r--r--   0 ci        (1000) ci        (1000)    10443 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/build/openedx/bin/
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     7042 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/bin/openedx-assets
+-rwxr-xr-x   0 ci        (1000) ci        (1000)      116 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/bin/reload-uwsgi
+-rw-r--r--   0 ci        (1000) ci        (1000)     2329 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/bin/site-configuration
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/build/openedx/locale/
+-rw-r--r--   0 ci        (1000) ci        (1000)      438 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/locale/customlocales.md
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/build/openedx/requirements/
+-rw-r--r--   0 ci        (1000) ci        (1000)      305 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/requirements/private-sample.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       29 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/revisions.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/build/openedx/settings/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/build/openedx/settings/cms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/settings/cms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      317 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/settings/cms/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/settings/cms/i18n.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/build/openedx/settings/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/settings/lms/__init__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      306 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/settings/lms/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)       56 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/settings/lms/i18n.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/build/openedx/settings/partials/
+-rw-r--r--   0 ci        (1000) ci        (1000)      441 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/settings/partials/assets.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      420 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/settings/partials/i18n.py
+-rw-r--r--   0 ci        (1000) ci        (1000)      262 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/settings/uwsgi.ini
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/build/openedx/themes/
+-rw-r--r--   0 ci        (1000) ci        (1000)       75 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/openedx/themes/README
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/build/permissions/
+-rw-r--r--   0 ci        (1000) ci        (1000)      189 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/permissions/Dockerfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      302 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/build/permissions/setowner.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/config/
+-rw-r--r--   0 ci        (1000) ci        (1000)      515 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/config/base.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2627 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/config/defaults.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/dev/
+-rw-r--r--   0 ci        (1000) ci        (1000)      885 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/dev/docker-compose.jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1721 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/dev/docker-compose.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/jobs/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/jobs/init/
+-rw-r--r--   0 ci        (1000) ci        (1000)      418 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/jobs/init/cms.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)     1807 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/jobs/init/lms.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)      756 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/jobs/init/mounted-edx-platform.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)     1455 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/jobs/init/mysql.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/k8s/
+-rw-r--r--   0 ci        (1000) ci        (1000)    13208 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/k8s/deployments.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2090 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/k8s/jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)      125 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/k8s/namespace.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)       28 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/k8s/override.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2416 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/k8s/services.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     1428 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/k8s/volumes.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     2142 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/kustomization.yml
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor/templates/local/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1979 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/local/docker-compose.jobs.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)      950 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/local/docker-compose.prod.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)     6701 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/local/docker-compose.yml
+-rw-r--r--   0 ci        (1000) ci        (1000)       19 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/templates/version
+-rw-r--r--   0 ci        (1000) ci        (1000)     1327 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/types.py
+-rw-r--r--   0 ci        (1000) ci        (1000)    11298 2023-05-22 16:58:51.000000 tutor-15.3.6/tutor/utils.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     6664 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     3998 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       51 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)      397 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        6 2023-05-22 16:59:42.000000 tutor-15.3.6/tutor.egg-info/top_level.txt
```

### Comparing `tutor-15.3.5/PKG-INFO` & `tutor-15.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor
-Version: 15.3.5
+Version: 15.3.6
 Summary: The Docker-based Open edX distribution designed for peace of mind
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.io
 Author-email: contact@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor
```

### Comparing `tutor-15.3.5/README.rst` & `tutor-15.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/setup.py` & `tutor-15.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/__about__.py` & `tutor-15.3.6/tutor/__about__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 # Increment this version number to trigger a new release. See
 # docs/tutor.html#versioning for information on the versioning scheme.
-__version__ = "15.3.5"
+__version__ = "15.3.6"
 
 # The version suffix will be appended to the actual version, separated by a
 # dash. Use this suffix to differentiate between the actual released version and
 # the versions from other branches. For instance: set the suffix to "nightly" in
 # the nightly branch.
 # The suffix is cleanly separated from the __version__ in this module to avoid
 # conflicts when merging branches.
```

### Comparing `tutor-15.3.5/tutor/bindmounts.py` & `tutor-15.3.6/tutor/bindmounts.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/commands/cli.py` & `tutor-15.3.6/tutor/commands/cli.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/commands/compose.py` & `tutor-15.3.6/tutor/commands/compose.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/commands/config.py` & `tutor-15.3.6/tutor/commands/config.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/commands/context.py` & `tutor-15.3.6/tutor/commands/context.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/commands/dev.py` & `tutor-15.3.6/tutor/commands/dev.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/commands/images.py` & `tutor-15.3.6/tutor/commands/images.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/commands/jobs.py` & `tutor-15.3.6/tutor/commands/jobs.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/commands/k8s.py` & `tutor-15.3.6/tutor/commands/k8s.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/commands/local.py` & `tutor-15.3.6/tutor/commands/local.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/commands/plugins.py` & `tutor-15.3.6/tutor/commands/plugins.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/commands/upgrade/common.py` & `tutor-15.3.6/tutor/commands/upgrade/common.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/commands/upgrade/k8s.py` & `tutor-15.3.6/tutor/commands/upgrade/k8s.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/commands/upgrade/local.py` & `tutor-15.3.6/tutor/commands/upgrade/local.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/config.py` & `tutor-15.3.6/tutor/config.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/core/hooks/actions.py` & `tutor-15.3.6/tutor/core/hooks/actions.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/core/hooks/contexts.py` & `tutor-15.3.6/tutor/core/hooks/contexts.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/core/hooks/filters.py` & `tutor-15.3.6/tutor/core/hooks/filters.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/core/hooks/priorities.py` & `tutor-15.3.6/tutor/core/hooks/priorities.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/env.py` & `tutor-15.3.6/tutor/env.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/fmt.py` & `tutor-15.3.6/tutor/fmt.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/hooks/catalog.py` & `tutor-15.3.6/tutor/hooks/catalog.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/images.py` & `tutor-15.3.6/tutor/images.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/interactive.py` & `tutor-15.3.6/tutor/interactive.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/plugins/__init__.py` & `tutor-15.3.6/tutor/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/plugins/base.py` & `tutor-15.3.6/tutor/plugins/base.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/plugins/indexes.py` & `tutor-15.3.6/tutor/plugins/indexes.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/plugins/v0.py` & `tutor-15.3.6/tutor/plugins/v0.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/plugins/v1.py` & `tutor-15.3.6/tutor/plugins/v1.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/serialize.py` & `tutor-15.3.6/tutor/serialize.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/tasks.py` & `tutor-15.3.6/tutor/tasks.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/apps/caddy/Caddyfile` & `tutor-15.3.6/tutor/templates/apps/caddy/Caddyfile`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/apps/openedx/config/cms.env.yml` & `tutor-15.3.6/tutor/templates/apps/openedx/config/cms.env.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/apps/openedx/config/lms.env.yml` & `tutor-15.3.6/tutor/templates/apps/openedx/config/lms.env.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/apps/openedx/config/partials/auth.yml` & `tutor-15.3.6/tutor/templates/apps/openedx/config/partials/auth.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/apps/openedx/settings/cms/development.py` & `tutor-15.3.6/tutor/templates/apps/openedx/settings/cms/development.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/apps/openedx/settings/cms/production.py` & `tutor-15.3.6/tutor/templates/apps/openedx/settings/cms/production.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/apps/openedx/settings/lms/development.py` & `tutor-15.3.6/tutor/templates/apps/openedx/settings/lms/development.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/apps/openedx/settings/lms/production.py` & `tutor-15.3.6/tutor/templates/apps/openedx/settings/lms/production.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/apps/openedx/settings/partials/common_all.py` & `tutor-15.3.6/tutor/templates/apps/openedx/settings/partials/common_all.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/apps/openedx/settings/partials/common_cms.py` & `tutor-15.3.6/tutor/templates/apps/openedx/settings/partials/common_cms.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/apps/openedx/settings/partials/common_lms.py` & `tutor-15.3.6/tutor/templates/apps/openedx/settings/partials/common_lms.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/apps/redis/redis.conf` & `tutor-15.3.6/tutor/templates/apps/redis/redis.conf`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/build/openedx/Dockerfile` & `tutor-15.3.6/tutor/templates/build/openedx/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/build/openedx/bin/openedx-assets` & `tutor-15.3.6/tutor/templates/build/openedx/bin/openedx-assets`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/build/openedx/bin/site-configuration` & `tutor-15.3.6/tutor/templates/build/openedx/bin/site-configuration`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/config/base.yml` & `tutor-15.3.6/tutor/templates/config/base.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/config/defaults.yml` & `tutor-15.3.6/tutor/templates/config/defaults.yml`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 OPENEDX_AWS_SECRET_ACCESS_KEY: ""
 OPENEDX_CACHE_REDIS_DB: 1
 OPENEDX_CELERY_REDIS_DB: 0
 OPENEDX_CMS_UWSGI_WORKERS: 2
 OPENEDX_LMS_UWSGI_WORKERS: 2
 OPENEDX_MYSQL_DATABASE: "openedx"
 OPENEDX_MYSQL_USERNAME: "openedx"
-OPENEDX_COMMON_VERSION: "open-release/olive.3"
+OPENEDX_COMMON_VERSION: "open-release/olive.4"
 OPENEDX_EXTRA_PIP_REQUIREMENTS:
   - "openedx-scorm-xblock>=15.0.0,<16.0.0"
 MYSQL_HOST: "mysql"
 MYSQL_PORT: 3306
 MYSQL_ROOT_USERNAME: "root"
 NPM_REGISTRY: "https://registry.npmjs.org/"
 PLATFORM_NAME: "My Open edX"
```

### Comparing `tutor-15.3.5/tutor/templates/dev/docker-compose.jobs.yml` & `tutor-15.3.6/tutor/templates/dev/docker-compose.jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/dev/docker-compose.yml` & `tutor-15.3.6/tutor/templates/dev/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/jobs/init/lms.sh` & `tutor-15.3.6/tutor/templates/jobs/init/lms.sh`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/jobs/init/mounted-edx-platform.sh` & `tutor-15.3.6/tutor/templates/jobs/init/mounted-edx-platform.sh`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/jobs/init/mysql.sh` & `tutor-15.3.6/tutor/templates/jobs/init/mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/k8s/deployments.yml` & `tutor-15.3.6/tutor/templates/k8s/deployments.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/k8s/jobs.yml` & `tutor-15.3.6/tutor/templates/k8s/jobs.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/k8s/services.yml` & `tutor-15.3.6/tutor/templates/k8s/services.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/k8s/volumes.yml` & `tutor-15.3.6/tutor/templates/k8s/volumes.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/kustomization.yml` & `tutor-15.3.6/tutor/templates/kustomization.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/local/docker-compose.prod.yml` & `tutor-15.3.6/tutor/templates/local/docker-compose.prod.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/templates/local/docker-compose.yml` & `tutor-15.3.6/tutor/templates/local/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/types.py` & `tutor-15.3.6/tutor/types.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor/utils.py` & `tutor-15.3.6/tutor/utils.py`

 * *Files identical despite different names*

### Comparing `tutor-15.3.5/tutor.egg-info/PKG-INFO` & `tutor-15.3.6/tutor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor
-Version: 15.3.5
+Version: 15.3.6
 Summary: The Docker-based Open edX distribution designed for peace of mind
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.io
 Author-email: contact@overhang.io
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor
```

### Comparing `tutor-15.3.5/tutor.egg-info/SOURCES.txt` & `tutor-15.3.6/tutor.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,21 @@
+LICENSE.txt
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 requirements/base.in
 requirements/plugins.txt
+tests/test_config.py
+tests/test_env.py
+tests/test_images.py
+tests/test_plugin_indexes.py
+tests/test_plugins_v0.py
+tests/test_serialize.py
+tests/test_utils.py
 tutor/__about__.py
 tutor/__init__.py
 tutor/bindmounts.py
 tutor/config.py
 tutor/env.py
 tutor/exceptions.py
 tutor/fmt.py
```

