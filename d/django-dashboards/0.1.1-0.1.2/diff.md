# Comparing `tmp/django-dashboards-0.1.1.tar.gz` & `tmp/django-dashboards-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-dashboards-0.1.1.tar", last modified: Fri Apr 14 15:08:16 2023, max compression
+gzip compressed data, was "django-dashboards-0.1.2.tar", last modified: Mon May 22 08:17:33 2023, max compression
```

## Comparing `django-dashboards-0.1.1.tar` & `django-dashboards-0.1.2.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8641 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7707 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/component/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/component/chart/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/chart/chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/chart/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/form.py
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/component/table/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/table/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/table/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/table/table.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/component/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/menus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/menus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/menus/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/menus/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.344059 django-dashboards-0.1.1/dashboards/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.344059 django-dashboards-0.1.1/dashboards/static/dashboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/static/dashboards/css/
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/css/dashboards.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/static/dashboards/css/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/css/src/dashboards.css
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/css/src/grid.css
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/css/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/css/src/layout.css
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/css/src/menu.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.344059 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.352059 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/css/
--rw-r--r--   0 runner    (1001) docker     (123)    28778 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/css/datatables.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.356059 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/
--rw-r--r--   0 runner    (1001) docker     (123)    39713 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/alpine.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   190782 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/datatables.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    39433 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/htmx.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/htmx.sse.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    89663 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  3682474 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/plotly.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.344059 django-dashboards-0.1.1/dashboards/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/components/chart/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/chart/chart.html
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/component.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/components/form/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/form/form.html
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/loading.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/components/map/
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/map/map.html
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/partial.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/components/table/
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/table/basic.html
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/table/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/components/text/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/text/html.html
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/text/stat.html
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/components/text/text.html
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/dashboard_partial.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.344059 django-dashboards-0.1.1/dashboards/templates/dashboards/includes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/includes/static/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/includes/static/js.html
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/includes/static/style.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.348059 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/card.html
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/div.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/tabs/container.html
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/tabs/content.html
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/tabs/tab.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/dashboards/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/templatetags/dashboards.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/dashboards/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.360059 django-dashboards-0.1.1/django_dashboards.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8641 2023-04-14 15:08:16.000000 django-dashboards-0.1.1/django_dashboards.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-04-14 15:08:16.000000 django-dashboards-0.1.1/django_dashboards.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:08:16.000000 django-dashboards-0.1.1/django_dashboards.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-14 15:08:16.000000 django-dashboards-0.1.1/django_dashboards.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-14 15:08:16.000000 django-dashboards-0.1.1/django_dashboards.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.364059 django-dashboards-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.364059 django-dashboards-0.1.1/docs/dashboards/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.364059 django-dashboards-0.1.1/docs/dashboards/howto/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.372059 django-dashboards-0.1.1/docs/dashboards/howto/_images/
--rw-r--r--   0 runner    (1001) docker     (123)   100655 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/async_component.gif
--rw-r--r--   0 runner    (1001) docker     (123)    40145 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/components_add_form.png
--rw-r--r--   0 runner    (1001) docker     (123)   102530 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/components_chart_example.png
--rw-r--r--   0 runner    (1001) docker     (123)    22585 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/components_gauge.png
--rw-r--r--   0 runner    (1001) docker     (123)    85957 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/components_map_examples.png
--rw-r--r--   0 runner    (1001) docker     (123)    54151 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/components_table.png
--rw-r--r--   0 runner    (1001) docker     (123)  5090771 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/demo.gif
--rw-r--r--   0 runner    (1001) docker     (123)   152677 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/dependent_table_dashboard.gif
--rw-r--r--   0 runner    (1001) docker     (123)    29811 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/layout_basic.png
--rw-r--r--   0 runner    (1001) docker     (123)    52925 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/layout_complex.png
--rw-r--r--   0 runner    (1001) docker     (123)  1040391 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/quickstart_dashboard.gif
--rw-r--r--   0 runner    (1001) docker     (123)    35761 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/quickstart_dashboard.png
--rw-r--r--   0 runner    (1001) docker     (123)    86305 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/serializers_chart.png
--rw-r--r--   0 runner    (1001) docker     (123)    97282 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/serializers_layout.png
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_custom_component_template.png
--rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_custom_loading.png
--rw-r--r--   0 runner    (1001) docker     (123)   100070 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_custom_template.png
--rw-r--r--   0 runner    (1001) docker     (123)    79174 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_style.png
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/async.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.376059 django-dashboards-0.1.1/docs/dashboards/howto/components/
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/components/attributes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/components/custom.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/components/included.rst
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/components/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/dashboards.rst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/demo.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/dynamic.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/layout.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/menus.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/permissions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/quickstart.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.376059 django-dashboards-0.1.1/docs/dashboards/howto/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/serializers/chart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/serializers/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/serializers/table.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/settings.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/sse.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/templates.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/howto/views.rst
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/dashboards/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/docs_dj_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-14 15:08:16.384060 django-dashboards-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.376059 django-dashboards-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.376059 django-dashboards-0.1.1/tests/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.376059 django-dashboards-0.1.1/tests/dashboards/app1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/app1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/app1/dashboards.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.376059 django-dashboards-0.1.1/tests/dashboards/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.376059 django-dashboards-0.1.1/tests/dashboards/components/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     8179 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/test_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/test_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/components/test_text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/tests/dashboards/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/tests/dashboards/dashboard/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/snapshots/snap_test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/snapshots/snap_test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     4527 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/snapshots/snap_test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/test_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/test_model_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/dashboard/test_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/tests/dashboards/menu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/menu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/menu/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/menu/test_menutags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/tests/dashboards/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/snapshots/snap_test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/snapshots/snap_test_dashboard_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/snapshots/snap_test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/snapshots/snap_test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/test_urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/tests/dashboards/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/tests/dashboards/views/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/snapshots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/snapshots/snap_test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/snapshots/snap_test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/snapshots/snap_test_form_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/test_component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/dashboards/views/test_form_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:16.380059 django-dashboards-0.1.1/tests/meta/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/meta/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-14 15:08:12.000000 django-dashboards-0.1.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-22 08:17:33.613286 django-dashboards-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.569285 django-dashboards-0.1.2/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.569285 django-dashboards-0.1.2/dashboards/component/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.573285 django-dashboards-0.1.2/dashboards/component/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/chart/chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/chart/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8808 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.573285 django-dashboards-0.1.2/dashboards/component/table/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/table/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/table/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/table/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/component/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.573285 django-dashboards-0.1.2/dashboards/menus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/menus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/menus/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/menus/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.573285 django-dashboards-0.1.2/dashboards/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.553284 django-dashboards-0.1.2/dashboards/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.557284 django-dashboards-0.1.2/dashboards/static/dashboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.573285 django-dashboards-0.1.2/dashboards/static/dashboards/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/css/dashboards.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.573285 django-dashboards-0.1.2/dashboards/static/dashboards/css/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/css/src/dashboards.css
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/css/src/grid.css
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/css/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/css/src/layout.css
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/css/src/menu.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.557284 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.573285 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    28778 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/css/datatables.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.577285 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    39713 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/alpine.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   190782 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/datatables.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    39433 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/htmx.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/htmx.sse.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89663 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3682474 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/plotly.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.557284 django-dashboards-0.1.2/dashboards/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/components/chart/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/chart/chart.html
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/component.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/components/form/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/form/form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/loading.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/components/map/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/map/map.html
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/partial.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/components/table/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/table/basic.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/table/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/components/text/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/text/html.html
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/text/stat.html
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/components/text/text.html
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/dashboard_partial.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.561284 django-dashboards-0.1.2/dashboards/templates/dashboards/includes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.581285 django-dashboards-0.1.2/dashboards/templates/dashboards/includes/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/includes/static/js.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/includes/static/style.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.561284 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.585285 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/card.html
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/div.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.585285 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/tabs/container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/tabs/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/tabs/tab.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.585285 django-dashboards-0.1.2/dashboards/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/templatetags/dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/dashboards/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.585285 django-dashboards-0.1.2/django_dashboards.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-05-22 08:17:33.000000 django-dashboards-0.1.2/django_dashboards.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-05-22 08:17:33.000000 django-dashboards-0.1.2/django_dashboards.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:17:33.000000 django-dashboards-0.1.2/django_dashboards.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-22 08:17:33.000000 django-dashboards-0.1.2/django_dashboards.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 08:17:33.000000 django-dashboards-0.1.2/django_dashboards.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.585285 django-dashboards-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.585285 django-dashboards-0.1.2/docs/dashboards/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.585285 django-dashboards-0.1.2/docs/dashboards/howto/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.601286 django-dashboards-0.1.2/docs/dashboards/howto/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)   100655 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/async_component.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    40145 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/components_add_form.png
+-rw-r--r--   0 runner    (1001) docker     (123)   102530 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/components_chart_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22585 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/components_gauge.png
+-rw-r--r--   0 runner    (1001) docker     (123)    85957 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/components_map_examples.png
+-rw-r--r--   0 runner    (1001) docker     (123)    54151 2023-05-22 08:17:19.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/components_table.png
+-rw-r--r--   0 runner    (1001) docker     (123)  5090771 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/demo.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   152677 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/dependent_table_dashboard.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    29811 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/layout_basic.png
+-rw-r--r--   0 runner    (1001) docker     (123)    52925 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/layout_complex.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1040391 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/quickstart_dashboard.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    35761 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/quickstart_dashboard.png
+-rw-r--r--   0 runner    (1001) docker     (123)    86305 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/serializers_chart.png
+-rw-r--r--   0 runner    (1001) docker     (123)    97282 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/serializers_layout.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_custom_component_template.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16328 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_custom_loading.png
+-rw-r--r--   0 runner    (1001) docker     (123)   100070 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_custom_template.png
+-rw-r--r--   0 runner    (1001) docker     (123)    79174 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_style.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/async.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.605286 django-dashboards-0.1.2/docs/dashboards/howto/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/components/attributes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/components/custom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19130 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/components/included.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/components/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5421 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/dashboards.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/demo.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/dynamic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/layout.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/menus.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/permissions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/quickstart.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.605286 django-dashboards-0.1.2/docs/dashboards/howto/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7278 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/serializers/chart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/serializers/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/serializers/table.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4415 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/sse.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15378 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/howto/views.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/dashboards/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/docs_dj_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-22 08:17:33.613286 django-dashboards-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.605286 django-dashboards-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.605286 django-dashboards-0.1.2/tests/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.605286 django-dashboards-0.1.2/tests/dashboards/app1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/app1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/app1/dashboards.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.605286 django-dashboards-0.1.2/tests/dashboards/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/dashboards/components/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16334 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12204 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/test_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13790 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/components/test_text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/dashboards/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/dashboards/dashboard/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/snapshots/snap_test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/snapshots/snap_test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/snapshots/snap_test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/test_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4668 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/test_model_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/dashboard/test_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/dashboards/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/menu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/menu/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/menu/test_menutags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/dashboards/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/snapshots/snap_test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/snapshots/snap_test_dashboard_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/snapshots/snap_test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/snapshots/snap_test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/test_urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/dashboards/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/dashboards/views/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/snapshots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/snapshots/snap_test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/snapshots/snap_test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/snapshots/snap_test_form_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/test_component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/dashboards/views/test_form_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:33.609286 django-dashboards-0.1.2/tests/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/meta/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-22 08:17:20.000000 django-dashboards-0.1.2/tests/utils.py
```

### Comparing `django-dashboards-0.1.1/LICENSE` & `django-dashboards-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/PKG-INFO` & `django-dashboards-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dashboards
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tools for building data dashboards with Django
 Home-page: https://github.com/wildfish/django-dashboards
 Author: Wildfish
 Author-email: developers@wildfish.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -31,16 +31,22 @@
 Tools to help you build data dashboards in Django.
 
 https://github.com/wildfish/django-dashboards
 
 .. image:: https://github.com/wildfish/django-dashboards/actions/workflows/build.yml/badge.svg
     :target: https://github.com/wildfish/django-dashboards
 
