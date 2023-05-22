# Comparing `tmp/Flask-AppBuilder-4.3.2rc1.tar.gz` & `tmp/Flask-AppBuilder-4.3.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-AppBuilder-4.3.2rc1.tar", last modified: Fri May 12 13:48:07 2023, max compression
+gzip compressed data, was "Flask-AppBuilder-4.3.2rc2.tar", last modified: Mon May 22 10:31:57 2023, max compression
```

## Comparing `Flask-AppBuilder-4.3.2rc1.tar` & `Flask-AppBuilder-4.3.2rc2.tar`

### file list

```diff
@@ -1,1208 +1,1208 @@
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.154280 Flask-AppBuilder-4.3.2rc1/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       97 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/.coveragerc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      113 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/.env
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.099463 Flask-AppBuilder-4.3.2rc1/.github/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      642 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 dpgaspar   (501) staff       (20)      681 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 dpgaspar   (501) staff       (20)      202 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/.github/prlint.json
--rw-r--r--   0 dpgaspar   (501) staff       (20)      709 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/.github/stale.yml
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.101435 Flask-AppBuilder-4.3.2rc1/.github/workflows/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8087 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.2rc1/.github/workflows/ci.yml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      137 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/.github/workflows/odbcinst.ini
--rw-r--r--   0 dpgaspar   (501) staff       (20)      951 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/.github/workflows/ptlint.yml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      147 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/.gitignore
--rw-r--r--   0 dpgaspar   (501) staff       (20)    63188 2023-05-12 13:46:46.000000 Flask-AppBuilder-4.3.2rc1/CHANGELOG.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/CONTRIBUTING.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.105784 Flask-AppBuilder-4.3.2rc1/Flask_AppBuilder.egg-info/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9290 2023-05-12 13:48:05.000000 Flask-AppBuilder-4.3.2rc1/Flask_AppBuilder.egg-info/PKG-INFO
--rw-r--r--   0 dpgaspar   (501) staff       (20)    38050 2023-05-12 13:48:06.000000 Flask-AppBuilder-4.3.2rc1/Flask_AppBuilder.egg-info/SOURCES.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2023-05-12 13:48:05.000000 Flask-AppBuilder-4.3.2rc1/Flask_AppBuilder.egg-info/dependency_links.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)      110 2023-05-12 13:48:05.000000 Flask-AppBuilder-4.3.2rc1/Flask_AppBuilder.egg-info/entry_points.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-12 08:40:39.000000 Flask-AppBuilder-4.3.2rc1/Flask_AppBuilder.egg-info/not-zip-safe
--rw-r--r--   0 dpgaspar   (501) staff       (20)      540 2023-05-12 13:48:05.000000 Flask-AppBuilder-4.3.2rc1/Flask_AppBuilder.egg-info/requires.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)       17 2023-05-12 13:48:05.000000 Flask-AppBuilder-4.3.2rc1/Flask_AppBuilder.egg-info/top_level.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1493 2023-04-05 15:10:33.000000 Flask-AppBuilder-4.3.2rc1/LICENSE
--rw-r--r--   0 dpgaspar   (501) staff       (20)      257 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/MANIFEST.in
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9290 2023-05-12 13:48:07.154466 Flask-AppBuilder-4.3.2rc1/PKG-INFO
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6684 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/README.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/RELEASE.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.107241 Flask-AppBuilder-4.3.2rc1/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)    36590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/babel/messages.pot
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.097082 Flask-AppBuilder-4.3.2rc1/bin/
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      176 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/bin/babel_extract.sh
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/bin/babel_init.sh
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      422 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/bin/bootswatch_update.sh
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1632 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/bin/config.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/bin/db_create.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      840 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/bin/db_migrate.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/bin/db_upgrade.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1419 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/bin/hash_db_password.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/bin/migrate_db_0.7.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)     4001 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/bin/migrate_db_1.3.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1917 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/bin/sqlite_upgrade_1.3.sql
--rw-r--r--   0 dpgaspar   (501) staff       (20)      999 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.2rc1/docker-compose.yml
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.127965 Flask-AppBuilder-4.3.2rc1/docs/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6802 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/Makefile
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.128554 Flask-AppBuilder-4.3.2rc1/docs/_static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/_static/Flask-AppBuilder.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.129373 Flask-AppBuilder-4.3.2rc1/docs/_templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/_templates/layout.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.131199 Flask-AppBuilder-4.3.2rc1/docs/_themes/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/_themes/LICENSE
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1093 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/_themes/README
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.133039 Flask-AppBuilder-4.3.2rc1/docs/_themes/flask/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      954 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/_themes/flask/layout.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/_themes/flask/relations.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.134328 Flask-AppBuilder-4.3.2rc1/docs/_themes/flask/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/_themes/flask/static/Flask-AppBuilder.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9062 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/_themes/flask/static/flasky.css_t
--rw-r--r--   0 dpgaspar   (501) staff       (20)      181 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/_themes/flask/theme.conf
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.135541 Flask-AppBuilder-4.3.2rc1/docs/_themes/flask_small/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      683 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/_themes/flask_small/layout.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.136136 Flask-AppBuilder-4.3.2rc1/docs/_themes/flask_small/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/_themes/flask_small/static/flasky.css_t
--rw-r--r--   0 dpgaspar   (501) staff       (20)      184 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/_themes/flask_small/theme.conf
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4875 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/_themes/flask_theme_support.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2277 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/actions.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3828 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/addons.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10881 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.2rc1/docs/advanced.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/api.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/cli.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8834 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/conf.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)    33481 2023-05-05 08:39:47.000000 Flask-AppBuilder-4.3.2rc1/docs/config.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10806 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/customizing.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4109 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/diagrams.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/generic_datasource.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3817 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/docs/i18n.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.160516 Flask-AppBuilder-4.3.2rc1/docs/images/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/ListThumbnail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/chart_time1.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/chart_time2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/charts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/contact_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/contacts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/direct_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/fab.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/group_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/grouped_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/groups.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/images_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/list_cascade.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/list_cascade_block.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/list_compact_inline.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/list_master_detail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/login.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/login_db.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/login_oid.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    82437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/oauth_login.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    48690 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/oauth_login_one_provider.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    42827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/security.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/simpleview2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    41274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/swagger001.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26185 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/images/swagger002.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1389 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/docs/index.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4377 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.2rc1/docs/installation.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2634 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/intro.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6721 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/make.bat
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/multipledbs.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/quickcharts.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/quickfiles.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/quickhowto.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4829 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/quickhowto_mongo.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1676 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/quickminimal.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8990 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/relations.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    47286 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/rest_api.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    35876 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.2rc1/docs/security.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17032 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/templates.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4335 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/user_registration.rst
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)    12302 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/versionmigration.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/docs/views.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.161668 Flask-AppBuilder-4.3.2rc1/examples/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.163993 Flask-AppBuilder-4.3.2rc1/examples/base_api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/base_api/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.166279 Flask-AppBuilder-4.3.2rc1/examples/base_api/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      380 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/base_api/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/base_api/app/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1809 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/base_api/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.171602 Flask-AppBuilder-4.3.2rc1/examples/basefilter/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/basefilter/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      429 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/basefilter/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.175771 Flask-AppBuilder-4.3.2rc1/examples/basefilter/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/basefilter/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1458 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/basefilter/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.031859 Flask-AppBuilder-4.3.2rc1/examples/basefilter/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.031974 Flask-AppBuilder-4.3.2rc1/examples/basefilter/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.178111 Flask-AppBuilder-4.3.2rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1413 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/basefilter/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.181655 Flask-AppBuilder-4.3.2rc1/examples/basefilter/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/basefilter/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/basefilter/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/basefilter/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/basefilter/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2423 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/basefilter/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.185493 Flask-AppBuilder-4.3.2rc1/examples/composite_keys/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      254 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/composite_keys/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.188752 Flask-AppBuilder-4.3.2rc1/examples/composite_keys/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/composite_keys/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/composite_keys/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/composite_keys/app/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2182 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/composite_keys/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1477 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/composite_keys/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.193970 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.197722 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2485 2023-02-15 14:55:19.000000 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/app/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1943 2022-12-21 14:38:19.000000 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.032776 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.032827 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.200212 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.202498 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2459 2023-05-05 09:39:55.000000 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2580 2022-12-20 19:18:45.000000 Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.205701 Flask-AppBuilder-4.3.2rc1/examples/dash/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      291 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/dash/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.208135 Flask-AppBuilder-4.3.2rc1/examples/dash/app/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.212705 Flask-AppBuilder-4.3.2rc1/examples/dash/app/Dashboard/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      797 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/dash/app/Dashboard/Dash_App1.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/dash/app/Dashboard/Dash_App2.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1568 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/dash/app/Dashboard/Dash_fun.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/dash/app/Dashboard/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/dash/app/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.213764 Flask-AppBuilder-4.3.2rc1/examples/dash/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      701 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/dash/app/templates/dash.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1031 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/dash/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.216767 Flask-AppBuilder-4.3.2rc1/examples/dash/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/dash/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/dash/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/dash/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/dash/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.219391 Flask-AppBuilder-4.3.2rc1/examples/employees/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      276 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/employees/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.224182 Flask-AppBuilder-4.3.2rc1/examples/employees/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/employees/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/employees/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/employees/app/security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1972 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.2rc1/examples/employees/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.225550 Flask-AppBuilder-4.3.2rc1/examples/employees/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/employees/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/employees/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.230722 Flask-AppBuilder-4.3.2rc1/examples/enums/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/enums/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/enums/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.234836 Flask-AppBuilder-4.3.2rc1/examples/enums/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/enums/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1158 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/enums/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.033773 Flask-AppBuilder-4.3.2rc1/examples/enums/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.033827 Flask-AppBuilder-4.3.2rc1/examples/enums/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.237520 Flask-AppBuilder-4.3.2rc1/examples/enums/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3436 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/enums/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.239969 Flask-AppBuilder-4.3.2rc1/examples/enums/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/enums/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/enums/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/enums/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1841 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/enums/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.245913 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.253407 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2607 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/sec.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/sec_forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1923 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/sec_views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.034221 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.034275 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.255636 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1589 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.259079 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1961 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2977 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.263879 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      560 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.302329 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2831 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/sec.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/sec_forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1929 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/sec_views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.034675 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.034727 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.306623 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2133 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.309968 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.316770 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      432 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.320300 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.035136 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.035192 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.322562 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2121 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.325948 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1904 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/config2.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1867 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/examples/factoryapp/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.328070 Flask-AppBuilder-4.3.2rc1/examples/issue_789/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1610 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/issue_789/README.rst
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4740 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/issue_789/app.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.332013 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/NAMES.DIC
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.335535 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1164 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.035676 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.035731 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.337863 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.342873 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/masterdetail/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.351488 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.359839 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/mysecurity.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.036097 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.036144 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.363922 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2988 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.368054 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.378787 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.384899 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.036483 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.036535 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.388898 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2623 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.394877 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoengine/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.404883 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      296 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.411023 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2732 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.036882 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.036931 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.415171 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4050 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.421130 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/mongoimages/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.431655 Flask-AppBuilder-4.3.2rc1/examples/oauth/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/oauth/.gitignore
--rw-r--r--   0 dpgaspar   (501) staff       (20)      531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/oauth/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.450756 Flask-AppBuilder-4.3.2rc1/examples/oauth/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      743 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/oauth/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      399 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/oauth/app/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/oauth/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      928 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/examples/oauth/app/security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2395 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/examples/oauth/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.458209 Flask-AppBuilder-4.3.2rc1/examples/oauth/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/oauth/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/oauth/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8905 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/examples/oauth/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/oauth/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.469355 Flask-AppBuilder-4.3.2rc1/examples/productsale/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      192 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/productsale/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.480612 Flask-AppBuilder-4.3.2rc1/examples/productsale/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/productsale/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1755 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/productsale/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.037588 Flask-AppBuilder-4.3.2rc1/examples/productsale/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.037515 Flask-AppBuilder-4.3.2rc1/examples/productsale/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.488045 Flask-AppBuilder-4.3.2rc1/examples/productsale/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.037632 Flask-AppBuilder-4.3.2rc1/examples/productsale/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.495600 Flask-AppBuilder-4.3.2rc1/examples/productsale/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1304 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/productsale/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.499370 Flask-AppBuilder-4.3.2rc1/examples/productsale/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/productsale/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/productsale/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/productsale/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.510741 Flask-AppBuilder-4.3.2rc1/examples/quickactions/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.521872 Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      554 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      263 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.038427 Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.038342 Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.529271 Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.038475 Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.536863 Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1067 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.540727 Flask-AppBuilder-4.3.2rc1/examples/quickactions/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickactions/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1945 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickactions/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickactions/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      279 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickactions/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.548294 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.563345 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1685 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/app/data.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.038793 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.038838 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.570717 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2928 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.581846 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1775 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.589058 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.599935 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      352 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.039158 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.039203 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.607271 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5073 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.618147 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/babel/messages.pot~
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.039566 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.039442 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/bdist.linux-i686/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.039492 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/bdist.linux-i686/egg/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.629184 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.039615 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/lib/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.640041 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/lib/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/lib/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/lib/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/lib/app/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1726 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.651051 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      225 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.662029 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1188 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.665664 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.039969 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.676950 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16804 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.040090 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.688084 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16794 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1395 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.695504 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1795 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickfiles/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.712061 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.734455 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-07-29 16:17:15.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.040417 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.040461 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.749159 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3166 2022-08-16 10:09:18.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.770675 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2758 2023-05-05 09:39:55.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.799796 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/NAMES.DIC
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.857143 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      556 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      105 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/indexview.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3024 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      300 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/sec.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/sec_models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2047 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/sec_views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.041119 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.896979 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/abBtnAdd.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      171 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/abBtnDelete.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/abBtnEdit.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      179 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/abBtnShow.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/abDate.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/abMenuPageSize.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      548 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1633 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/abModelSearch.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2033 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/abModelTable.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/abPagination.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/abSelect.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.897545 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/css/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7059 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/css/clean-blog.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1446 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/css/scrolling-nav.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.898145 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/img/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      783 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/img/brand.jpg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3208 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/img/loading.gif
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.899568 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.900370 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/Controllers/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1781 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      240 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/Controllers/searchCtrl.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.900922 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/Directives/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3764 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/Directives/bigDirectives.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9587 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/Directives/btnDirectives.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.901204 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/Services/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2825 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/Services/apiService.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)   125321 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/angular.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/app.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17294 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/clean-blog.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      612 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/scrolling-nav.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.903072 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.903426 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/appbuilder/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10245 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/list_angulajs.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      332 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/list_contacts.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/list_json.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      199 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/mylist.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/new_base.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      371 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/show_contacts.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.903950 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/widgets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2549 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/widgets/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      280 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/widgets/list_override.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.041678 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.041727 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.904535 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2511 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.905316 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2387 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2327 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1533 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.907943 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    92965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/.coverage
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      220 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.908643 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      753 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.042238 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.042312 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.909101 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.909800 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1942 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/migrate_db_0.7.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1397 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.910232 Flask-AppBuilder-4.3.2rc1/examples/quickimages/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickimages/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.910913 Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2636 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.043095 Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.042769 Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.911330 Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.043208 Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.916359 Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4155 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.916631 Flask-AppBuilder-4.3.2rc1/examples/quickimages/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickimages/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1704 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickimages/config.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.922271 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.922915 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      418 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.043891 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.043972 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.923349 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3627 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.923727 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.923955 Flask-AppBuilder-4.3.2rc1/examples/quickminimal/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      430 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quickminimal/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.925485 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.931148 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/.idea/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      159 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/.idea/encodings.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      679 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/.idea/misc.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      278 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/.idea/modules.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)      284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/.idea/quicksqlviews.iml
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1846 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/.idea/workspace.xml
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.931803 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.044883 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.044943 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.932232 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.932655 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.933912 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      257 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.934528 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      386 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.045302 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/static/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.937017 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/static/css/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2891 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/static/css/landing-page.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.937262 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3245 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/templates/mybase.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.045499 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.045547 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.937667 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3658 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.938317 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.942070 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.942943 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1553 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.950211 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       66 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/.babelrc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      398 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/README.md
--rw-r--r--   0 dpgaspar   (501) staff       (20)   838924 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/package-lock.json
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3522 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/package.json
--rw-r--r--   0 dpgaspar   (501) staff       (20)      746 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/package.json.react-original
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.950854 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/public/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/public/favicon.ico
--rw-r--r--   0 dpgaspar   (501) staff       (20)      283 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/public/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/public/manifest.json
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.951256 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/src/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      375 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/src/App.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.951464 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/src/api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      959 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/src/api/Api.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.954401 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/src/components/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3602 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/src/components/CRUDButtons.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4478 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/src/components/Forms.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15937 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/src/components/Table.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      349 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/src/index.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      285 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/webpack.config.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.954852 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      856 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/templates/base.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/templates/react.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.046454 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.046505 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.955225 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.955821 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2462 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.957495 Flask-AppBuilder-4.3.2rc1/examples/related_fields/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/related_fields/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      221 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/related_fields/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.958062 Flask-AppBuilder-4.3.2rc1/examples/related_fields/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/related_fields/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/related_fields/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.046905 Flask-AppBuilder-4.3.2rc1/examples/related_fields/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.046957 Flask-AppBuilder-4.3.2rc1/examples/related_fields/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.958435 Flask-AppBuilder-4.3.2rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5719 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/related_fields/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.958823 Flask-AppBuilder-4.3.2rc1/examples/related_fields/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/related_fields/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/related_fields/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/related_fields/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/related_fields/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2739 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/related_fields/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.959514 Flask-AppBuilder-4.3.2rc1/examples/simpleform/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleform/.gitignore
--rw-r--r--   0 dpgaspar   (501) staff       (20)      286 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleform/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.964516 Flask-AppBuilder-4.3.2rc1/examples/simpleform/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleform/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      507 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleform/app/forms.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.964858 Flask-AppBuilder-4.3.2rc1/examples/simpleform/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleform/app/templates/404.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.047410 Flask-AppBuilder-4.3.2rc1/examples/simpleform/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.047454 Flask-AppBuilder-4.3.2rc1/examples/simpleform/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.965315 Flask-AppBuilder-4.3.2rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)      940 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleform/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.965752 Flask-AppBuilder-4.3.2rc1/examples/simpleform/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleform/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      662 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleform/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3697 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleform/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleform/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.966378 Flask-AppBuilder-4.3.2rc1/examples/simpleview1/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      173 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleview1/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.966792 Flask-AppBuilder-4.3.2rc1/examples/simpleview1/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleview1/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      601 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleview1/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.967150 Flask-AppBuilder-4.3.2rc1/examples/simpleview1/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleview1/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleview1/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleview1/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleview1/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.967504 Flask-AppBuilder-4.3.2rc1/examples/simpleview2/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.970170 Flask-AppBuilder-4.3.2rc1/examples/simpleview2/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      381 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleview2/app/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.970385 Flask-AppBuilder-4.3.2rc1/examples/simpleview2/app/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      108 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleview2/app/templates/method3.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1198 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleview2/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.970834 Flask-AppBuilder-4.3.2rc1/examples/simpleview2/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleview2/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleview2/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleview2/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/simpleview2/run.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.972503 Flask-AppBuilder-4.3.2rc1/examples/user_registration/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/user_registration/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      267 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/user_registration/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.973045 Flask-AppBuilder-4.3.2rc1/examples/user_registration/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/user_registration/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1639 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/user_registration/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.048481 Flask-AppBuilder-4.3.2rc1/examples/user_registration/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.048543 Flask-AppBuilder-4.3.2rc1/examples/user_registration/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.973421 Flask-AppBuilder-4.3.2rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3981 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/user_registration/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.973947 Flask-AppBuilder-4.3.2rc1/examples/user_registration/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/user_registration/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/user_registration/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/user_registration/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/user_registration/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/user_registration/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/user_registration/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.975114 Flask-AppBuilder-4.3.2rc1/examples/widgets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/widgets/NAMES.DIC
--rw-r--r--   0 dpgaspar   (501) staff       (20)      229 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/widgets/README.rst
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.975753 Flask-AppBuilder-4.3.2rc1/examples/widgets/app/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/widgets/app/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/widgets/app/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.048944 Flask-AppBuilder-4.3.2rc1/examples/widgets/app/translations/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.048991 Flask-AppBuilder-4.3.2rc1/examples/widgets/app/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.976180 Flask-AppBuilder-4.3.2rc1/examples/widgets/app/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4839 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/widgets/app/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.976759 Flask-AppBuilder-4.3.2rc1/examples/widgets/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/widgets/babel/babel.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/widgets/babel/messages.pot
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/widgets/babel/messages.pot~
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/widgets/config.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/widgets/run.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1491 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/examples/widgets/testdata.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.991680 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2023-05-12 13:46:37.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1970 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/_compat.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1233 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/actions.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.995367 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/api/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    76068 2023-02-23 14:18:46.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/api/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9338 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/api/convert.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3368 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/api/manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/api/schemas.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.995867 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/babel/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/babel/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2275 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/babel/manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/babel/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26094 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      346 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/basemanager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    48877 2023-05-08 11:18:50.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/baseviews.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.996589 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/charts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/charts/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/charts/jsontools.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17665 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/charts/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/charts/widgets.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14981 2023-05-05 08:39:47.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/cli.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14159 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/console.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8459 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/const.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1138 2022-09-30 13:30:31.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/exceptions.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8785 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/fields.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5984 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/fieldwidgets.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8534 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/filemanager.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)     6206 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11138 2023-02-15 14:55:26.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3131 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/hooks.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7648 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/menu.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      290 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/messages.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.998151 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9631 2022-10-10 15:29:42.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      846 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/decorators.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10375 2022-12-22 10:35:46.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/filters.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.000971 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/generic/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13059 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/generic/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/generic/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2253 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/generic/interface.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10979 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/group.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2633 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/mixins.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.001628 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/mongoengine/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1765 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/mongoengine/fields.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4184 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/mongoengine/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10027 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/mongoengine/interface.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.002564 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/sqla/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4145 2022-10-27 13:02:57.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/sqla/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11046 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/sqla/filters.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39635 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/sqla/interface.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.007809 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5220 2023-05-08 09:55:27.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10693 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/decorators.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4162 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/forms.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    77461 2023-04-20 12:25:04.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/manager.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.008614 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/mongoengine/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15641 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/mongoengine/manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3219 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/mongoengine/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10650 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/registerviews.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1359 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/schemas.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.009456 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.009726 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.010354 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/permission/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       45 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/permission/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      624 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/permission/api.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.010732 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       53 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      647 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.011180 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/role/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/role/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5053 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/role/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      359 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/role/schema.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.011775 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/user/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/user/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6695 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/user/api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2176 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/user/schema.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1100 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/user/validator.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.014358 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/view_menu/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       43 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/view_menu/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      569 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/view_menu/api.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)    27043 2022-11-09 14:23:15.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/manager.py
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)     5260 2022-10-27 13:02:57.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/models.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/utils.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    25771 2023-03-16 10:28:12.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/views.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.051086 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.052077 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.014799 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/ab.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121457 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/bootstrap.min.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.015116 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/flags/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/flags/flags16.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.017319 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/fontawesome/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18600 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    80761 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)      586 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)      578 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1760 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    27593 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.026462 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   105250 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/amelia.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   120090 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/cerulean.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   119768 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/cosmo.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   119799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/cyborg.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121625 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/darkly.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121354 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/flatly.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118666 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/journal.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   124431 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/lumen.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   132318 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/paper.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118678 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/readable.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/sandstone.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   120186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/simplex.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   129014 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/slate.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   125030 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/solar.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/spacelab.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   120731 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/superhero.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   117016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/united.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)   121865 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/yeti.css
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.026892 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/datepicker/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.030294 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/fonts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20127 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 dpgaspar   (501) staff       (20)   108738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 dpgaspar   (501) staff       (20)    45404 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)    23424 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 dpgaspar   (501) staff       (20)    18028 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.031631 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/aol.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/fab.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.031789 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/flags/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    63284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/flags/flags16.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1595 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/flickr.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8777 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    12799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2558 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/google.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2882 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/myopenid.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/yahoo.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.034640 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3176 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/ab.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4228 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/ab_actions.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4834 2023-05-12 13:46:20.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/ab_filters.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1526 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39680 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/bootstrap.min.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)   117065 2023-01-10 15:35:16.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/fontawesome.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    46151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/google_charts.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    89501 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/jquery-latest.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)    27347 2023-01-10 15:34:59.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/v4-shims.min.js
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.040859 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/select2/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16792 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1849 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/select2/select2-spinner.gif
--rw-r--r--   0 dpgaspar   (501) staff       (20)    17358 2022-12-22 10:31:26.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/select2/select2.css
--rw-r--r--   0 dpgaspar   (501) staff       (20)    79212 2022-12-22 10:31:26.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/select2/select2.js
--rw-r--r--   0 dpgaspar   (501) staff       (20)      613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/select2/select2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)      845 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/select2/select2x2.png
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.051167 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   186124 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)   107656 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.woff2
--rw-r--r--   0 dpgaspar   (501) staff       (20)    62320 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)    25236 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.woff2
--rw-r--r--   0 dpgaspar   (501) staff       (20)   397420 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)   150516 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.woff2
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10140 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4568 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.woff2
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.052258 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.057849 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/_formhelpers.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)       28 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/base.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      874 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/baselayout.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/baselib.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      486 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/flash.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      143 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/footer.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.058325 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/alert.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.058875 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/charts/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      778 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/charts/chart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      890 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      717 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/confirm.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13876 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/lib.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.064783 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/add.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1147 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/edit.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      779 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      653 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      496 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      517 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      417 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/search.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1173 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/show.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.066320 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/security/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/security/activation.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2949 2023-01-10 15:41:47.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/security/login_db.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1996 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2023-02-15 14:55:26.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/security/login_oid.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      230 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/security/register_mail.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1057 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      754 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/security/resetpassword.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.073840 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1091 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2908 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/chart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2541 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/form.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1326 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1328 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/group_form_list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2745 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1331 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2038 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2843 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      572 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1167 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1559 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.074134 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1080 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/search.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/show.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1833 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1544 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)      145 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2773 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/init.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1299 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/navbar.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1264 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/navbar_menu.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1581 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/navbar_right.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.074278 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/swagger/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      764 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/swagger/swagger.html
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.083141 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.083698 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/A_fixture/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/A_fixture/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.084235 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/A_fixture/__pycache__/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      184 2022-06-17 10:46:19.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/A_fixture/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1882 2023-02-23 14:02:46.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/A_fixture/__pycache__/test_0_fixture.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      370 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/A_fixture/addon_manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1372 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/A_fixture/test_0_fixture.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.091886 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      174 2022-06-17 10:46:19.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)     5453 2022-07-29 12:58:36.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/base.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      601 2023-03-16 10:39:04.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/config_api.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      993 2023-05-08 12:37:37.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/config_oauth.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      629 2023-05-03 11:58:50.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/config_security.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)      443 2023-02-23 14:03:19.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/const.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)    81512 2022-12-22 12:24:31.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/test_api.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7970 2023-05-03 12:02:06.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/test_fab_cli.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)    52431 2023-05-08 12:13:02.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/test_mvc.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4712 2023-05-08 12:38:18.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/test_mvc_oauth.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)   229376 2022-12-22 12:25:31.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/app.db
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4453 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      463 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/config_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1029 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/config_oauth.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      479 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/config_security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      515 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/config_security_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      250 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/const.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.092202 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/data/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7636 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/data/roles.json
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.092598 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/mongoengine/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/mongoengine/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1006 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/mongoengine/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.094290 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.095435 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/__pycache__/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      183 2023-02-23 14:04:47.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19332 2023-05-08 10:31:28.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/__pycache__/test_auth_ldap.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10255 2023-05-08 10:42:47.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/__pycache__/test_mvc_security.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3436 2023-02-23 14:57:17.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/__pycache__/test_rate_limiter.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)    34243 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/test_auth_ldap.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14028 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/test_auth_oauth.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2434 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/test_base_security_manager.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    14235 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/test_mvc_security.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1715 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/test_password_complexity.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2962 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/test_rate_limiter.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.095761 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/sqla/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/sqla/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.100797 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/sqla/__pycache__/
--rw-r--r--   0 dpgaspar   (501) staff       (20)      179 2022-06-17 10:46:19.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/sqla/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10026 2022-12-22 12:24:31.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/sqla/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10276 2022-12-21 14:37:56.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/sqla/models.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.101065 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/templates/
--rw-r--r--   0 dpgaspar   (501) staff       (20)       29 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/templates/custom_index.html
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1335 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_addon.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)   118599 2022-12-21 14:37:56.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1245 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_custom_indexview.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8776 2023-05-05 08:39:47.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_fab_cli.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6503 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_menu.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    24066 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_mongoengine.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    68524 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_mvc.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4465 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_mvc_oauth.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    44396 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_security_api.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     6056 2022-11-09 14:23:15.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_security_permissions.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_sqlalchemy.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2540 2022-08-17 09:07:58.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_urltools.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.101279 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/__init__.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.060629 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/de/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.106263 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/de/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9681 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    26578 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.061633 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/el/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.106835 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/el/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    11017 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    22936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.062662 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/es/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.107178 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/es/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8468 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20079 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.063645 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/fr/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.107517 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/fr/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8504 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20065 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.064555 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/it/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.107854 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/it/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9121 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    24545 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.065474 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ja_JP/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.108446 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9412 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20790 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.066436 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ko/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.108769 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ko/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9513 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    39930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.067337 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/nl/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.109114 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/nl/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8252 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19648 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.068227 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pl/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.109428 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pl/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8136 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.069127 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pt/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.110267 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pt/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8441 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20002 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.070056 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pt_BR/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.111261 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     8336 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19734 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.070969 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ru/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.111816 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ru/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10674 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    22035 2023-03-13 10:27:18.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.071872 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/sl/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.112579 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/sl/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     9682 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    20841 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.072786 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/zh/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.114729 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/zh/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7528 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:06.073725 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/zh_HK/
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.115421 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo
--rw-r--r--   0 dpgaspar   (501) staff       (20)    19104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po
--rw-r--r--   0 dpgaspar   (501) staff       (20)     7576 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/upload.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3226 2022-08-17 09:07:58.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/urltools.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.123374 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/utils/
--rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/utils/__init__.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2284 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/utils/base.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)      734 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/utils/limit.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     3360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/validators.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)    31361 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/views.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     4997 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/flask_appbuilder/widgets.py
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.153641 Flask-AppBuilder-4.3.2rc1/images/
--rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/ListThumbnail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/chart_time1.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/chart_time2.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/charts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/contact_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/contacts.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/direct_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/fab.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/group_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/grouped_chart.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/groups.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/images_list.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/list_cascade.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/list_cascade_block.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/list_compact_inline.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/list_master_detail.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/login.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/login_db.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    84309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/login_oauth.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/login_oid.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)   417827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/security.png
--rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/images/simpleview2.png
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      181 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/release.sh
--rw-r--r--   0 dpgaspar   (501) staff       (20)      218 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.2rc1/requirements-dev.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)      157 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.2rc1/requirements-extra.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2967 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.2rc1/requirements.txt
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2320 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.2rc1/rtd_requirements.txt
-drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-12 13:48:07.154103 Flask-AppBuilder-4.3.2rc1/scripts/
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      217 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/scripts/babel_extract.sh
--rwxr-xr-x   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/scripts/babel_init.sh
--rw-r--r--   0 dpgaspar   (501) staff       (20)      755 2023-05-12 13:48:07.154952 Flask-AppBuilder-4.3.2rc1/setup.cfg
--rw-r--r--   0 dpgaspar   (501) staff       (20)     2827 2023-04-20 12:20:38.000000 Flask-AppBuilder-4.3.2rc1/setup.py
--rw-r--r--   0 dpgaspar   (501) staff       (20)     1766 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc1/tox.ini
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.969629 Flask-AppBuilder-4.3.2rc2/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       97 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/.coveragerc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      113 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/.env
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.702607 Flask-AppBuilder-4.3.2rc2/.github/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      642 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      681 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      202 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/.github/prlint.json
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      709 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/.github/stale.yml
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.704724 Flask-AppBuilder-4.3.2rc2/.github/workflows/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8087 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.2rc2/.github/workflows/ci.yml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      137 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/.github/workflows/odbcinst.ini
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      951 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/.github/workflows/ptlint.yml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      147 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/.gitignore
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    63244 2023-05-22 10:16:16.000000 Flask-AppBuilder-4.3.2rc2/CHANGELOG.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/CONTRIBUTING.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.709708 Flask-AppBuilder-4.3.2rc2/Flask_AppBuilder.egg-info/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9290 2023-05-22 10:31:56.000000 Flask-AppBuilder-4.3.2rc2/Flask_AppBuilder.egg-info/PKG-INFO
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    38050 2023-05-22 10:31:56.000000 Flask-AppBuilder-4.3.2rc2/Flask_AppBuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2023-05-22 10:31:56.000000 Flask-AppBuilder-4.3.2rc2/Flask_AppBuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      110 2023-05-22 10:31:56.000000 Flask-AppBuilder-4.3.2rc2/Flask_AppBuilder.egg-info/entry_points.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-12 08:40:39.000000 Flask-AppBuilder-4.3.2rc2/Flask_AppBuilder.egg-info/not-zip-safe
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      540 2023-05-22 10:31:56.000000 Flask-AppBuilder-4.3.2rc2/Flask_AppBuilder.egg-info/requires.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       17 2023-05-22 10:31:56.000000 Flask-AppBuilder-4.3.2rc2/Flask_AppBuilder.egg-info/top_level.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1493 2023-04-05 15:10:33.000000 Flask-AppBuilder-4.3.2rc2/LICENSE
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      257 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/MANIFEST.in
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9290 2023-05-22 10:31:57.969776 Flask-AppBuilder-4.3.2rc2/PKG-INFO
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6684 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/README.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/RELEASE.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.710974 Flask-AppBuilder-4.3.2rc2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    36590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/babel/messages.pot
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.700159 Flask-AppBuilder-4.3.2rc2/bin/
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      176 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/bin/babel_extract.sh
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/bin/babel_init.sh
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      422 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/bin/bootswatch_update.sh
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1632 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/bin/config.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/bin/db_create.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      840 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/bin/db_migrate.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/bin/db_upgrade.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1419 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/bin/hash_db_password.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/bin/migrate_db_0.7.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)     4001 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/bin/migrate_db_1.3.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1917 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/bin/sqlite_upgrade_1.3.sql
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      999 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.2rc2/docker-compose.yml
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.733358 Flask-AppBuilder-4.3.2rc2/docs/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6802 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/Makefile
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.733991 Flask-AppBuilder-4.3.2rc2/docs/_static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/_static/Flask-AppBuilder.png
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.734825 Flask-AppBuilder-4.3.2rc2/docs/_templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/_templates/layout.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.736778 Flask-AppBuilder-4.3.2rc2/docs/_themes/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/_themes/LICENSE
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1093 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/_themes/README
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.738685 Flask-AppBuilder-4.3.2rc2/docs/_themes/flask/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      954 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/_themes/flask/layout.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/_themes/flask/relations.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.740084 Flask-AppBuilder-4.3.2rc2/docs/_themes/flask/static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/_themes/flask/static/Flask-AppBuilder.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9062 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/_themes/flask/static/flasky.css_t
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      181 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/_themes/flask/theme.conf
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.741381 Flask-AppBuilder-4.3.2rc2/docs/_themes/flask_small/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      683 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/_themes/flask_small/layout.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.741980 Flask-AppBuilder-4.3.2rc2/docs/_themes/flask_small/static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/_themes/flask_small/static/flasky.css_t
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      184 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/_themes/flask_small/theme.conf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4875 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/_themes/flask_theme_support.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2277 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/actions.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3828 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/addons.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10881 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.2rc2/docs/advanced.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/api.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/cli.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8834 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/conf.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)    33481 2023-05-05 08:39:47.000000 Flask-AppBuilder-4.3.2rc2/docs/config.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10806 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/customizing.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4109 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/diagrams.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/generic_datasource.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3817 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/docs/i18n.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.761981 Flask-AppBuilder-4.3.2rc2/docs/images/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/ListThumbnail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/chart_time1.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/chart_time2.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/charts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/contact_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/contacts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/direct_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/fab.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/group_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/grouped_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/groups.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/images_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/list_cascade.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/list_cascade_block.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/list_compact_inline.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/list_master_detail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/login.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/login_db.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/login_oid.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    82437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/oauth_login.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    48690 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/oauth_login_one_provider.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    42827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/security.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/simpleview2.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    41274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/swagger001.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26185 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/images/swagger002.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1389 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/docs/index.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4377 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.2rc2/docs/installation.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2634 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/intro.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6721 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/make.bat
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/multipledbs.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/quickcharts.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/quickfiles.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/quickhowto.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4829 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/quickhowto_mongo.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1676 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/quickminimal.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8990 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/relations.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    47286 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/rest_api.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    35876 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.2rc2/docs/security.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17032 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/templates.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4335 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/user_registration.rst
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)    12302 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/versionmigration.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/docs/views.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.762606 Flask-AppBuilder-4.3.2rc2/examples/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2036 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.763875 Flask-AppBuilder-4.3.2rc2/examples/base_api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      209 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/base_api/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.765109 Flask-AppBuilder-4.3.2rc2/examples/base_api/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      380 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/base_api/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3789 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/base_api/app/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1809 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/base_api/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.768314 Flask-AppBuilder-4.3.2rc2/examples/basefilter/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/basefilter/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      429 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/basefilter/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.770173 Flask-AppBuilder-4.3.2rc2/examples/basefilter/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/basefilter/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1458 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/basefilter/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.639124 Flask-AppBuilder-4.3.2rc2/examples/basefilter/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.639180 Flask-AppBuilder-4.3.2rc2/examples/basefilter/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.771430 Flask-AppBuilder-4.3.2rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1413 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/basefilter/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.773269 Flask-AppBuilder-4.3.2rc2/examples/basefilter/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/basefilter/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/basefilter/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/basefilter/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/basefilter/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2423 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/basefilter/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.775155 Flask-AppBuilder-4.3.2rc2/examples/composite_keys/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      254 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/composite_keys/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.776933 Flask-AppBuilder-4.3.2rc2/examples/composite_keys/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/composite_keys/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1464 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/composite_keys/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/composite_keys/app/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2182 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/composite_keys/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1477 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/composite_keys/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.780912 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.783429 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2485 2023-02-15 14:55:19.000000 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/app/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1943 2022-12-21 14:38:19.000000 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.639789 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.639845 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.785003 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.786313 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2459 2023-05-05 09:39:55.000000 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2580 2022-12-20 19:18:45.000000 Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.788712 Flask-AppBuilder-4.3.2rc2/examples/dash/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      291 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/dash/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.790821 Flask-AppBuilder-4.3.2rc2/examples/dash/app/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.795271 Flask-AppBuilder-4.3.2rc2/examples/dash/app/Dashboard/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      797 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/dash/app/Dashboard/Dash_App1.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/dash/app/Dashboard/Dash_App2.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1568 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/dash/app/Dashboard/Dash_fun.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/dash/app/Dashboard/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/dash/app/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.796342 Flask-AppBuilder-4.3.2rc2/examples/dash/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      701 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/dash/app/templates/dash.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1031 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/dash/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.798545 Flask-AppBuilder-4.3.2rc2/examples/dash/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/dash/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/dash/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/dash/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/dash/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.800755 Flask-AppBuilder-4.3.2rc2/examples/employees/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      276 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/employees/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.805176 Flask-AppBuilder-4.3.2rc2/examples/employees/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/employees/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/employees/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/employees/app/security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1972 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.2rc2/examples/employees/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.806430 Flask-AppBuilder-4.3.2rc2/examples/employees/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/employees/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/employees/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.811007 Flask-AppBuilder-4.3.2rc2/examples/enums/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/enums/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/enums/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.814147 Flask-AppBuilder-4.3.2rc2/examples/enums/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      358 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/enums/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1158 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/enums/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.640967 Flask-AppBuilder-4.3.2rc2/examples/enums/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.641024 Flask-AppBuilder-4.3.2rc2/examples/enums/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.816294 Flask-AppBuilder-4.3.2rc2/examples/enums/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3436 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/enums/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.818311 Flask-AppBuilder-4.3.2rc2/examples/enums/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/enums/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/enums/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/enums/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1841 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/enums/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.823225 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      614 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.829980 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2607 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/sec.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/sec_forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1923 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/sec_views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.641416 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.641469 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.832217 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1589 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.835543 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1961 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2977 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.840290 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      560 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.846713 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2831 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      453 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/sec.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      880 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/sec_forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1929 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/sec_views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.641839 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.641894 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.848818 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2133 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.850960 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.857433 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      432 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.860682 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.642250 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.642295 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.863053 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2121 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.866301 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1904 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/config2.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1867 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/examples/factoryapp/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.868494 Flask-AppBuilder-4.3.2rc2/examples/issue_789/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1610 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/issue_789/README.rst
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4740 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/issue_789/app.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.872180 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/NAMES.DIC
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.875543 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1164 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.642728 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.642788 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.877704 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2711 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.880964 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1519 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/masterdetail/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.885502 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.889929 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/mysecurity.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.643130 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.643183 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.892062 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2988 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.894260 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.900442 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.903900 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.643509 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.643557 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.906166 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2623 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.909340 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1652 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoengine/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.914947 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      296 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.918075 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      508 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2732 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.643903 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.643948 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.920256 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4050 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.926090 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1906 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/mongoimages/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.933924 Flask-AppBuilder-4.3.2rc2/examples/oauth/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/oauth/.gitignore
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      531 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/oauth/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.943678 Flask-AppBuilder-4.3.2rc2/examples/oauth/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      743 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/oauth/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      399 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/oauth/app/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      256 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/oauth/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      928 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/examples/oauth/app/security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2395 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/examples/oauth/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.947574 Flask-AppBuilder-4.3.2rc2/examples/oauth/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/oauth/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/oauth/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8905 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/examples/oauth/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/oauth/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.953463 Flask-AppBuilder-4.3.2rc2/examples/productsale/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      192 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/productsale/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.959175 Flask-AppBuilder-4.3.2rc2/examples/productsale/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/productsale/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1755 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/productsale/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.644592 Flask-AppBuilder-4.3.2rc2/examples/productsale/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.644522 Flask-AppBuilder-4.3.2rc2/examples/productsale/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.963118 Flask-AppBuilder-4.3.2rc2/examples/productsale/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.644636 Flask-AppBuilder-4.3.2rc2/examples/productsale/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.967173 Flask-AppBuilder-4.3.2rc2/examples/productsale/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1304 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/productsale/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.969106 Flask-AppBuilder-4.3.2rc2/examples/productsale/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/productsale/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/productsale/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/productsale/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.975082 Flask-AppBuilder-4.3.2rc2/examples/quickactions/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.980920 Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      554 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      263 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.645079 Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.645007 Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.987159 Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.645124 Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.991160 Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1067 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.993135 Flask-AppBuilder-4.3.2rc2/examples/quickactions/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickactions/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1945 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickactions/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickactions/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      279 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickactions/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.997046 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.004970 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1685 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/app/data.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.645445 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.645491 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.008827 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2928 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.017051 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1775 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.024280 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.035236 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      352 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1342 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.645818 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.645861 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.042604 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5073 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.053539 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/babel/messages.pot~
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.646223 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.646108 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/bdist.linux-i686/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.646152 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/bdist.linux-i686/egg/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.064593 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.646268 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/lib/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.076634 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/lib/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      356 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/lib/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1322 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/lib/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5082 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/lib/app/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1726 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.091054 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      225 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.102021 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      351 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1188 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.105696 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.646587 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.116873 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16804 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.646715 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.128317 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16794 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1395 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.135862 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1795 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickfiles/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.151346 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      214 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.163357 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-07-29 16:17:15.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.647052 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.647100 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.171121 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3166 2022-08-16 10:09:18.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.182029 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2758 2023-05-19 13:12:13.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.197323 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/NAMES.DIC
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.227980 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      574 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      556 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      105 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/indexview.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3024 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      300 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/sec.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/sec_models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2047 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/sec_views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.647620 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.269484 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/abBtnAdd.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      171 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/abBtnDelete.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      177 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/abBtnEdit.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      179 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/abBtnShow.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/abDate.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      437 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/abMenuPageSize.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      548 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1633 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/abModelSearch.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2033 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/abModelTable.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/abPagination.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/abSelect.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.276924 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/css/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7059 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/css/clean-blog.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1446 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/css/scrolling-nav.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.284222 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/img/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      783 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/img/brand.jpg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3208 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/img/loading.gif
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.299244 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.313649 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/Controllers/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1781 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      240 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/Controllers/searchCtrl.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3803 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.327864 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/Directives/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3764 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/Directives/bigDirectives.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9587 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/Directives/btnDirectives.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.334881 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/Services/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2825 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/Services/apiService.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   125321 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/angular.min.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/app.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17294 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/clean-blog.min.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      612 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/scrolling-nav.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.384444 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.391575 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/appbuilder/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/appbuilder/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10245 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/list_angulajs.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      332 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/list_contacts.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2251 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/list_json.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      199 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/mylist.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      324 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/new_base.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      371 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/show_contacts.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.405700 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/widgets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2549 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/widgets/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      280 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/widgets/list_override.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.648195 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.648247 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.419873 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2511 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.441079 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2387 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2327 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1533 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.491570 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    92965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/.coverage
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      220 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.513310 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      753 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.648582 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.648635 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.527708 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.549269 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1942 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/migrate_db_0.7.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1397 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.563734 Flask-AppBuilder-4.3.2rc2/examples/quickimages/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickimages/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.592458 Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      628 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2636 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.649131 Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.649057 Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.607554 Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5786 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19912 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.649179 Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.622243 Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5780 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19896 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4155 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.629661 Flask-AppBuilder-4.3.2rc2/examples/quickimages/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       84 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickimages/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1704 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickimages/config.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.659355 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.681171 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      418 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.649656 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.649716 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.691238 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3627 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.691928 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2226 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2119 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.694303 Flask-AppBuilder-4.3.2rc2/examples/quickminimal/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      430 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quickminimal/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.701508 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.703350 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/.idea/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      159 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/.idea/encodings.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      679 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/.idea/misc.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      278 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/.idea/modules.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/.idea/quicksqlviews.iml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1846 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/.idea/workspace.xml
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.706468 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.650290 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.650339 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.706937 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.707406 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.715253 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      257 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.716056 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      386 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.650696 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/static/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.716267 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/static/css/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2891 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/static/css/landing-page.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.716473 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3245 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/templates/mybase.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.651011 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.651071 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.724036 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3658 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.724755 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.728860 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      295 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.732475 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1553 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.742171 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       66 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/.babelrc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      398 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/README.md
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   838924 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/package-lock.json
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3522 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/package.json
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      746 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/package.json.react-original
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.742752 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/public/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3870 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/public/favicon.ico
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      283 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/public/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/public/manifest.json
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.743164 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/src/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      375 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/src/App.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.743378 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/src/api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      959 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/src/api/Api.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.743986 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/src/components/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3602 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/src/components/CRUDButtons.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4478 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/src/components/Forms.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15937 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/src/components/Table.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      349 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/src/index.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      285 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/webpack.config.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.744389 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      856 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/templates/base.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/templates/react.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.651907 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.651951 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.744790 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.745151 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2462 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.746477 Flask-AppBuilder-4.3.2rc2/examples/related_fields/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/related_fields/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      221 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/related_fields/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.747139 Flask-AppBuilder-4.3.2rc2/examples/related_fields/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/related_fields/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/related_fields/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.652283 Flask-AppBuilder-4.3.2rc2/examples/related_fields/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.652328 Flask-AppBuilder-4.3.2rc2/examples/related_fields/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.747666 Flask-AppBuilder-4.3.2rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5719 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/related_fields/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.754952 Flask-AppBuilder-4.3.2rc2/examples/related_fields/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/related_fields/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/related_fields/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2045 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/related_fields/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/related_fields/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2739 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/related_fields/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.755726 Flask-AppBuilder-4.3.2rc2/examples/simpleform/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       67 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleform/.gitignore
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      286 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleform/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.756256 Flask-AppBuilder-4.3.2rc2/examples/simpleform/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleform/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      507 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleform/app/forms.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.761099 Flask-AppBuilder-4.3.2rc2/examples/simpleform/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      125 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleform/app/templates/404.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.652718 Flask-AppBuilder-4.3.2rc2/examples/simpleform/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.652765 Flask-AppBuilder-4.3.2rc2/examples/simpleform/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.761494 Flask-AppBuilder-4.3.2rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      727 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      940 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleform/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.761851 Flask-AppBuilder-4.3.2rc2/examples/simpleform/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleform/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      662 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleform/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3697 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleform/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleform/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.762351 Flask-AppBuilder-4.3.2rc2/examples/simpleview1/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      173 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleview1/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.762673 Flask-AppBuilder-4.3.2rc2/examples/simpleview1/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleview1/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      601 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleview1/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.767684 Flask-AppBuilder-4.3.2rc2/examples/simpleview1/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleview1/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleview1/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleview1/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleview1/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.768043 Flask-AppBuilder-4.3.2rc2/examples/simpleview2/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.768402 Flask-AppBuilder-4.3.2rc2/examples/simpleview2/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      381 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleview2/app/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.768582 Flask-AppBuilder-4.3.2rc2/examples/simpleview2/app/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      108 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleview2/app/templates/method3.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1198 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleview2/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.768999 Flask-AppBuilder-4.3.2rc2/examples/simpleview2/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleview2/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        1 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleview2/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleview2/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/simpleview2/run.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.770660 Flask-AppBuilder-4.3.2rc2/examples/user_registration/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   201246 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/user_registration/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      267 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/user_registration/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.778162 Flask-AppBuilder-4.3.2rc2/examples/user_registration/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/user_registration/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1639 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/user_registration/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.653635 Flask-AppBuilder-4.3.2rc2/examples/user_registration/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.653683 Flask-AppBuilder-4.3.2rc2/examples/user_registration/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.778538 Flask-AppBuilder-4.3.2rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3981 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/user_registration/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.779075 Flask-AppBuilder-4.3.2rc2/examples/user_registration/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/user_registration/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/user_registration/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/user_registration/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/user_registration/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/user_registration/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1490 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/user_registration/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.780181 Flask-AppBuilder-4.3.2rc2/examples/widgets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   228852 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/widgets/NAMES.DIC
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      229 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/widgets/README.rst
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.780630 Flask-AppBuilder-4.3.2rc2/examples/widgets/app/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      357 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/widgets/app/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1392 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/widgets/app/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.654026 Flask-AppBuilder-4.3.2rc2/examples/widgets/app/translations/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.654092 Flask-AppBuilder-4.3.2rc2/examples/widgets/app/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.780944 Flask-AppBuilder-4.3.2rc2/examples/widgets/app/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      516 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4839 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/widgets/app/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.781498 Flask-AppBuilder-4.3.2rc2/examples/widgets/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       64 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/widgets/babel/babel.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      702 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/widgets/babel/messages.pot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14858 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/widgets/babel/messages.pot~
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1862 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/widgets/config.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       68 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/widgets/run.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1491 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/examples/widgets/testdata.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.799193 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      737 2023-05-22 10:16:39.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1970 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/_compat.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1233 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/actions.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.805164 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/api/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    76068 2023-02-23 14:18:46.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/api/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9338 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/api/convert.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3368 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/api/manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4782 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/api/schemas.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.805777 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/babel/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/babel/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2311 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/babel/manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      506 2023-05-19 13:25:49.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/babel/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26094 2023-05-19 14:36:03.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      346 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/basemanager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    48877 2023-05-08 11:18:50.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/baseviews.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.811135 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/charts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/charts/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1355 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/charts/jsontools.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17665 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/charts/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/charts/widgets.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14981 2023-05-05 08:39:47.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/cli.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14159 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/console.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8459 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/const.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1138 2022-09-30 13:30:31.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/exceptions.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8785 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/fields.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5984 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/fieldwidgets.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8534 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/filemanager.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)     6206 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11138 2023-02-15 14:55:26.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3131 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/hooks.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7648 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/menu.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      290 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/messages.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.812397 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9580 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      846 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/decorators.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10375 2022-12-22 10:35:46.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/filters.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.813066 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/generic/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    13059 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/generic/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2649 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/generic/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2253 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/generic/interface.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10979 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/group.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2633 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/mixins.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.813738 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/mongoengine/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1765 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/mongoengine/fields.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4184 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/mongoengine/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10027 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/mongoengine/interface.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.814648 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/sqla/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4145 2022-10-27 13:02:57.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/sqla/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11046 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/sqla/filters.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    39175 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/sqla/interface.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.822167 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5220 2023-05-08 09:55:27.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10693 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/decorators.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4162 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/forms.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    77461 2023-04-20 12:25:04.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/manager.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.822834 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/mongoengine/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15641 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/mongoengine/manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3219 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/mongoengine/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10650 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/registerviews.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1359 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/schemas.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.823722 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.823986 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      435 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.825465 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/permission/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       45 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/permission/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      624 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/permission/api.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.826017 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       53 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      647 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.826723 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/role/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/role/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5053 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/role/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      359 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/role/schema.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.827417 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/user/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       39 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/user/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6695 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/user/api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2176 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/user/schema.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1100 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/user/validator.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.827739 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/view_menu/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       43 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/view_menu/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      569 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/view_menu/api.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)    27043 2022-11-09 14:23:15.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/manager.py
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)     5260 2022-10-27 13:02:57.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/models.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/utils.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    25771 2023-03-16 10:28:12.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/views.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.657006 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.657856 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.828153 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      573 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/ab.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121457 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/bootstrap.min.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.828843 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/flags/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10274 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/flags/flags16.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.830863 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/fontawesome/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18600 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    80761 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      586 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      578 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1760 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    27593 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.853716 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   105250 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/amelia.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   120090 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/cerulean.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   119768 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/cosmo.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   119799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/cyborg.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121625 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/darkly.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121354 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/flatly.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   118666 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/journal.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   124431 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/lumen.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   132318 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/paper.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   118678 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/readable.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   118965 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/sandstone.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   120186 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/simplex.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   129014 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/slate.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   125030 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/solar.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/spacelab.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   120731 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/superhero.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   117016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/united.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   121865 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/yeti.css
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.854148 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/datepicker/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26667 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.855436 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/fonts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20127 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   108738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    45404 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    23424 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18028 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.861555 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2483 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/aol.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/fab.png
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.861733 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/flags/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    63284 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/flags/flags16.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1595 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/flickr.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8777 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    12799 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2558 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/google.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2882 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/myopenid.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2842 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/yahoo.png
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.864526 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3176 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/ab.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4228 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/ab_actions.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4834 2023-05-12 13:46:20.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/ab_filters.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1526 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    39680 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/bootstrap.min.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   117065 2023-01-10 15:35:16.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/fontawesome.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    46151 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/google_charts.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    89501 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/jquery-latest.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    27347 2023-01-10 15:34:59.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/v4-shims.min.js
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.869746 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/select2/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16792 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1849 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/select2/select2-spinner.gif
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    17358 2022-12-22 10:31:26.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/select2/select2.css
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    79212 2022-12-22 10:31:26.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/select2/select2.js
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      613 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/select2/select2.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      845 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/select2/select2x2.png
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.883049 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   186124 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   107656 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    62320 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    25236 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   397420 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   150516 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10140 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4568 2023-01-20 08:53:27.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.woff2
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.657974 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.894208 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/_formhelpers.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       28 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/base.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      874 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/baselayout.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4499 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/baselib.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      486 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/flash.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      143 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/footer.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.894704 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      444 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/alert.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.895273 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/charts/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      778 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/charts/chart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      890 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      717 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/confirm.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    13876 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/lib.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.896616 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      271 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/add.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1147 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/edit.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      779 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      653 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      496 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      517 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      417 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/search.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1173 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/show.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      750 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.905168 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/security/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      216 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/security/activation.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2949 2023-01-10 15:41:47.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/security/login_db.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1996 2022-10-27 13:03:01.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1396 2023-02-15 14:55:26.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/security/login_oid.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      230 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/security/register_mail.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1057 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      754 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/security/resetpassword.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.910487 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1091 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2908 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/chart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2541 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2016 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/form.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1382 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1326 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1328 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      247 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/group_form_list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2745 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1331 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2038 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1317 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2843 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      572 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1167 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1559 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.910798 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3249 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2132 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1080 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/search.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1738 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/show.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1833 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1544 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      145 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2773 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/init.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1299 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/navbar.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1264 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/navbar_menu.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1581 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/navbar_right.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.910956 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/swagger/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      764 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/swagger/swagger.html
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.920771 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.921337 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/A_fixture/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/A_fixture/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.921815 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/A_fixture/__pycache__/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      184 2022-06-17 10:46:19.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/A_fixture/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1882 2023-02-23 14:02:46.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/A_fixture/__pycache__/test_0_fixture.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      370 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/A_fixture/addon_manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1372 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/A_fixture/test_0_fixture.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.933701 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      174 2022-06-17 10:46:19.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     5453 2022-07-29 12:58:36.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      601 2023-03-16 10:39:04.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/config_api.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      993 2023-05-08 12:37:37.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/config_oauth.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      629 2023-05-03 11:58:50.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/config_security.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      443 2023-02-23 14:03:19.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/const.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    81512 2022-12-22 12:24:31.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/test_api.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7970 2023-05-03 12:02:06.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/test_fab_cli.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    52431 2023-05-08 12:13:02.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/test_mvc.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4712 2023-05-08 12:38:18.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/test_mvc_oauth.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   229376 2023-05-19 13:22:19.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/app.db
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4453 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      463 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/config_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1029 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/config_oauth.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      479 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/config_security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      515 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/config_security_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      250 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/const.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.933969 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/data/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7636 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/data/roles.json
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.934327 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/mongoengine/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/mongoengine/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1006 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/mongoengine/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.936390 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.937655 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/__pycache__/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      183 2023-02-23 14:04:47.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19332 2023-05-08 10:31:28.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/__pycache__/test_auth_ldap.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    12669 2023-05-19 13:54:28.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/__pycache__/test_mvc_security.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3436 2023-02-23 14:57:17.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/__pycache__/test_rate_limiter.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    34243 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/test_auth_ldap.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    14028 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/test_auth_oauth.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2434 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/test_base_security_manager.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    18130 2023-05-22 07:41:54.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/test_mvc_security.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1715 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/test_password_complexity.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2962 2023-02-23 15:20:20.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/test_rate_limiter.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.938050 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/sqla/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/sqla/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.938542 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/sqla/__pycache__/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      179 2022-06-17 10:46:19.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/sqla/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10026 2022-12-22 12:24:31.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/sqla/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10276 2022-12-21 14:37:56.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/sqla/models.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.938813 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/templates/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)       29 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/templates/custom_index.html
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1335 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_addon.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   118599 2022-12-21 14:37:56.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1245 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_custom_indexview.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8776 2023-05-05 08:39:47.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_fab_cli.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6503 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_menu.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    24066 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_mongoengine.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    68524 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_mvc.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4465 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_mvc_oauth.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    44396 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_security_api.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     6056 2022-11-09 14:23:15.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_security_permissions.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      670 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_sqlalchemy.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2540 2022-08-17 09:07:58.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_urltools.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.939029 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/__init__.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.664753 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/de/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.944011 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/de/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9681 2022-09-30 09:43:30.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    26578 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.665699 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/el/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.946722 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/el/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    11017 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    22936 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.666786 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/es/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.947053 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/es/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8468 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20079 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.667783 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/fr/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.947379 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8504 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20065 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.668829 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/it/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.947718 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/it/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9121 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    24545 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.669875 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ja_JP/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.948324 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9412 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20790 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.671024 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ko/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.948660 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ko/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9513 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    39930 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.671983 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/nl/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.948995 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8252 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19648 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.672918 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pl/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.951600 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8136 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20115 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.673941 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pt/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.952138 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pt/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8441 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20002 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20509 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.674889 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pt_BR/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.952526 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     8336 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19734 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.675802 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ru/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.952896 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10674 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    22035 2023-03-13 10:27:18.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.676731 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/sl/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.953473 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/sl/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     9682 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    20841 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.677624 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/zh/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.953810 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/zh/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7528 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19095 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:56.678536 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/zh_HK/
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.954158 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7493 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    19104 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     7576 2022-09-05 09:07:43.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/upload.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3226 2022-08-17 09:07:58.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/urltools.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.954683 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/utils/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)        0 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/utils/__init__.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2284 2022-07-27 09:49:08.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/utils/base.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      734 2023-02-23 12:15:32.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/utils/limit.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     3360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/validators.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    31361 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/views.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     4997 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/flask_appbuilder/widgets.py
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.966472 Flask-AppBuilder-4.3.2rc2/images/
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   190476 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/ListThumbnail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    63609 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    33854 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/chart_time1.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    41838 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/chart_time2.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    65563 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/charts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   275455 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/contact_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    52500 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/contacts.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    32505 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/direct_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2591 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/fab.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   144592 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/group_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    35236 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/grouped_chart.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    16975 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/groups.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   173978 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/images_list.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    13590 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/list_cascade.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    10792 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/list_cascade_block.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    51248 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/list_compact_inline.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    70360 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/list_master_detail.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15868 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/login.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    86223 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/login_db.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    84309 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/login_oauth.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    31562 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/login_oid.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)   417827 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/security.png
+-rw-r--r--   0 dpgaspar   (501) staff       (20)    15977 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/images/simpleview2.png
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      181 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/release.sh
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      218 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.2rc2/requirements-dev.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      157 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.2rc2/requirements-extra.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2967 2023-05-09 12:52:54.000000 Flask-AppBuilder-4.3.2rc2/requirements.txt
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2320 2023-05-03 08:19:59.000000 Flask-AppBuilder-4.3.2rc2/rtd_requirements.txt
+drwxr-xr-x   0 dpgaspar   (501) staff       (20)        0 2023-05-22 10:31:57.969437 Flask-AppBuilder-4.3.2rc2/scripts/
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      217 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/scripts/babel_extract.sh
+-rwxr-xr-x   0 dpgaspar   (501) staff       (20)      130 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/scripts/babel_init.sh
+-rw-r--r--   0 dpgaspar   (501) staff       (20)      755 2023-05-22 10:31:57.970183 Flask-AppBuilder-4.3.2rc2/setup.cfg
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     2827 2023-04-20 12:20:38.000000 Flask-AppBuilder-4.3.2rc2/setup.py
+-rw-r--r--   0 dpgaspar   (501) staff       (20)     1766 2022-05-07 22:20:23.000000 Flask-AppBuilder-4.3.2rc2/tox.ini
```

### Comparing `Flask-AppBuilder-4.3.2rc1/.github/ISSUE_TEMPLATE.md` & `Flask-AppBuilder-4.3.2rc2/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/.github/PULL_REQUEST_TEMPLATE.md` & `Flask-AppBuilder-4.3.2rc2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/.github/stale.yml` & `Flask-AppBuilder-4.3.2rc2/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/.github/workflows/ci.yml` & `Flask-AppBuilder-4.3.2rc2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/.github/workflows/ptlint.yml` & `Flask-AppBuilder-4.3.2rc2/.github/workflows/ptlint.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/CHANGELOG.rst` & `Flask-AppBuilder-4.3.2rc2/CHANGELOG.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Flask-AppBuilder ChangeLog
 ==========================
 
 Improvements and Bug fixes on 4.3.2
 -----------------------------------
 