-.. image:: https://coveralls.io/repos/wildfish/django-dashboards/badge.svg?branch=master&service=github
-    :target: https://coveralls.io/github/wildfish/django-dashboards?branch=main
+.. image:: https://codecov.io/gh/wildfish/django-dashboards/branch/main/graph/badge.svg
+  :target: https://codecov.io/gh/wildfish/django-dashboards
+
+.. image:: https://badge.fury.io/py/django-dashboards.svg
+    :target: https://pypi.python.org/pypi/django-dashboards/
+
+.. image:: https://img.shields.io/pypi/pyversions/django-dashboards.svg
+    :target: https://pypi.python.org/pypi/django-dashboards/
 
 Features
 ========
 
 * Dashboard view generation with components including stats, tables, charts and more.
 * HTMX driven dashboards and templates for a modern MPA interface.
```

### Comparing `django-dashboards-0.1.1/README.rst` & `django-dashboards-0.1.2/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,22 @@
 Tools to help you build data dashboards in Django.
 
 https://github.com/wildfish/django-dashboards
 
 .. image:: https://github.com/wildfish/django-dashboards/actions/workflows/build.yml/badge.svg
     :target: https://github.com/wildfish/django-dashboards
 
-.. image:: https://coveralls.io/repos/wildfish/django-dashboards/badge.svg?branch=master&service=github
-    :target: https://coveralls.io/github/wildfish/django-dashboards?branch=main
+.. image:: https://codecov.io/gh/wildfish/django-dashboards/branch/main/graph/badge.svg
+  :target: https://codecov.io/gh/wildfish/django-dashboards
+
+.. image:: https://badge.fury.io/py/django-dashboards.svg
+    :target: https://pypi.python.org/pypi/django-dashboards/
+
+.. image:: https://img.shields.io/pypi/pyversions/django-dashboards.svg
+    :target: https://pypi.python.org/pypi/django-dashboards/
 
 Features
 ========
 
 * Dashboard view generation with components including stats, tables, charts and more.
 * HTMX driven dashboards and templates for a modern MPA interface.
```

### Comparing `django-dashboards-0.1.1/dashboards/component/base.py` & `django-dashboards-0.1.2/dashboards/component/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from django.db.models import QuerySet
 from django.http import HttpRequest
 from django.template import Context
 from django.template.loader import render_to_string
 from django.urls import reverse, reverse_lazy
 from django.utils.module_loading import import_string
 from django.utils.safestring import mark_safe
+from django.utils.text import slugify
 
 from dashboards import config
 
 from ..types import ValueData
 
 
 if TYPE_CHECKING:
@@ -187,14 +188,17 @@
         if self.defer_url:
             url = self.defer_url(reverse_args=args)
         else:
             url = reverse("dashboards:dashboard_component", args=args)
 
         return url
 
+    def template_id(self):
+        return slugify(self.get_absolute_url())
+
     def __str__(self):
         return self.render(context=Context({}))
 
     def __repr__(self):
         return f"{self.key}={self.value}"
```

### Comparing `django-dashboards-0.1.1/dashboards/component/chart/chart.py` & `django-dashboards-0.1.2/dashboards/component/chart/chart.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/component/chart/serializers.py` & `django-dashboards-0.1.2/dashboards/component/chart/serializers.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/component/form.py` & `django-dashboards-0.1.2/dashboards/component/form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/component/layout.py` & `django-dashboards-0.1.2/dashboards/component/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     template wrapper for components
     """
 
     def get_component_context(self):
         component_context = self.component_context
         component_context.update(
             {
-                "css": css_template("dashboard-component", self.grid_css_classes),
+                "css": css_template(self.grid_css_classes),
                 "component_css": self.component_css,
             }
         )
 
         return component_context
 
     def render(self, dashboard, context: Context, **kwargs) -> str:
```

### Comparing `django-dashboards-0.1.1/dashboards/component/map.py` & `django-dashboards-0.1.2/dashboards/component/map.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/component/table/mixins.py` & `django-dashboards-0.1.2/dashboards/component/table/mixins.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/component/table/serializers.py` & `django-dashboards-0.1.2/dashboards/component/table/serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 
 @dataclass
 class SerializedTable:
     data: List[Dict[str, Any]]
     columns: Dict[str, Any]
     columns_datatables: List[Dict[str, Any]]
+    order: List[Any]
     draw: Optional[int] = 0
     total: Optional[int] = 0
     filtered: Optional[int] = 0
 
 
 class TableSerializer(TableMixin, ClassWithMeta):
     """