+- fix: CRUD MVC log message (#2045) [Daniel Vaz Gaspar]
 - fix: deprecated method for getting value on select2 (#2039) [Viacheslav]
 - chore: bump Flask and werkzeug (#2034) [Daniel Vaz Gaspar]
 - ci: improve codeql configuration  (#2032) [Daniel Vaz Gaspar]
 - ci: add codeQL analysis (#2031) [Daniel Vaz Gaspar]
 - fix: cli create app ask for initial secret key (#2029) [Daniel Vaz Gaspar]
 - fix: using base_filters with FilterEqualFunction not working for relation fields (#2011) [ThomasP0815]
 - ci: bump ubuntu version, remove mockldap (#2013) [Daniel Vaz Gaspar]
```

### Comparing `Flask-AppBuilder-4.3.2rc1/CONTRIBUTING.rst` & `Flask-AppBuilder-4.3.2rc2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/Flask_AppBuilder.egg-info/PKG-INFO` & `Flask-AppBuilder-4.3.2rc2/Flask_AppBuilder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-AppBuilder
-Version: 4.3.2rc1
+Version: 4.3.2rc2
 Summary: Simple and rapid application development framework, built on top of Flask. includes detailed security, auto CRUD generation for your models, google charts and much more.
 Home-page: https://github.com/dpgaspar/flask-appbuilder/
 Author: Daniel Vaz Gaspar
 Author-email: danielvazgaspar@gmail.com
 License: BSD
 Description: Flask App Builder
         =================
```

### Comparing `Flask-AppBuilder-4.3.2rc1/Flask_AppBuilder.egg-info/SOURCES.txt` & `Flask-AppBuilder-4.3.2rc2/Flask_AppBuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/Flask_AppBuilder.egg-info/requires.txt` & `Flask-AppBuilder-4.3.2rc2/Flask_AppBuilder.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/LICENSE` & `Flask-AppBuilder-4.3.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/PKG-INFO` & `Flask-AppBuilder-4.3.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-AppBuilder
-Version: 4.3.2rc1
+Version: 4.3.2rc2
 Summary: Simple and rapid application development framework, built on top of Flask. includes detailed security, auto CRUD generation for your models, google charts and much more.
 Home-page: https://github.com/dpgaspar/flask-appbuilder/
 Author: Daniel Vaz Gaspar
 Author-email: danielvazgaspar@gmail.com
 License: BSD
 Description: Flask App Builder
         =================
```

### Comparing `Flask-AppBuilder-4.3.2rc1/README.rst` & `Flask-AppBuilder-4.3.2rc2/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/bin/config.py` & `Flask-AppBuilder-4.3.2rc2/bin/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/bin/db_migrate.py` & `Flask-AppBuilder-4.3.2rc2/bin/db_migrate.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/bin/hash_db_password.py` & `Flask-AppBuilder-4.3.2rc2/bin/hash_db_password.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/bin/migrate_db_0.7.py` & `Flask-AppBuilder-4.3.2rc2/bin/migrate_db_0.7.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/bin/migrate_db_1.3.py` & `Flask-AppBuilder-4.3.2rc2/bin/migrate_db_1.3.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/bin/sqlite_upgrade_1.3.sql` & `Flask-AppBuilder-4.3.2rc2/bin/sqlite_upgrade_1.3.sql`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docker-compose.yml` & `Flask-AppBuilder-4.3.2rc2/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/Makefile` & `Flask-AppBuilder-4.3.2rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/_static/Flask-AppBuilder.png` & `Flask-AppBuilder-4.3.2rc2/docs/_static/Flask-AppBuilder.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/_templates/layout.html` & `Flask-AppBuilder-4.3.2rc2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/_themes/LICENSE` & `Flask-AppBuilder-4.3.2rc2/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/_themes/README` & `Flask-AppBuilder-4.3.2rc2/docs/_themes/README`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/_themes/flask/layout.html` & `Flask-AppBuilder-4.3.2rc2/docs/_themes/flask/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/_themes/flask/relations.html` & `Flask-AppBuilder-4.3.2rc2/docs/_themes/flask/relations.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/_themes/flask/static/Flask-AppBuilder.png` & `Flask-AppBuilder-4.3.2rc2/docs/_themes/flask/static/Flask-AppBuilder.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/_themes/flask/static/flasky.css_t` & `Flask-AppBuilder-4.3.2rc2/docs/_themes/flask/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/_themes/flask_small/layout.html` & `Flask-AppBuilder-4.3.2rc2/docs/_themes/flask_small/layout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/_themes/flask_small/static/flasky.css_t` & `Flask-AppBuilder-4.3.2rc2/docs/_themes/flask_small/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/_themes/flask_theme_support.py` & `Flask-AppBuilder-4.3.2rc2/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/actions.rst` & `Flask-AppBuilder-4.3.2rc2/docs/actions.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/addons.rst` & `Flask-AppBuilder-4.3.2rc2/docs/addons.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/advanced.rst` & `Flask-AppBuilder-4.3.2rc2/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/api.rst` & `Flask-AppBuilder-4.3.2rc2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/cli.rst` & `Flask-AppBuilder-4.3.2rc2/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/conf.py` & `Flask-AppBuilder-4.3.2rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/config.rst` & `Flask-AppBuilder-4.3.2rc2/docs/config.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/customizing.rst` & `Flask-AppBuilder-4.3.2rc2/docs/customizing.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/diagrams.rst` & `Flask-AppBuilder-4.3.2rc2/docs/diagrams.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/generic_datasource.rst` & `Flask-AppBuilder-4.3.2rc2/docs/generic_datasource.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/i18n.rst` & `Flask-AppBuilder-4.3.2rc2/docs/i18n.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/ListThumbnail.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/ListThumbnail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/chart.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/chart_time1.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/chart_time1.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/chart_time2.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/chart_time2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/charts.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/charts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/contact_list.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/contact_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/contacts.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/contacts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/direct_chart.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/direct_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/fab.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/fab.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/group_list.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/group_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/grouped_chart.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/grouped_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/groups.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/groups.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/images_list.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/images_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/list_cascade.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/list_cascade.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/list_cascade_block.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/list_cascade_block.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/list_compact_inline.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/list_compact_inline.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/list_master_detail.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/list_master_detail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/login.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/login.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/login_db.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/login_db.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/login_oid.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/login_oid.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/oauth_login.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/oauth_login.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/oauth_login_one_provider.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/oauth_login_one_provider.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/security.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/security.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/simpleview2.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/simpleview2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/swagger001.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/swagger001.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/images/swagger002.png` & `Flask-AppBuilder-4.3.2rc2/docs/images/swagger002.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/index.rst` & `Flask-AppBuilder-4.3.2rc2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/installation.rst` & `Flask-AppBuilder-4.3.2rc2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/intro.rst` & `Flask-AppBuilder-4.3.2rc2/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/make.bat` & `Flask-AppBuilder-4.3.2rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/multipledbs.rst` & `Flask-AppBuilder-4.3.2rc2/docs/multipledbs.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/quickcharts.rst` & `Flask-AppBuilder-4.3.2rc2/docs/quickcharts.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/quickfiles.rst` & `Flask-AppBuilder-4.3.2rc2/docs/quickfiles.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/quickhowto.rst` & `Flask-AppBuilder-4.3.2rc2/docs/quickhowto.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/quickhowto_mongo.rst` & `Flask-AppBuilder-4.3.2rc2/docs/quickhowto_mongo.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/quickminimal.rst` & `Flask-AppBuilder-4.3.2rc2/docs/quickminimal.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/relations.rst` & `Flask-AppBuilder-4.3.2rc2/docs/relations.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/rest_api.rst` & `Flask-AppBuilder-4.3.2rc2/docs/rest_api.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/security.rst` & `Flask-AppBuilder-4.3.2rc2/docs/security.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/templates.rst` & `Flask-AppBuilder-4.3.2rc2/docs/templates.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/user_registration.rst` & `Flask-AppBuilder-4.3.2rc2/docs/user_registration.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/versionmigration.rst` & `Flask-AppBuilder-4.3.2rc2/docs/versionmigration.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/docs/views.rst` & `Flask-AppBuilder-4.3.2rc2/docs/views.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/README.rst` & `Flask-AppBuilder-4.3.2rc2/examples/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/base_api/app/api.py` & `Flask-AppBuilder-4.3.2rc2/examples/base_api/app/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/base_api/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/base_api/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/basefilter/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/basefilter/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/basefilter/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/basefilter/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/basefilter/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/basefilter/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/basefilter/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/basefilter/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/basefilter/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/basefilter/babel/messages.pot~` & `Flask-AppBuilder-4.3.2rc2/examples/basefilter/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/basefilter/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/basefilter/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/basefilter/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/basefilter/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/composite_keys/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/composite_keys/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/composite_keys/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/composite_keys/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/composite_keys/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/composite_keys/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/composite_keys/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/composite_keys/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/app/api.py` & `Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/app/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/crud_rest_api/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/crud_rest_api/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/dash/app/Dashboard/Dash_App1.py` & `Flask-AppBuilder-4.3.2rc2/examples/dash/app/Dashboard/Dash_App1.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/dash/app/Dashboard/Dash_App2.py` & `Flask-AppBuilder-4.3.2rc2/examples/dash/app/Dashboard/Dash_App2.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/dash/app/Dashboard/Dash_fun.py` & `Flask-AppBuilder-4.3.2rc2/examples/dash/app/Dashboard/Dash_fun.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/dash/app/templates/dash.html` & `Flask-AppBuilder-4.3.2rc2/examples/dash/app/templates/dash.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/dash/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/dash/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/dash/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/dash/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/employees/app/__init__.py` & `Flask-AppBuilder-4.3.2rc2/examples/employees/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/employees/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/employees/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/employees/app/security.py` & `Flask-AppBuilder-4.3.2rc2/examples/employees/app/security.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/employees/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/employees/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/employees/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/employees/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/enums/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/enums/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/enums/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/enums/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/enums/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/enums/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/enums/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/enums/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/enums/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/enums/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/enums/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/enums/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/enums/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/enums/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/README.rst` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/__init__.py` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/sec_forms.py` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/sec_forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/sec_views.py` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/sec_views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/babel/messages.pot~` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/README.rst` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/sec_forms.py` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/sec_forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/sec_views.py` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/sec_views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/extendsecurity2/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/extendsecurity2/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/factoryapp/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/factoryapp/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/factoryapp/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/factoryapp/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/factoryapp/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/factoryapp/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/factoryapp/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/factoryapp/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/factoryapp/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/factoryapp/babel/messages.pot~` & `Flask-AppBuilder-4.3.2rc2/examples/factoryapp/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/factoryapp/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/factoryapp/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/factoryapp/config2.py` & `Flask-AppBuilder-4.3.2rc2/examples/factoryapp/config2.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/factoryapp/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/factoryapp/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/issue_789/README.rst` & `Flask-AppBuilder-4.3.2rc2/examples/issue_789/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/issue_789/app.py` & `Flask-AppBuilder-4.3.2rc2/examples/issue_789/app.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/masterdetail/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/masterdetail/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/masterdetail/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/masterdetail/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/masterdetail/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/masterdetail/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/masterdetail/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/masterdetail/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/masterdetail/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/masterdetail/babel/messages.pot~` & `Flask-AppBuilder-4.3.2rc2/examples/masterdetail/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/masterdetail/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/masterdetail/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/masterdetail/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/masterdetail/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/__init__.py` & `Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/mysecurity.py` & `Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/mysecurity.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongo_extendedsecurity/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/mongo_extendedsecurity/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoengine/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/mongoengine/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoengine/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/mongoengine/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/mongoengine/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoengine/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/mongoengine/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoengine/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/mongoengine/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoengine/babel/messages.pot~` & `Flask-AppBuilder-4.3.2rc2/examples/mongoengine/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoengine/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/mongoengine/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoengine/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/mongoengine/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoimages/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/mongoimages/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoimages/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/mongoimages/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/mongoimages/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoimages/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/mongoimages/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoimages/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/mongoimages/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoimages/babel/messages.pot~` & `Flask-AppBuilder-4.3.2rc2/examples/mongoimages/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoimages/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/mongoimages/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/mongoimages/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/mongoimages/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/oauth/README.rst` & `Flask-AppBuilder-4.3.2rc2/examples/oauth/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/oauth/app/__init__.py` & `Flask-AppBuilder-4.3.2rc2/examples/oauth/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/oauth/app/security.py` & `Flask-AppBuilder-4.3.2rc2/examples/oauth/app/security.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/oauth/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/oauth/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/oauth/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/oauth/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/productsale/app/__init__.py` & `Flask-AppBuilder-4.3.2rc2/examples/productsale/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/productsale/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/productsale/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/productsale/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/productsale/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/productsale/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/productsale/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/productsale/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/productsale/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/productsale/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/__init__.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickactions/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickactions/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickactions/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickactions/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts/app/data.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts/app/data.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts/babel/messages.pot~` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/babel/messages.pot~` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/bdist.linux-i686/egg/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/lib/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/lib/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/build/lib/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/build/lib/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickcharts2/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickcharts2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~` & `Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/es/LC_MESSAGES/messages.po~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~` & `Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/translations/pt/LC_MESSAGES/messages.po~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickfiles/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickfiles/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickfiles/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/quickfiles/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickfiles/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickfiles/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto/babel/messages.pot~` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/__init__.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/forms.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/sec_views.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/sec_views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/abModalOkCancel.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/abModelSearch.html` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/abModelSearch.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/abModelTable.html` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/abModelTable.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/angularAssets/abPagination.html` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/angularAssets/abPagination.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/css/clean-blog.min.css` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/css/clean-blog.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/css/scrolling-nav.css` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/css/scrolling-nav.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/img/brand.jpg` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/img/brand.jpg`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/img/loading.gif` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/Controllers/alertsCtrl.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/Controllers/tableCtrl.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/Directives/bigDirectives.js` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/Directives/bigDirectives.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/Directives/btnDirectives.js` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/Directives/btnDirectives.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/Services/apiService.js` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/Services/apiService.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/angular.min.js` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/angular.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/app.js` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/app.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/clean-blog.min.js` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/clean-blog.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/static/js/scrolling-nav.js` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/static/js/scrolling-nav.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/list_angulajs.html` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/list_angulajs.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/list_json.html` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/list_json.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/templates/widgets/list.html` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/templates/widgets/list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/babel/messages.pot~` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto2/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto2/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/.coverage` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/.coverage`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/app/__init__.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/babel/messages.pot~` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/migrate_db_0.7.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/migrate_db_0.7.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickhowto3/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickhowto3/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/__init__.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickimages/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickimages/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickimages/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickimages/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quickmigrate/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/quickmigrate/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/.idea/misc.xml` & `Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/.idea/misc.xml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/.idea/workspace.xml` & `Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicksqlviews/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/quicksqlviews/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/static/css/landing-page.css` & `Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/static/css/landing-page.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/templates/mybase.html` & `Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/templates/mybase.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/babel/messages.pot~` & `Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/quicktemplates/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/quicktemplates/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/api.py` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/package-lock.json` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/package.json` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/package.json`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/package.json.react-original` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/package.json.react-original`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/public/favicon.ico` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/src/api/Api.js` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/src/api/Api.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/src/components/CRUDButtons.js` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/src/components/CRUDButtons.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/src/components/Forms.js` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/src/components/Forms.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/static/src/components/Table.js` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/static/src/components/Table.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/templates/base.html` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/react-rest-api/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/react-rest-api/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/related_fields/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/related_fields/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/related_fields/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/related_fields/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/related_fields/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/related_fields/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/related_fields/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/related_fields/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/related_fields/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/related_fields/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/related_fields/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/related_fields/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/related_fields/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/simpleform/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/simpleform/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/simpleform/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/simpleform/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/simpleform/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/simpleform/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/simpleform/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/simpleview1/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/simpleview1/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/simpleview1/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/simpleview1/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/simpleview2/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/simpleview2/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/simpleview2/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/simpleview2/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/user_registration/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/user_registration/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/user_registration/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/user_registration/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/user_registration/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/user_registration/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/user_registration/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/user_registration/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/user_registration/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/user_registration/babel/messages.pot~` & `Flask-AppBuilder-4.3.2rc2/examples/user_registration/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/user_registration/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/user_registration/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/user_registration/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/user_registration/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/widgets/NAMES.DIC` & `Flask-AppBuilder-4.3.2rc2/examples/widgets/NAMES.DIC`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/widgets/app/models.py` & `Flask-AppBuilder-4.3.2rc2/examples/widgets/app/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/examples/widgets/app/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/widgets/app/views.py` & `Flask-AppBuilder-4.3.2rc2/examples/widgets/app/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/widgets/babel/messages.pot` & `Flask-AppBuilder-4.3.2rc2/examples/widgets/babel/messages.pot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/widgets/babel/messages.pot~` & `Flask-AppBuilder-4.3.2rc2/examples/widgets/babel/messages.pot~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/widgets/config.py` & `Flask-AppBuilder-4.3.2rc2/examples/widgets/config.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/examples/widgets/testdata.py` & `Flask-AppBuilder-4.3.2rc2/examples/widgets/testdata.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/__init__.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __author__ = "Daniel Vaz Gaspar"
-__version__ = "4.3.2rc1"
+__version__ = "4.3.2rc2"
 
 from .actions import action  # noqa: F401
 from .api import ModelRestApi  # noqa: F401
 from .base import AppBuilder  # noqa: F401
 from .baseviews import BaseView, expose  # noqa: F401
 from .charts.views import DirectByChartView, GroupByChartView  # noqa: F401
 from .models.group import aggregate_avg, aggregate_count, aggregate_sum  # noqa: F401
```

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/_compat.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/_compat.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/actions.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/actions.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/api/__init__.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/api/convert.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/api/convert.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/api/manager.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/api/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/api/schemas.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/api/schemas.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/babel/manager.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/babel/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 
 from flask import has_request_context, request, session
+from flask_appbuilder.babel.views import LocaleView
+from flask_appbuilder.basemanager import BaseManager
 from flask_babel import Babel
 
-from .views import LocaleView
-from ..basemanager import BaseManager
-
 
 class BabelManager(BaseManager):
 
     babel = None
     locale_view = None
 
     def __init__(self, appbuilder):
```

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/base.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/baseviews.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/baseviews.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/charts/jsontools.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/charts/jsontools.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/charts/views.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/charts/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/cli.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/cli.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/console.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/console.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/const.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/const.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/exceptions.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/exceptions.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/fields.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/fields.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/fieldwidgets.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/fieldwidgets.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/filemanager.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/filemanager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/filters.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/forms.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/hooks.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/hooks.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/menu.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/menu.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/base.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         "Integrity error, probably unique constraint"
     )
     edit_integrity_error_message = lazy_gettext(
         "Integrity error, probably unique constraint"
     )
     general_error_message = lazy_gettext("General Error")
 
+    database_error_message = lazy_gettext("Database Error")
+
     """ Tuple with message and text with severity type ex: ("Added Row", "info") """
     message = ()
 
     def __init__(self, obj: Type[Any]):
         self.obj = obj
 
     def __getattr__(self, name: str) -> Any:
@@ -99,49 +101,49 @@
         )
 
     def get_values_item(self, item, show_columns):
         return [self._get_attr_value(item, col) for col in show_columns]
 
     def _get_values(self, lst, list_columns):
         """
-            Get Values: formats values for list template.
-            returns [{'col_name':'col_value',....},{'col_name':'col_value',....}]
+        Get Values: formats values for list template.
+        returns [{'col_name':'col_value',....},{'col_name':'col_value',....}]
 
-            :param lst:
-                The list of item objects from query
-            :param list_columns:
-                The list of columns to include
+        :param lst:
+            The list of item objects from query
+        :param list_columns:
+            The list of columns to include
         """
         retlst = []
         for item in lst:
             retdict = {}
             for col in list_columns:
                 retdict[col] = self._get_attr_value(item, col)
             retlst.append(retdict)
         return retlst
 
     def get_values(self, lst, list_columns):
         """
-            Get Values: formats values for list template.
-            returns [{'col_name':'col_value',....},{'col_name':'col_value',....}]
+        Get Values: formats values for list template.
+        returns [{'col_name':'col_value',....},{'col_name':'col_value',....}]
 
-            :param lst:
-                The list of item objects from query
-            :param list_columns:
-                The list of columns to include
+        :param lst:
+            The list of item objects from query
+        :param list_columns:
+            The list of columns to include
         """
         for item in lst:
             retdict = {}
             for col in list_columns:
                 retdict[col] = self._get_attr_value(item, col)
             yield retdict
 
     def get_values_json(self, lst, list_columns):
         """
-            Converts list of objects from query to JSON
+        Converts list of objects from query to JSON
         """
         result = []
         for item in self.get_values(lst, list_columns):
             for key, value in list(item.items()):
                 if isinstance(value, datetime.datetime) or isinstance(
                     value, datetime.date
                 ):
@@ -260,101 +262,101 @@
     -----------------------------------------
            FUNCTIONS FOR CRUD OPERATIONS
     -----------------------------------------
     """
 
     def add(self, item):
         """
-            Adds object
+        Adds object
         """
         raise NotImplementedError
 
     def edit(self, item):
         """
-            Edit (change) object
+        Edit (change) object
         """
         raise NotImplementedError
 
     def delete(self, item):
         """
-            Deletes object
+        Deletes object
         """
         raise NotImplementedError
 
     def get_col_default(self, col_name):
         pass
 
     def get_keys(self, lst):
         """
-            return a list of pk values from object list
+        return a list of pk values from object list
         """
         pk_name = self.get_pk_name()
         if self.is_pk_composite():
             return [[getattr(item, pk) for pk in pk_name] for item in lst]
         else:
             return [getattr(item, pk_name) for item in lst]
 
     def get_pk_name(self):
         """
-            Returns the primary key name
+        Returns the primary key name
         """
         raise NotImplementedError
 
     def get_pk_value(self, item):
         pk_name = self.get_pk_name()
         if self.is_pk_composite():
             return [getattr(item, pk) for pk in pk_name]
         else:
             return getattr(item, pk_name)
 
     def get(self, pk, filter=None):
         """
-            return the record from key, you can optionally pass filters
-            if pk exits on the db but filters exclude it it will return none.
+        return the record from key, you can optionally pass filters
+        if pk exits on the db but filters exclude it it will return none.
         """
         pass
 
     def get_related_model(self, prop):
         raise NotImplementedError
 
     def get_related_interface(self, col_name):
         """
-            Returns a BaseInterface for the related model
-            of column name.
+        Returns a BaseInterface for the related model
+        of column name.
 
-            :param col_name: Column name with relation
-            :return: BaseInterface
+        :param col_name: Column name with relation
+        :return: BaseInterface
         """
         raise NotImplementedError
 
     def get_related_obj(self, col_name, value):
         raise NotImplementedError
 
     def get_related_fk(self, model):
         raise NotImplementedError
 
     def get_columns_list(self):
         """
-            Returns a list of all the columns names
+        Returns a list of all the columns names
         """
         return []
 
     def get_user_columns_list(self):
         """
-            Returns a list of user viewable columns names
+        Returns a list of user viewable columns names
         """
         return self.get_columns_list()
 
     def get_search_columns_list(self):
         """
-            Returns a list of searchable columns names
+        Returns a list of searchable columns names
         """
         return []
 
     def get_order_columns_list(self, list_columns=None):
         """
-            Returns a list of order columns names
+        Returns a list of order columns names
         """
         return []
 
     def get_relation_fk(self, prop):
         pass
```

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/decorators.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/decorators.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/filters.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/generic/__init__.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/generic/filters.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/generic/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/generic/interface.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/generic/interface.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/group.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/group.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/mixins.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/mixins.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/mongoengine/fields.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/mongoengine/fields.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/mongoengine/filters.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/mongoengine/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/mongoengine/interface.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/mongoengine/interface.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/sqla/__init__.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/sqla/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/sqla/filters.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/sqla/filters.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/models/sqla/interface.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/models/sqla/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 # -*- coding: utf-8 -*-
 from contextlib import suppress
 import logging
-import sys
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 from flask_appbuilder._compat import as_unicode
 from flask_appbuilder.const import (
-    LOGMSG_ERR_DBI_ADD_GENERIC,
     LOGMSG_ERR_DBI_DEL_GENERIC,
-    LOGMSG_ERR_DBI_EDIT_GENERIC,
     LOGMSG_WAR_DBI_ADD_INTEGRITY,
     LOGMSG_WAR_DBI_DEL_INTEGRITY,
     LOGMSG_WAR_DBI_EDIT_INTEGRITY,
 )
 from flask_appbuilder.exceptions import InterfaceQueryWithoutSession
 from flask_appbuilder.filemanager import FileManager, ImageManager
 from flask_appbuilder.models.base import BaseInterface
@@ -732,19 +729,16 @@
             self.message = (as_unicode(self.add_integrity_error_message), "warning")
             log.warning(LOGMSG_WAR_DBI_ADD_INTEGRITY.format(str(e)))
             self.session.rollback()
             if raise_exception:
                 raise e
             return False
         except Exception as e:
-            self.message = (
-                as_unicode(self.general_error_message + " " + str(sys.exc_info()[0])),
-                "danger",
-            )
-            log.exception(LOGMSG_ERR_DBI_ADD_GENERIC.format(str(e)))
+            self.message = (as_unicode(self.database_error_message), "danger")
+            log.exception("Database error")
             self.session.rollback()
             if raise_exception:
                 raise e
             return False
 
     def edit(self, item: Model, raise_exception: bool = False) -> bool:
         try:
@@ -756,19 +750,16 @@
             self.message = (as_unicode(self.edit_integrity_error_message), "warning")
             log.warning(LOGMSG_WAR_DBI_EDIT_INTEGRITY.format(str(e)))
             self.session.rollback()
             if raise_exception:
                 raise e
             return False
         except Exception as e:
-            self.message = (
-                as_unicode(self.general_error_message + " " + str(sys.exc_info()[0])),
-                "danger",
-            )
-            log.exception(LOGMSG_ERR_DBI_EDIT_GENERIC.format(str(e)))
+            self.message = (as_unicode(self.database_error_message), "danger")
+            log.exception("Database error")
             self.session.rollback()
             if raise_exception:
                 raise e
             return False
 
     def delete(self, item: Model, raise_exception: bool = False) -> bool:
         try:
@@ -781,19 +772,16 @@
             self.message = (as_unicode(self.delete_integrity_error_message), "warning")
             log.warning(LOGMSG_WAR_DBI_DEL_INTEGRITY.format(str(e)))
             self.session.rollback()
             if raise_exception:
                 raise e
             return False
         except Exception as e:
-            self.message = (
-                as_unicode(self.general_error_message + " " + str(sys.exc_info()[0])),
-                "danger",
-            )
-            log.exception(LOGMSG_ERR_DBI_DEL_GENERIC.format(str(e)))
+            self.message = (as_unicode(self.database_error_message), "danger")
+            log.exception("Database error")
             self.session.rollback()
             if raise_exception:
                 raise e
             return False
 
     def delete_all(self, items: List[Model]) -> bool:
         try:
@@ -805,18 +793,15 @@
             return True
         except IntegrityError as e:
             self.message = (as_unicode(self.delete_integrity_error_message), "warning")
             log.warning(LOGMSG_WAR_DBI_DEL_INTEGRITY.format(str(e)))
             self.session.rollback()
             return False
         except Exception as e:
-            self.message = (
-                as_unicode(self.general_error_message + " " + str(sys.exc_info()[0])),
-                "danger",
-            )
+            self.message = (as_unicode(self.database_error_message), "danger")
             log.exception(LOGMSG_ERR_DBI_DEL_GENERIC.format(str(e)))
             self.session.rollback()
             return False
 
     """
     -----------------------
      FILE HANDLING METHODS
```

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/api.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/decorators.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/decorators.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/forms.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/forms.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/manager.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/mongoengine/manager.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/mongoengine/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/mongoengine/models.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/mongoengine/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/registerviews.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/registerviews.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/schemas.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/schemas.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/permission/api.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/permission/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/permission_view_menu/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/role/api.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/role/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/user/api.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/user/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/user/schema.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/user/schema.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/user/validator.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/user/validator.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/apis/view_menu/api.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/apis/view_menu/api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/manager.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/sqla/models.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/sqla/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/security/views.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/security/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/ab.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/ab.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/bootstrap.min.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/flags/flags16.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/flags/flags16.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/fontawesome/brands.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/fontawesome/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/fontawesome/regular.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/fontawesome/solid.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-font-face.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/fontawesome/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/amelia.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/amelia.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/cerulean.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/cerulean.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/cosmo.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/cosmo.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/cyborg.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/cyborg.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/darkly.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/darkly.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/flatly.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/flatly.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/journal.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/journal.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/lumen.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/lumen.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/paper.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/paper.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/readable.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/readable.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/sandstone.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/sandstone.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/simplex.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/simplex.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/slate.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/slate.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/solar.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/solar.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/spacelab.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/spacelab.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/superhero.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/superhero.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/united.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/united.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/css/themes/yeti.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/css/themes/yeti.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.js` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/datepicker/bootstrap-datepicker.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/aol.png` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/aol.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/fab.png` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/fab.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/flags/flags16.png` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/flags/flags16.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/flickr.png` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/flickr.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings-white.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/glyphicons-halflings.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/google.png` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/google.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/myopenid.png` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/myopenid.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/img/yahoo.png` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/img/yahoo.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/ab.js` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/ab.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/ab_actions.js` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/ab_actions.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/ab_filters.js` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/ab_filters.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/ab_keep_tab.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/bootstrap.min.js` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/fontawesome.js` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/fontawesome.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/google_charts.js` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/google_charts.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/jquery-latest.js` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/jquery-latest.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/js/v4-shims.min.js` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/js/v4-shims.min.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/select2/select2-bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/select2/select2-spinner.gif` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/select2/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/select2/select2.css` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/select2/select2.css`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/select2/select2.js` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/select2/select2.js`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/select2/select2.png` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/select2/select2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/select2/select2x2.png` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/select2/select2x2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.ttf` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.woff2` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.ttf` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.woff2` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.ttf` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.woff2` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.ttf` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.woff2` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/static/appbuilder/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/baselayout.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/baselayout.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/baselib.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/baselib.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/charts/chart.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/charts/chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/charts/chart_time.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/charts/jsonchart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/confirm.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/confirm.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/lib.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/lib.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/edit.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/edit.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/edit_cascade.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/left_master_detail.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/multiple_views.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/show.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/show.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/model/show_cascade.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/security/login_db.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/security/login_db.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/security/login_ldap.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/security/login_oauth.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/security/login_oid.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/security/login_oid.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/security/register_oauth.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/security/resetpassword.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/security/resetpassword.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/base_list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/chart.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/direct_chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/form.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/form.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_horizontal.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_inline.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/form_vertical.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/list.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_block.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_carousel.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_item.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_link.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_master.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/list_thumbnail.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/multiple_chart.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/list.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/roles/show.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/search.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/search.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/show.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/show.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_block.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/general/widgets/show_vertical.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/init.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/init.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/navbar.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/navbar.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/navbar_menu.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/navbar_menu.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/navbar_right.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/navbar_right.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/templates/appbuilder/swagger/swagger.html` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/templates/appbuilder/swagger/swagger.html`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/A_fixture/__pycache__/test_0_fixture.cpython-38.pyc` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/A_fixture/__pycache__/test_0_fixture.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/A_fixture/test_0_fixture.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/A_fixture/test_0_fixture.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/base.cpython-38.pyc` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/base.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/config_api.cpython-38.pyc` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/config_api.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/config_oauth.cpython-38.pyc` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/config_oauth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/config_security.cpython-38.pyc` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/config_security.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/test_api.cpython-38.pyc` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/test_api.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/test_fab_cli.cpython-38.pyc` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/test_fab_cli.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/test_mvc.cpython-38.pyc` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/test_mvc.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/__pycache__/test_mvc_oauth.cpython-38.pyc` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/__pycache__/test_mvc_oauth.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/app.db` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/app.db`

 * *Files 2% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -34,15 +34,14 @@
 INSERT INTO model1 VALUES(24,'test23',23,23.0,NULL);
 INSERT INTO model1 VALUES(25,'test24',24,24.0,NULL);
 INSERT INTO model1 VALUES(26,'test25',25,25.0,NULL);
 INSERT INTO model1 VALUES(27,'test26',26,26.0,NULL);
 INSERT INTO model1 VALUES(28,'test27',27,27.0,NULL);
 INSERT INTO model1 VALUES(29,'test28',28,28.0,NULL);
 INSERT INTO model1 VALUES(30,'test29',29,29.0,NULL);
-INSERT INTO model1 VALUES(31,'test0',0,0.0,NULL);
 CREATE TABLE model3 (
 	pk1 INTEGER NOT NULL, 
 	pk2 DATETIME NOT NULL, 
 	field_string VARCHAR(50) NOT NULL, 
 	PRIMARY KEY (pk1, pk2), 
 	UNIQUE (field_string)
 );
@@ -116,14 +115,17 @@
 INSERT INTO model_with_enums VALUES(25,'e1','e2');
 INSERT INTO model_with_enums VALUES(26,'e1','e2');
 INSERT INTO model_with_enums VALUES(27,'e1','e2');
 INSERT INTO model_with_enums VALUES(28,'e1','e2');
 INSERT INTO model_with_enums VALUES(29,'e1','e2');
 INSERT INTO model_with_enums VALUES(30,'e1','e2');
 INSERT INTO model_with_enums VALUES(31,NULL,'e1');
+INSERT INTO model_with_enums VALUES(32,NULL,'e1');
+INSERT INTO model_with_enums VALUES(33,NULL,'e1');
+INSERT INTO model_with_enums VALUES(34,NULL,'e1');
 CREATE TABLE parent (
 	id INTEGER NOT NULL, 
 	field_string VARCHAR(50) NOT NULL, 
 	PRIMARY KEY (id), 
 	UNIQUE (field_string)
 );
 INSERT INTO parent VALUES(1,'0');
@@ -270,16 +272,18 @@
 INSERT INTO ab_permission VALUES(15,'menu_access');
 INSERT INTO ab_permission VALUES(16,'copyrole');
 INSERT INTO ab_permission VALUES(17,'can_chart');
 INSERT INTO ab_permission VALUES(18,'can_test1');
 INSERT INTO ab_permission VALUES(19,'can_test2');
 INSERT INTO ab_permission VALUES(20,'can_put');
 INSERT INTO ab_permission VALUES(21,'can_post');
-INSERT INTO ab_permission VALUES(22,'can_access');
 INSERT INTO ab_permission VALUES(23,'can_write');
+INSERT INTO ab_permission VALUES(24,'can_read');
+INSERT INTO ab_permission VALUES(25,'can_access2');
+INSERT INTO ab_permission VALUES(26,'can_access');
 CREATE TABLE ab_view_menu (
 	id INTEGER NOT NULL, 
 	name VARCHAR(250) NOT NULL, 
 	PRIMARY KEY (id), 
 	UNIQUE (name)
 );
 INSERT INTO ab_view_menu VALUES(1,'.*');
@@ -318,15 +322,14 @@
 INSERT INTO ab_view_menu VALUES(34,'UserOAuthModelView');
 INSERT INTO ab_view_menu VALUES(35,'RegisterUserModelView');
 INSERT INTO ab_view_menu VALUES(36,'Model2View');
 INSERT INTO ab_view_menu VALUES(37,'Model3View');
 INSERT INTO ab_view_menu VALUES(38,'Model4View');
 INSERT INTO ab_view_menu VALUES(39,'ModelDBView');
 INSERT INTO ab_view_menu VALUES(40,'Base1Api');
-INSERT INTO ab_view_menu VALUES(41,'Model1Api');
 INSERT INTO ab_view_menu VALUES(42,'Model2ApiInvalidSearchColumns');
 INSERT INTO ab_view_menu VALUES(43,'Model1ApiSearchFilters');
 INSERT INTO ab_view_menu VALUES(44,'Model1ApiFieldsInfo');
 INSERT INTO ab_view_menu VALUES(45,'Model1FuncApi');
 INSERT INTO ab_view_menu VALUES(46,'Model1ApiExcludeCols');
 INSERT INTO ab_view_menu VALUES(47,'Model1ApiExcludeRoutes');
 INSERT INTO ab_view_menu VALUES(48,'Model1ApiOrder');
@@ -340,33 +343,41 @@
 INSERT INTO ab_view_menu VALUES(56,'ModelDottedOMParentApi');
 INSERT INTO ab_view_menu VALUES(57,'ModelMMRequiredApi');
 INSERT INTO ab_view_menu VALUES(58,'Model1CustomValidationApi');
 INSERT INTO ab_view_menu VALUES(59,'Model2Api');
 INSERT INTO ab_view_menu VALUES(60,'Model2DottedNotationApi');
 INSERT INTO ab_view_menu VALUES(61,'Model2ApiFilteredRelFields');
 INSERT INTO ab_view_menu VALUES(62,'Model2CallableColApi');
-INSERT INTO ab_view_menu VALUES(63,'api');
 INSERT INTO ab_view_menu VALUES(64,'ModelWithPropertyApi');
 INSERT INTO ab_view_menu VALUES(65,'Model1ApiIncludeRoutes');
 INSERT INTO ab_view_menu VALUES(66,'Model1BeforeRequest');
 INSERT INTO ab_view_menu VALUES(67,'ModelOOParentApi');
 INSERT INTO ab_view_menu VALUES(68,'ModelDottedOOParentApi');
 INSERT INTO ab_view_menu VALUES(69,'Model2PermOverride3');
 INSERT INTO ab_view_menu VALUES(70,'Model1ApiCustomSchema');
+INSERT INTO ab_view_menu VALUES(71,'Model2');
+INSERT INTO ab_view_menu VALUES(72,'Model1PageSizeOverride');
+INSERT INTO ab_view_menu VALUES(73,'Model4Api');
+INSERT INTO ab_view_menu VALUES(74,'Model2PermOverride2');
+INSERT INTO ab_view_menu VALUES(75,'api2');
+INSERT INTO ab_view_menu VALUES(77,'Model1PermOverride');
+INSERT INTO ab_view_menu VALUES(81,'Model1Api');
+INSERT INTO ab_view_menu VALUES(82,'api');
 CREATE TABLE ab_role (
 	id INTEGER NOT NULL, 
 	name VARCHAR(64) NOT NULL, 
 	PRIMARY KEY (id), 
 	UNIQUE (name)
 );
 INSERT INTO ab_role VALUES(1,'ReadOnly');
 INSERT INTO ab_role VALUES(2,'Admin');
 INSERT INTO ab_role VALUES(3,'Public');
 INSERT INTO ab_role VALUES(4,'FAB_ROLE1');
 INSERT INTO ab_role VALUES(5,'FAB_ROLE2');
+INSERT INTO ab_role VALUES(6,'Test');
 CREATE TABLE ab_user (
 	id INTEGER NOT NULL, 
 	first_name VARCHAR(64) NOT NULL, 
 	last_name VARCHAR(64) NOT NULL, 
 	username VARCHAR(64) NOT NULL, 
 	password VARCHAR(256), 
 	active BOOLEAN, 
@@ -380,16 +391,17 @@
 	changed_by_fk INTEGER, 
 	PRIMARY KEY (id), 
 	UNIQUE (username), 
 	UNIQUE (email), 
 	FOREIGN KEY(created_by_fk) REFERENCES ab_user (id), 
 	FOREIGN KEY(changed_by_fk) REFERENCES ab_user (id)
 );
-INSERT INTO ab_user VALUES(1,'admin','user','testadmin','pbkdf2:sha256:260000$Fw1TMa6sEbpzxOpj$749bca4eb82f2a485305987478e666fe12e689c092961a540d68dc7bd4dc93a4',1,'admin@fab.org','2022-12-22 12:24:54.136462',69,0,'2020-01-01 00:00:00.000000','2020-01-01 00:00:00.000000',NULL,NULL);
-INSERT INTO ab_user VALUES(2,'readonly','readonly','readonly','pbkdf2:sha256:260000$9xVo850WOL4NuLpF$10ea139275a6f7d4ef3feaab50fd40394613b23a1bb535881c6904001c89ec2c',1,'readonly@fab.org','2022-12-22 12:24:32.813604',1,0,'2020-01-01 00:00:00.000000','2020-01-01 00:00:00.000000',NULL,NULL);
+INSERT INTO ab_user VALUES(1,'admin','user','testadmin','pbkdf2:sha256:260000$gkfp7KKMfSUfFRKw$3d401b6755b70729e931e6a8cbc47f391aeda30dd33bed50f57da50769e78373',1,'admin@fab.org','2023-05-19 14:22:19.711864',378,0,'2020-01-01 00:00:00.000000','2020-01-01 00:00:00.000000',NULL,NULL);
+INSERT INTO ab_user VALUES(2,'readonly','readonly','readonly','pbkdf2:sha256:260000$9xVo850WOL4NuLpF$10ea139275a6f7d4ef3feaab50fd40394613b23a1bb535881c6904001c89ec2c',0,'readonly@fab.org','2022-12-22 12:24:32.813604',1,0,'2020-01-01 00:00:00.000000','2023-05-19 13:50:42.229836',NULL,1);
+INSERT INTO ab_user VALUES(3,'test','user','test','pbkdf2:sha256:260000$pEwMm2pjhzBdfzPQ$a65b2f3320e16862a9d307deedb2b02b86741acc470f3a97c8d6db7bc15b7d19',1,'test@fab.org','2023-05-19 14:22:14.231401',6,0,'2023-05-19 14:14:07.523474','2023-05-19 14:14:07.523483',NULL,NULL);
 CREATE TABLE ab_register_user (
 	id INTEGER NOT NULL, 
 	first_name VARCHAR(64) NOT NULL, 
 	last_name VARCHAR(64) NOT NULL, 
 	username VARCHAR(64) NOT NULL, 
 	password VARCHAR(256), 
 	email VARCHAR(64) NOT NULL, 
@@ -436,15 +448,14 @@
 INSERT INTO model2 VALUES(25,'test24',24,24.0,'2007-07-06','EXCLUDED','DEFAULT',25);
 INSERT INTO model2 VALUES(26,'test25',25,25.0,'1982-06-18','EXCLUDED','DEFAULT',26);
 INSERT INTO model2 VALUES(27,'test26',26,26.0,'1955-09-24','EXCLUDED','DEFAULT',27);
 INSERT INTO model2 VALUES(28,'test27',27,27.0,'1934-02-09','EXCLUDED','DEFAULT',28);
 INSERT INTO model2 VALUES(29,'test28',28,28.0,'2000-03-04','EXCLUDED','DEFAULT',29);
 INSERT INTO model2 VALUES(30,'test29',29,29.0,'2007-09-08','EXCLUDED','DEFAULT',30);
 INSERT INTO model2 VALUES(31,'test0',0,0.0,'1934-08-20','EXCLUDED','DEFAULT',1);
-INSERT INTO model2 VALUES(32,'test2',2,2.0,'1913-10-02','EXCLUDED','DEFAULT',3);
 CREATE TABLE model4 (
 	id INTEGER NOT NULL, 
 	field_string VARCHAR(50) NOT NULL, 
 	model1_1_id INTEGER NOT NULL, 
 	model1_2_id INTEGER NOT NULL, 
 	PRIMARY KEY (id), 
 	UNIQUE (field_string), 
@@ -486,17 +497,14 @@
 	parent_id INTEGER, 
 	child_id INTEGER, 
 	PRIMARY KEY (id), 
 	UNIQUE (parent_id, child_id), 
 	FOREIGN KEY(parent_id) REFERENCES parent (id), 
 	FOREIGN KEY(child_id) REFERENCES child (id)
 );
-INSERT INTO parent_child VALUES(1,1,1);
-INSERT INTO parent_child VALUES(2,1,2);
-INSERT INTO parent_child VALUES(3,1,3);
 INSERT INTO parent_child VALUES(4,2,1);
 INSERT INTO parent_child VALUES(5,2,2);
 INSERT INTO parent_child VALUES(6,2,3);
 INSERT INTO parent_child VALUES(7,3,1);
 INSERT INTO parent_child VALUES(8,3,2);
 INSERT INTO parent_child VALUES(9,3,3);
 INSERT INTO parent_child VALUES(10,4,1);
@@ -576,14 +584,17 @@
 INSERT INTO parent_child VALUES(84,28,3);
 INSERT INTO parent_child VALUES(85,29,1);
 INSERT INTO parent_child VALUES(86,29,2);
 INSERT INTO parent_child VALUES(87,29,3);
 INSERT INTO parent_child VALUES(88,30,1);
 INSERT INTO parent_child VALUES(89,30,2);
 INSERT INTO parent_child VALUES(90,30,3);
+INSERT INTO parent_child VALUES(91,1,1);
+INSERT INTO parent_child VALUES(92,1,2);
+INSERT INTO parent_child VALUES(93,1,3);
 CREATE TABLE parent_child_required (
 	id INTEGER NOT NULL, 
 	parent_id INTEGER, 
 	child_id INTEGER, 
 	PRIMARY KEY (id), 
 	UNIQUE (parent_id, child_id), 
 	FOREIGN KEY(parent_id) REFERENCES parent_required (id), 
@@ -1633,19 +1644,14 @@
 INSERT INTO ab_permission_view VALUES(65,4,35);
 INSERT INTO ab_permission_view VALUES(66,8,35);
 INSERT INTO ab_permission_view VALUES(67,3,36);
 INSERT INTO ab_permission_view VALUES(68,3,37);
 INSERT INTO ab_permission_view VALUES(69,3,38);
 INSERT INTO ab_permission_view VALUES(70,18,40);
 INSERT INTO ab_permission_view VALUES(71,19,40);
-INSERT INTO ab_permission_view VALUES(72,1,41);
-INSERT INTO ab_permission_view VALUES(73,20,41);
-INSERT INTO ab_permission_view VALUES(74,8,41);
-INSERT INTO ab_permission_view VALUES(75,2,41);
-INSERT INTO ab_permission_view VALUES(76,21,41);
 INSERT INTO ab_permission_view VALUES(77,1,42);
 INSERT INTO ab_permission_view VALUES(78,20,42);
 INSERT INTO ab_permission_view VALUES(79,8,42);
 INSERT INTO ab_permission_view VALUES(80,2,42);
 INSERT INTO ab_permission_view VALUES(81,21,42);
 INSERT INTO ab_permission_view VALUES(82,1,43);
 INSERT INTO ab_permission_view VALUES(83,20,43);
@@ -1738,15 +1744,14 @@
 INSERT INTO ab_permission_view VALUES(170,2,61);
 INSERT INTO ab_permission_view VALUES(171,21,61);
 INSERT INTO ab_permission_view VALUES(172,1,62);
 INSERT INTO ab_permission_view VALUES(173,20,62);
 INSERT INTO ab_permission_view VALUES(174,8,62);
 INSERT INTO ab_permission_view VALUES(175,2,62);
 INSERT INTO ab_permission_view VALUES(176,21,62);
-INSERT INTO ab_permission_view VALUES(177,22,63);
 INSERT INTO ab_permission_view VALUES(178,1,64);
 INSERT INTO ab_permission_view VALUES(179,20,64);
 INSERT INTO ab_permission_view VALUES(180,8,64);
 INSERT INTO ab_permission_view VALUES(181,2,64);
 INSERT INTO ab_permission_view VALUES(182,21,64);
 INSERT INTO ab_permission_view VALUES(183,1,65);
 INSERT INTO ab_permission_view VALUES(184,1,66);
@@ -1766,25 +1771,56 @@
 INSERT INTO ab_permission_view VALUES(198,8,68);
 INSERT INTO ab_permission_view VALUES(199,23,69);
 INSERT INTO ab_permission_view VALUES(200,2,70);
 INSERT INTO ab_permission_view VALUES(201,21,70);
 INSERT INTO ab_permission_view VALUES(202,20,70);
 INSERT INTO ab_permission_view VALUES(203,1,70);
 INSERT INTO ab_permission_view VALUES(204,8,70);
+INSERT INTO ab_permission_view VALUES(205,10,36);
+INSERT INTO ab_permission_view VALUES(206,7,36);
+INSERT INTO ab_permission_view VALUES(207,4,36);
+INSERT INTO ab_permission_view VALUES(208,8,36);
+INSERT INTO ab_permission_view VALUES(209,11,36);
+INSERT INTO ab_permission_view VALUES(210,15,71);
+INSERT INTO ab_permission_view VALUES(211,21,72);
+INSERT INTO ab_permission_view VALUES(212,20,72);
+INSERT INTO ab_permission_view VALUES(213,8,72);
+INSERT INTO ab_permission_view VALUES(214,1,72);
+INSERT INTO ab_permission_view VALUES(215,2,72);
+INSERT INTO ab_permission_view VALUES(216,21,73);
+INSERT INTO ab_permission_view VALUES(217,20,73);
+INSERT INTO ab_permission_view VALUES(218,8,73);
+INSERT INTO ab_permission_view VALUES(219,1,73);
+INSERT INTO ab_permission_view VALUES(220,2,73);
+INSERT INTO ab_permission_view VALUES(221,23,74);
+INSERT INTO ab_permission_view VALUES(222,24,74);
+INSERT INTO ab_permission_view VALUES(223,25,75);
+INSERT INTO ab_permission_view VALUES(229,21,77);
+INSERT INTO ab_permission_view VALUES(230,20,77);
+INSERT INTO ab_permission_view VALUES(231,8,77);
+INSERT INTO ab_permission_view VALUES(232,1,77);
+INSERT INTO ab_permission_view VALUES(233,2,77);
+INSERT INTO ab_permission_view VALUES(241,21,81);
+INSERT INTO ab_permission_view VALUES(242,20,81);
+INSERT INTO ab_permission_view VALUES(243,1,81);
+INSERT INTO ab_permission_view VALUES(244,8,81);
+INSERT INTO ab_permission_view VALUES(245,2,81);
+INSERT INTO ab_permission_view VALUES(246,26,82);
 CREATE TABLE ab_user_role (
 	id INTEGER NOT NULL, 
 	user_id INTEGER, 
 	role_id INTEGER, 
 	PRIMARY KEY (id), 
 	UNIQUE (user_id, role_id), 
 	FOREIGN KEY(user_id) REFERENCES ab_user (id), 
 	FOREIGN KEY(role_id) REFERENCES ab_role (id)
 );
 INSERT INTO ab_user_role VALUES(1,1,2);
 INSERT INTO ab_user_role VALUES(2,2,1);
+INSERT INTO ab_user_role VALUES(3,3,6);
 CREATE TABLE ab_permission_view_role (
 	id INTEGER NOT NULL, 
 	permission_view_id INTEGER, 
 	role_id INTEGER, 
 	PRIMARY KEY (id), 
 	UNIQUE (permission_view_id, role_id), 
 	FOREIGN KEY(permission_view_id) REFERENCES ab_permission_view (id), 
@@ -1858,19 +1894,14 @@
 INSERT INTO ab_permission_view_role VALUES(66,66,2);
 INSERT INTO ab_permission_view_role VALUES(67,47,4);
 INSERT INTO ab_permission_view_role VALUES(68,67,4);
 INSERT INTO ab_permission_view_role VALUES(69,68,5);
 INSERT INTO ab_permission_view_role VALUES(70,69,5);
 INSERT INTO ab_permission_view_role VALUES(71,70,2);
 INSERT INTO ab_permission_view_role VALUES(72,71,2);
-INSERT INTO ab_permission_view_role VALUES(73,72,2);
-INSERT INTO ab_permission_view_role VALUES(74,73,2);
-INSERT INTO ab_permission_view_role VALUES(75,74,2);
-INSERT INTO ab_permission_view_role VALUES(76,75,2);
-INSERT INTO ab_permission_view_role VALUES(77,76,2);
 INSERT INTO ab_permission_view_role VALUES(78,77,2);
 INSERT INTO ab_permission_view_role VALUES(79,78,2);
 INSERT INTO ab_permission_view_role VALUES(80,79,2);
 INSERT INTO ab_permission_view_role VALUES(81,80,2);
 INSERT INTO ab_permission_view_role VALUES(82,81,2);
 INSERT INTO ab_permission_view_role VALUES(83,82,2);
 INSERT INTO ab_permission_view_role VALUES(84,83,2);
@@ -1963,15 +1994,14 @@
 INSERT INTO ab_permission_view_role VALUES(171,170,2);
 INSERT INTO ab_permission_view_role VALUES(172,171,2);
 INSERT INTO ab_permission_view_role VALUES(173,172,2);
 INSERT INTO ab_permission_view_role VALUES(174,173,2);
 INSERT INTO ab_permission_view_role VALUES(175,174,2);
 INSERT INTO ab_permission_view_role VALUES(176,175,2);
 INSERT INTO ab_permission_view_role VALUES(177,176,2);
-INSERT INTO ab_permission_view_role VALUES(178,177,2);
 INSERT INTO ab_permission_view_role VALUES(179,178,2);
 INSERT INTO ab_permission_view_role VALUES(180,179,2);
 INSERT INTO ab_permission_view_role VALUES(181,180,2);
 INSERT INTO ab_permission_view_role VALUES(182,181,2);
 INSERT INTO ab_permission_view_role VALUES(183,182,2);
 INSERT INTO ab_permission_view_role VALUES(184,183,2);
 INSERT INTO ab_permission_view_role VALUES(185,184,2);
@@ -1991,8 +2021,46 @@
 INSERT INTO ab_permission_view_role VALUES(199,198,2);
 INSERT INTO ab_permission_view_role VALUES(200,199,2);
 INSERT INTO ab_permission_view_role VALUES(201,200,2);
 INSERT INTO ab_permission_view_role VALUES(202,201,2);
 INSERT INTO ab_permission_view_role VALUES(203,202,2);
 INSERT INTO ab_permission_view_role VALUES(204,203,2);
 INSERT INTO ab_permission_view_role VALUES(205,204,2);
+INSERT INTO ab_permission_view_role VALUES(206,205,2);
+INSERT INTO ab_permission_view_role VALUES(207,206,2);
+INSERT INTO ab_permission_view_role VALUES(208,207,2);
+INSERT INTO ab_permission_view_role VALUES(209,208,2);
+INSERT INTO ab_permission_view_role VALUES(210,209,2);
+INSERT INTO ab_permission_view_role VALUES(211,67,2);
+INSERT INTO ab_permission_view_role VALUES(212,210,2);
+INSERT INTO ab_permission_view_role VALUES(214,211,2);
+INSERT INTO ab_permission_view_role VALUES(215,212,2);
+INSERT INTO ab_permission_view_role VALUES(216,213,2);
+INSERT INTO ab_permission_view_role VALUES(217,214,2);
+INSERT INTO ab_permission_view_role VALUES(218,215,2);
+INSERT INTO ab_permission_view_role VALUES(219,216,2);
+INSERT INTO ab_permission_view_role VALUES(220,217,2);
+INSERT INTO ab_permission_view_role VALUES(221,218,2);
+INSERT INTO ab_permission_view_role VALUES(222,219,2);
+INSERT INTO ab_permission_view_role VALUES(223,220,2);
+INSERT INTO ab_permission_view_role VALUES(224,221,2);
+INSERT INTO ab_permission_view_role VALUES(225,222,2);
+INSERT INTO ab_permission_view_role VALUES(226,222,6);
+INSERT INTO ab_permission_view_role VALUES(227,223,2);
+INSERT INTO ab_permission_view_role VALUES(229,223,6);
+INSERT INTO ab_permission_view_role VALUES(235,229,2);
+INSERT INTO ab_permission_view_role VALUES(236,230,2);
+INSERT INTO ab_permission_view_role VALUES(237,231,2);
+INSERT INTO ab_permission_view_role VALUES(238,232,2);
+INSERT INTO ab_permission_view_role VALUES(239,233,2);
+INSERT INTO ab_permission_view_role VALUES(240,233,6);
+INSERT INTO ab_permission_view_role VALUES(241,229,6);
+INSERT INTO ab_permission_view_role VALUES(242,232,6);
+INSERT INTO ab_permission_view_role VALUES(243,231,6);
+INSERT INTO ab_permission_view_role VALUES(244,230,6);
+INSERT INTO ab_permission_view_role VALUES(254,241,2);
+INSERT INTO ab_permission_view_role VALUES(255,242,2);
+INSERT INTO ab_permission_view_role VALUES(256,243,2);
+INSERT INTO ab_permission_view_role VALUES(257,244,2);
+INSERT INTO ab_permission_view_role VALUES(258,245,2);
+INSERT INTO ab_permission_view_role VALUES(259,246,2);
 COMMIT;
```

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/base.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/config_oauth.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/config_oauth.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/config_security_api.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/config_security_api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/data/roles.json` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/data/roles.json`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/mongoengine/models.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/mongoengine/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/__pycache__/test_auth_ldap.cpython-38.pyc` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/__pycache__/test_auth_ldap.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/__pycache__/test_mvc_security.cpython-38.pyc` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/__pycache__/test_mvc_security.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon May  8 10:42:42 2023 UTC, .py size: 14235 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 19% similar despite different names*

```diff
@@ -1,641 +1,792 @@
-00000000: 550d 0d0a 0000 0000 22d2 5864 9b37 0000  U.......".Xd.7..
+00000000: 550d 0d0a 0000 0000 8f7f 6764 ee47 0000  U.........gd.G..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 9c00 0000 6400  .....@...s....d.
-00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
-00000060: 6405 6c08 6d09 5a09 0100 6406 6407 6c0a  d.l.m.Z...d.d.l.
-00000070: 6d0b 5a0b 0100 6406 6408 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
-00000080: 6d0e 5a0e 6d0f 5a0f 6d10 5a10 6d11 5a11  m.Z.m.Z.m.Z.m.Z.
-00000090: 0100 6406 6409 6c12 6d13 5a13 6d14 5a14  ..d.d.l.m.Z.m.Z.
-000000a0: 0100 640a 5a15 6516 640b 640c 9c02 640d  ..d.Z.e.d.d...d.
-000000b0: 640e 8404 5a17 4700 640f 6410 8400 6410  d...Z.G.d.d...d.
-000000c0: 650b 8303 5a18 640b 5300 2911 e900 0000  e...Z.d.S.).....
-000000d0: 0029 01da 094d 6f64 656c 5669 6577 a901  .)...ModelView..
-000000e0: da21 5061 7373 776f 7264 436f 6d70 6c65  .!PasswordComple
-000000f0: 7869 7479 5661 6c69 6461 7469 6f6e 4572  xityValidationEr
-00000100: 726f 7229 01da 0b46 696c 7465 7245 7175  ror)...FilterEqu
-00000110: 616c 2901 da0d 5351 4c41 496e 7465 7266  al)...SQLAInterf
-00000120: 6163 6529 01da 0455 7365 72e9 0200 0000  ace)...User.....
-00000130: 2901 da0f 4261 7365 4d56 4354 6573 7443  )...BaseMVCTestC
-00000140: 6173 6529 05da 1449 4e56 414c 4944 5f4c  ase)...INVALID_L
-00000150: 4f47 494e 5f53 5452 494e 47da 0e50 4153  OGIN_STRING..PAS
-00000160: 5357 4f52 445f 4144 4d49 4eda 1150 4153  SWORD_ADMIN..PAS
-00000170: 5357 4f52 445f 5245 4144 4f4e 4c59 da0e  SWORD_READONLY..
-00000180: 5553 4552 4e41 4d45 5f41 444d 494e da11  USERNAME_ADMIN..
-00000190: 5553 4552 4e41 4d45 5f52 4541 444f 4e4c  USERNAME_READONL
-000001a0: 5929 02da 064d 6f64 656c 31da 064d 6f64  Y)...Model1..Mod
-000001b0: 656c 327a 7e4d 7573 7420 6861 7665 2061  el2z~Must have a
-000001c0: 7420 6c65 6173 7420 7477 6f20 6361 7069  t least two capi
-000001d0: 7461 6c20 6c65 7474 6572 732c 206f 6e65  tal letters, one
-000001e0: 2073 7065 6369 616c 2063 6861 7261 6374   special charact
-000001f0: 6572 2c20 7477 6f20 6469 6769 7473 2c20  er, two digits, 
-00000200: 7468 7265 6520 6c6f 7765 7220 6361 7365  three lower case
-00000210: 206c 6574 7465 7273 2061 6e64 2061 206d   letters and a m
-00000220: 696e 696d 616c 206c 656e 6774 6820 6f66  inimal length of
-00000230: 2031 304e 2902 da08 7061 7373 776f 7264   10N)...password
-00000240: da06 7265 7475 726e 6301 0000 0000 0000  ..returnc.......
-00000250: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
-00000260: 0073 1400 0000 7c00 6401 6b03 7210 7400  .s....|.d.k.r.t.
-00000270: 6402 8301 8201 6403 5300 2904 7a37 0a20  d.....d.S.).z7. 
-00000280: 2020 2041 2073 696d 706c 6973 7469 6320     A simplistic 
-00000290: 6578 616d 706c 6520 666f 7220 6120 7061  example for a pa
-000002a0: 7373 776f 7264 2076 616c 6964 6174 6f72  ssword validator
-000002b0: 0a20 2020 2072 1100 0000 fa19 5061 7373  .    r......Pass
-000002c0: 776f 7264 206d 7573 7420 6265 2070 6173  word must be pas
-000002d0: 7377 6f72 644e 7203 0000 0029 0172 1100  swordNr....).r..
-000002e0: 0000 a900 7214 0000 00fa 652f 5573 6572  ....r.....e/User
-000002f0: 732f 6470 6761 7370 6172 2f77 6f72 6b61  s/dpgaspar/worka
-00000300: 7265 612f 7072 6573 6574 2f46 6c61 736b  rea/preset/Flask
-00000310: 2d41 7070 4275 696c 6465 722f 666c 6173  -AppBuilder/flas
-00000320: 6b5f 6170 7062 7569 6c64 6572 2f74 6573  k_appbuilder/tes
-00000330: 7473 2f73 6563 7572 6974 792f 7465 7374  ts/security/test
-00000340: 5f6d 7663 5f73 6563 7572 6974 792e 7079  _mvc_security.py
-00000350: da19 6375 7374 6f6d 5f70 6173 7377 6f72  ..custom_passwor
-00000360: 645f 7661 6c69 6461 746f 7218 0000 0073  d_validator....s
-00000370: 0400 0000 0004 0801 7216 0000 0063 0000  ........r....c..
-00000380: 0000 0000 0000 0000 0000 0000 0000 0300  ................
-00000390: 0000 0000 0000 739c 0000 0065 005a 0164  ......s....e.Z.d
-000003a0: 005a 0287 0066 0164 0164 0284 085a 0364  .Z...f.d.d...Z.d
-000003b0: 0364 0484 005a 0464 0564 0684 005a 0564  .d...Z.d.d...Z.d
-000003c0: 0764 0884 005a 0664 0964 0a84 005a 0764  .d...Z.d.d...Z.d
-000003d0: 0b64 0c84 005a 0864 0d64 0e84 005a 0964  .d...Z.d.d...Z.d
-000003e0: 0f64 1084 005a 0a64 1164 1284 005a 0b64  .d...Z.d.d...Z.d
-000003f0: 1364 1484 005a 0c64 1564 1684 005a 0d64  .d...Z.d.d...Z.d
-00000400: 1764 1884 005a 0e64 1964 1a84 005a 0f64  .d...Z.d.d...Z.d
-00000410: 1b64 1c84 005a 1064 1d64 1e84 005a 1164  .d...Z.d.d...Z.d
-00000420: 1f64 2084 005a 1264 2164 2284 005a 1387  .d ..Z.d!d"..Z..
-00000430: 0004 005a 1453 0029 23da 134d 5643 5365  ...Z.S.)#..MVCSe
-00000440: 6375 7269 7479 5465 7374 4361 7365 6301  curityTestCasec.
-00000450: 0000 0000 0000 0000 0000 0002 0000 0005  ................
-00000460: 0000 0003 0000 0073 5e00 0000 7400 8300  .......s^...t...
-00000470: a001 a100 0100 7c00 6a02 a003 a100 7c00  ......|.j.....|.
-00000480: 5f04 4700 6401 6402 8400 6402 7405 8303  _.G.d.d...d.t...
-00000490: 8900 7c00 6a06 a007 8800 6403 a102 0100  ..|.j.....d.....
-000004a0: 4700 8700 6601 6404 6405 8408 6405 7405  G...f.d.d...d.t.
-000004b0: 8303 7d01 7c00 6a06 6a07 7c01 6406 6406  ..}.|.j.j.|.d.d.
-000004c0: 6407 8d03 0100 6400 5300 2908 4e63 0000  d.....d.S.).Nc..
-000004d0: 0000 0000 0000 0000 0000 0000 0000 0500  ................
-000004e0: 0000 4000 0000 734a 0000 0065 005a 0164  ..@...sJ...e.Z.d
-000004f0: 005a 0265 0365 0483 015a 0564 0164 0264  .Z.e.e...Z.d.d.d
-00000500: 0364 0464 0567 055a 0664 0664 0365 0764  .d.d.g.Z.d.d.e.d
-00000510: 0767 0367 0169 015a 0864 0664 0365 0764  .g.g.i.Z.d.d.e.d
-00000520: 0867 0367 0169 015a 0964 0364 0567 025a  .g.g.i.Z.d.d.g.Z
-00000530: 0a64 0953 0029 0a7a 2d4d 5643 5365 6375  .d.S.).z-MVCSecu
-00000540: 7269 7479 5465 7374 4361 7365 2e73 6574  rityTestCase.set
-00000550: 5570 2e3c 6c6f 6361 6c73 3e2e 4d6f 6465  Up.<locals>.Mode
-00000560: 6c32 5669 6577 da0d 6669 656c 645f 696e  l2View..field_in
-00000570: 7465 6765 725a 0b66 6965 6c64 5f66 6c6f  tegerZ.field_flo
-00000580: 6174 da0c 6669 656c 645f 7374 7269 6e67  at..field_string
-00000590: 5a0c 6669 656c 645f 6d65 7468 6f64 7a12  Z.field_methodz.
-000005a0: 6772 6f75 702e 6669 656c 645f 7374 7269  group.field_stri
-000005b0: 6e67 da05 6772 6f75 705a 0574 6573 7431  ng..groupZ.test1
-000005c0: 5a05 7465 7374 304e 290b da08 5f5f 6e61  Z.test0N)...__na
-000005d0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000005e0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7206  ..__qualname__r.
-000005f0: 0000 0072 1000 0000 da09 6461 7461 6d6f  ...r......datamo
-00000600: 6465 6cda 0c6c 6973 745f 636f 6c75 6d6e  del..list_column
-00000610: 7372 0500 0000 da1a 6564 6974 5f66 6f72  sr......edit_for
-00000620: 6d5f 7175 6572 795f 7265 6c5f 6669 656c  m_query_rel_fiel
-00000630: 6473 da19 6164 645f 666f 726d 5f71 7565  ds..add_form_que
-00000640: 7279 5f72 656c 5f66 6965 6c64 73da 0d6f  ry_rel_fields..o
-00000650: 7264 6572 5f63 6f6c 756d 6e73 7214 0000  rder_columnsr...
-00000660: 0072 1400 0000 7214 0000 0072 1500 0000  .r....r....r....
-00000670: da0a 4d6f 6465 6c32 5669 6577 2500 0000  ..Model2View%...
-00000680: 731c 0000 0008 0108 0202 0102 0102 0102  s...............
-00000690: 0102 fb04 0802 000a ff04 0402 000a ff04  ................
-000006a0: 0472 2300 0000 7210 0000 0063 0000 0000  .r#...r....c....
-000006b0: 0000 0000 0000 0000 0000 0000 0200 0000  ................
-000006c0: 0000 0000 7322 0000 0065 005a 0164 005a  ....s"...e.Z.d.Z
-000006d0: 0265 0365 0483 015a 0594 0067 015a 0664  .e.e...Z...g.Z.d
-000006e0: 0164 0267 025a 0764 0353 0029 047a 2d4d  .d.g.Z.d.S.).z-M
-000006f0: 5643 5365 6375 7269 7479 5465 7374 4361  VCSecurityTestCa
-00000700: 7365 2e73 6574 5570 2e3c 6c6f 6361 6c73  se.setUp.<locals
-00000710: 3e2e 4d6f 6465 6c31 5669 6577 7219 0000  >.Model1Viewr...
-00000720: 0072 1800 0000 4e29 0872 1b00 0000 721c  .r....N).r....r.
-00000730: 0000 0072 1d00 0000 7206 0000 0072 0f00  ...r....r....r..
-00000740: 0000 721e 0000 00da 0d72 656c 6174 6564  ..r......related
-00000750: 5f76 6965 7773 721f 0000 0072 1400 0000  _viewsr....r....
-00000760: a901 7223 0000 0072 1400 0000 7215 0000  ..r#...r....r...
-00000770: 00da 0a4d 6f64 656c 3156 6965 7739 0000  ...Model1View9..
-00000780: 0073 0600 0000 0801 0801 0601 7226 0000  .s..........r&..
-00000790: 0072 0f00 0000 2901 da08 6361 7465 676f  .r....)...catego
-000007a0: 7279 2908 da05 7375 7065 72da 0573 6574  ry)...super..set
-000007b0: 5570 da03 6170 70da 0b74 6573 745f 636c  Up..app..test_cl
-000007c0: 6965 6e74 da06 636c 6965 6e74 7202 0000  ient..clientr...
-000007d0: 00da 0a61 7070 6275 696c 6465 72da 0861  ...appbuilder..a
-000007e0: 6464 5f76 6965 7729 02da 0473 656c 6672  dd_view)...selfr
-000007f0: 2600 0000 a901 da09 5f5f 636c 6173 735f  &.......__class_
-00000800: 5f72 2500 0000 7215 0000 0072 2900 0000  _r%...r....r)...
-00000810: 2100 0000 730c 0000 0000 010a 010c 0210  !...s...........
-00000820: 120e 0214 057a 194d 5643 5365 6375 7269  .....z.MVCSecuri
-00000830: 7479 5465 7374 4361 7365 2e73 6574 5570  tyTestCase.setUp
-00000840: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00000850: 0005 0000 0043 0000 0073 e400 0000 7c00  .....C...s....|.
-00000860: 6a00 a001 6401 a101 7d01 7c00 a002 7c01  j...d...}.|...|.
-00000870: 6a03 6402 a102 0100 7c00 6a00 a001 6403  j.d.....|.j...d.
-00000880: a101 7d01 7c00 a002 7c01 6a03 6402 a102  ..}.|...|.j.d...
-00000890: 0100 7c00 a004 7c00 6a00 7405 7406 a103  ..|...|.j.t.t...
-000008a0: 0100 7c00 6a00 a001 6401 a101 7d01 7c00  ..|.j...d...}.|.
-000008b0: a002 7c01 6a03 6404 a102 0100 7c00 6a00  ..|.j.d.....|.j.
-000008c0: a001 6403 a101 7d01 7c00 a002 7c01 6a03  ..d...}.|...|.j.
-000008d0: 6404 a102 0100 7c00 a007 7c00 6a00 a101  d.....|...|.j...
-000008e0: 0100 7c00 6a00 a001 6401 a101 7d01 7c00  ..|.j...d...}.|.
-000008f0: a002 7c01 6a03 6402 a102 0100 7c00 6a00  ..|.j.d.....|.j.
-00000900: a001 6403 a101 7d01 7c00 a002 7c01 6a03  ..d...}.|...|.j.
-00000910: 6402 a102 0100 7c00 a004 7c00 6a00 7405  d.....|...|.j.t.
-00000920: 6405 a103 7d01 7c01 6a08 a009 6406 a101  d...}.|.j...d...
-00000930: 7d02 7c00 a00a 740b 7c02 a102 0100 6407  }.|...t.|.....d.
-00000940: 5300 2908 7a4c 0a20 2020 2020 2020 2054  S.).zL.        T
-00000950: 6573 7420 5365 6375 7269 7479 204c 6f67  est Security Log
-00000960: 696e 2c20 4c6f 676f 7574 2c20 696e 7661  in, Logout, inva
-00000970: 6c69 6420 6c6f 6769 6e2c 2069 6e76 616c  lid login, inval
-00000980: 6964 2061 6363 6573 730a 2020 2020 2020  id access.      
-00000990: 2020 fa11 2f6d 6f64 656c 3176 6965 772f    ../model1view/
-000009a0: 6c69 7374 2fe9 2e01 0000 7a11 2f6d 6f64  list/.....z./mod
-000009b0: 656c 3276 6965 772f 6c69 7374 2fe9 c800  el2view/list/...
-000009c0: 0000 5a0e 7772 6f6e 675f 7061 7373 776f  ..Z.wrong_passwo
-000009d0: 7264 fa05 7574 662d 384e 290c 722c 0000  rd..utf-8N).r,..
-000009e0: 00da 0367 6574 da0b 6173 7365 7274 4571  ...get..assertEq
-000009f0: 7561 6cda 0b73 7461 7475 735f 636f 6465  ual..status_code
-00000a00: da0d 6272 6f77 7365 725f 6c6f 6769 6e72  ..browser_loginr
-00000a10: 0d00 0000 720b 0000 00da 0e62 726f 7773  ....r......brows
-00000a20: 6572 5f6c 6f67 6f75 74da 0464 6174 61da  er_logout..data.
-00000a30: 0664 6563 6f64 65da 0861 7373 6572 7449  .decode..assertI
-00000a40: 6e72 0a00 0000 2903 722f 0000 00da 0272  nr....).r/.....r
-00000a50: 7672 3b00 0000 7214 0000 0072 1400 0000  vr;...r....r....
-00000a60: 7215 0000 00da 0e74 6573 745f 7365 635f  r......test_sec_
-00000a70: 6c6f 6769 6e40 0000 0073 2200 0000 0006  login@...s".....
-00000a80: 0c01 0e01 0c01 0e03 1001 0c01 0e01 0c01  ................
-00000a90: 0e03 0c01 0c01 0e01 0c01 0e03 1001 0c01  ................
-00000aa0: 7a22 4d56 4353 6563 7572 6974 7954 6573  z"MVCSecurityTes
-00000ab0: 7443 6173 652e 7465 7374 5f73 6563 5f6c  tCase.test_sec_l
-00000ac0: 6f67 696e 6301 0000 0000 0000 0000 0000  oginc...........
-00000ad0: 0002 0000 0006 0000 0043 0000 0073 3200  .........C...s2.
-00000ae0: 0000 7c00 a000 7c00 6a01 a101 0100 7c00  ..|...|.j.....|.
-00000af0: 6a02 7c00 6a01 7403 7404 6401 6402 8d04  j.|.j.t.t.d.d...
-00000b00: 7d01 7c01 6a05 6403 6b02 732e 7406 8201  }.|.j.d.k.s.t...
-00000b10: 6404 5300 2905 7a2b 0a20 2020 2020 2020  d.S.).z+.       
-00000b20: 2054 6573 7420 5365 6375 7269 7479 206e   Test Security n
-00000b30: 6f20 6e65 7874 2055 524c 0a20 2020 2020  o next URL.     
-00000b40: 2020 2046 a901 da10 666f 6c6c 6f77 5f72     F....follow_r
-00000b50: 6564 6972 6563 7473 fa01 2f4e a907 723a  edirects../N..r:
-00000b60: 0000 0072 2c00 0000 7239 0000 0072 0d00  ...r,...r9...r..
-00000b70: 0000 720b 0000 00da 086c 6f63 6174 696f  ..r......locatio
-00000b80: 6eda 0e41 7373 6572 7469 6f6e 4572 726f  n..AssertionErro
-00000b90: 72a9 0272 2f00 0000 da08 7265 7370 6f6e  r..r/.....respon
-00000ba0: 7365 7214 0000 0072 1400 0000 7215 0000  ser....r....r...
-00000bb0: 00da 1974 6573 745f 6462 5f6c 6f67 696e  ...test_db_login
-00000bc0: 5f6e 6f5f 6e65 7874 5f75 726c 5e00 0000  _no_next_url^...
-00000bd0: 7310 0000 0000 040c 0104 0104 0002 0002  s...............
-00000be0: 0002 ff06 037a 2d4d 5643 5365 6375 7269  .....z-MVCSecuri
-00000bf0: 7479 5465 7374 4361 7365 2e74 6573 745f  tyTestCase.test_
-00000c00: 6462 5f6c 6f67 696e 5f6e 6f5f 6e65 7874  db_login_no_next
-00000c10: 5f75 726c 6301 0000 0000 0000 0000 0000  _urlc...........
-00000c20: 0002 0000 0007 0000 0043 0000 0073 3400  .........C...s4.
-00000c30: 0000 7c00 a000 7c00 6a01 a101 0100 7c00  ..|...|.j.....|.
-00000c40: 6a02 7c00 6a01 7403 7404 6401 6402 6403  j.|.j.t.t.d.d.d.
-00000c50: 8d05 7d01 7c01 6a05 6401 6b02 7330 7406  ..}.|.j.d.k.s0t.
-00000c60: 8201 6404 5300 2905 7a36 0a20 2020 2020  ..d.S.).z6.     
-00000c70: 2020 2054 6573 7420 5365 6375 7269 7479     Test Security
-00000c80: 2076 616c 6964 2070 6172 7469 616c 206e   valid partial n
-00000c90: 6578 7420 5552 4c0a 2020 2020 2020 2020  ext URL.        
-00000ca0: fa0c 2f75 7365 7273 2f6c 6973 742f 46a9  ../users/list/F.
-00000cb0: 02da 086e 6578 745f 7572 6c72 4100 0000  ...next_urlrA...
-00000cc0: 4e72 4300 0000 7246 0000 0072 1400 0000  NrC...rF...r....
-00000cd0: 7214 0000 0072 1500 0000 da1c 7465 7374  r....r......test
-00000ce0: 5f64 625f 6c6f 6769 6e5f 7661 6c69 645f  _db_login_valid_
-00000cf0: 6e65 7874 5f75 726c 6800 0000 7312 0000  next_urlh...s...
-00000d00: 0000 040c 0104 0104 0102 0102 0102 0102  ................
-00000d10: fb06 077a 304d 5643 5365 6375 7269 7479  ...z0MVCSecurity
-00000d20: 5465 7374 4361 7365 2e74 6573 745f 6462  TestCase.test_db
-00000d30: 5f6c 6f67 696e 5f76 616c 6964 5f6e 6578  _login_valid_nex
-00000d40: 745f 7572 6c63 0100 0000 0000 0000 0000  t_urlc..........
-00000d50: 0000 0200 0000 0700 0000 4300 0000 7334  ..........C...s4
-00000d60: 0000 007c 00a0 007c 006a 01a1 0101 007c  ...|...|.j.....|
-00000d70: 006a 027c 006a 0174 0374 0464 0164 0264  .j.|.j.t.t.d.d.d
-00000d80: 038d 057d 017c 016a 0564 016b 0273 3074  ...}.|.j.d.k.s0t
-00000d90: 0682 0164 0453 0029 057a 3a0a 2020 2020  ...d.S.).z:.    
-00000da0: 2020 2020 5465 7374 2053 6563 7572 6974      Test Securit
-00000db0: 7920 7661 6c69 6420 6874 7470 2073 6368  y valid http sch
-00000dc0: 656d 6520 6e65 7874 2055 524c 0a20 2020  eme next URL.   
-00000dd0: 2020 2020 207a 1568 7474 703a 2f2f 6c6f       z.http://lo
-00000de0: 6361 6c68 6f73 742f 7061 7468 4672 4a00  calhost/pathFrJ.
-00000df0: 0000 4e72 4300 0000 7246 0000 0072 1400  ..NrC...rF...r..
-00000e00: 0000 7214 0000 0072 1500 0000 da23 7465  ..r....r.....#te
-00000e10: 7374 5f64 625f 6c6f 6769 6e5f 7661 6c69  st_db_login_vali
-00000e20: 645f 6874 7470 5f73 6368 656d 655f 7572  d_http_scheme_ur
-00000e30: 6c76 0000 0073 1200 0000 0004 0c01 0401  lv...s..........
-00000e40: 0401 0201 0201 0201 02fb 0607 7a37 4d56  ............z7MV
-00000e50: 4353 6563 7572 6974 7954 6573 7443 6173  CSecurityTestCas
-00000e60: 652e 7465 7374 5f64 625f 6c6f 6769 6e5f  e.test_db_login_
-00000e70: 7661 6c69 645f 6874 7470 5f73 6368 656d  valid_http_schem
-00000e80: 655f 7572 6c63 0100 0000 0000 0000 0000  e_urlc..........
-00000e90: 0000 0200 0000 0700 0000 4300 0000 7334  ..........C...s4
-00000ea0: 0000 007c 00a0 007c 006a 01a1 0101 007c  ...|...|.j.....|
-00000eb0: 006a 027c 006a 0174 0374 0464 0164 0264  .j.|.j.t.t.d.d.d
-00000ec0: 038d 057d 017c 016a 0564 016b 0273 3074  ...}.|.j.d.k.s0t
-00000ed0: 0682 0164 0453 0029 057a 3b0a 2020 2020  ...d.S.).z;.    
-00000ee0: 2020 2020 5465 7374 2053 6563 7572 6974      Test Securit
-00000ef0: 7920 7661 6c69 6420 6874 7470 7320 7363  y valid https sc
-00000f00: 6865 6d65 206e 6578 7420 5552 4c0a 2020  heme next URL.  
-00000f10: 2020 2020 2020 7a16 6874 7470 733a 2f2f        z.https://
-00000f20: 6c6f 6361 6c68 6f73 742f 7061 7468 4672  localhost/pathFr
-00000f30: 4a00 0000 4e72 4300 0000 7246 0000 0072  J...NrC...rF...r
-00000f40: 1400 0000 7214 0000 0072 1500 0000 da24  ....r....r.....$
-00000f50: 7465 7374 5f64 625f 6c6f 6769 6e5f 7661  test_db_login_va
-00000f60: 6c69 645f 6874 7470 735f 7363 6865 6d65  lid_https_scheme
-00000f70: 5f75 726c 8400 0000 7312 0000 0000 040c  _url....s.......
-00000f80: 0104 0104 0102 0102 0102 0102 fb06 077a  ...............z
-00000f90: 384d 5643 5365 6375 7269 7479 5465 7374  8MVCSecurityTest
-00000fa0: 4361 7365 2e74 6573 745f 6462 5f6c 6f67  Case.test_db_log
-00000fb0: 696e 5f76 616c 6964 5f68 7474 7073 5f73  in_valid_https_s
-00000fc0: 6368 656d 655f 7572 6c63 0100 0000 0000  cheme_urlc......
-00000fd0: 0000 0000 0000 0200 0000 0700 0000 4300  ..............C.
-00000fe0: 0000 7334 0000 007c 00a0 007c 006a 01a1  ..s4...|...|.j..
-00000ff0: 0101 007c 006a 027c 006a 0174 0374 0464  ...|.j.|.j.t.t.d
-00001000: 0164 0264 038d 057d 017c 016a 0564 046b  .d.d...}.|.j.d.k
-00001010: 0273 3074 0682 0164 0553 0029 067a 390a  .s0t...d.S.).z9.
-00001020: 2020 2020 2020 2020 5465 7374 2053 6563          Test Sec
-00001030: 7572 6974 7920 696e 7661 6c69 6420 6578  urity invalid ex
-00001040: 7465 726e 616c 206e 6578 7420 5552 4c0a  ternal next URL.
-00001050: 2020 2020 2020 2020 7a12 6874 7470 733a          z.https:
-00001060: 2f2f 676f 6f67 6c65 2e63 6f6d 4672 4a00  //google.comFrJ.
-00001070: 0000 7242 0000 004e 7243 0000 0072 4600  ..rB...NrC...rF.
-00001080: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
-00001090: 00da 2774 6573 745f 6462 5f6c 6f67 696e  ..'test_db_login
-000010a0: 5f69 6e76 616c 6964 5f65 7874 6572 6e61  _invalid_externa
-000010b0: 6c5f 6e65 7874 5f75 726c 9200 0000 7312  l_next_url....s.
-000010c0: 0000 0000 040c 0104 0104 0102 0102 0102  ................
-000010d0: 0102 fb06 077a 3b4d 5643 5365 6375 7269  .....z;MVCSecuri
-000010e0: 7479 5465 7374 4361 7365 2e74 6573 745f  tyTestCase.test_
-000010f0: 6462 5f6c 6f67 696e 5f69 6e76 616c 6964  db_login_invalid
-00001100: 5f65 7874 6572 6e61 6c5f 6e65 7874 5f75  _external_next_u
-00001110: 726c 6301 0000 0000 0000 0000 0000 0002  rlc.............
-00001120: 0000 0007 0000 0043 0000 0073 3400 0000  .......C...s4...
-00001130: 7c00 a000 7c00 6a01 a101 0100 7c00 6a02  |...|.j.....|.j.
-00001140: 7c00 6a01 7403 7404 6401 6402 6403 8d05  |.j.t.t.d.d.d...
-00001150: 7d01 7c01 6a05 6404 6b02 7330 7406 8201  }.|.j.d.k.s0t...
-00001160: 6405 5300 2906 7a37 0a20 2020 2020 2020  d.S.).z7.       
-00001170: 2054 6573 7420 5365 6375 7269 7479 2069   Test Security i
-00001180: 6e76 616c 6964 2073 6368 656d 6520 6e65  nvalid scheme ne
-00001190: 7874 2055 524c 0a20 2020 2020 2020 207a  xt URL.        z
-000011a0: 0c66 7470 3a2f 2f73 616d 706c 6546 724a  .ftp://sampleFrJ
-000011b0: 0000 0072 4200 0000 4e72 4300 0000 7246  ...rB...NrC...rF
-000011c0: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
-000011d0: 0000 da25 7465 7374 5f64 625f 6c6f 6769  ...%test_db_logi
-000011e0: 6e5f 696e 7661 6c69 645f 7363 6865 6d65  n_invalid_scheme
-000011f0: 5f6e 6578 745f 7572 6ca0 0000 0073 1200  _next_url....s..
-00001200: 0000 0004 0c01 0401 0401 0201 0201 0201  ................
-00001210: 02fb 0607 7a39 4d56 4353 6563 7572 6974  ....z9MVCSecurit
-00001220: 7954 6573 7443 6173 652e 7465 7374 5f64  yTestCase.test_d
-00001230: 625f 6c6f 6769 6e5f 696e 7661 6c69 645f  b_login_invalid_
-00001240: 7363 6865 6d65 5f6e 6578 745f 7572 6c63  scheme_next_urlc
-00001250: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001260: 0700 0000 4300 0000 7334 0000 007c 00a0  ....C...s4...|..
-00001270: 007c 006a 01a1 0101 007c 006a 027c 006a  .|.j.....|.j.|.j
-00001280: 0174 0374 0464 0164 0264 038d 057d 017c  .t.t.d.d.d...}.|
-00001290: 016a 0564 046b 0273 3074 0682 0164 0553  .j.d.k.s0t...d.S
-000012a0: 0029 067a 470a 2020 2020 2020 2020 5465  .).zG.        Te
-000012b0: 7374 2053 6563 7572 6974 7920 696e 7661  st Security inva
-000012c0: 6c69 6420 7061 7468 2074 6f20 6c6f 6361  lid path to loca
-000012d0: 6c68 6f73 7420 6669 6c65 206e 6578 7420  lhost file next 
-000012e0: 5552 4c0a 2020 2020 2020 2020 7a0c 6669  URL.        z.fi
-000012f0: 6c65 3a2f 2f2f 7061 7468 4672 4a00 0000  le:///pathFrJ...
-00001300: 7242 0000 004e 7243 0000 0072 4600 0000  rB...NrC...rF...
-00001310: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-00001320: 2d74 6573 745f 6462 5f6c 6f67 696e 5f69  -test_db_login_i
-00001330: 6e76 616c 6964 5f6c 6f63 616c 686f 7374  nvalid_localhost
-00001340: 5f66 696c 655f 6e65 7874 5f75 726c ae00  _file_next_url..
-00001350: 0000 7312 0000 0000 040c 0104 0104 0102  ..s.............
-00001360: 0102 0102 0102 fb06 077a 414d 5643 5365  .........zAMVCSe
-00001370: 6375 7269 7479 5465 7374 4361 7365 2e74  curityTestCase.t
-00001380: 6573 745f 6462 5f6c 6f67 696e 5f69 6e76  est_db_login_inv
-00001390: 616c 6964 5f6c 6f63 616c 686f 7374 5f66  alid_localhost_f
-000013a0: 696c 655f 6e65 7874 5f75 726c 6301 0000  ile_next_urlc...
-000013b0: 0000 0000 0000 0000 0002 0000 0007 0000  ................
-000013c0: 0043 0000 0073 3400 0000 7c00 a000 7c00  .C...s4...|...|.
-000013d0: 6a01 a101 0100 7c00 6a02 7c00 6a01 7403  j.....|.j.|.j.t.
-000013e0: 7404 6401 6402 6403 8d05 7d01 7c01 6a05  t.d.d.d...}.|.j.
-000013f0: 6404 6b02 7330 7406 8201 6405 5300 2906  d.k.s0t...d.S.).
-00001400: 7a4f 0a20 2020 2020 2020 2054 6573 7420  zO.        Test 
-00001410: 5365 6375 7269 7479 2069 6e76 616c 6964  Security invalid
-00001420: 206e 6578 7420 5552 4c20 7769 7468 206e   next URL with n
-00001430: 6f20 6e65 746c 6f63 2062 7574 2077 6974  o netloc but wit
-00001440: 6820 7363 6865 6d65 0a20 2020 2020 2020  h scheme.       
-00001450: 207a 1368 7474 703a 2f2f 2f73 616d 706c   z.http:///sampl
-00001460: 652e 636f 6d20 4672 4a00 0000 7242 0000  e.com FrJ...rB..
-00001470: 004e 7243 0000 0072 4600 0000 7214 0000  .NrC...rF...r...
-00001480: 0072 1400 0000 7215 0000 00da 3474 6573  .r....r.....4tes
-00001490: 745f 6462 5f6c 6f67 696e 5f69 6e76 616c  t_db_login_inval
-000014a0: 6964 5f6e 6f5f 6e65 746c 6f63 5f77 6974  id_no_netloc_wit
-000014b0: 685f 7363 6865 6d65 5f6e 6578 745f 7572  h_scheme_next_ur
-000014c0: 6cbc 0000 0073 1200 0000 0004 0c01 0401  l....s..........
-000014d0: 0401 0201 0201 0201 02fb 0607 7a48 4d56  ............zHMV
-000014e0: 4353 6563 7572 6974 7954 6573 7443 6173  CSecurityTestCas
-000014f0: 652e 7465 7374 5f64 625f 6c6f 6769 6e5f  e.test_db_login_
-00001500: 696e 7661 6c69 645f 6e6f 5f6e 6574 6c6f  invalid_no_netlo
-00001510: 635f 7769 7468 5f73 6368 656d 655f 6e65  c_with_scheme_ne
-00001520: 7874 5f75 726c 6301 0000 0000 0000 0000  xt_urlc.........
-00001530: 0000 0002 0000 0007 0000 0043 0000 0073  ...........C...s
-00001540: 3400 0000 7c00 a000 7c00 6a01 a101 0100  4...|...|.j.....
-00001550: 7c00 6a02 7c00 6a01 7403 7404 6401 6402  |.j.|.j.t.t.d.d.
-00001560: 6403 8d05 7d01 7c01 6a05 6404 6b02 7330  d...}.|.j.d.k.s0
-00001570: 7406 8201 6405 5300 2906 7a48 0a20 2020  t...d.S.).zH.   
-00001580: 2020 2020 2054 6573 7420 5365 6375 7269       Test Securi
-00001590: 7479 2069 6e76 616c 6964 206e 6578 7420  ty invalid next 
-000015a0: 5552 4c20 7769 7468 2063 6f6e 7472 6f6c  URL with control
-000015b0: 2063 6861 7261 6374 6572 730a 2020 2020   characters.    
-000015c0: 2020 2020 7a0b 0173 616d 706c 652e 636f      z..sample.co
-000015d0: 6d46 724a 0000 0072 4200 0000 4e72 4300  mFrJ...rB...NrC.
-000015e0: 0000 7246 0000 0072 1400 0000 7214 0000  ..rF...r....r...
-000015f0: 0072 1500 0000 da31 7465 7374 5f64 625f  .r.....1test_db_
-00001600: 6c6f 6769 6e5f 696e 7661 6c69 645f 636f  login_invalid_co
-00001610: 6e74 726f 6c5f 6368 6172 6163 7465 7273  ntrol_characters
-00001620: 5f6e 6578 745f 7572 6cca 0000 0073 1200  _next_url....s..
-00001630: 0000 0004 0c01 0401 0401 0201 0201 0201  ................
-00001640: 02fb 0607 7a45 4d56 4353 6563 7572 6974  ....zEMVCSecurit
-00001650: 7954 6573 7443 6173 652e 7465 7374 5f64  yTestCase.test_d
-00001660: 625f 6c6f 6769 6e5f 696e 7661 6c69 645f  b_login_invalid_
-00001670: 636f 6e74 726f 6c5f 6368 6172 6163 7465  control_characte
-00001680: 7273 5f6e 6578 745f 7572 6c63 0100 0000  rs_next_urlc....
-00001690: 0000 0000 0000 0000 0200 0000 0700 0000  ................
-000016a0: 4300 0000 7356 0000 007c 00a0 007c 006a  C...sV...|...|.j
-000016b0: 01a1 0101 007c 006a 027c 006a 0174 0364  .....|.j.|.j.t.d
-000016c0: 0174 049b 009d 0264 0264 0364 048d 057d  .t.....d.d.d...}
-000016d0: 017c 006a 016a 057c 016a 0674 0774 0374  .|.j.j.|.j.t.t.t
-000016e0: 0464 058d 0264 0364 068d 037d 017c 016a  .d...d.d...}.|.j
-000016f0: 0664 026b 0273 5274 0882 0164 0753 0029  .d.k.sRt...d.S.)
-00001700: 087a 4b0a 2020 2020 2020 2020 5465 7374  .zK.        Test
-00001710: 2053 6563 7572 6974 7920 4b65 6570 696e   Security Keepin
-00001720: 6720 6e65 7874 2075 726c 2061 6674 6572  g next url after
-00001730: 2066 6169 6c65 6420 6c6f 6769 6e20 6174   failed login at
-00001740: 7465 6d70 740a 2020 2020 2020 2020 5a06  tempt.        Z.
-00001750: 7772 6f6e 675f 7249 0000 0046 724a 0000  wrong_rI...FrJ..
-00001760: 0029 02da 0875 7365 726e 616d 6572 1100  .)...usernamer..
-00001770: 0000 a902 723b 0000 0072 4100 0000 4e29  ....r;...rA...N)
-00001780: 0972 3a00 0000 722c 0000 0072 3900 0000  .r:...r,...r9...
-00001790: 720d 0000 0072 0b00 0000 da04 706f 7374  r....r......post
-000017a0: 7244 0000 00da 0464 6963 7472 4500 0000  rD.....dictrE...
-000017b0: 7246 0000 0072 1400 0000 7214 0000 0072  rF...r....r....r
-000017c0: 1500 0000 da22 7465 7374 5f64 625f 6c6f  ....."test_db_lo
-000017d0: 6769 6e5f 6661 696c 6564 5f6b 6565 705f  gin_failed_keep_
-000017e0: 6e65 7874 5f75 726c d800 0000 731c 0000  next_url....s...
-000017f0: 0000 040c 0104 0104 0102 0108 0102 0102  ................
-00001800: fb06 0706 0104 010a 0102 fd06 067a 364d  .............z6M
-00001810: 5643 5365 6375 7269 7479 5465 7374 4361  VCSecurityTestCa
-00001820: 7365 2e74 6573 745f 6462 5f6c 6f67 696e  se.test_db_login
-00001830: 5f66 6169 6c65 645f 6b65 6570 5f6e 6578  _failed_keep_nex
-00001840: 745f 7572 6c63 0100 0000 0000 0000 0000  t_urlc..........
-00001850: 0000 0300 0000 0500 0000 4300 0000 737c  ..........C...s|
-00001860: 0000 007c 006a 00a0 01a1 007d 017c 00a0  ...|.j.....}.|..
-00001870: 027c 0174 0374 04a1 0301 007c 01a0 0564  .|.t.t.....|...d
-00001880: 01a1 017d 027c 00a0 067c 026a 0764 02a1  ...}.|...|.j.d..
-00001890: 0201 007c 01a0 0564 03a1 017d 027c 00a0  ...|...d...}.|..
-000018a0: 067c 026a 0764 02a1 0201 007c 01a0 0564  .|.j.d.....|...d
-000018b0: 04a1 017d 027c 00a0 067c 026a 0764 05a1  ...}.|...|.j.d..
-000018c0: 0201 007c 01a0 0564 06a1 017d 027c 00a0  ...|...d...}.|..
-000018d0: 067c 026a 0764 05a1 0201 0064 0753 0029  .|.j.d.....d.S.)
-000018e0: 087a 360a 2020 2020 2020 2020 5465 7374  .z6.        Test
-000018f0: 2053 6563 7572 6974 7920 6275 696c 7469   Security builti
-00001900: 6e20 726f 6c65 7320 7265 6164 6f6e 6c79  n roles readonly
-00001910: 0a20 2020 2020 2020 2072 3200 0000 7234  .        r2...r4
-00001920: 0000 007a 122f 6d6f 6465 6c31 7669 6577  ...z./model1view
-00001930: 2f73 686f 772f 317a 122f 6d6f 6465 6c31  /show/1z./model1
-00001940: 7669 6577 2f65 6469 742f 3172 3300 0000  view/edit/1r3...
-00001950: 7a14 2f6d 6f64 656c 3176 6965 772f 6465  z./model1view/de
-00001960: 6c65 7465 2f31 4e29 0872 2a00 0000 722b  lete/1N).r*...r+
-00001970: 0000 0072 3900 0000 720e 0000 0072 0c00  ...r9...r....r..
-00001980: 0000 7236 0000 0072 3700 0000 7238 0000  ..r6...r7...r8..
-00001990: 0029 0372 2f00 0000 722c 0000 0072 3e00  .).r/...r,...r>.
-000019a0: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
-000019b0: 00da 1774 6573 745f 6175 7468 5f62 7569  ...test_auth_bui
-000019c0: 6c74 696e 5f72 6f6c 6573 ec00 0000 7314  ltin_roles....s.
-000019d0: 0000 0000 040a 010e 020a 010e 020a 010e  ................
-000019e0: 020a 010e 020a 017a 2b4d 5643 5365 6375  .......z+MVCSecu
-000019f0: 7269 7479 5465 7374 4361 7365 2e74 6573  rityTestCase.tes
-00001a00: 745f 6175 7468 5f62 7569 6c74 696e 5f72  t_auth_builtin_r
-00001a10: 6f6c 6573 6301 0000 0000 0000 0000 0000  olesc...........
-00001a20: 0005 0000 0006 0000 0043 0000 0073 0e01  .........C...s..
-00001a30: 0000 7c00 6a00 a001 a100 7d01 7c01 6a02  ..|.j.....}.|.j.
-00001a40: 6401 6402 6403 8d02 7d02 7c00 a003 7c02  d.d.d...}.|...|.
-00001a50: 6a04 6404 a102 0100 7c00 a005 7c01 7406  j.d.....|...|.t.
-00001a60: 7407 a103 7d03 7c01 6a02 6401 6402 6403  t...}.|.j.d.d.d.
-00001a70: 8d02 7d02 7c02 6a08 a009 6405 a101 7d04  ..}.|.j...d...}.
-00001a80: 7c00 a00a 6406 7c04 a102 0100 7c01 6a0b  |...d.|.....|.j.
-00001a90: 6407 740c 6408 6408 6409 8d02 6402 640a  d.t.d.d.d...d.d.
-00001aa0: 8d03 7d02 7c00 a003 7c02 6a04 640b a102  ..}.|...|.j.d...
-00001ab0: 0100 7c00 a00d 7c01 a101 0100 7c00 a005  ..|...|.....|...
-00001ac0: 7c01 7406 6408 a103 0100 7c01 6a0b 6407  |.t.d.....|.j.d.
-00001ad0: 740c 7407 7407 6409 8d02 6402 640a 8d03  t.t.t.d...d.d...
-00001ae0: 7d02 7c00 a003 7c02 6a04 640b a102 0100  }.|...|.j.d.....
-00001af0: 7c01 6a02 640c 6402 6403 8d02 7d02 7c02  |.j.d.d.d...}.|.
-00001b00: 6a08 a009 6405 a101 7d04 7c00 a00a 6406  j...d...}.|...d.
-00001b10: 7c04 a102 0100 7c01 6a0b 6407 740c 7407  |.....|.j.d.t.t.
-00001b20: 7407 6409 8d02 6402 640a 8d03 7d02 7c00  t.d...d.d...}.|.
-00001b30: a003 7c02 6a04 640b a102 0100 640d 5300  ..|.j.d.....d.S.
-00001b40: 290e 7a2e 0a20 2020 2020 2020 2054 6573  ).z..        Tes
-00001b50: 7420 5365 6375 7269 7479 2072 6573 6574  t Security reset
-00001b60: 2070 6173 7377 6f72 640a 2020 2020 2020   password.      
-00001b70: 2020 fa1f 2f75 7365 7273 2f61 6374 696f    ../users/actio
-00001b80: 6e2f 7265 7365 746d 7970 6173 7377 6f72  n/resetmypasswor
-00001b90: 642f 3154 7240 0000 0069 9401 0000 7235  d/1Tr@...i....r5
-00001ba0: 0000 00fa 1352 6573 6574 2050 6173 7377  .....Reset Passw
-00001bb0: 6f72 6420 466f 726d fa15 2f72 6573 6574  ord Form../reset
-00001bc0: 6d79 7061 7373 776f 7264 2f66 6f72 6d72  mypassword/formr
-00001bd0: 1100 0000 a902 7211 0000 00da 0d63 6f6e  ......r......con
-00001be0: 665f 7061 7373 776f 7264 7255 0000 0072  f_passwordrU...r
-00001bf0: 3400 0000 7a1e 2f75 7365 7273 2f61 6374  4...z./users/act
-00001c00: 696f 6e2f 7265 7365 7470 6173 7377 6f72  ion/resetpasswor
-00001c10: 6473 2f31 4e29 0e72 2a00 0000 722b 0000  ds/1N).r*...r+..
-00001c20: 0072 3600 0000 7237 0000 0072 3800 0000  .r6...r7...r8...
-00001c30: 7239 0000 0072 0d00 0000 720b 0000 0072  r9...r....r....r
-00001c40: 3b00 0000 723c 0000 0072 3d00 0000 7256  ;...r<...r=...rV
-00001c50: 0000 0072 5700 0000 723a 0000 0029 0572  ...rW...r:...).r
-00001c60: 2f00 0000 722c 0000 0072 3e00 0000 da01  /...r,...r>.....
-00001c70: 5f72 3b00 0000 7214 0000 0072 1400 0000  _r;...r....r....
-00001c80: 7215 0000 00da 1774 6573 745f 7365 635f  r......test_sec_
-00001c90: 7265 7365 745f 7061 7373 776f 7264 ff00  reset_password..
-00001ca0: 0000 733c 0000 0000 040a 030e 050e 030e  ..s<............
-00001cb0: 010e 010c 010c 0104 0102 010a 0102 fd06  ................
-00001cc0: 050e 010a 010e 0104 0102 010a 0102 fd06  ................
-00001cd0: 050e 030e 010c 010c 0104 0102 010a 0102  ................
-00001ce0: fd06 057a 2b4d 5643 5365 6375 7269 7479  ...z+MVCSecurity
-00001cf0: 5465 7374 4361 7365 2e74 6573 745f 7365  TestCase.test_se
-00001d00: 635f 7265 7365 745f 7061 7373 776f 7264  c_reset_password
-00001d10: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
-00001d20: 0006 0000 0043 0000 0073 dc00 0000 7c00  .....C...s....|.
-00001d30: 6a00 a001 a100 7d01 6401 7c00 6a00 6a02  j.....}.d.|.j.j.
-00001d40: 6402 3c00 7c00 a003 7c01 7404 7405 a103  d.<.|...|.t.t...
-00001d50: 7d02 7c01 6a06 6403 6401 6404 8d02 7d03  }.|.j.d.d.d...}.
-00001d60: 7c03 6a07 a008 6405 a101 7d04 7c00 a009  |.j...d...}.|...
-00001d70: 6406 7c04 a102 0100 7c01 6a0a 6407 740b  d.|.....|.j.d.t.
-00001d80: 6408 6408 6409 8d02 6401 640a 8d03 7d03  d.d.d...d.d...}.
-00001d90: 7c03 6a07 a008 6405 a101 7d04 7c00 a009  |.j...d...}.|...
-00001da0: 740c 7c04 a102 0100 7c01 6a0a 6407 740b  t.|.....|.j.d.t.
-00001db0: 640b 640b 6409 8d02 6401 640a 8d03 7d03  d.d.d...d.d...}.
-00001dc0: 7c03 6a07 a008 6405 a101 7d04 7c00 a00d  |.j...d...}.|...
-00001dd0: 740c 7c04 a102 0100 640c 7c00 6a00 6a02  t.|.....d.|.j.j.
-00001de0: 6402 3c00 7c01 6a0a 6407 740b 6408 6408  d.<.|.j.d.t.d.d.
-00001df0: 6409 8d02 6401 640a 8d03 7d02 7c00 a00e  d...d.d...}.|...
-00001e00: 7c01 a101 0100 640d 5300 290e 7a46 0a20  |.....d.S.).zF. 
-00001e10: 2020 2020 2020 2054 6573 7420 5365 6375         Test Secu
-00001e20: 7269 7479 2072 6573 6574 2070 6173 7377  rity reset passw
-00001e30: 6f72 6420 7769 7468 2064 6566 6175 6c74  ord with default
-00001e40: 2063 6f6d 706c 6578 6974 790a 2020 2020   complexity.    
-00001e50: 2020 2020 54da 1f46 4142 5f50 4153 5357      T..FAB_PASSW
-00001e60: 4f52 445f 434f 4d50 4c45 5849 5459 5f45  ORD_COMPLEXITY_E
-00001e70: 4e41 424c 4544 725a 0000 0072 4000 0000  NABLEDrZ...r@...
-00001e80: 7235 0000 0072 5b00 0000 725c 0000 0072  r5...r[...r\...r
-00001e90: 1100 0000 725d 0000 0072 5500 0000 7a0c  ....r]...rU...z.
-00001ea0: 5041 7373 776f 7264 3132 3321 464e 290f  PAssword123!FN).
-00001eb0: 722a 0000 0072 2b00 0000 da06 636f 6e66  r*...r+.....conf
-00001ec0: 6967 7239 0000 0072 0d00 0000 720b 0000  igr9...r....r...
-00001ed0: 0072 3600 0000 723b 0000 0072 3c00 0000  .r6...r;...r<...
-00001ee0: 723d 0000 0072 5600 0000 7257 0000 00da  r=...rV...rW....
-00001ef0: 1950 4153 5357 4f52 445f 434f 4d50 4c45  .PASSWORD_COMPLE
-00001f00: 5849 5459 5f45 5252 4f52 da0b 6173 7365  XITY_ERROR..asse
-00001f10: 7274 4e6f 7449 6e72 3a00 0000 a905 722f  rtNotInr:.....r/
-00001f20: 0000 0072 2c00 0000 725f 0000 0072 3e00  ...r,...r_...r>.
-00001f30: 0000 723b 0000 0072 1400 0000 7214 0000  ..r;...r....r...
-00001f40: 0072 1500 0000 da2a 7465 7374 5f73 6563  .r.....*test_sec
-00001f50: 5f72 6573 6574 5f70 6173 7377 6f72 645f  _reset_password_
-00001f60: 6465 6661 756c 745f 636f 6d70 6c65 7869  default_complexi
-00001f70: 7479 2c01 0000 7336 0000 0000 040a 010c  ty,...s6........
-00001f80: 030e 010e 010c 010c 0104 0102 010a 0102  ................
-00001f90: fd06 050c 020c 0204 0102 010a 0102 fd06  ................
-00001fa0: 050c 020c 030c 0104 0102 010a 0102 fd06  ................
-00001fb0: 067a 3e4d 5643 5365 6375 7269 7479 5465  .z>MVCSecurityTe
-00001fc0: 7374 4361 7365 2e74 6573 745f 7365 635f  stCase.test_sec_
-00001fd0: 7265 7365 745f 7061 7373 776f 7264 5f64  reset_password_d
-00001fe0: 6566 6175 6c74 5f63 6f6d 706c 6578 6974  efault_complexit
-00001ff0: 7963 0100 0000 0000 0000 0000 0000 0500  yc..............
-00002000: 0000 0600 0000 4300 0000 73ac 0000 007c  ......C...s....|
-00002010: 006a 00a0 01a1 007d 0164 017c 006a 006a  .j.....}.d.|.j.j
-00002020: 0264 023c 0074 037c 006a 006a 0264 033c  .d.<.t.|.j.j.d.<
-00002030: 007c 00a0 047c 0174 0574 06a1 037d 027c  .|...|.t.t...}.|
-00002040: 016a 0764 0464 0164 058d 027d 037c 036a  .j.d.d.d...}.|.j
-00002050: 08a0 0964 06a1 017d 047c 00a0 0a64 077c  ...d...}.|...d.|
-00002060: 04a1 0201 007c 016a 0b64 0874 0c64 0964  .....|.j.d.t.d.d
-00002070: 0964 0a8d 0264 0164 0b8d 037d 037c 036a  .d...d.d...}.|.j
-00002080: 08a0 0964 06a1 017d 047c 00a0 0a64 0c7c  ...d...}.|...d.|
-00002090: 04a1 0201 007c 016a 0b64 0874 0c64 0d64  .....|.j.d.t.d.d
-000020a0: 0d64 0a8d 0264 0164 0b8d 037d 037c 00a0  .d...d.d...}.|..
-000020b0: 0d7c 01a1 0101 0064 0e53 0029 0f7a 450a  .|.....d.S.).zE.
-000020c0: 2020 2020 2020 2020 5465 7374 2053 6563          Test Sec
-000020d0: 7572 6974 7920 7265 7365 7420 7061 7373  urity reset pass
-000020e0: 776f 7264 2077 6974 6820 6375 7374 6f6d  word with custom
-000020f0: 2063 6f6d 706c 6578 6974 790a 2020 2020   complexity.    
-00002100: 2020 2020 5472 6100 0000 da21 4641 425f      Tra....!FAB_
-00002110: 5041 5353 574f 5244 5f43 4f4d 504c 4558  PASSWORD_COMPLEX
-00002120: 4954 595f 5641 4c49 4441 544f 5272 5a00  ITY_VALIDATORrZ.
-00002130: 0000 7240 0000 0072 3500 0000 725b 0000  ..r@...r5...r[..
-00002140: 0072 5c00 0000 5a03 3132 3372 5d00 0000  .r\...Z.123r]...
-00002150: 7255 0000 0072 1300 0000 7211 0000 004e  rU...r....r....N
-00002160: 290e 722a 0000 0072 2b00 0000 7262 0000  ).r*...r+...rb..
-00002170: 0072 1600 0000 7239 0000 0072 0d00 0000  .r....r9...r....
-00002180: 720b 0000 0072 3600 0000 723b 0000 0072  r....r6...r;...r
-00002190: 3c00 0000 723d 0000 0072 5600 0000 7257  <...r=...rV...rW
-000021a0: 0000 0072 3a00 0000 7265 0000 0072 1400  ...r:...re...r..
-000021b0: 0000 7214 0000 0072 1500 0000 da29 7465  ..r....r.....)te
-000021c0: 7374 5f73 6563 5f72 6573 6574 5f70 6173  st_sec_reset_pas
-000021d0: 7377 6f72 645f 6375 7374 6f6d 5f63 6f6d  sword_custom_com
-000021e0: 706c 6578 6974 7954 0100 0073 2800 0000  plexityT...s(...
-000021f0: 0004 0a01 0c01 0c03 0e01 0e01 0c01 0c01  ................
-00002200: 0401 0201 0a01 02fd 0605 0c02 0c02 0401  ................
-00002210: 0201 0a01 02fd 0605 7a3d 4d56 4353 6563  ........z=MVCSec
-00002220: 7572 6974 7954 6573 7443 6173 652e 7465  urityTestCase.te
-00002230: 7374 5f73 6563 5f72 6573 6574 5f70 6173  st_sec_reset_pas
-00002240: 7377 6f72 645f 6375 7374 6f6d 5f63 6f6d  sword_custom_com
-00002250: 706c 6578 6974 7963 0100 0000 0000 0000  plexityc........
-00002260: 0000 0000 0600 0000 0b00 0000 4300 0000  ............C...
-00002270: 732c 0100 007c 006a 00a0 01a1 007d 017c  s,...|.j.....}.|
-00002280: 00a0 027c 0174 0374 04a1 037d 027c 016a  ...|.t.t...}.|.j
-00002290: 0564 0164 0264 038d 027d 037c 036a 06a0  .d.d.d...}.|.j..
-000022a0: 0764 04a1 017d 047c 00a0 0864 057c 04a1  .d...}.|...d.|..
-000022b0: 0201 007c 016a 0964 0174 0a64 0664 0764  ...|.j.d.t.d.d.d
-000022c0: 0864 0964 0a67 0164 0b64 0b64 0c8d 0764  .d.d.g.d.d.d...d
-000022d0: 0264 0d8d 037d 037c 036a 06a0 0764 04a1  .d...}.|.j...d..
-000022e0: 017d 047c 00a0 0864 0e7c 04a1 0201 007c  .}.|...d.|.....|
-000022f0: 016a 0564 0164 0264 038d 027d 037c 036a  .j.d.d.d...}.|.j
-00002300: 06a0 0764 04a1 017d 047c 00a0 0864 057c  ...d...}.|...d.|
-00002310: 04a1 0201 007c 016a 0964 0174 0a64 0664  .....|.j.d.t.d.d
-00002320: 0764 0f64 1067 0064 0b64 0b64 0c8d 0764  .d.d.g.d.d.d...d
-00002330: 0264 0d8d 037d 037c 036a 06a0 0764 04a1  .d...}.|.j...d..
-00002340: 017d 047c 00a0 0b64 0e7c 04a1 0201 007c  .}.|...d.|.....|
-00002350: 00a0 0864 117c 04a1 0201 007c 00a0 0c7c  ...d.|.....|...|
-00002360: 01a1 0101 007c 006a 0d6a 0ea0 0f74 10a1  .....|.j.j...t..
-00002370: 01a0 1174 106a 1264 086b 02a1 01a0 13a1  ...t.j.d.k......
-00002380: 007d 057c 006a 0d6a 0ea0 147c 05a1 0101  .}.|.j.j...|....
-00002390: 007c 006a 0d6a 0ea0 15a1 0001 0064 1253  .|.j.j.......d.S
-000023a0: 0029 137a 240a 2020 2020 2020 2020 5465  .).z$.        Te
-000023b0: 7374 2072 6567 6973 7465 7220 7573 6572  st register user
-000023c0: 0a20 2020 2020 2020 207a 0a2f 7573 6572  .        z./user
-000023d0: 732f 6164 6454 7240 0000 0072 3500 0000  s/addTr@...r5...
-000023e0: 7a08 4164 6420 5573 6572 da05 6669 7273  z.Add User..firs
-000023f0: 74da 046c 6173 747a 0d66 726f 6d20 7465  t..lastz.from te
-00002400: 7374 2031 2d31 7a13 7465 7374 3140 6672  st 1-1z.test1@fr
-00002410: 6f6d 7465 7374 312e 636f 6de9 0100 0000  omtest1.com.....
-00002420: 7211 0000 0029 075a 0a66 6972 7374 5f6e  r....).Z.first_n
-00002430: 616d 65da 096c 6173 745f 6e61 6d65 7254  ame..last_namerT
-00002440: 0000 00da 0565 6d61 696c da05 726f 6c65  .....email..role
-00002450: 7372 1100 0000 725e 0000 0072 5500 0000  sr....r^...rU...
-00002460: 7a09 4164 6465 6420 526f 777a 0d66 726f  z.Added Rowz.fro
-00002470: 6d20 7465 7374 2032 2d31 7a13 7465 7374  m test 2-1z.test
-00002480: 3240 6672 6f6d 7465 7374 322e 636f 6d7a  2@fromtest2.comz
-00002490: 1654 6869 7320 6669 656c 6420 6973 2072  .This field is r
-000024a0: 6571 7569 7265 644e 2916 722a 0000 0072  equiredN).r*...r
-000024b0: 2b00 0000 7239 0000 0072 0d00 0000 720b  +...r9...r....r.
-000024c0: 0000 0072 3600 0000 723b 0000 0072 3c00  ...r6...r;...r<.
-000024d0: 0000 723d 0000 0072 5600 0000 7257 0000  ..r=...rV...rW..
-000024e0: 0072 6400 0000 723a 0000 00da 0264 62da  .rd...r:.....db.
-000024f0: 0773 6573 7369 6f6e da05 7175 6572 7972  .session..queryr
-00002500: 0700 0000 da06 6669 6c74 6572 7254 0000  ......filterrT..
-00002510: 00da 0b6f 6e65 5f6f 725f 6e6f 6e65 da06  ...one_or_none..
-00002520: 6465 6c65 7465 da06 636f 6d6d 6974 2906  delete..commit).
-00002530: 722f 0000 0072 2c00 0000 725f 0000 0072  r/...r,...r_...r
-00002540: 3e00 0000 723b 0000 00da 0475 7365 7272  >...r;.....userr
-00002550: 1400 0000 7214 0000 0072 1500 0000 da12  ....r....r......
-00002560: 7465 7374 5f72 6567 6973 7465 725f 7573  test_register_us
-00002570: 6572 7101 0000 735c 0000 0000 040a 010e  erq...s\........
-00002580: 030e 010c 010c 0104 0102 0102 0102 0102  ................
-00002590: 0102 0102 0104 0102 0102 f904 0902 f506  ................
-000025a0: 0d0c 010c 030e 010c 010c 0104 0102 0102  ................
-000025b0: 0102 0102 0102 0102 0102 0102 0102 f904  ................
-000025c0: 0902 f506 0d0c 010c 010c 010a 030e 0108  ................
-000025d0: ff06 ff02 050e 017a 264d 5643 5365 6375  .......z&MVCSecu
-000025e0: 7269 7479 5465 7374 4361 7365 2e74 6573  rityTestCase.tes
-000025f0: 745f 7265 6769 7374 6572 5f75 7365 7229  t_register_user)
-00002600: 1572 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00002610: 7229 0000 0072 3f00 0000 7248 0000 0072  r)...r?...rH...r
-00002620: 4c00 0000 724d 0000 0072 4e00 0000 724f  L...rM...rN...rO
-00002630: 0000 0072 5000 0000 7251 0000 0072 5200  ...rP...rQ...rR.
-00002640: 0000 7253 0000 0072 5800 0000 7259 0000  ..rS...rX...rY..
-00002650: 0072 6000 0000 7266 0000 0072 6800 0000  .r`...rf...rh...
-00002660: 7277 0000 00da 0d5f 5f63 6c61 7373 6365  rw.....__classce
-00002670: 6c6c 5f5f 7214 0000 0072 1400 0000 7230  ll__r....r....r0
-00002680: 0000 0072 1500 0000 7217 0000 0020 0000  ...r....r.... ..
-00002690: 0073 2200 0000 0801 0c1f 081e 080a 080e  .s".............
-000026a0: 080e 080e 080e 080e 080e 080e 080e 0814  ................
-000026b0: 0813 082d 0828 081d 7217 0000 0029 195a  ...-.(..r....).Z
-000026c0: 1066 6c61 736b 5f61 7070 6275 696c 6465  .flask_appbuilde
-000026d0: 7272 0200 0000 da1b 666c 6173 6b5f 6170  rr......flask_ap
-000026e0: 7062 7569 6c64 6572 2e65 7863 6570 7469  pbuilder.excepti
-000026f0: 6f6e 7372 0400 0000 5a24 666c 6173 6b5f  onsr....Z$flask_
-00002700: 6170 7062 7569 6c64 6572 2e6d 6f64 656c  appbuilder.model
-00002710: 732e 7371 6c61 2e66 696c 7465 7273 7205  s.sqla.filtersr.
-00002720: 0000 00da 2666 6c61 736b 5f61 7070 6275  ....&flask_appbu
-00002730: 696c 6465 722e 6d6f 6465 6c73 2e73 716c  ilder.models.sql
-00002740: 612e 696e 7465 7266 6163 6572 0600 0000  a.interfacer....
-00002750: 5a25 666c 6173 6b5f 6170 7062 7569 6c64  Z%flask_appbuild
-00002760: 6572 2e73 6563 7572 6974 792e 7371 6c61  er.security.sqla
-00002770: 2e6d 6f64 656c 7372 0700 0000 da04 6261  .modelsr......ba
-00002780: 7365 7209 0000 00da 0563 6f6e 7374 720a  ser......constr.
-00002790: 0000 0072 0b00 0000 720c 0000 0072 0d00  ...r....r....r..
-000027a0: 0000 720e 0000 005a 0b73 716c 612e 6d6f  ..r....Z.sqla.mo
-000027b0: 6465 6c73 720f 0000 0072 1000 0000 7263  delsr....r....rc
-000027c0: 0000 00da 0373 7472 7216 0000 0072 1700  .....strr....r..
-000027d0: 0000 7214 0000 0072 1400 0000 7214 0000  ..r....r....r...
-000027e0: 0072 1500 0000 da08 3c6d 6f64 756c 653e  .r......<module>
-000027f0: 0100 0000 7316 0000 000c 010c 010c 010c  ....s...........
-00002800: 010c 020c 011c 0710 0302 ff02 0710 08    ...............
+00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
+00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
+00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
+00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0b 5a0b  m.Z...d.d.l.m.Z.
+00000070: 0100 6400 6406 6c0c 6d0d 5a0d 0100 6407  ..d.d.l.m.Z...d.
+00000080: 6408 6c0e 6d0f 5a0f 0100 6407 6409 6c10  d.l.m.Z...d.d.l.
+00000090: 6d11 5a11 6d12 5a12 6d13 5a13 6d14 5a14  m.Z.m.Z.m.Z.m.Z.
+000000a0: 6d15 5a15 0100 6407 640a 6c16 6d17 5a17  m.Z...d.d.l.m.Z.
+000000b0: 6d18 5a18 0100 640b 5a19 651a 640c 640d  m.Z...d.Z.e.d.d.
+000000c0: 9c02 640e 640f 8404 5a1b 4700 6410 6411  ..d.d...Z.G.d.d.
+000000d0: 8400 6411 650f 8303 5a1c 640c 5300 2912  ..d.e...Z.d.S.).
+000000e0: e900 0000 0029 03da 094d 6167 6963 4d6f  .....)...MagicMo
+000000f0: 636b da04 4d6f 636b da05 7061 7463 6829  ck..Mock..patch)
+00000100: 01da 094d 6f64 656c 5669 6577 a901 da21  ...ModelView...!
+00000110: 5061 7373 776f 7264 436f 6d70 6c65 7869  PasswordComplexi
+00000120: 7479 5661 6c69 6461 7469 6f6e 4572 726f  tyValidationErro
+00000130: 7229 01da 0b46 696c 7465 7245 7175 616c  r)...FilterEqual
+00000140: 2901 da0d 5351 4c41 496e 7465 7266 6163  )...SQLAInterfac
+00000150: 6529 01da 0455 7365 72e9 0200 0000 2901  e)...User.....).
+00000160: da0f 4261 7365 4d56 4354 6573 7443 6173  ..BaseMVCTestCas
+00000170: 6529 05da 1449 4e56 414c 4944 5f4c 4f47  e)...INVALID_LOG
+00000180: 494e 5f53 5452 494e 47da 0e50 4153 5357  IN_STRING..PASSW
+00000190: 4f52 445f 4144 4d49 4eda 1150 4153 5357  ORD_ADMIN..PASSW
+000001a0: 4f52 445f 5245 4144 4f4e 4c59 da0e 5553  ORD_READONLY..US
+000001b0: 4552 4e41 4d45 5f41 444d 494e da11 5553  ERNAME_ADMIN..US
+000001c0: 4552 4e41 4d45 5f52 4541 444f 4e4c 5929  ERNAME_READONLY)
+000001d0: 02da 064d 6f64 656c 31da 064d 6f64 656c  ...Model1..Model
+000001e0: 327a 7e4d 7573 7420 6861 7665 2061 7420  2z~Must have at 
+000001f0: 6c65 6173 7420 7477 6f20 6361 7069 7461  least two capita
+00000200: 6c20 6c65 7474 6572 732c 206f 6e65 2073  l letters, one s
+00000210: 7065 6369 616c 2063 6861 7261 6374 6572  pecial character
+00000220: 2c20 7477 6f20 6469 6769 7473 2c20 7468  , two digits, th
+00000230: 7265 6520 6c6f 7765 7220 6361 7365 206c  ree lower case l
+00000240: 6574 7465 7273 2061 6e64 2061 206d 696e  etters and a min
+00000250: 696d 616c 206c 656e 6774 6820 6f66 2031  imal length of 1
+00000260: 304e 2902 da08 7061 7373 776f 7264 da06  0N)...password..
+00000270: 7265 7475 726e 6301 0000 0000 0000 0000  returnc.........
+00000280: 0000 0001 0000 0002 0000 0043 0000 0073  ...........C...s
+00000290: 1400 0000 7c00 6401 6b03 7210 7400 6402  ....|.d.k.r.t.d.
+000002a0: 8301 8201 6403 5300 2904 7a37 0a20 2020  ....d.S.).z7.   
+000002b0: 2041 2073 696d 706c 6973 7469 6320 6578   A simplistic ex
+000002c0: 616d 706c 6520 666f 7220 6120 7061 7373  ample for a pass
+000002d0: 776f 7264 2076 616c 6964 6174 6f72 0a20  word validator. 
+000002e0: 2020 2072 1400 0000 fa19 5061 7373 776f     r......Passwo
+000002f0: 7264 206d 7573 7420 6265 2070 6173 7377  rd must be passw
+00000300: 6f72 644e 7206 0000 0029 0172 1400 0000  ordNr....).r....
+00000310: a900 7217 0000 00fa 652f 5573 6572 732f  ..r.....e/Users/
+00000320: 6470 6761 7370 6172 2f77 6f72 6b61 7265  dpgaspar/workare
+00000330: 612f 7072 6573 6574 2f46 6c61 736b 2d41  a/preset/Flask-A
+00000340: 7070 4275 696c 6465 722f 666c 6173 6b5f  ppBuilder/flask_
+00000350: 6170 7062 7569 6c64 6572 2f74 6573 7473  appbuilder/tests
+00000360: 2f73 6563 7572 6974 792f 7465 7374 5f6d  /security/test_m
+00000370: 7663 5f73 6563 7572 6974 792e 7079 da19  vc_security.py..
+00000380: 6375 7374 6f6d 5f70 6173 7377 6f72 645f  custom_password_
+00000390: 7661 6c69 6461 746f 721a 0000 0073 0400  validator....s..
+000003a0: 0000 0004 0801 7219 0000 0063 0000 0000  ......r....c....
+000003b0: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+000003c0: 0000 0000 73b4 0000 0065 005a 0164 005a  ....s....e.Z.d.Z
+000003d0: 0287 0066 0164 0164 0284 085a 0364 0364  ...f.d.d...Z.d.d
+000003e0: 0484 005a 0464 0564 0684 005a 0564 0764  ...Z.d.d...Z.d.d
+000003f0: 0884 005a 0664 0964 0a84 005a 0764 0b64  ...Z.d.d...Z.d.d
+00000400: 0c84 005a 0864 0d64 0e84 005a 0964 0f64  ...Z.d.d...Z.d.d
+00000410: 1084 005a 0a64 1164 1284 005a 0b64 1364  ...Z.d.d...Z.d.d
+00000420: 1484 005a 0c64 1564 1684 005a 0d64 1764  ...Z.d.d...Z.d.d
+00000430: 1884 005a 0e64 1964 1a84 005a 0f64 1b64  ...Z.d.d...Z.d.d
+00000440: 1c84 005a 1064 1d64 1e84 005a 1164 1f64  ...Z.d.d...Z.d.d
+00000450: 2084 005a 1264 2164 2284 005a 1364 2364   ..Z.d!d"..Z.d#d
+00000460: 2484 005a 1464 2564 2684 005a 1564 2764  $..Z.d%d&..Z.d'd
+00000470: 2884 005a 1687 0004 005a 1753 0029 29da  (..Z.....Z.S.)).
+00000480: 134d 5643 5365 6375 7269 7479 5465 7374  .MVCSecurityTest
+00000490: 4361 7365 6301 0000 0000 0000 0000 0000  Casec...........
+000004a0: 0002 0000 0005 0000 0003 0000 0073 5e00  .............s^.
+000004b0: 0000 7400 8300 a001 a100 0100 7c00 6a02  ..t.........|.j.
+000004c0: a003 a100 7c00 5f04 4700 6401 6402 8400  ....|._.G.d.d...
+000004d0: 6402 7405 8303 8900 7c00 6a06 a007 8800  d.t.....|.j.....
+000004e0: 6403 a102 0100 4700 8700 6601 6404 6405  d.....G...f.d.d.
+000004f0: 8408 6405 7405 8303 7d01 7c00 6a06 6a07  ..d.t...}.|.j.j.
+00000500: 7c01 6406 6406 6407 8d03 0100 6400 5300  |.d.d.d.....d.S.
+00000510: 2908 4e63 0000 0000 0000 0000 0000 0000  ).Nc............
+00000520: 0000 0000 0500 0000 4000 0000 734a 0000  ........@...sJ..
+00000530: 0065 005a 0164 005a 0265 0365 0483 015a  .e.Z.d.Z.e.e...Z
+00000540: 0564 0164 0264 0364 0464 0567 055a 0664  .d.d.d.d.d.g.Z.d
+00000550: 0664 0365 0764 0767 0367 0169 015a 0864  .d.e.d.g.g.i.Z.d
+00000560: 0664 0365 0764 0867 0367 0169 015a 0964  .d.e.d.g.g.i.Z.d
+00000570: 0364 0567 025a 0a64 0953 0029 0a7a 2d4d  .d.g.Z.d.S.).z-M
+00000580: 5643 5365 6375 7269 7479 5465 7374 4361  VCSecurityTestCa
+00000590: 7365 2e73 6574 5570 2e3c 6c6f 6361 6c73  se.setUp.<locals
+000005a0: 3e2e 4d6f 6465 6c32 5669 6577 da0d 6669  >.Model2View..fi
+000005b0: 656c 645f 696e 7465 6765 725a 0b66 6965  eld_integerZ.fie
+000005c0: 6c64 5f66 6c6f 6174 da0c 6669 656c 645f  ld_float..field_
+000005d0: 7374 7269 6e67 5a0c 6669 656c 645f 6d65  stringZ.field_me
+000005e0: 7468 6f64 7a12 6772 6f75 702e 6669 656c  thodz.group.fiel
+000005f0: 645f 7374 7269 6e67 da05 6772 6f75 705a  d_string..groupZ
+00000600: 0574 6573 7431 5a05 7465 7374 304e 290b  .test1Z.test0N).
+00000610: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
+00000620: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
+00000630: 6d65 5f5f 7209 0000 0072 1300 0000 da09  me__r....r......
+00000640: 6461 7461 6d6f 6465 6cda 0c6c 6973 745f  datamodel..list_
+00000650: 636f 6c75 6d6e 7372 0800 0000 da1a 6564  columnsr......ed
+00000660: 6974 5f66 6f72 6d5f 7175 6572 795f 7265  it_form_query_re
+00000670: 6c5f 6669 656c 6473 da19 6164 645f 666f  l_fields..add_fo
+00000680: 726d 5f71 7565 7279 5f72 656c 5f66 6965  rm_query_rel_fie
+00000690: 6c64 73da 0d6f 7264 6572 5f63 6f6c 756d  lds..order_colum
+000006a0: 6e73 7217 0000 0072 1700 0000 7217 0000  nsr....r....r...
+000006b0: 0072 1800 0000 da0a 4d6f 6465 6c32 5669  .r......Model2Vi
+000006c0: 6577 2700 0000 731c 0000 0008 0108 0202  ew'...s.........
+000006d0: 0102 0102 0102 0102 fb04 0802 000a ff04  ................
+000006e0: 0402 000a ff04 0472 2600 0000 7213 0000  .......r&...r...
+000006f0: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00000700: 0000 0200 0000 0000 0000 7322 0000 0065  ..........s"...e
+00000710: 005a 0164 005a 0265 0365 0483 015a 0594  .Z.d.Z.e.e...Z..
+00000720: 0067 015a 0664 0164 0267 025a 0764 0353  .g.Z.d.d.g.Z.d.S
+00000730: 0029 047a 2d4d 5643 5365 6375 7269 7479  .).z-MVCSecurity
+00000740: 5465 7374 4361 7365 2e73 6574 5570 2e3c  TestCase.setUp.<
+00000750: 6c6f 6361 6c73 3e2e 4d6f 6465 6c31 5669  locals>.Model1Vi
+00000760: 6577 721c 0000 0072 1b00 0000 4e29 0872  ewr....r....N).r
+00000770: 1e00 0000 721f 0000 0072 2000 0000 7209  ....r....r ...r.
+00000780: 0000 0072 1200 0000 7221 0000 00da 0d72  ...r....r!.....r
+00000790: 656c 6174 6564 5f76 6965 7773 7222 0000  elated_viewsr"..
+000007a0: 0072 1700 0000 a901 7226 0000 0072 1700  .r......r&...r..
+000007b0: 0000 7218 0000 00da 0a4d 6f64 656c 3156  ..r......Model1V
+000007c0: 6965 773b 0000 0073 0600 0000 0801 0801  iew;...s........
+000007d0: 0601 7229 0000 0072 1200 0000 2901 da08  ..r)...r....)...
+000007e0: 6361 7465 676f 7279 2908 da05 7375 7065  category)...supe
+000007f0: 72da 0573 6574 5570 da03 6170 70da 0b74  r..setUp..app..t
+00000800: 6573 745f 636c 6965 6e74 da06 636c 6965  est_client..clie
+00000810: 6e74 7205 0000 00da 0a61 7070 6275 696c  ntr......appbuil
+00000820: 6465 72da 0861 6464 5f76 6965 7729 02da  der..add_view)..
+00000830: 0473 656c 6672 2900 0000 a901 da09 5f5f  .selfr).......__
+00000840: 636c 6173 735f 5f72 2800 0000 7218 0000  class__r(...r...
+00000850: 0072 2c00 0000 2300 0000 730c 0000 0000  .r,...#...s.....
+00000860: 010a 010c 0210 120e 0214 057a 194d 5643  ...........z.MVC
+00000870: 5365 6375 7269 7479 5465 7374 4361 7365  SecurityTestCase
+00000880: 2e73 6574 5570 6301 0000 0000 0000 0000  .setUpc.........
+00000890: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
+000008a0: e400 0000 7c00 6a00 a001 6401 a101 7d01  ....|.j...d...}.
+000008b0: 7c00 a002 7c01 6a03 6402 a102 0100 7c00  |...|.j.d.....|.
+000008c0: 6a00 a001 6403 a101 7d01 7c00 a002 7c01  j...d...}.|...|.
+000008d0: 6a03 6402 a102 0100 7c00 a004 7c00 6a00  j.d.....|...|.j.
+000008e0: 7405 7406 a103 0100 7c00 6a00 a001 6401  t.t.....|.j...d.
+000008f0: a101 7d01 7c00 a002 7c01 6a03 6404 a102  ..}.|...|.j.d...
+00000900: 0100 7c00 6a00 a001 6403 a101 7d01 7c00  ..|.j...d...}.|.
+00000910: a002 7c01 6a03 6404 a102 0100 7c00 a007  ..|.j.d.....|...
+00000920: 7c00 6a00 a101 0100 7c00 6a00 a001 6401  |.j.....|.j...d.
+00000930: a101 7d01 7c00 a002 7c01 6a03 6402 a102  ..}.|...|.j.d...
+00000940: 0100 7c00 6a00 a001 6403 a101 7d01 7c00  ..|.j...d...}.|.
+00000950: a002 7c01 6a03 6402 a102 0100 7c00 a004  ..|.j.d.....|...
+00000960: 7c00 6a00 7405 6405 a103 7d01 7c01 6a08  |.j.t.d...}.|.j.
+00000970: a009 6406 a101 7d02 7c00 a00a 740b 7c02  ..d...}.|...t.|.
+00000980: a102 0100 6407 5300 2908 7a4c 0a20 2020  ....d.S.).zL.   
+00000990: 2020 2020 2054 6573 7420 5365 6375 7269       Test Securi
+000009a0: 7479 204c 6f67 696e 2c20 4c6f 676f 7574  ty Login, Logout
+000009b0: 2c20 696e 7661 6c69 6420 6c6f 6769 6e2c  , invalid login,
+000009c0: 2069 6e76 616c 6964 2061 6363 6573 730a   invalid access.
+000009d0: 2020 2020 2020 2020 fa11 2f6d 6f64 656c          ../model
+000009e0: 3176 6965 772f 6c69 7374 2fe9 2e01 0000  1view/list/.....
+000009f0: 7a11 2f6d 6f64 656c 3276 6965 772f 6c69  z./model2view/li
+00000a00: 7374 2fe9 c800 0000 5a0e 7772 6f6e 675f  st/.....Z.wrong_
+00000a10: 7061 7373 776f 7264 fa05 7574 662d 384e  password..utf-8N
+00000a20: 290c 722f 0000 00da 0367 6574 da0b 6173  ).r/.....get..as
+00000a30: 7365 7274 4571 7561 6cda 0b73 7461 7475  sertEqual..statu
+00000a40: 735f 636f 6465 da0d 6272 6f77 7365 725f  s_code..browser_
+00000a50: 6c6f 6769 6e72 1000 0000 720e 0000 00da  loginr....r.....
+00000a60: 0e62 726f 7773 6572 5f6c 6f67 6f75 74da  .browser_logout.
+00000a70: 0464 6174 61da 0664 6563 6f64 65da 0861  .data..decode..a
+00000a80: 7373 6572 7449 6e72 0d00 0000 2903 7232  ssertInr....).r2
+00000a90: 0000 00da 0272 7672 3e00 0000 7217 0000  .....rvr>...r...
+00000aa0: 0072 1700 0000 7218 0000 00da 0e74 6573  .r....r......tes
+00000ab0: 745f 7365 635f 6c6f 6769 6e42 0000 0073  t_sec_loginB...s
+00000ac0: 2200 0000 0006 0c01 0e01 0c01 0e03 1001  "...............
+00000ad0: 0c01 0e01 0c01 0e03 0c01 0c01 0e01 0c01  ................
+00000ae0: 0e03 1001 0c01 7a22 4d56 4353 6563 7572  ......z"MVCSecur
+00000af0: 6974 7954 6573 7443 6173 652e 7465 7374  ityTestCase.test
+00000b00: 5f73 6563 5f6c 6f67 696e 6301 0000 0000  _sec_loginc.....
+00000b10: 0000 0000 0000 0002 0000 0006 0000 0043  ...............C
+00000b20: 0000 0073 3200 0000 7c00 a000 7c00 6a01  ...s2...|...|.j.
+00000b30: a101 0100 7c00 6a02 7c00 6a01 7403 7404  ....|.j.|.j.t.t.
+00000b40: 6401 6402 8d04 7d01 7c01 6a05 6403 6b02  d.d...}.|.j.d.k.
+00000b50: 732e 7406 8201 6404 5300 2905 7a2b 0a20  s.t...d.S.).z+. 
+00000b60: 2020 2020 2020 2054 6573 7420 5365 6375         Test Secu
+00000b70: 7269 7479 206e 6f20 6e65 7874 2055 524c  rity no next URL
+00000b80: 0a20 2020 2020 2020 2046 a901 da10 666f  .        F....fo
+00000b90: 6c6c 6f77 5f72 6564 6972 6563 7473 fa01  llow_redirects..
+00000ba0: 2f4e a907 723d 0000 0072 2f00 0000 723c  /N..r=...r/...r<
+00000bb0: 0000 0072 1000 0000 720e 0000 00da 086c  ...r....r......l
+00000bc0: 6f63 6174 696f 6eda 0e41 7373 6572 7469  ocation..Asserti
+00000bd0: 6f6e 4572 726f 72a9 0272 3200 0000 da08  onError..r2.....
+00000be0: 7265 7370 6f6e 7365 7217 0000 0072 1700  responser....r..
+00000bf0: 0000 7218 0000 00da 1974 6573 745f 6462  ..r......test_db
+00000c00: 5f6c 6f67 696e 5f6e 6f5f 6e65 7874 5f75  _login_no_next_u
+00000c10: 726c 6000 0000 7310 0000 0000 040c 0104  rl`...s.........
+00000c20: 0104 0002 0002 0002 ff06 037a 2d4d 5643  ...........z-MVC
+00000c30: 5365 6375 7269 7479 5465 7374 4361 7365  SecurityTestCase
+00000c40: 2e74 6573 745f 6462 5f6c 6f67 696e 5f6e  .test_db_login_n
+00000c50: 6f5f 6e65 7874 5f75 726c 6301 0000 0000  o_next_urlc.....
+00000c60: 0000 0000 0000 0002 0000 0007 0000 0043  ...............C
+00000c70: 0000 0073 3400 0000 7c00 a000 7c00 6a01  ...s4...|...|.j.
+00000c80: a101 0100 7c00 6a02 7c00 6a01 7403 7404  ....|.j.|.j.t.t.
+00000c90: 6401 6402 6403 8d05 7d01 7c01 6a05 6401  d.d.d...}.|.j.d.
+00000ca0: 6b02 7330 7406 8201 6404 5300 2905 7a36  k.s0t...d.S.).z6
+00000cb0: 0a20 2020 2020 2020 2054 6573 7420 5365  .        Test Se
+00000cc0: 6375 7269 7479 2076 616c 6964 2070 6172  curity valid par
+00000cd0: 7469 616c 206e 6578 7420 5552 4c0a 2020  tial next URL.  
+00000ce0: 2020 2020 2020 fa0c 2f75 7365 7273 2f6c        ../users/l
+00000cf0: 6973 742f 46a9 02da 086e 6578 745f 7572  ist/F....next_ur
+00000d00: 6c72 4400 0000 4e72 4600 0000 7249 0000  lrD...NrF...rI..
+00000d10: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00000d20: da1c 7465 7374 5f64 625f 6c6f 6769 6e5f  ..test_db_login_
+00000d30: 7661 6c69 645f 6e65 7874 5f75 726c 6a00  valid_next_urlj.
+00000d40: 0000 7312 0000 0000 040c 0104 0104 0102  ..s.............
+00000d50: 0102 0102 0102 fb06 077a 304d 5643 5365  .........z0MVCSe
+00000d60: 6375 7269 7479 5465 7374 4361 7365 2e74  curityTestCase.t
+00000d70: 6573 745f 6462 5f6c 6f67 696e 5f76 616c  est_db_login_val
+00000d80: 6964 5f6e 6578 745f 7572 6c63 0100 0000  id_next_urlc....
+00000d90: 0000 0000 0000 0000 0200 0000 0700 0000  ................
+00000da0: 4300 0000 7334 0000 007c 00a0 007c 006a  C...s4...|...|.j
+00000db0: 01a1 0101 007c 006a 027c 006a 0174 0374  .....|.j.|.j.t.t
+00000dc0: 0464 0164 0264 038d 057d 017c 016a 0564  .d.d.d...}.|.j.d
+00000dd0: 016b 0273 3074 0682 0164 0453 0029 057a  .k.s0t...d.S.).z
+00000de0: 3a0a 2020 2020 2020 2020 5465 7374 2053  :.        Test S
+00000df0: 6563 7572 6974 7920 7661 6c69 6420 6874  ecurity valid ht
+00000e00: 7470 2073 6368 656d 6520 6e65 7874 2055  tp scheme next U
+00000e10: 524c 0a20 2020 2020 2020 207a 1568 7474  RL.        z.htt
+00000e20: 703a 2f2f 6c6f 6361 6c68 6f73 742f 7061  p://localhost/pa
+00000e30: 7468 4672 4d00 0000 4e72 4600 0000 7249  thFrM...NrF...rI
+00000e40: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00000e50: 0000 da23 7465 7374 5f64 625f 6c6f 6769  ...#test_db_logi
+00000e60: 6e5f 7661 6c69 645f 6874 7470 5f73 6368  n_valid_http_sch
+00000e70: 656d 655f 7572 6c78 0000 0073 1200 0000  eme_urlx...s....
+00000e80: 0004 0c01 0401 0401 0201 0201 0201 02fb  ................
+00000e90: 0607 7a37 4d56 4353 6563 7572 6974 7954  ..z7MVCSecurityT
+00000ea0: 6573 7443 6173 652e 7465 7374 5f64 625f  estCase.test_db_
+00000eb0: 6c6f 6769 6e5f 7661 6c69 645f 6874 7470  login_valid_http
+00000ec0: 5f73 6368 656d 655f 7572 6c63 0100 0000  _scheme_urlc....
+00000ed0: 0000 0000 0000 0000 0200 0000 0700 0000  ................
+00000ee0: 4300 0000 7334 0000 007c 00a0 007c 006a  C...s4...|...|.j
+00000ef0: 01a1 0101 007c 006a 027c 006a 0174 0374  .....|.j.|.j.t.t
+00000f00: 0464 0164 0264 038d 057d 017c 016a 0564  .d.d.d...}.|.j.d
+00000f10: 016b 0273 3074 0682 0164 0453 0029 057a  .k.s0t...d.S.).z
+00000f20: 3b0a 2020 2020 2020 2020 5465 7374 2053  ;.        Test S
+00000f30: 6563 7572 6974 7920 7661 6c69 6420 6874  ecurity valid ht
+00000f40: 7470 7320 7363 6865 6d65 206e 6578 7420  tps scheme next 
+00000f50: 5552 4c0a 2020 2020 2020 2020 7a16 6874  URL.        z.ht
+00000f60: 7470 733a 2f2f 6c6f 6361 6c68 6f73 742f  tps://localhost/
+00000f70: 7061 7468 4672 4d00 0000 4e72 4600 0000  pathFrM...NrF...
+00000f80: 7249 0000 0072 1700 0000 7217 0000 0072  rI...r....r....r
+00000f90: 1800 0000 da24 7465 7374 5f64 625f 6c6f  .....$test_db_lo
+00000fa0: 6769 6e5f 7661 6c69 645f 6874 7470 735f  gin_valid_https_
+00000fb0: 7363 6865 6d65 5f75 726c 8600 0000 7312  scheme_url....s.
+00000fc0: 0000 0000 040c 0104 0104 0102 0102 0102  ................
+00000fd0: 0102 fb06 077a 384d 5643 5365 6375 7269  .....z8MVCSecuri
+00000fe0: 7479 5465 7374 4361 7365 2e74 6573 745f  tyTestCase.test_
+00000ff0: 6462 5f6c 6f67 696e 5f76 616c 6964 5f68  db_login_valid_h
+00001000: 7474 7073 5f73 6368 656d 655f 7572 6c63  ttps_scheme_urlc
+00001010: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00001020: 0700 0000 4300 0000 7334 0000 007c 00a0  ....C...s4...|..
+00001030: 007c 006a 01a1 0101 007c 006a 027c 006a  .|.j.....|.j.|.j
+00001040: 0174 0374 0464 0164 0264 038d 057d 017c  .t.t.d.d.d...}.|
+00001050: 016a 0564 046b 0273 3074 0682 0164 0553  .j.d.k.s0t...d.S
+00001060: 0029 067a 390a 2020 2020 2020 2020 5465  .).z9.        Te
+00001070: 7374 2053 6563 7572 6974 7920 696e 7661  st Security inva
+00001080: 6c69 6420 6578 7465 726e 616c 206e 6578  lid external nex
+00001090: 7420 5552 4c0a 2020 2020 2020 2020 7a12  t URL.        z.
+000010a0: 6874 7470 733a 2f2f 676f 6f67 6c65 2e63  https://google.c
+000010b0: 6f6d 4672 4d00 0000 7245 0000 004e 7246  omFrM...rE...NrF
+000010c0: 0000 0072 4900 0000 7217 0000 0072 1700  ...rI...r....r..
+000010d0: 0000 7218 0000 00da 2774 6573 745f 6462  ..r.....'test_db
+000010e0: 5f6c 6f67 696e 5f69 6e76 616c 6964 5f65  _login_invalid_e
+000010f0: 7874 6572 6e61 6c5f 6e65 7874 5f75 726c  xternal_next_url
+00001100: 9400 0000 7312 0000 0000 040c 0104 0104  ....s...........
+00001110: 0102 0102 0102 0102 fb06 077a 3b4d 5643  ...........z;MVC
+00001120: 5365 6375 7269 7479 5465 7374 4361 7365  SecurityTestCase
+00001130: 2e74 6573 745f 6462 5f6c 6f67 696e 5f69  .test_db_login_i
+00001140: 6e76 616c 6964 5f65 7874 6572 6e61 6c5f  nvalid_external_
+00001150: 6e65 7874 5f75 726c 6301 0000 0000 0000  next_urlc.......
+00001160: 0000 0000 0002 0000 0007 0000 0043 0000  .............C..
+00001170: 0073 3400 0000 7c00 a000 7c00 6a01 a101  .s4...|...|.j...
+00001180: 0100 7c00 6a02 7c00 6a01 7403 7404 6401  ..|.j.|.j.t.t.d.
+00001190: 6402 6403 8d05 7d01 7c01 6a05 6404 6b02  d.d...}.|.j.d.k.
+000011a0: 7330 7406 8201 6405 5300 2906 7a37 0a20  s0t...d.S.).z7. 
+000011b0: 2020 2020 2020 2054 6573 7420 5365 6375         Test Secu
+000011c0: 7269 7479 2069 6e76 616c 6964 2073 6368  rity invalid sch
+000011d0: 656d 6520 6e65 7874 2055 524c 0a20 2020  eme next URL.   
+000011e0: 2020 2020 207a 0c66 7470 3a2f 2f73 616d       z.ftp://sam
+000011f0: 706c 6546 724d 0000 0072 4500 0000 4e72  pleFrM...rE...Nr
+00001200: 4600 0000 7249 0000 0072 1700 0000 7217  F...rI...r....r.
+00001210: 0000 0072 1800 0000 da25 7465 7374 5f64  ...r.....%test_d
+00001220: 625f 6c6f 6769 6e5f 696e 7661 6c69 645f  b_login_invalid_
+00001230: 7363 6865 6d65 5f6e 6578 745f 7572 6ca2  scheme_next_url.
+00001240: 0000 0073 1200 0000 0004 0c01 0401 0401  ...s............
+00001250: 0201 0201 0201 02fb 0607 7a39 4d56 4353  ..........z9MVCS
+00001260: 6563 7572 6974 7954 6573 7443 6173 652e  ecurityTestCase.
+00001270: 7465 7374 5f64 625f 6c6f 6769 6e5f 696e  test_db_login_in
+00001280: 7661 6c69 645f 7363 6865 6d65 5f6e 6578  valid_scheme_nex
+00001290: 745f 7572 6c63 0100 0000 0000 0000 0000  t_urlc..........
+000012a0: 0000 0200 0000 0700 0000 4300 0000 7334  ..........C...s4
+000012b0: 0000 007c 00a0 007c 006a 01a1 0101 007c  ...|...|.j.....|
+000012c0: 006a 027c 006a 0174 0374 0464 0164 0264  .j.|.j.t.t.d.d.d
+000012d0: 038d 057d 017c 016a 0564 046b 0273 3074  ...}.|.j.d.k.s0t
+000012e0: 0682 0164 0553 0029 067a 470a 2020 2020  ...d.S.).zG.    
+000012f0: 2020 2020 5465 7374 2053 6563 7572 6974      Test Securit
+00001300: 7920 696e 7661 6c69 6420 7061 7468 2074  y invalid path t
+00001310: 6f20 6c6f 6361 6c68 6f73 7420 6669 6c65  o localhost file
+00001320: 206e 6578 7420 5552 4c0a 2020 2020 2020   next URL.      
+00001330: 2020 7a0c 6669 6c65 3a2f 2f2f 7061 7468    z.file:///path
+00001340: 4672 4d00 0000 7245 0000 004e 7246 0000  FrM...rE...NrF..
+00001350: 0072 4900 0000 7217 0000 0072 1700 0000  .rI...r....r....
+00001360: 7218 0000 00da 2d74 6573 745f 6462 5f6c  r.....-test_db_l
+00001370: 6f67 696e 5f69 6e76 616c 6964 5f6c 6f63  ogin_invalid_loc
+00001380: 616c 686f 7374 5f66 696c 655f 6e65 7874  alhost_file_next
+00001390: 5f75 726c b000 0000 7312 0000 0000 040c  _url....s.......
+000013a0: 0104 0104 0102 0102 0102 0102 fb06 077a  ...............z
+000013b0: 414d 5643 5365 6375 7269 7479 5465 7374  AMVCSecurityTest
+000013c0: 4361 7365 2e74 6573 745f 6462 5f6c 6f67  Case.test_db_log
+000013d0: 696e 5f69 6e76 616c 6964 5f6c 6f63 616c  in_invalid_local
+000013e0: 686f 7374 5f66 696c 655f 6e65 7874 5f75  host_file_next_u
+000013f0: 726c 6301 0000 0000 0000 0000 0000 0002  rlc.............
+00001400: 0000 0007 0000 0043 0000 0073 3400 0000  .......C...s4...
+00001410: 7c00 a000 7c00 6a01 a101 0100 7c00 6a02  |...|.j.....|.j.
+00001420: 7c00 6a01 7403 7404 6401 6402 6403 8d05  |.j.t.t.d.d.d...
+00001430: 7d01 7c01 6a05 6404 6b02 7330 7406 8201  }.|.j.d.k.s0t...
+00001440: 6405 5300 2906 7a4f 0a20 2020 2020 2020  d.S.).zO.       
+00001450: 2054 6573 7420 5365 6375 7269 7479 2069   Test Security i
+00001460: 6e76 616c 6964 206e 6578 7420 5552 4c20  nvalid next URL 
+00001470: 7769 7468 206e 6f20 6e65 746c 6f63 2062  with no netloc b
+00001480: 7574 2077 6974 6820 7363 6865 6d65 0a20  ut with scheme. 
+00001490: 2020 2020 2020 207a 1368 7474 703a 2f2f         z.http://
+000014a0: 2f73 616d 706c 652e 636f 6d20 4672 4d00  /sample.com FrM.
+000014b0: 0000 7245 0000 004e 7246 0000 0072 4900  ..rE...NrF...rI.
+000014c0: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
+000014d0: 00da 3474 6573 745f 6462 5f6c 6f67 696e  ..4test_db_login
+000014e0: 5f69 6e76 616c 6964 5f6e 6f5f 6e65 746c  _invalid_no_netl
+000014f0: 6f63 5f77 6974 685f 7363 6865 6d65 5f6e  oc_with_scheme_n
+00001500: 6578 745f 7572 6cbe 0000 0073 1200 0000  ext_url....s....
+00001510: 0004 0c01 0401 0401 0201 0201 0201 02fb  ................
+00001520: 0607 7a48 4d56 4353 6563 7572 6974 7954  ..zHMVCSecurityT
+00001530: 6573 7443 6173 652e 7465 7374 5f64 625f  estCase.test_db_
+00001540: 6c6f 6769 6e5f 696e 7661 6c69 645f 6e6f  login_invalid_no
+00001550: 5f6e 6574 6c6f 635f 7769 7468 5f73 6368  _netloc_with_sch
+00001560: 656d 655f 6e65 7874 5f75 726c 6301 0000  eme_next_urlc...
+00001570: 0000 0000 0000 0000 0002 0000 0007 0000  ................
+00001580: 0043 0000 0073 3400 0000 7c00 a000 7c00  .C...s4...|...|.
+00001590: 6a01 a101 0100 7c00 6a02 7c00 6a01 7403  j.....|.j.|.j.t.
+000015a0: 7404 6401 6402 6403 8d05 7d01 7c01 6a05  t.d.d.d...}.|.j.
+000015b0: 6404 6b02 7330 7406 8201 6405 5300 2906  d.k.s0t...d.S.).
+000015c0: 7a48 0a20 2020 2020 2020 2054 6573 7420  zH.        Test 
+000015d0: 5365 6375 7269 7479 2069 6e76 616c 6964  Security invalid
+000015e0: 206e 6578 7420 5552 4c20 7769 7468 2063   next URL with c
+000015f0: 6f6e 7472 6f6c 2063 6861 7261 6374 6572  ontrol character
+00001600: 730a 2020 2020 2020 2020 7a0b 0173 616d  s.        z..sam
+00001610: 706c 652e 636f 6d46 724d 0000 0072 4500  ple.comFrM...rE.
+00001620: 0000 4e72 4600 0000 7249 0000 0072 1700  ..NrF...rI...r..
+00001630: 0000 7217 0000 0072 1800 0000 da31 7465  ..r....r.....1te
+00001640: 7374 5f64 625f 6c6f 6769 6e5f 696e 7661  st_db_login_inva
+00001650: 6c69 645f 636f 6e74 726f 6c5f 6368 6172  lid_control_char
+00001660: 6163 7465 7273 5f6e 6578 745f 7572 6ccc  acters_next_url.
+00001670: 0000 0073 1200 0000 0004 0c01 0401 0401  ...s............
+00001680: 0201 0201 0201 02fb 0607 7a45 4d56 4353  ..........zEMVCS
+00001690: 6563 7572 6974 7954 6573 7443 6173 652e  ecurityTestCase.
+000016a0: 7465 7374 5f64 625f 6c6f 6769 6e5f 696e  test_db_login_in
+000016b0: 7661 6c69 645f 636f 6e74 726f 6c5f 6368  valid_control_ch
+000016c0: 6172 6163 7465 7273 5f6e 6578 745f 7572  aracters_next_ur
+000016d0: 6c63 0100 0000 0000 0000 0000 0000 0200  lc..............
+000016e0: 0000 0700 0000 4300 0000 7356 0000 007c  ......C...sV...|
+000016f0: 00a0 007c 006a 01a1 0101 007c 006a 027c  ...|.j.....|.j.|
+00001700: 006a 0174 0364 0174 049b 009d 0264 0264  .j.t.d.t.....d.d
+00001710: 0364 048d 057d 017c 006a 016a 057c 016a  .d...}.|.j.j.|.j
+00001720: 0674 0774 0374 0464 058d 0264 0364 068d  .t.t.t.d...d.d..
+00001730: 037d 017c 016a 0664 026b 0273 5274 0882  .}.|.j.d.k.sRt..
+00001740: 0164 0753 0029 087a 4b0a 2020 2020 2020  .d.S.).zK.      
+00001750: 2020 5465 7374 2053 6563 7572 6974 7920    Test Security 
+00001760: 4b65 6570 696e 6720 6e65 7874 2075 726c  Keeping next url
+00001770: 2061 6674 6572 2066 6169 6c65 6420 6c6f   after failed lo
+00001780: 6769 6e20 6174 7465 6d70 740a 2020 2020  gin attempt.    
+00001790: 2020 2020 5a06 7772 6f6e 675f 724c 0000      Z.wrong_rL..
+000017a0: 0046 724d 0000 0029 02da 0875 7365 726e  .FrM...)...usern
+000017b0: 616d 6572 1400 0000 a902 723e 0000 0072  amer......r>...r
+000017c0: 4400 0000 4e29 0972 3d00 0000 722f 0000  D...N).r=...r/..
+000017d0: 0072 3c00 0000 7210 0000 0072 0e00 0000  .r<...r....r....
+000017e0: da04 706f 7374 7247 0000 00da 0464 6963  ..postrG.....dic
+000017f0: 7472 4800 0000 7249 0000 0072 1700 0000  trH...rI...r....
+00001800: 7217 0000 0072 1800 0000 da22 7465 7374  r....r....."test
+00001810: 5f64 625f 6c6f 6769 6e5f 6661 696c 6564  _db_login_failed
+00001820: 5f6b 6565 705f 6e65 7874 5f75 726c da00  _keep_next_url..
+00001830: 0000 731c 0000 0000 040c 0104 0104 0102  ..s.............
+00001840: 0108 0102 0102 fb06 0706 0104 010a 0102  ................
+00001850: fd06 067a 364d 5643 5365 6375 7269 7479  ...z6MVCSecurity
+00001860: 5465 7374 4361 7365 2e74 6573 745f 6462  TestCase.test_db
+00001870: 5f6c 6f67 696e 5f66 6169 6c65 645f 6b65  _login_failed_ke
+00001880: 6570 5f6e 6578 745f 7572 6c63 0100 0000  ep_next_urlc....
+00001890: 0000 0000 0000 0000 0300 0000 0500 0000  ................
+000018a0: 4300 0000 737c 0000 007c 006a 00a0 01a1  C...s|...|.j....
+000018b0: 007d 017c 00a0 027c 0174 0374 04a1 0301  .}.|...|.t.t....
+000018c0: 007c 01a0 0564 01a1 017d 027c 00a0 067c  .|...d...}.|...|
+000018d0: 026a 0764 02a1 0201 007c 01a0 0564 03a1  .j.d.....|...d..
+000018e0: 017d 027c 00a0 067c 026a 0764 02a1 0201  .}.|...|.j.d....
+000018f0: 007c 01a0 0564 04a1 017d 027c 00a0 067c  .|...d...}.|...|
+00001900: 026a 0764 05a1 0201 007c 01a0 0564 06a1  .j.d.....|...d..
+00001910: 017d 027c 00a0 067c 026a 0764 05a1 0201  .}.|...|.j.d....
+00001920: 0064 0753 0029 087a 360a 2020 2020 2020  .d.S.).z6.      
+00001930: 2020 5465 7374 2053 6563 7572 6974 7920    Test Security 
+00001940: 6275 696c 7469 6e20 726f 6c65 7320 7265  builtin roles re
+00001950: 6164 6f6e 6c79 0a20 2020 2020 2020 2072  adonly.        r
+00001960: 3500 0000 7237 0000 007a 122f 6d6f 6465  5...r7...z./mode
+00001970: 6c31 7669 6577 2f73 686f 772f 317a 122f  l1view/show/1z./
+00001980: 6d6f 6465 6c31 7669 6577 2f65 6469 742f  model1view/edit/
+00001990: 3172 3600 0000 7a14 2f6d 6f64 656c 3176  1r6...z./model1v
+000019a0: 6965 772f 6465 6c65 7465 2f31 4e29 0872  iew/delete/1N).r
+000019b0: 2d00 0000 722e 0000 0072 3c00 0000 7211  -...r....r<...r.
+000019c0: 0000 0072 0f00 0000 7239 0000 0072 3a00  ...r....r9...r:.
+000019d0: 0000 723b 0000 0029 0372 3200 0000 722f  ..r;...).r2...r/
+000019e0: 0000 0072 4100 0000 7217 0000 0072 1700  ...rA...r....r..
+000019f0: 0000 7218 0000 00da 1774 6573 745f 6175  ..r......test_au
+00001a00: 7468 5f62 7569 6c74 696e 5f72 6f6c 6573  th_builtin_roles
+00001a10: ee00 0000 7314 0000 0000 040a 010e 020a  ....s...........
+00001a20: 010e 020a 010e 020a 010e 020a 017a 2b4d  .............z+M
+00001a30: 5643 5365 6375 7269 7479 5465 7374 4361  VCSecurityTestCa
+00001a40: 7365 2e74 6573 745f 6175 7468 5f62 7569  se.test_auth_bui
+00001a50: 6c74 696e 5f72 6f6c 6573 6301 0000 0000  ltin_rolesc.....
+00001a60: 0000 0000 0000 0005 0000 0006 0000 0043  ...............C
+00001a70: 0000 0073 0e01 0000 7c00 6a00 a001 a100  ...s....|.j.....
+00001a80: 7d01 7c01 6a02 6401 6402 6403 8d02 7d02  }.|.j.d.d.d...}.
+00001a90: 7c00 a003 7c02 6a04 6404 a102 0100 7c00  |...|.j.d.....|.
+00001aa0: a005 7c01 7406 7407 a103 7d03 7c01 6a02  ..|.t.t...}.|.j.
+00001ab0: 6401 6402 6403 8d02 7d02 7c02 6a08 a009  d.d.d...}.|.j...
+00001ac0: 6405 a101 7d04 7c00 a00a 6406 7c04 a102  d...}.|...d.|...
+00001ad0: 0100 7c01 6a0b 6407 740c 6408 6408 6409  ..|.j.d.t.d.d.d.
+00001ae0: 8d02 6402 640a 8d03 7d02 7c00 a003 7c02  ..d.d...}.|...|.
+00001af0: 6a04 640b a102 0100 7c00 a00d 7c01 a101  j.d.....|...|...
+00001b00: 0100 7c00 a005 7c01 7406 6408 a103 0100  ..|...|.t.d.....
+00001b10: 7c01 6a0b 6407 740c 7407 7407 6409 8d02  |.j.d.t.t.t.d...
+00001b20: 6402 640a 8d03 7d02 7c00 a003 7c02 6a04  d.d...}.|...|.j.
+00001b30: 640b a102 0100 7c01 6a02 640c 6402 6403  d.....|.j.d.d.d.
+00001b40: 8d02 7d02 7c02 6a08 a009 6405 a101 7d04  ..}.|.j...d...}.
+00001b50: 7c00 a00a 6406 7c04 a102 0100 7c01 6a0b  |...d.|.....|.j.
+00001b60: 6407 740c 7407 7407 6409 8d02 6402 640a  d.t.t.t.d...d.d.
+00001b70: 8d03 7d02 7c00 a003 7c02 6a04 640b a102  ..}.|...|.j.d...
+00001b80: 0100 640d 5300 290e 7a2e 0a20 2020 2020  ..d.S.).z..     
+00001b90: 2020 2054 6573 7420 5365 6375 7269 7479     Test Security
+00001ba0: 2072 6573 6574 2070 6173 7377 6f72 640a   reset password.
+00001bb0: 2020 2020 2020 2020 fa1f 2f75 7365 7273          ../users
+00001bc0: 2f61 6374 696f 6e2f 7265 7365 746d 7970  /action/resetmyp
+00001bd0: 6173 7377 6f72 642f 3154 7243 0000 0069  assword/1TrC...i
+00001be0: 9401 0000 7238 0000 00fa 1352 6573 6574  ....r8.....Reset
+00001bf0: 2050 6173 7377 6f72 6420 466f 726d fa15   Password Form..
+00001c00: 2f72 6573 6574 6d79 7061 7373 776f 7264  /resetmypassword
+00001c10: 2f66 6f72 6d72 1400 0000 a902 7214 0000  /formr......r...
+00001c20: 00da 0d63 6f6e 665f 7061 7373 776f 7264  ...conf_password
+00001c30: 7258 0000 0072 3700 0000 7a1e 2f75 7365  rX...r7...z./use
+00001c40: 7273 2f61 6374 696f 6e2f 7265 7365 7470  rs/action/resetp
+00001c50: 6173 7377 6f72 6473 2f31 4e29 0e72 2d00  asswords/1N).r-.
+00001c60: 0000 722e 0000 0072 3900 0000 723a 0000  ..r....r9...r:..
+00001c70: 0072 3b00 0000 723c 0000 0072 1000 0000  .r;...r<...r....
+00001c80: 720e 0000 0072 3e00 0000 723f 0000 0072  r....r>...r?...r
+00001c90: 4000 0000 7259 0000 0072 5a00 0000 723d  @...rY...rZ...r=
+00001ca0: 0000 0029 0572 3200 0000 722f 0000 0072  ...).r2...r/...r
+00001cb0: 4100 0000 da01 5f72 3e00 0000 7217 0000  A....._r>...r...
+00001cc0: 0072 1700 0000 7218 0000 00da 1774 6573  .r....r......tes
+00001cd0: 745f 7365 635f 7265 7365 745f 7061 7373  t_sec_reset_pass
+00001ce0: 776f 7264 0101 0000 733c 0000 0000 040a  word....s<......
+00001cf0: 030e 050e 030e 010e 010c 010c 0104 0102  ................
+00001d00: 010a 0102 fd06 050e 010a 010e 0104 0102  ................
+00001d10: 010a 0102 fd06 050e 030e 010c 010c 0104  ................
+00001d20: 0102 010a 0102 fd06 057a 2b4d 5643 5365  .........z+MVCSe
+00001d30: 6375 7269 7479 5465 7374 4361 7365 2e74  curityTestCase.t
+00001d40: 6573 745f 7365 635f 7265 7365 745f 7061  est_sec_reset_pa
+00001d50: 7373 776f 7264 6301 0000 0000 0000 0000  sswordc.........
+00001d60: 0000 0005 0000 0006 0000 0043 0000 0073  ...........C...s
+00001d70: dc00 0000 7c00 6a00 a001 a100 7d01 6401  ....|.j.....}.d.
+00001d80: 7c00 6a00 6a02 6402 3c00 7c00 a003 7c01  |.j.j.d.<.|...|.
+00001d90: 7404 7405 a103 7d02 7c01 6a06 6403 6401  t.t...}.|.j.d.d.
+00001da0: 6404 8d02 7d03 7c03 6a07 a008 6405 a101  d...}.|.j...d...
+00001db0: 7d04 7c00 a009 6406 7c04 a102 0100 7c01  }.|...d.|.....|.
+00001dc0: 6a0a 6407 740b 6408 6408 6409 8d02 6401  j.d.t.d.d.d...d.
+00001dd0: 640a 8d03 7d03 7c03 6a07 a008 6405 a101  d...}.|.j...d...
+00001de0: 7d04 7c00 a009 740c 7c04 a102 0100 7c01  }.|...t.|.....|.
+00001df0: 6a0a 6407 740b 640b 640b 6409 8d02 6401  j.d.t.d.d.d...d.
+00001e00: 640a 8d03 7d03 7c03 6a07 a008 6405 a101  d...}.|.j...d...
+00001e10: 7d04 7c00 a00d 740c 7c04 a102 0100 640c  }.|...t.|.....d.
+00001e20: 7c00 6a00 6a02 6402 3c00 7c01 6a0a 6407  |.j.j.d.<.|.j.d.
+00001e30: 740b 6408 6408 6409 8d02 6401 640a 8d03  t.d.d.d...d.d...
+00001e40: 7d02 7c00 a00e 7c01 a101 0100 640d 5300  }.|...|.....d.S.
+00001e50: 290e 7a46 0a20 2020 2020 2020 2054 6573  ).zF.        Tes
+00001e60: 7420 5365 6375 7269 7479 2072 6573 6574  t Security reset
+00001e70: 2070 6173 7377 6f72 6420 7769 7468 2064   password with d
+00001e80: 6566 6175 6c74 2063 6f6d 706c 6578 6974  efault complexit
+00001e90: 790a 2020 2020 2020 2020 54da 1f46 4142  y.        T..FAB
+00001ea0: 5f50 4153 5357 4f52 445f 434f 4d50 4c45  _PASSWORD_COMPLE
+00001eb0: 5849 5459 5f45 4e41 424c 4544 725d 0000  XITY_ENABLEDr]..
+00001ec0: 0072 4300 0000 7238 0000 0072 5e00 0000  .rC...r8...r^...
+00001ed0: 725f 0000 0072 1400 0000 7260 0000 0072  r_...r....r`...r
+00001ee0: 5800 0000 7a0c 5041 7373 776f 7264 3132  X...z.PAssword12
+00001ef0: 3321 464e 290f 722d 0000 0072 2e00 0000  3!FN).r-...r....
+00001f00: da06 636f 6e66 6967 723c 0000 0072 1000  ..configr<...r..
+00001f10: 0000 720e 0000 0072 3900 0000 723e 0000  ..r....r9...r>..
+00001f20: 0072 3f00 0000 7240 0000 0072 5900 0000  .r?...r@...rY...
+00001f30: 725a 0000 00da 1950 4153 5357 4f52 445f  rZ.....PASSWORD_
+00001f40: 434f 4d50 4c45 5849 5459 5f45 5252 4f52  COMPLEXITY_ERROR
+00001f50: da0b 6173 7365 7274 4e6f 7449 6e72 3d00  ..assertNotInr=.
+00001f60: 0000 a905 7232 0000 0072 2f00 0000 7262  ....r2...r/...rb
+00001f70: 0000 0072 4100 0000 723e 0000 0072 1700  ...rA...r>...r..
+00001f80: 0000 7217 0000 0072 1800 0000 da2a 7465  ..r....r.....*te
+00001f90: 7374 5f73 6563 5f72 6573 6574 5f70 6173  st_sec_reset_pas
+00001fa0: 7377 6f72 645f 6465 6661 756c 745f 636f  sword_default_co
+00001fb0: 6d70 6c65 7869 7479 2e01 0000 7336 0000  mplexity....s6..
+00001fc0: 0000 040a 010c 030e 010e 010c 010c 0104  ................
+00001fd0: 0102 010a 0102 fd06 050c 020c 0204 0102  ................
+00001fe0: 010a 0102 fd06 050c 020c 030c 0104 0102  ................
+00001ff0: 010a 0102 fd06 067a 3e4d 5643 5365 6375  .......z>MVCSecu
+00002000: 7269 7479 5465 7374 4361 7365 2e74 6573  rityTestCase.tes
+00002010: 745f 7365 635f 7265 7365 745f 7061 7373  t_sec_reset_pass
+00002020: 776f 7264 5f64 6566 6175 6c74 5f63 6f6d  word_default_com
+00002030: 706c 6578 6974 7963 0100 0000 0000 0000  plexityc........
+00002040: 0000 0000 0500 0000 0600 0000 4300 0000  ............C...
+00002050: 73ac 0000 007c 006a 00a0 01a1 007d 0164  s....|.j.....}.d
+00002060: 017c 006a 006a 0264 023c 0074 037c 006a  .|.j.j.d.<.t.|.j
+00002070: 006a 0264 033c 007c 00a0 047c 0174 0574  .j.d.<.|...|.t.t
+00002080: 06a1 037d 027c 016a 0764 0464 0164 058d  ...}.|.j.d.d.d..
+00002090: 027d 037c 036a 08a0 0964 06a1 017d 047c  .}.|.j...d...}.|
+000020a0: 00a0 0a64 077c 04a1 0201 007c 016a 0b64  ...d.|.....|.j.d
+000020b0: 0874 0c64 0964 0964 0a8d 0264 0164 0b8d  .t.d.d.d...d.d..
+000020c0: 037d 037c 036a 08a0 0964 06a1 017d 047c  .}.|.j...d...}.|
+000020d0: 00a0 0a64 0c7c 04a1 0201 007c 016a 0b64  ...d.|.....|.j.d
+000020e0: 0874 0c64 0d64 0d64 0a8d 0264 0164 0b8d  .t.d.d.d...d.d..
+000020f0: 037d 037c 00a0 0d7c 01a1 0101 0064 0e53  .}.|...|.....d.S
+00002100: 0029 0f7a 450a 2020 2020 2020 2020 5465  .).zE.        Te
+00002110: 7374 2053 6563 7572 6974 7920 7265 7365  st Security rese
+00002120: 7420 7061 7373 776f 7264 2077 6974 6820  t password with 
+00002130: 6375 7374 6f6d 2063 6f6d 706c 6578 6974  custom complexit
+00002140: 790a 2020 2020 2020 2020 5472 6400 0000  y.        Trd...
+00002150: da21 4641 425f 5041 5353 574f 5244 5f43  .!FAB_PASSWORD_C
+00002160: 4f4d 504c 4558 4954 595f 5641 4c49 4441  OMPLEXITY_VALIDA
+00002170: 544f 5272 5d00 0000 7243 0000 0072 3800  TORr]...rC...r8.
+00002180: 0000 725e 0000 0072 5f00 0000 5a03 3132  ..r^...r_...Z.12
+00002190: 3372 6000 0000 7258 0000 0072 1600 0000  3r`...rX...r....
+000021a0: 7214 0000 004e 290e 722d 0000 0072 2e00  r....N).r-...r..
+000021b0: 0000 7265 0000 0072 1900 0000 723c 0000  ..re...r....r<..
+000021c0: 0072 1000 0000 720e 0000 0072 3900 0000  .r....r....r9...
+000021d0: 723e 0000 0072 3f00 0000 7240 0000 0072  r>...r?...r@...r
+000021e0: 5900 0000 725a 0000 0072 3d00 0000 7268  Y...rZ...r=...rh
+000021f0: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00002200: 0000 da29 7465 7374 5f73 6563 5f72 6573  ...)test_sec_res
+00002210: 6574 5f70 6173 7377 6f72 645f 6375 7374  et_password_cust
+00002220: 6f6d 5f63 6f6d 706c 6578 6974 7956 0100  om_complexityV..
+00002230: 0073 2800 0000 0004 0a01 0c01 0c03 0e01  .s(.............
+00002240: 0e01 0c01 0c01 0401 0201 0a01 02fd 0605  ................
+00002250: 0c02 0c02 0401 0201 0a01 02fd 0605 7a3d  ..............z=
+00002260: 4d56 4353 6563 7572 6974 7954 6573 7443  MVCSecurityTestC
+00002270: 6173 652e 7465 7374 5f73 6563 5f72 6573  ase.test_sec_res
+00002280: 6574 5f70 6173 7377 6f72 645f 6375 7374  et_password_cust
+00002290: 6f6d 5f63 6f6d 706c 6578 6974 7963 0100  om_complexityc..
+000022a0: 0000 0000 0000 0000 0000 0600 0000 0b00  ................
+000022b0: 0000 4300 0000 732c 0100 007c 006a 00a0  ..C...s,...|.j..
+000022c0: 01a1 007d 017c 00a0 027c 0174 0374 04a1  ...}.|...|.t.t..
+000022d0: 037d 027c 016a 0564 0164 0264 038d 027d  .}.|.j.d.d.d...}
+000022e0: 037c 036a 06a0 0764 04a1 017d 047c 00a0  .|.j...d...}.|..
+000022f0: 0864 057c 04a1 0201 007c 016a 0964 0174  .d.|.....|.j.d.t
+00002300: 0a64 0664 0764 0864 0964 0a67 0164 0b64  .d.d.d.d.d.g.d.d
+00002310: 0b64 0c8d 0764 0264 0d8d 037d 037c 036a  .d...d.d...}.|.j
+00002320: 06a0 0764 04a1 017d 047c 00a0 0864 0e7c  ...d...}.|...d.|
+00002330: 04a1 0201 007c 016a 0564 0164 0264 038d  .....|.j.d.d.d..
+00002340: 027d 037c 036a 06a0 0764 04a1 017d 047c  .}.|.j...d...}.|
+00002350: 00a0 0864 057c 04a1 0201 007c 016a 0964  ...d.|.....|.j.d
+00002360: 0174 0a64 0664 0764 0f64 1067 0064 0b64  .t.d.d.d.d.g.d.d
+00002370: 0b64 0c8d 0764 0264 0d8d 037d 037c 036a  .d...d.d...}.|.j
+00002380: 06a0 0764 04a1 017d 047c 00a0 0b64 0e7c  ...d...}.|...d.|
+00002390: 04a1 0201 007c 00a0 0864 117c 04a1 0201  .....|...d.|....
+000023a0: 007c 00a0 0c7c 01a1 0101 007c 006a 0d6a  .|...|.....|.j.j
+000023b0: 0ea0 0f74 10a1 01a0 1174 106a 1264 086b  ...t.....t.j.d.k
+000023c0: 02a1 01a0 13a1 007d 057c 006a 0d6a 0ea0  .......}.|.j.j..
+000023d0: 147c 05a1 0101 007c 006a 0d6a 0ea0 15a1  .|.....|.j.j....
+000023e0: 0001 0064 1253 0029 137a 240a 2020 2020  ...d.S.).z$.    
+000023f0: 2020 2020 5465 7374 2072 6567 6973 7465      Test registe
+00002400: 7220 7573 6572 0a20 2020 2020 2020 207a  r user.        z
+00002410: 0a2f 7573 6572 732f 6164 6454 7243 0000  ./users/addTrC..
+00002420: 0072 3800 0000 7a08 4164 6420 5573 6572  .r8...z.Add User
+00002430: da05 6669 7273 74da 046c 6173 747a 0d66  ..first..lastz.f
+00002440: 726f 6d20 7465 7374 2031 2d31 7a13 7465  rom test 1-1z.te
+00002450: 7374 3140 6672 6f6d 7465 7374 312e 636f  st1@fromtest1.co
+00002460: 6de9 0100 0000 7214 0000 0029 07da 0a66  m.....r....)...f
+00002470: 6972 7374 5f6e 616d 65da 096c 6173 745f  irst_name..last_
+00002480: 6e61 6d65 7257 0000 00da 0565 6d61 696c  namerW.....email
+00002490: da05 726f 6c65 7372 1400 0000 7261 0000  ..rolesr....ra..
+000024a0: 0072 5800 0000 7a09 4164 6465 6420 526f  .rX...z.Added Ro
+000024b0: 777a 0d66 726f 6d20 7465 7374 2032 2d31  wz.from test 2-1
+000024c0: 7a13 7465 7374 3240 6672 6f6d 7465 7374  z.test2@fromtest
+000024d0: 322e 636f 6dfa 1654 6869 7320 6669 656c  2.com..This fiel
+000024e0: 6420 6973 2072 6571 7569 7265 644e 2916  d is requiredN).
+000024f0: 722d 0000 0072 2e00 0000 723c 0000 0072  r-...r....r<...r
+00002500: 1000 0000 720e 0000 0072 3900 0000 723e  ....r....r9...r>
+00002510: 0000 0072 3f00 0000 7240 0000 0072 5900  ...r?...r@...rY.
+00002520: 0000 725a 0000 0072 6700 0000 723d 0000  ..rZ...rg...r=..
+00002530: 00da 0264 62da 0773 6573 7369 6f6e da05  ...db..session..
+00002540: 7175 6572 7972 0a00 0000 da06 6669 6c74  queryr......filt
+00002550: 6572 7257 0000 00da 0b6f 6e65 5f6f 725f  errW.....one_or_
+00002560: 6e6f 6e65 da06 6465 6c65 7465 da06 636f  none..delete..co
+00002570: 6d6d 6974 2906 7232 0000 0072 2f00 0000  mmit).r2...r/...
+00002580: 7262 0000 0072 4100 0000 723e 0000 00da  rb...rA...r>....
+00002590: 0475 7365 7272 1700 0000 7217 0000 0072  .userr....r....r
+000025a0: 1800 0000 da12 7465 7374 5f72 6567 6973  ......test_regis
+000025b0: 7465 725f 7573 6572 7301 0000 735c 0000  ter_users...s\..
+000025c0: 0000 040a 010e 030e 010c 010c 0104 0102  ................
+000025d0: 0102 0102 0102 0102 0102 0104 0102 0102  ................
+000025e0: f904 0902 f506 0d0c 010c 030e 010c 010c  ................
+000025f0: 0104 0102 0102 0102 0102 0102 0102 0102  ................
+00002600: 0102 0102 f904 0902 f506 0d0c 010c 010c  ................
+00002610: 010a 030e 0108 ff06 ff02 050e 017a 264d  .............z&M
+00002620: 5643 5365 6375 7269 7479 5465 7374 4361  VCSecurityTestCa
+00002630: 7365 2e74 6573 745f 7265 6769 7374 6572  se.test_register
+00002640: 5f75 7365 7263 0100 0000 0000 0000 0000  _userc..........
+00002650: 0000 0700 0000 0a00 0000 4300 0000 73fc  ..........C...s.
+00002660: 0000 007c 006a 00a0 01a1 007d 017c 00a0  ...|.j.....}.|..
+00002670: 027c 0174 0374 04a1 037d 027c 006a 057c  .|.t.t...}.|.j.|
+00002680: 006a 0664 0164 0264 0364 0464 0564 0664  .j.d.d.d.d.d.d.d
+00002690: 0767 0164 088d 087d 037c 016a 0764 097c  .g.d...}.|.j.d.|
+000026a0: 036a 089b 009d 0264 0a64 0b8d 027d 047c  .j.....d.d...}.|
+000026b0: 046a 09a0 0a64 0ca1 017d 057c 00a0 0b64  .j...d...}.|...d
+000026c0: 0d7c 05a1 0201 007c 016a 0c64 097c 036a  .|.....|.j.d.|.j
+000026d0: 089b 009d 0274 0d7c 036a 0e7c 036a 0f7c  .....t.|.j.|.j.|
+000026e0: 036a 1064 0e7c 036a 1164 0f19 006a 0864  .j.d.|.j.d...j.d
+000026f0: 108d 0564 0a64 118d 037d 047c 046a 09a0  ...d.d...}.|.j..
+00002700: 0a64 0ca1 017d 057c 00a0 0b64 127c 05a1  .d...}.|...d.|..
+00002710: 0201 007c 006a 126a 13a0 1474 15a1 01a0  ...|.j.j...t....
+00002720: 1674 156a 107c 036a 106b 02a1 01a0 17a1  .t.j.|.j.k......
+00002730: 007d 067c 066a 1864 0e6b 0273 de74 1982  .}.|.j.d.k.s.t..
+00002740: 017c 006a 126a 13a0 1a7c 06a1 0101 007c  .|.j.j...|.....|
+00002750: 006a 126a 13a0 1ba1 0001 0064 1353 0029  .j.j.......d.S.)
+00002760: 147a 200a 2020 2020 2020 2020 5465 7374  .z .        Test
+00002770: 2065 6469 7420 7573 6572 0a20 2020 2020   edit user.     
+00002780: 2020 205a 0874 6d70 5f75 7365 725a 0970     Z.tmp_userZ.p
+00002790: 6173 7377 6f72 6431 da00 da03 746d 7072  assword1....tmpr
+000027a0: 7b00 0000 7a0b 746d 7040 6661 622e 6f72  {...z.tmp@fab.or
+000027b0: 675a 0541 646d 696e 2904 726f 0000 0072  gZ.Admin).ro...r
+000027c0: 7000 0000 7271 0000 005a 0a72 6f6c 655f  p...rq...Z.role_
+000027d0: 6e61 6d65 73fa 0c2f 7573 6572 732f 6564  names../users/ed
+000027e0: 6974 2f54 7243 0000 0072 3800 0000 fa09  it/TrC...r8.....
+000027f0: 4564 6974 2055 7365 72fa 1363 6861 6e67  Edit User..chang
+00002800: 6564 4063 6861 6e67 6564 2e6f 7267 7201  ed@changed.orgr.
+00002810: 0000 00a9 0572 6f00 0000 7270 0000 0072  .....ro...rp...r
+00002820: 5700 0000 7271 0000 0072 7200 0000 7258  W...rq...rr...rX
+00002830: 0000 007a 0b43 6861 6e67 6564 2052 6f77  ...z.Changed Row
+00002840: 4e29 1c72 2d00 0000 722e 0000 0072 3c00  N).r-...r....r<.
+00002850: 0000 7210 0000 0072 0e00 0000 5a0b 6372  ..r....r....Z.cr
+00002860: 6561 7465 5f75 7365 7272 3000 0000 7239  eate_userr0...r9
+00002870: 0000 00da 0269 6472 3e00 0000 723f 0000  .....idr>...r?..
+00002880: 0072 4000 0000 7259 0000 0072 5a00 0000  .r@...rY...rZ...
+00002890: 726f 0000 0072 7000 0000 7257 0000 0072  ro...rp...rW...r
+000028a0: 7200 0000 7274 0000 0072 7500 0000 7276  r...rt...ru...rv
+000028b0: 0000 0072 0a00 0000 7277 0000 0072 7800  ...r....rw...rx.
+000028c0: 0000 7271 0000 0072 4800 0000 7279 0000  ..rq...rH...ry..
+000028d0: 0072 7a00 0000 2907 7232 0000 0072 2f00  .rz...).r2...r/.
+000028e0: 0000 7262 0000 005a 095f 746d 705f 7573  ..rb...Z._tmp_us
+000028f0: 6572 7241 0000 0072 3e00 0000 727b 0000  errA...r>...r{..
+00002900: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00002910: da0e 7465 7374 5f65 6469 745f 7573 6572  ..test_edit_user
+00002920: ac01 0000 7346 0000 0000 040a 010e 0204  ....sF..........
+00002930: 0104 0102 0102 0102 0102 0102 0102 0104  ................
+00002940: f806 0c16 010c 010c 0104 010a 0102 0104  ................
+00002950: 0104 0104 0102 010a fb04 0702 f706 0b0c  ................
+00002960: 010c 030e 010a ff06 ff02 060e 010e 017a  ...............z
+00002970: 224d 5643 5365 6375 7269 7479 5465 7374  "MVCSecurityTest
+00002980: 4361 7365 2e74 6573 745f 6564 6974 5f75  Case.test_edit_u
+00002990: 7365 7263 0100 0000 0000 0000 0000 0000  serc............
+000029a0: 0600 0000 0900 0000 4300 0000 73b4 0000  ........C...s...
+000029b0: 007c 006a 00a0 01a1 007d 017c 00a0 027c  .|.j.....}.|...|
+000029c0: 0174 0374 04a1 037d 027c 006a 056a 06a0  .t.t...}.|.j.j..
+000029d0: 0774 08a1 01a0 0974 086a 0a74 0b6b 02a1  .t.....t.j.t.k..
+000029e0: 01a0 0ca1 007d 037c 016a 0d64 017c 036a  .....}.|.j.d.|.j
+000029f0: 0e9b 009d 0264 0264 038d 027d 047c 046a  .....d.d...}.|.j
+00002a00: 0fa0 1064 04a1 017d 057c 00a0 1164 057c  ...d...}.|...d.|
+00002a10: 05a1 0201 007c 016a 1264 017c 036a 0e9b  .....|.j.d.|.j..
+00002a20: 009d 0274 137c 036a 147c 036a 157c 036a  ...t.|.j.|.j.|.j
+00002a30: 0a64 067c 036a 1664 0719 006a 0e64 088d  .d.|.j.d...j.d..
+00002a40: 0564 0264 098d 037d 047c 046a 0fa0 1064  .d.d...}.|.j...d
+00002a50: 04a1 017d 057c 00a0 1164 0a7c 05a1 0201  ...}.|...d.|....
+00002a60: 0064 0653 0029 0b7a 3f0a 2020 2020 2020  .d.S.).z?.      
+00002a70: 2020 5465 7374 2065 6469 7420 7573 6572    Test edit user
+00002a80: 2077 6974 6820 656d 6169 6c20 6e6f 7420   with email not 
+00002a90: 6e75 6c6c 2076 616c 6964 6174 696f 6e0a  null validation.
+00002aa0: 2020 2020 2020 2020 727f 0000 0054 7243          r....TrC
+00002ab0: 0000 0072 3800 0000 7280 0000 004e 7201  ...r8...r....Nr.
+00002ac0: 0000 0072 8200 0000 7258 0000 0072 7300  ...r....rX...rs.
+00002ad0: 0000 2917 722d 0000 0072 2e00 0000 723c  ..).r-...r....r<
+00002ae0: 0000 0072 1000 0000 720e 0000 0072 7400  ...r....r....rt.
+00002af0: 0000 7275 0000 0072 7600 0000 720a 0000  ..ru...rv...r...
+00002b00: 0072 7700 0000 7257 0000 0072 1100 0000  .rw...rW...r....
+00002b10: 7278 0000 0072 3900 0000 7283 0000 0072  rx...r9...r....r
+00002b20: 3e00 0000 723f 0000 0072 4000 0000 7259  >...r?...r@...rY
+00002b30: 0000 0072 5a00 0000 726f 0000 0072 7000  ...rZ...ro...rp.
+00002b40: 0000 7272 0000 0029 0672 3200 0000 722f  ..rr...).r2...r/
+00002b50: 0000 0072 6200 0000 da0d 7265 6164 5f6f  ...rb.....read_o
+00002b60: 6e79 5f75 7365 7272 4100 0000 723e 0000  ny_userrA...r>..
+00002b70: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00002b80: da1f 7465 7374 5f65 6469 745f 7573 6572  ..test_edit_user
+00002b90: 5f65 6d61 696c 5f76 616c 6964 6174 696f  _email_validatio
+00002ba0: 6eda 0100 0073 2c00 0000 0004 0a01 0e03  n....s,.........
+00002bb0: 0e01 08ff 06ff 0207 1601 0c01 0c01 0401  ................
+00002bc0: 0a01 0201 0401 0401 0401 0201 0afb 0407  ................
+00002bd0: 02f7 060b 0c01 7a33 4d56 4353 6563 7572  ......z3MVCSecur
+00002be0: 6974 7954 6573 7443 6173 652e 7465 7374  ityTestCase.test
+00002bf0: 5f65 6469 745f 7573 6572 5f65 6d61 696c  _edit_user_email
+00002c00: 5f76 616c 6964 6174 696f 6e63 0100 0000  _validationc....
+00002c10: 0000 0000 0000 0000 0800 0000 0b00 0000  ................
+00002c20: 4300 0000 73fa 0000 007c 006a 00a0 01a1  C...s....|.j....
+00002c30: 007d 017c 00a0 027c 0174 0374 04a1 037d  .}.|...|.t.t...}
+00002c40: 027c 006a 056a 06a0 0774 08a1 01a0 0974  .|.j.j...t.....t
+00002c50: 086a 0a74 0b6b 02a1 01a0 0ca1 007d 037c  .j.t.k.......}.|
+00002c60: 016a 0d64 017c 036a 0e9b 009d 0264 0264  .j.d.|.j.....d.d
+00002c70: 038d 027d 047c 046a 0fa0 1064 04a1 017d  ...}.|.j...d...}
+00002c80: 057c 00a0 1164 057c 05a1 0201 0074 12a0  .|...d.|.....t..
+00002c90: 137c 006a 146a 0664 06a1 028f 7c7d 0674  .|.j.j.d....|}.t
+00002ca0: 126a 137c 006a 146a 1564 0764 0264 088d  .j.|.j.j.d.d.d..
+00002cb0: 038f 5c7d 0774 1664 0983 017c 065f 177c  ..\}.t.d...|._.|
+00002cc0: 016a 1864 017c 036a 0e9b 009d 0274 197c  .j.d.|.j.....t.|
+00002cd0: 036a 1a7c 036a 1b7c 036a 0a64 0a7c 036a  .j.|.j.|.j.d.|.j
+00002ce0: 1c64 0b19 006a 0e64 0c8d 0564 0264 0d8d  .d...j.d...d.d..
+00002cf0: 037d 047c 046a 0fa0 1064 04a1 017d 057c  .}.|.j...d...}.|
+00002d00: 00a0 1164 0e7c 05a1 0201 0057 0035 0051  ...d.|.....W.5.Q
+00002d10: 0052 0058 0057 0035 0051 0052 0058 0064  .R.X.W.5.Q.R.X.d
+00002d20: 0f53 0029 107a 2d0a 2020 2020 2020 2020  .S.).z-.        
+00002d30: 5465 7374 2065 6469 7420 7573 6572 2077  Test edit user w
+00002d40: 6974 6820 4442 2066 6169 6c0a 2020 2020  ith DB fail.    
+00002d50: 2020 2020 727f 0000 0054 7243 0000 0072      r....TrC...r
+00002d60: 3800 0000 7280 0000 00da 056d 6572 6765  8...r......merge
+00002d70: da0a 6861 735f 6163 6365 7373 2901 da0c  ..has_access)...
+00002d80: 7265 7475 726e 5f76 616c 7565 7a05 4241  return_valuez.BA
+00002d90: 4e47 2172 8100 0000 7201 0000 0072 8200  NG!r....r....r..
+00002da0: 0000 7258 0000 007a 0e44 6174 6162 6173  ..rX...z.Databas
+00002db0: 6520 4572 726f 724e 291d 722d 0000 0072  e ErrorN).r-...r
+00002dc0: 2e00 0000 723c 0000 0072 1000 0000 720e  ....r<...r....r.
+00002dd0: 0000 0072 7400 0000 7275 0000 0072 7600  ...rt...ru...rv.
+00002de0: 0000 720a 0000 0072 7700 0000 7257 0000  ..r....rw...rW..
+00002df0: 0072 1100 0000 7278 0000 0072 3900 0000  .r....rx...r9...
+00002e00: 7283 0000 0072 3e00 0000 723f 0000 0072  r....r>...r?...r
+00002e10: 4000 0000 7204 0000 00da 066f 626a 6563  @...r......objec
+00002e20: 7472 3000 0000 da02 736d da09 4578 6365  tr0.....sm..Exce
+00002e30: 7074 696f 6e5a 0b73 6964 655f 6566 6665  ptionZ.side_effe
+00002e40: 6374 7259 0000 0072 5a00 0000 726f 0000  ctrY...rZ...ro..
+00002e50: 0072 7000 0000 7272 0000 0029 0872 3200  .rp...rr...).r2.
+00002e60: 0000 722f 0000 0072 6200 0000 7285 0000  ..r/...rb...r...
+00002e70: 0072 4100 0000 723e 0000 005a 0a6d 6f63  .rA...r>...Z.moc
+00002e80: 6b5f 6d65 7267 655a 0f6d 6f63 6b5f 6861  k_mergeZ.mock_ha
+00002e90: 735f 6163 6365 7373 7217 0000 0072 1700  s_accessr....r..
+00002ea0: 0000 7218 0000 00da 1674 6573 745f 6564  ..r......test_ed
+00002eb0: 6974 5f75 7365 725f 6462 5f66 6169 6cf9  it_user_db_fail.
+00002ec0: 0100 0073 4400 0000 0004 0a01 0e03 0e01  ...sD...........
+00002ed0: 08ff 06ff 0207 1601 0c01 0c02 0401 0601  ................
+00002ee0: 02fe 0403 0201 0401 0600 0200 02ff 0602  ................
+00002ef0: 0205 0a02 0401 0a01 0201 0401 0401 0401  ................
+00002f00: 0201 0afb 0407 02f7 060c 0c01 7a2a 4d56  ............z*MV
+00002f10: 4353 6563 7572 6974 7954 6573 7443 6173  CSecurityTestCas
+00002f20: 652e 7465 7374 5f65 6469 745f 7573 6572  e.test_edit_user
+00002f30: 5f64 625f 6661 696c 2918 721e 0000 0072  _db_fail).r....r
+00002f40: 1f00 0000 7220 0000 0072 2c00 0000 7242  ....r ...r,...rB
+00002f50: 0000 0072 4b00 0000 724f 0000 0072 5000  ...rK...rO...rP.
+00002f60: 0000 7251 0000 0072 5200 0000 7253 0000  ..rQ...rR...rS..
+00002f70: 0072 5400 0000 7255 0000 0072 5600 0000  .rT...rU...rV...
+00002f80: 725b 0000 0072 5c00 0000 7263 0000 0072  r[...r\...rc...r
+00002f90: 6900 0000 726b 0000 0072 7c00 0000 7284  i...rk...r|...r.
+00002fa0: 0000 0072 8600 0000 728d 0000 00da 0d5f  ...r....r......_
+00002fb0: 5f63 6c61 7373 6365 6c6c 5f5f 7217 0000  _classcell__r...
+00002fc0: 0072 1700 0000 7233 0000 0072 1800 0000  .r....r3...r....
+00002fd0: 721a 0000 0022 0000 0073 2800 0000 0801  r...."...s(.....
+00002fe0: 0c1f 081e 080a 080e 080e 080e 080e 080e  ................
+00002ff0: 080e 080e 080e 0814 0813 082d 0828 081d  ...........-.(..
+00003000: 0839 082e 081f 721a 0000 0029 1d5a 0d75  .9....r....).Z.u
+00003010: 6e69 7474 6573 742e 6d6f 636b 7202 0000  nittest.mockr...
+00003020: 0072 0300 0000 7204 0000 005a 1066 6c61  .r....r....Z.fla
+00003030: 736b 5f61 7070 6275 696c 6465 7272 0500  sk_appbuilderr..
+00003040: 0000 da1b 666c 6173 6b5f 6170 7062 7569  ....flask_appbui
+00003050: 6c64 6572 2e65 7863 6570 7469 6f6e 7372  lder.exceptionsr
+00003060: 0700 0000 5a24 666c 6173 6b5f 6170 7062  ....Z$flask_appb
+00003070: 7569 6c64 6572 2e6d 6f64 656c 732e 7371  uilder.models.sq
+00003080: 6c61 2e66 696c 7465 7273 7208 0000 00da  la.filtersr.....
+00003090: 2666 6c61 736b 5f61 7070 6275 696c 6465  &flask_appbuilde
+000030a0: 722e 6d6f 6465 6c73 2e73 716c 612e 696e  r.models.sqla.in
+000030b0: 7465 7266 6163 6572 0900 0000 5a25 666c  terfacer....Z%fl
+000030c0: 6173 6b5f 6170 7062 7569 6c64 6572 2e73  ask_appbuilder.s
+000030d0: 6563 7572 6974 792e 7371 6c61 2e6d 6f64  ecurity.sqla.mod
+000030e0: 656c 7372 0a00 0000 da04 6261 7365 720c  elsr......baser.
+000030f0: 0000 00da 0563 6f6e 7374 720d 0000 0072  .....constr....r
+00003100: 0e00 0000 720f 0000 0072 1000 0000 7211  ....r....r....r.
+00003110: 0000 005a 0b73 716c 612e 6d6f 6465 6c73  ...Z.sqla.models
+00003120: 7212 0000 0072 1300 0000 7266 0000 00da  r....r....rf....
+00003130: 0373 7472 7219 0000 0072 1a00 0000 7217  .strr....r....r.
+00003140: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00003150: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
+00003160: 7318 0000 0014 020c 010c 010c 010c 010c  s...............
+00003170: 020c 011c 0710 0302 ff02 0710 08         .............
```

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/__pycache__/test_rate_limiter.cpython-38.pyc` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/__pycache__/test_rate_limiter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/test_auth_ldap.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/test_auth_ldap.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/test_auth_oauth.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/test_auth_oauth.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/test_base_security_manager.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/test_base_security_manager.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/test_mvc_security.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/test_mvc_security.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from unittest.mock import patch
+
 from flask_appbuilder import ModelView
 from flask_appbuilder.exceptions import PasswordComplexityValidationError
 from flask_appbuilder.models.sqla.filters import FilterEqual
 from flask_appbuilder.models.sqla.interface import SQLAInterface
 from flask_appbuilder.security.sqla.models import User
 
 from ..base import BaseMVCTestCase
@@ -418,7 +420,121 @@
         user = (
             self.db.session.query(User)
             .filter(User.username == "from test 1-1")
             .one_or_none()
         )
         self.db.session.delete(user)
         self.db.session.commit()
+
+    def test_edit_user(self):
+        """
+        Test edit user
+        """
+        client = self.app.test_client()
+        _ = self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
+
+        _tmp_user = self.create_user(
+            self.appbuilder,
+            "tmp_user",
+            "password1",
+            "",
+            first_name="tmp",
+            last_name="user",
+            email="tmp@fab.org",
+            role_names=["Admin"],
+        )
+
+        # use all required params
+        rv = client.get(f"/users/edit/{_tmp_user.id}", follow_redirects=True)
+        data = rv.data.decode("utf-8")
+        self.assertIn("Edit User", data)
+        rv = client.post(
+            f"/users/edit/{_tmp_user.id}",
+            data=dict(
+                first_name=_tmp_user.first_name,
+                last_name=_tmp_user.last_name,
+                username=_tmp_user.username,
+                email="changed@changed.org",
+                roles=_tmp_user.roles[0].id,
+            ),
+            follow_redirects=True,
+        )
+        data = rv.data.decode("utf-8")
+        self.assertIn("Changed Row", data)
+
+        user = (
+            self.db.session.query(User)
+            .filter(User.username == _tmp_user.username)
+            .one_or_none()
+        )
+
+        assert user.email == "changed@changed.org"
+        self.db.session.delete(user)
+        self.db.session.commit()
+
+    def test_edit_user_email_validation(self):
+        """
+        Test edit user with email not null validation
+        """
+        client = self.app.test_client()
+        _ = self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
+
+        read_ony_user: User = (
+            self.db.session.query(User)
+            .filter(User.username == USERNAME_READONLY)
+            .one_or_none()
+        )
+
+        # use all required params
+        rv = client.get(f"/users/edit/{read_ony_user.id}", follow_redirects=True)
+        data = rv.data.decode("utf-8")
+        self.assertIn("Edit User", data)
+        rv = client.post(
+            f"/users/edit/{read_ony_user.id}",
+            data=dict(
+                first_name=read_ony_user.first_name,
+                last_name=read_ony_user.last_name,
+                username=read_ony_user.username,
+                email=None,
+                roles=read_ony_user.roles[0].id,
+            ),
+            follow_redirects=True,
+        )
+        data = rv.data.decode("utf-8")
+        self.assertIn("This field is required", data)
+
+    def test_edit_user_db_fail(self):
+        """
+        Test edit user with DB fail
+        """
+        client = self.app.test_client()
+        _ = self.browser_login(client, USERNAME_ADMIN, PASSWORD_ADMIN)
+
+        read_ony_user: User = (
+            self.db.session.query(User)
+            .filter(User.username == USERNAME_READONLY)
+            .one_or_none()
+        )
+
+        # use all required params
+        rv = client.get(f"/users/edit/{read_ony_user.id}", follow_redirects=True)
+        data = rv.data.decode("utf-8")
+        self.assertIn("Edit User", data)
+
+        with patch.object(self.appbuilder.session, "merge") as mock_merge:
+            with patch.object(self.appbuilder.sm, "has_access", return_value=True) as _:
+                mock_merge.side_effect = Exception("BANG!")
+
+                rv = client.post(
+                    f"/users/edit/{read_ony_user.id}",
+                    data=dict(
+                        first_name=read_ony_user.first_name,
+                        last_name=read_ony_user.last_name,
+                        username=read_ony_user.username,
+                        email="changed@changed.org",
+                        roles=read_ony_user.roles[0].id,
+                    ),
+                    follow_redirects=True,
+                )
+
+                data = rv.data.decode("utf-8")
+                self.assertIn("Database Error", data)
```

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/test_password_complexity.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/test_password_complexity.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/security/test_rate_limiter.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/security/test_rate_limiter.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/sqla/__pycache__/models.cpython-38.pyc` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/sqla/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/sqla/models.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/sqla/models.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_addon.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_addon.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_api.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_custom_indexview.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_custom_indexview.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_fab_cli.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_fab_cli.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_menu.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_mongoengine.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_mongoengine.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_mvc.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_mvc.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_mvc_oauth.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_mvc_oauth.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_security_api.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_security_api.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_security_permissions.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_security_permissions.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_sqlalchemy.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/tests/test_urltools.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/tests/test_urltools.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/de/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/el/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/el/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/es/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/it/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ja_JP/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ko/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/nl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pt/LC_MESSAGES/messages.po~`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/sl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/zh/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/translations/zh_HK/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/upload.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/upload.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/urltools.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/urltools.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/utils/base.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/utils/base.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/utils/limit.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/utils/limit.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/validators.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/validators.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/views.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/views.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/flask_appbuilder/widgets.py` & `Flask-AppBuilder-4.3.2rc2/flask_appbuilder/widgets.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/ListThumbnail.png` & `Flask-AppBuilder-4.3.2rc2/images/ListThumbnail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/chart.png` & `Flask-AppBuilder-4.3.2rc2/images/chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/chart_time1.png` & `Flask-AppBuilder-4.3.2rc2/images/chart_time1.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/chart_time2.png` & `Flask-AppBuilder-4.3.2rc2/images/chart_time2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/charts.png` & `Flask-AppBuilder-4.3.2rc2/images/charts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/contact_list.png` & `Flask-AppBuilder-4.3.2rc2/images/contact_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/contacts.png` & `Flask-AppBuilder-4.3.2rc2/images/contacts.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/direct_chart.png` & `Flask-AppBuilder-4.3.2rc2/images/direct_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/fab.png` & `Flask-AppBuilder-4.3.2rc2/images/fab.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/group_list.png` & `Flask-AppBuilder-4.3.2rc2/images/group_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/grouped_chart.png` & `Flask-AppBuilder-4.3.2rc2/images/grouped_chart.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/groups.png` & `Flask-AppBuilder-4.3.2rc2/images/groups.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/images_list.png` & `Flask-AppBuilder-4.3.2rc2/images/images_list.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/list_cascade.png` & `Flask-AppBuilder-4.3.2rc2/images/list_cascade.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/list_cascade_block.png` & `Flask-AppBuilder-4.3.2rc2/images/list_cascade_block.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/list_compact_inline.png` & `Flask-AppBuilder-4.3.2rc2/images/list_compact_inline.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/list_master_detail.png` & `Flask-AppBuilder-4.3.2rc2/images/list_master_detail.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/login.png` & `Flask-AppBuilder-4.3.2rc2/images/login.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/login_db.png` & `Flask-AppBuilder-4.3.2rc2/images/login_db.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/login_oauth.png` & `Flask-AppBuilder-4.3.2rc2/images/login_oauth.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/login_oid.png` & `Flask-AppBuilder-4.3.2rc2/images/login_oid.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/security.png` & `Flask-AppBuilder-4.3.2rc2/images/security.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/images/simpleview2.png` & `Flask-AppBuilder-4.3.2rc2/images/simpleview2.png`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/requirements.txt` & `Flask-AppBuilder-4.3.2rc2/requirements.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/rtd_requirements.txt` & `Flask-AppBuilder-4.3.2rc2/rtd_requirements.txt`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/setup.cfg` & `Flask-AppBuilder-4.3.2rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/setup.py` & `Flask-AppBuilder-4.3.2rc2/setup.py`

 * *Files identical despite different names*

### Comparing `Flask-AppBuilder-4.3.2rc1/tox.ini` & `Flask-AppBuilder-4.3.2rc2/tox.ini`

 * *Files identical despite different names*