@@ -31,14 +32,15 @@
     SerializedTable returns the in a format accepted by datatables.js
     """
 
     _meta: Type["TableSerializer.Meta"]
 
     class Meta:
         columns: Dict[str, str]
+        order: List[str]
         title: Optional[str] = None
         model: Optional[str] = None
         first_as_absolute_url = False
         force_lower = True
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
@@ -128,20 +130,31 @@
                     if hasattr(self, f"get_{field}_value"):
                         value = getattr(self, f"get_{field}_value")(obj)
 
                     values[field] = value
 
                 processed_data.append(values)
 
+        order = [0, "asc"]
+        if hasattr(self._meta, "order"):
+            order = [
+                [
+                    list(self._meta.columns.keys()).index(v.replace("-", "")),
+                    "desc" if "-" in v else "asc",
+                ]
+                for v in self._meta.order
+            ]
+
         return SerializedTable(
             data=processed_data,
             columns=self._meta.columns,
             columns_datatables=[
                 {"data": d, "title": t} for d, t in self._meta.columns.items()
             ],
+            order=order,
             draw=draw,
             total=initial_count,
             filtered=filtered_count,
         )
 
     @staticmethod
     def apply_paginator(
```

### Comparing `django-dashboards-0.1.1/dashboards/component/table/table.py` & `django-dashboards-0.1.2/dashboards/component/table/table.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/component/text.py` & `django-dashboards-0.1.2/dashboards/component/text.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/config.py` & `django-dashboards-0.1.2/dashboards/config.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/dashboard.py` & `django-dashboards-0.1.2/dashboards/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/forms.py` & `django-dashboards-0.1.2/dashboards/forms.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/menus/menu.py` & `django-dashboards-0.1.2/dashboards/menus/menu.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/meta/__init__.py` & `django-dashboards-0.1.2/dashboards/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/permissions.py` & `django-dashboards-0.1.2/dashboards/permissions.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/registry.py` & `django-dashboards-0.1.2/dashboards/registry.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/static/dashboards/css/dashboards.css` & `django-dashboards-0.1.2/dashboards/static/dashboards/css/dashboards.css`

 * *Files 4% similar despite different names*

```diff
@@ -162,27 +162,27 @@
   width: 100%;
 }
 
 h1, h2, h3, h4, p, .tab-container {
   grid-column: 1 / 13;
 }
 
-.dashboard-component{
+.card{
   border-radius: 15px;
   background-color: var(--dark-two);
   display: grid;
   grid-template-columns: repeat(12, 1fr);
 }
 
-.dashboard-component *{
+.card *{
     /* allow sub nesting, by assuming not set is 12 */
     grid-column-end: span 12;
 }
 
-.tab-content div.active .dashboard-component{
+.tab-content div.active .card{
     border-radius: 0 15px 15px 15px;
 }
 
 .dashboard-component-inner {
   padding: 2rem;
 }
```

### Comparing `django-dashboards-0.1.1/dashboards/static/dashboards/css/src/dashboards.css` & `django-dashboards-0.1.2/dashboards/static/dashboards/css/src/dashboards.css`

 * *Files 5% similar despite different names*

```diff
@@ -6,27 +6,27 @@
   width: 100%;
 }
 
 h1, h2, h3, h4, p, .tab-container {
   grid-column: 1 / 13;
 }
 
-.dashboard-component{
+.card{
   border-radius: 15px;
   background-color: var(--dark-two);
   display: grid;
   grid-template-columns: repeat(12, 1fr);
 }
 
-.dashboard-component *{
+.card *{
     /* allow sub nesting, by assuming not set is 12 */
     grid-column-end: span 12;
 }
 
-.tab-content div.active .dashboard-component{
+.tab-content div.active .card{
     border-radius: 0 15px 15px 15px;
 }
 
 .dashboard-component-inner {
   padding: 2rem;
 }
```

### Comparing `django-dashboards-0.1.1/dashboards/static/dashboards/css/src/grid.css` & `django-dashboards-0.1.2/dashboards/static/dashboards/css/src/grid.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/static/dashboards/css/src/layout.css` & `django-dashboards-0.1.2/dashboards/static/dashboards/css/src/layout.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/static/dashboards/css/src/menu.css` & `django-dashboards-0.1.2/dashboards/static/dashboards/css/src/menu.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/static/dashboards/vendor/css/datatables.min.css` & `django-dashboards-0.1.2/dashboards/static/dashboards/vendor/css/datatables.min.css`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/alpine.min.js` & `django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/alpine.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/datatables.min.js` & `django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/datatables.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/htmx.min.js` & `django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/htmx.sse.min.js` & `django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/htmx.sse.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/jquery.min.js` & `django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/static/dashboards/vendor/js/plotly.min.js` & `django-dashboards-0.1.2/dashboards/static/dashboards/vendor/js/plotly.min.js`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/templates/dashboards/base.html` & `django-dashboards-0.1.2/dashboards/templates/dashboards/base.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/templates/dashboards/components/chart/chart.html` & `django-dashboards-0.1.2/dashboards/templates/dashboards/components/chart/chart.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-{% with "data_"|add:component.key as data_key %}
+{% with "data_"|add:component.template_id as data_key %}
     <script type="module">
-        var data_{{ component.key }} = {{rendered_value|safe}};
+        var data_{{ component.template_id }} = {{rendered_value|safe}};
         Plotly.newPlot(
-            '{{ component.key }}',
-            data_{{ component.key }}.data,
-            data_{{ component.key }}.layout,
+            '{{ component.template_id }}',
+            data_{{ component.template_id }}.data,
+            data_{{ component.template_id }}.layout,
             {
                 displayModeBar: {{ component.displayModeBar|yesno:'"hover",false'|safe }},
                 staticPlot: {{ component.staticPlot|yesno:"true,false" }},
                 responsive: {{ component.responsive|yesno:"true,false" }}
             },
         );
     </script>
 {% endwith %}
 
-<div id="{{ component.key }}" class="{{ component.css_classes|default_if_none:"" }}"></div>
+<div id="{{ component.template_id }}" class="{{ component.css_classes|default_if_none:"" }}"></div>
```

#### html2text {}

```diff
@@ -1,3 +1,3 @@
-{% with "data_"|add:component.key as data_key %}
+{% with "data_"|add:component.template_id as data_key %}
  {% endwith %}
  }}">
```

### Comparing `django-dashboards-0.1.1/dashboards/templates/dashboards/components/component.html` & `django-dashboards-0.1.2/dashboards/templates/dashboards/components/component.html`

 * *Files 2% similar despite different names*

```diff
@@ -6,13 +6,13 @@
          hx-trigger="{{ component.htmx_trigger_on }}intersect once{% if component.htmx_poll_rate %}, {{ component.htmx_poll_rate }}{% endif %} delay:{{ delay }}">
         <div class="htmx-indicator">
             {% include component.defer_loading_template_name %}
         </div>
     </div>
 {% else %}
     {% if component.cta %}<a href="{{ component.cta|cta_href:component.object }}">{% endif %}
-        <div id="component-{{ component.key }}-inner" class="dashboard-component-inner fade-in">
+        <div id="component-{{ component.template_id }}-inner" class="dashboard-component-inner fade-in">
             {% include component.template_name %}
         </div>
     {% if component.cta %}</a>{% endif %}
 {% endif %}
```

### Comparing `django-dashboards-0.1.1/dashboards/templates/dashboards/components/form/form.html` & `django-dashboards-0.1.2/dashboards/templates/dashboards/components/form/form.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% spaceless %}
-  <form hx-{{ rendered_value.method }}="{{ rendered_value.action }}?key={{ component.key }}" hx-trigger="{{ component.trigger }}" hx-swap="outerHTML" hx-target="#component-{{ component.key }}-inner">
+  <form hx-{{ rendered_value.method }}="{{ rendered_value.action }}?key={{ component.template_id }}" hx-trigger="{{ component.trigger }}" hx-swap="outerHTML" hx-target="#component-{{ component.template_id }}-inner">
     <table class="{{ component.css_classes.table }}">
       <tbody>
       {{ rendered_value.form.as_table }}
       {% if component.trigger == "submit" %}
         <tr>
           <td>&nbsp;</td>
           <td>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 {% spaceless %}
-{ rendered_value.method }}="{{ rendered_value.action }}?key={{ component.key
-}}" hx-trigger="{{ component.trigger }}" hx-swap="outerHTML" hx-
-target="#component-{{ component.key }}-inner">
+{ rendered_value.method }}="{{ rendered_value.action }}?key={
+{ component.template_id }}" hx-trigger="{{ component.trigger }}" hx-
+swap="outerHTML" hx-target="#component-{{ component.template_id }}-inner">
  [Submit]
 {% endspaceless %}
```

### Comparing `django-dashboards-0.1.1/dashboards/templates/dashboards/components/map/map.html` & `django-dashboards-0.1.2/dashboards/templates/dashboards/components/map/map.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-{% with "data_"|add:component.key as data_key %}
+{% with "data_"|add:component.template_id as data_key %}
     <script type="module">
-        var data_{{ component.key }} = {{rendered_value|safe}};
+        var data_{{ component.template_id }} = {{rendered_value|safe}};
 
         Plotly.newPlot(
-            '{{ component.key }}',
-            data_{{ component.key }}.data,
-            data_{{ component.key }}.layout,
+            '{{ component.template_id }}',
+            data_{{ component.template_id }}.data,
+            data_{{ component.template_id }}.layout,
             {
                 showLink: false,
                 responsive: {{ component.responsive|yesno:"true,false" }}
             },
         );
     </script>
 {% endwith %}
 
-<div id="{{ component.key }}" class="{{ component.css_classes }}"></div>
+<div id="{{ component.template_id }}" class="{{ component.css_classes }}"></div>
```

#### html2text {}

```diff
@@ -1,2 +1,2 @@
-{% with "data_"|add:component.key as data_key %}
+{% with "data_"|add:component.template_id as data_key %}
  {% endwith %}
```

### Comparing `django-dashboards-0.1.1/dashboards/templates/dashboards/components/table/basic.html` & `django-dashboards-0.1.2/dashboards/templates/dashboards/components/table/basic.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% load dashboards %}
 {% with columns=rendered_value.columns %}
-<div id="{{ component.key }}">
-  <table id="{{ component.key }}_table" class="{{ component.css_classes.table }}" style="width:100%">
+<div id="{{ component.template_id }}">
+  <table id="{{ component.template_id }}_table" class="{{ component.css_classes.table }}" style="width:100%">
     <thead>
     {% for title in columns.values %}
       <th>{{ title|safe }}</th>
     {% endfor %}
     </thead>
     <tbody>
     {% for row in rendered_value.data %}
```

### Comparing `django-dashboards-0.1.1/dashboards/templates/dashboards/components/text/stat.html` & `django-dashboards-0.1.2/dashboards/templates/dashboards/components/text/stat.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/templates/dashboards/dashboard.html` & `django-dashboards-0.1.2/dashboards/templates/dashboards/dashboard.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/templates/dashboards/layout/components/card.html` & `django-dashboards-0.1.2/dashboards/templates/dashboards/layout/components/card.html`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/templatetags/dashboards.py` & `django-dashboards-0.1.2/dashboards/templatetags/dashboards.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/urls.py` & `django-dashboards-0.1.2/dashboards/urls.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/dashboards/views.py` & `django-dashboards-0.1.2/dashboards/views.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/django_dashboards.egg-info/PKG-INFO` & `django-dashboards-0.1.2/django_dashboards.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-dashboards
-Version: 0.1.1
+Version: 0.1.2
 Summary: Tools for building data dashboards with Django
 Home-page: https://github.com/wildfish/django-dashboards
 Author: Wildfish
 Author-email: developers@wildfish.com
 License: BSD-3-Clause
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -31,16 +31,22 @@
 Tools to help you build data dashboards in Django.
 
 https://github.com/wildfish/django-dashboards
 
 .. image:: https://github.com/wildfish/django-dashboards/actions/workflows/build.yml/badge.svg
     :target: https://github.com/wildfish/django-dashboards
 
-.. image:: https://coveralls.io/repos/wildfish/django-dashboards/badge.svg?branch=master&service=github
-    :target: https://coveralls.io/github/wildfish/django-dashboards?branch=main
+.. image:: https://codecov.io/gh/wildfish/django-dashboards/branch/main/graph/badge.svg
+  :target: https://codecov.io/gh/wildfish/django-dashboards
+
+.. image:: https://badge.fury.io/py/django-dashboards.svg
+    :target: https://pypi.python.org/pypi/django-dashboards/
+
+.. image:: https://img.shields.io/pypi/pyversions/django-dashboards.svg
+    :target: https://pypi.python.org/pypi/django-dashboards/
 
 Features
 ========
 
 * Dashboard view generation with components including stats, tables, charts and more.
 * HTMX driven dashboards and templates for a modern MPA interface.
```

### Comparing `django-dashboards-0.1.1/django_dashboards.egg-info/SOURCES.txt` & `django-dashboards-0.1.2/django_dashboards.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/Makefile` & `django-dashboards-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/conf.py` & `django-dashboards-0.1.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "django-dashboards"
 copyright = "2023, Wildfish"
 author = "Wildfish"
-release = "0.1.1"
+release = "0.1.2"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ["sphinx.ext.autodoc"]
 
 templates_path = ["_templates"]
```

### Comparing `django-dashboards-0.1.1/docs/contributing.rst` & `django-dashboards-0.1.2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/async_component.gif` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/async_component.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/components_add_form.png` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/components_add_form.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/components_chart_example.png` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/components_chart_example.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/components_gauge.png` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/components_gauge.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/components_map_examples.png` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/components_map_examples.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/components_table.png` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/components_table.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/demo.gif` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/demo.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/dependent_table_dashboard.gif` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/dependent_table_dashboard.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/layout_basic.png` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/layout_basic.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/layout_complex.png` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/layout_complex.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/quickstart_dashboard.gif` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/quickstart_dashboard.gif`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/quickstart_dashboard.png` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/quickstart_dashboard.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/serializers_chart.png` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/serializers_chart.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/serializers_layout.png` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/serializers_layout.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_custom_component_template.png` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_custom_component_template.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_custom_loading.png` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_custom_loading.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_custom_template.png` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_custom_template.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/_images/templates_style.png` & `django-dashboards-0.1.2/docs/dashboards/howto/_images/templates_style.png`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/async.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/async.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/components/attributes.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/components/attributes.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/components/custom.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/components/custom.rst`

 * *Files 8% similar despite different names*

```diff
@@ -77,27 +77,27 @@
         {% if component.icon %}
             <div class="float-end">
                 {{ component.icon|safe }}
             </div>
         {% endif %}
 
         <script type="module">
-            var componentGauge = Gauge(document.getElementById("{{ component.key }}"), {
+            var componentGauge = Gauge(document.getElementById("{{ component.template_id }}"), {
                 max: {{rendered_value.max_value}},
                 label: function (value) {
                     return value;
                 },
                 value: {{rendered_value.value}},
             });
 
             componentGauge.setValue({{rendered_value.value}});
             componentGauge.setValueAnimated({{rendered_value.value}}, 2);
         </script>
 
-        <div id="{{ component.key }}" class="gauge-container">
+        <div id="{{ component.template_id }}" class="gauge-container">
             <span class="title-text">{{ rendered_value.title }}</span>
         </div>
         {% if component.href %}</a>{% endif %}
     </div>
 
 
 When creating a new template, the href, icon sections are boilerplate for base component features, you
```

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/components/included.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/components/included.rst`

 * *Files 1% similar despite different names*

```diff
@@ -346,14 +346,15 @@
     class StaffSerializer(TableSerializer):
         class Meta:
             title = "Staff table"
             columns = {
                 "id": "ID",
                 "first_name": "First Name",
             }
+            order = ["-first_name", "id"]
             # model = User
 
         @classmethod
         def get_queryset(cls, **kwargs):
             """
             kwargs are passed through from value/defer as above
             """
@@ -378,14 +379,15 @@
 * ``page_size`` (``int`` - ``default=10``): set the paging size
 * ``searching/paging/ordering`` (``bool`` - ``default=True``): enable/disable relevant datatables features.
 
 Additional `TableSerializer` Meta attributes
 
 * ``first_as_absolute_url`` (``bool`` - ``default=False``): if the model or object has a get_absolute_url use it in the first column.
 * ``force_lower`` - (``bool`` - ``default=True``): forces searching and sorting of data to use lower values.
+* ``order`` - (``list``): list of fields from columns to order by, prefix with - for descending.
 
 BasicTable
 ++++++++++
 
 Basic tables work the same as table, with the js, search & sort disabled.
 
 ::
```

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/components/index.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/components/index.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/dashboards.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/dashboards.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/demo.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/demo.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/dynamic.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/dynamic.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/layout.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/layout.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/menus.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/menus.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/permissions.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/permissions.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/quickstart.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/serializers/chart.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/serializers/chart.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/serializers/table.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/serializers/table.rst`

 * *Files 1% similar despite different names*

```diff
@@ -138,13 +138,13 @@
 **********************************
 
 Under the hood the Table component uses the Javascript library Datatables.
 This gives you the ability to filter, sort and paginate your data out the box.
 The TableSerializer has been built to accommodate this, knowing how to process and
 apply this to your dataset without you needing to do anything extra.
 
-If you decide to swap out the Table compoent for something other than Datatables
+If you decide to swap out the Table component for something other than Datatables
 you may need to implement your own ``filter()`` and ``sort()`` methods on the TableSerializer
 class.
 
 If you use the BasicTable component you do not have to worry about this as these features
 are not included.
```

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/settings.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/settings.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/sse.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/sse.rst`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         ...
 
 
 At a template level, taking SSEStat as an example, we can the built in SSE features in HTMX to connect to pushpin
 
 ::
 
-    <div hx-ext="sse" sse-connect="{{ component.pushpin_url }}" sse-swap="{{ component.key }}">
+    <div hx-ext="sse" sse-connect="{{ component.pushpin_url }}" sse-swap="{{ component.template_id }}">
       Contents of this box will be updated in real time
       with every SSE received.
     </div>
 
 
 In order for events to be sent you could either have a cron job, management command, celery task or one even
 one of our django-pipelines. For example in our demo, we render the Stat fully into an event:
```

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/templates.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/templates.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/howto/views.rst` & `django-dashboards-0.1.2/docs/dashboards/howto/views.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/dashboards/index.rst` & `django-dashboards-0.1.2/docs/dashboards/index.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/docs_dj_settings.py` & `django-dashboards-0.1.2/docs/docs_dj_settings.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/index.rst` & `django-dashboards-0.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/make.bat` & `django-dashboards-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/docs/requirements.txt` & `django-dashboards-0.1.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/setup.cfg` & `django-dashboards-0.1.2/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-dashboards
-version = 0.1.1
+version = 0.1.2
 description = Tools for building data dashboards with Django
 long_description = file: README.rst
 url = https://github.com/wildfish/django-dashboards
 author = Wildfish
 author_email = developers@wildfish.com
 license = BSD-3-Clause
 classifiers =
```

### Comparing `django-dashboards-0.1.1/tests/conftest.py` & `django-dashboards-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/app1/dashboards.py` & `django-dashboards-0.1.2/tests/dashboards/app1/dashboards.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_chart.py` & `django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_chart.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_form.py` & `django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_form.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 snapshots[
     "test_form_component__renders_value[False] 1"
 ] = """
 
 
 
     
-        <div id="component-test-inner" class="dashboard-component-inner fade-in">
-            <form hx-get="/dash/app1/testdashboard/test/@form/?key=test" hx-trigger="change" hx-swap="outerHTML" hx-target="#component-test-inner"><table class="table form-table"><tbody><tr><th><label for="id_number">Number:</label></th><td><select name="number" id="id_number"><option value="one">one</option><option value="two">two</option><option value="three">three</option></select></td></tr></tbody></table></form>
+        <div id="component-dashapp1testdashboardcomponenttest-inner" class="dashboard-component-inner fade-in">
+            <form hx-get="/dash/app1/testdashboard/test/@form/?key=dashapp1testdashboardcomponenttest" hx-trigger="change" hx-swap="outerHTML" hx-target="#component-dashapp1testdashboardcomponenttest-inner"><table class="table form-table"><tbody><tr><th><label for="id_number">Number:</label></th><td><select name="number" id="id_number"><option value="one">one</option><option value="two">two</option><option value="three">three</option></select></td></tr></tbody></table></form>
         </div>
     
 
 
 """
 
 snapshots[
     "test_form_component__renders_value[True] 1"
 ] = """
 
 
 
     
-        <div id="component-test-inner" class="dashboard-component-inner fade-in">
-            <form hx-get="/dash/app1/testdashboard/test/@form/?key=test" hx-trigger="change" hx-swap="outerHTML" hx-target="#component-test-inner"><table class="table form-table"><tbody><tr><th><label for="id_number">Number:</label></th><td><select name="number" id="id_number"><option value="one">one</option><option value="two">two</option><option value="three">three</option></select></td></tr></tbody></table></form>
+        <div id="component-dashapp1testdashboardcomponenttest-inner" class="dashboard-component-inner fade-in">
+            <form hx-get="/dash/app1/testdashboard/test/@form/?key=dashapp1testdashboardcomponenttest" hx-trigger="change" hx-swap="outerHTML" hx-target="#component-dashapp1testdashboardcomponenttest-inner"><table class="table form-table"><tbody><tr><th><label for="id_number">Number:</label></th><td><select name="number" id="id_number"><option value="one">one</option><option value="two">two</option><option value="three">three</option></select></td></tr></tbody></table></form>
         </div>
     
 
 
 """
```

### Comparing `django-dashboards-0.1.1/tests/dashboards/components/snapshots/snap_test_text.py` & `django-dashboards-0.1.2/tests/dashboards/components/snapshots/snap_test_text.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 snapshots[
     "test_cta_component__renders_value[False] 1"
 ] = """
 
 
 
     <a href="/">
-        <div id="component-test-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponenttest-inner" class="dashboard-component-inner fade-in">
             
 click here
 
         </div>
     </a>
 
 
@@ -27,15 +27,15 @@
 snapshots[
     "test_cta_component__renders_value[True] 1"
 ] = """
 
 
 
     <a href="/">
-        <div id="component-test-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponenttest-inner" class="dashboard-component-inner fade-in">
             
 click here
 
         </div>
     </a>
 
 
@@ -44,15 +44,15 @@
 snapshots[
     "test_stat_component__renders_value[False-component_kwargs0] 1"
 ] = """
 
 
 
     
-        <div id="component-test-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponenttest-inner" class="dashboard-component-inner fade-in">
             <div class="stat">
   
   
   <h2 class="stat__heading">100%</h2>
   <p class="stat__text">
     
     <span>increase</span>
@@ -68,15 +68,15 @@
 snapshots[
     "test_stat_component__renders_value[False-component_kwargs1] 1"
 ] = """
 
 
 
     
-        <div id="component-test-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponenttest-inner" class="dashboard-component-inner fade-in">
             <div class="stat">
   
   
   <h2 class="stat__heading">100%</h2>
   <p class="stat__text">
     
     <span>increase</span>
@@ -92,15 +92,15 @@
 snapshots[
     "test_stat_component__renders_value[False-component_kwargs2] 1"
 ] = """
 
 
 
     
-        <div id="component-test-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponenttest-inner" class="dashboard-component-inner fade-in">
             <div class="stat">
   
   
   <h2 class="stat__heading">100%</h2>
   <p class="stat__text">
     
     <span class="text-success">
@@ -122,15 +122,15 @@
 snapshots[
     "test_stat_component__renders_value[True-component_kwargs0] 1"
 ] = """
 
 
 
     
-        <div id="component-test-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponenttest-inner" class="dashboard-component-inner fade-in">
             <div class="stat">
   
   
   <h2 class="stat__heading">100%</h2>
   <p class="stat__text">
     
     <span>increase</span>
@@ -162,15 +162,15 @@
 snapshots[
     "test_stat_component__renders_value[True-component_kwargs2] 1"
 ] = """
 
 
 
     
-        <div id="component-test-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponenttest-inner" class="dashboard-component-inner fade-in">
             <div class="stat">
   
   
   <h2 class="stat__heading">100%</h2>
   <p class="stat__text">
     
     <span class="text-success">
```

### Comparing `django-dashboards-0.1.1/tests/dashboards/components/test_base.py` & `django-dashboards-0.1.2/tests/dashboards/components/test_base.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/components/test_chart.py` & `django-dashboards-0.1.2/tests/dashboards/components/test_chart.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/components/test_form.py` & `django-dashboards-0.1.2/tests/dashboards/components/test_form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/components/test_table.py` & `django-dashboards-0.1.2/tests/dashboards/components/test_table.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/components/test_text.py` & `django-dashboards-0.1.2/tests/dashboards/components/test_text.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/dashboard/snapshots/snap_test_form.py` & `django-dashboards-0.1.2/tests/dashboards/dashboard/snapshots/snap_test_form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/dashboard/snapshots/snap_test_layout.py` & `django-dashboards-0.1.2/tests/dashboards/dashboard/snapshots/snap_test_layout.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,31 +5,31 @@
 from snapshottest import Snapshot
 
 
 snapshots = Snapshot()
 
 snapshots[
     "test_dashboard__render_layout 1"
-] = """}{<hr /><div class="dashboard-component span-6 ">
-  <div class="dashboard-component span-6 ">
+] = """}{<hr /><div class="span-6 ">
+  <div class="span-6 ">
   
 
 
 
     
-        <div id="component-component_1-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponentcomponent_1-inner" class="dashboard-component-inner fade-in">
             
 value
 
         </div>
     
 
 
 
-</div><div class="dashboard-component span-6 ">
+</div><div class="span-6 ">
   
 
 
 
     <div hx-get="/dash/app1/testdashboard/@component/component_2/"
          hx-trigger="intersect once delay:1ms">
         <div class="htmx-indicator">
@@ -44,25 +44,25 @@
 
 snapshots["test_header__render 1"] = "<h2>some text....</h2>"
 
 snapshots["test_html__render 1"] = "some text...."
 
 snapshots[
     "test_html_component__card__css_classes 1"
-] = """<div class="dashboard-component span-6">
+] = """<div class="span-6">
   <div class="css_class">
     
     
     <div class="card-body">
       
 
 
 
     
-        <div id="component-component_1-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponentcomponent_1-inner" class="dashboard-component-inner fade-in">
             
 value
 
         </div>
     
 
 
@@ -70,44 +70,44 @@
     </div>
     
   </div>
 </div>"""
 
 snapshots[
     "test_html_component__div__css_classes 1"
-] = """<div class="dashboard-component span-6 css_class">
+] = """<div class="span-6 css_class">
   
 
 
 
     
-        <div id="component-component_1-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponentcomponent_1-inner" class="dashboard-component-inner fade-in">
             
 value
 
         </div>
     
 
 
 
 </div>"""
 
 snapshots[
     "test_html_component__render[Card] 1"
-] = """<div class="dashboard-component span-6">
+] = """<div class="span-6">
   <div class="card">
     
     
     <div class="card-body">
       
 
 
 
     
-        <div id="component-component_1-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponentcomponent_1-inner" class="dashboard-component-inner fade-in">
             
 value
 
         </div>
     
 
 
@@ -115,21 +115,21 @@
     </div>
     
   </div>
 </div>"""
 
 snapshots[
     "test_html_component__render[Div] 1"
-] = """<div class="dashboard-component span-6 ">
+] = """<div class="span-6 ">
   
 
 
 
     
-        <div id="component-component_1-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponentcomponent_1-inner" class="dashboard-component-inner fade-in">
             
 value
 
         </div>
     
 
 
@@ -146,15 +146,15 @@
     "test_html_component__tab__css_classes 1"
 ] = """<div :class="{ \'css_class active show\': tab === \'component_1\' }" x-show="tab === \'component_1\'">
     
 </div>"""
 
 snapshots[
     "test_html_component__tabcontainer__css_classes 1"
-] = """<div class="dashboard-component span-6 css_class" x-data="{ tab: \'component_1\' }">
+] = """<div class="span-6 css_class" x-data="{ tab: \'component_1\' }">
     <div id="" class="tabs" >
         <div class="tab">
   <a :class="{ \'active\': tab === \'component_1\' }" x-on:click.prevent="tab = \'component_1\'" href="#" class="">
     component_1
   </a>
 </div>
     </div>
@@ -169,15 +169,15 @@
 snapshots[
     "test_layout_component__render 1"
 ] = """
 
 
 
     
-        <div id="component-component_1-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponentcomponent_1-inner" class="dashboard-component-inner fade-in">
             
 value
 
         </div>
     
 
 
@@ -198,15 +198,15 @@
 snapshots[
     "test_layout_component__unknown_component_ignored 1"
 ] = """
 
 
 
     
-        <div id="component-component_1-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponentcomponent_1-inner" class="dashboard-component-inner fade-in">
             
 value
 
         </div>
     
 
 
@@ -223,27 +223,27 @@
 
 
 
 
 
 
     
-        <div id="component-component_3-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponentcomponent_3-inner" class="dashboard-component-inner fade-in">
             
 value from callable
 
         </div>
     
 
 
 """
 
 snapshots[
     "test_tab_container__render 1"
-] = """<div class="dashboard-component span-6 tab-container" x-data="{ tab: \'htmlhtmlsome-text\' }">
+] = """<div class="span-6 tab-container" x-data="{ tab: \'htmlhtmlsome-text\' }">
     <div id="" class="tabs" >
         <div class="tab">
   <a :class="{ \'active\': tab === \'htmlhtmlsome-text\' }" x-on:click.prevent="tab = \'htmlhtmlsome-text\'" href="#" class="">
     HTML(html=&#x27;some text....&#x27;)
   </a>
 </div>
     </div>
```

### Comparing `django-dashboards-0.1.1/tests/dashboards/dashboard/test_dashboard.py` & `django-dashboards-0.1.2/tests/dashboards/dashboard/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/dashboard/test_layout.py` & `django-dashboards-0.1.2/tests/dashboards/dashboard/test_layout.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/dashboard/test_model_dashboard.py` & `django-dashboards-0.1.2/tests/dashboards/dashboard/test_model_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/dashboard/test_permissions.py` & `django-dashboards-0.1.2/tests/dashboards/dashboard/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/fixtures.py` & `django-dashboards-0.1.2/tests/dashboards/fixtures.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/menu/test_menu.py` & `django-dashboards-0.1.2/tests/dashboards/menu/test_menu.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/menu/test_menutags.py` & `django-dashboards-0.1.2/tests/dashboards/menu/test_menutags.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/snapshots/snap_test_dashboard_form.py` & `django-dashboards-0.1.2/tests/dashboards/snapshots/snap_test_dashboard_form.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/snapshots/snap_test_layout.py` & `django-dashboards-0.1.2/tests/dashboards/snapshots/snap_test_layout.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/snapshots/snap_test_schema.py` & `django-dashboards-0.1.2/tests/dashboards/snapshots/snap_test_schema.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/test_registry.py` & `django-dashboards-0.1.2/tests/dashboards/test_registry.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/test_urls.py` & `django-dashboards-0.1.2/tests/dashboards/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/views/snapshots/snap_test_component.py` & `django-dashboards-0.1.2/tests/dashboards/views/snapshots/snap_test_component.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ] = """
 
 
 
 
 
     
-        <div id="component-component_2-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testdashboardcomponentcomponent_2-inner" class="dashboard-component-inner fade-in">
             
 value
 
         </div>
     
 
 
@@ -36,15 +36,15 @@
 ] = """
 
 
 
 
 
     
-        <div id="component-component_1-inner" class="dashboard-component-inner fade-in">
+        <div id="component-dashapp1testmodeldashboard1componentcomponent_1-inner" class="dashboard-component-inner fade-in">
             
 value
 
         </div>
```

### Comparing `django-dashboards-0.1.1/tests/dashboards/views/snapshots/snap_test_dashboard.py` & `django-dashboards-0.1.2/tests/dashboards/views/snapshots/snap_test_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/views/test_component.py` & `django-dashboards-0.1.2/tests/dashboards/views/test_component.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/views/test_dashboard.py` & `django-dashboards-0.1.2/tests/dashboards/views/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/dashboards/views/test_form_component.py` & `django-dashboards-0.1.2/tests/dashboards/views/test_form_component.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/meta/test_meta.py` & `django-dashboards-0.1.2/tests/meta/test_meta.py`

 * *Files identical despite different names*

### Comparing `django-dashboards-0.1.1/tests/settings.py` & `django-dashboards-0.1.2/tests/settings.py`

 * *Files identical despite different names*

