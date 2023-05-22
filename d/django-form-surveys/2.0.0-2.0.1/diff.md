# Comparing `tmp/django-form-surveys-2.0.0.tar.gz` & `tmp/django-form-surveys-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-form-surveys-2.0.0.tar", last modified: Mon May 15 09:18:06 2023, max compression
+gzip compressed data, was "django-form-surveys-2.0.1.tar", last modified: Mon May 22 01:52:39 2023, max compression
```

## Comparing `django-form-surveys-2.0.0.tar` & `django-form-surveys-2.0.1.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.290770 django-form-surveys-2.0.0/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6504 2023-05-15 09:18:06.290770 django-form-surveys-2.0.0/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5256 2023-05-15 04:57:18.000000 django-form-surveys-2.0.0/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.238770 django-form-surveys-2.0.0/django_form_surveys.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6504 2023-05-15 09:18:06.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4870 2023-05-15 09:18:06.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4287 2023-05-12 07:36:56.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/SOURCES.txt.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-15 09:18:06.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-12 07:36:56.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/dependency_links.txt.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-12-03 04:02:38.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/not-zip-safe
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       17 2023-05-15 09:18:06.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       17 2023-05-12 07:36:56.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/requires.txt.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-15 09:18:06.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-12 07:36:56.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/top_level.txt.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.242770 django-form-surveys-2.0.0/djf_surveys/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       81 2023-05-15 04:59:14.000000 django-form-surveys-2.0.0/djf_surveys/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      977 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/admin.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.242770 django-form-surveys-2.0.0/djf_surveys/admins/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/admins/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1378 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/admins/urls.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8232 2023-05-12 08:29:19.000000 django-form-surveys-2.0.0/djf_surveys/admins/views.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1650 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/app_settings.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      194 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/apps.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      315 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/context_processors.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6449 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/forms.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.230770 django-form-surveys-2.0.0/djf_surveys/locale/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.230770 django-form-surveys-2.0.0/djf_surveys/locale/en/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.242770 django-form-surveys-2.0.0/djf_surveys/locale/en/LC_MESSAGES/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5632 2023-05-15 09:18:04.000000 django-form-surveys-2.0.0/djf_surveys/locale/en/LC_MESSAGES/django.mo
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.230770 django-form-surveys-2.0.0/djf_surveys/locale/fr/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.246770 django-form-surveys-2.0.0/djf_surveys/locale/fr/LC_MESSAGES/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6132 2023-05-15 09:18:04.000000 django-form-surveys-2.0.0/djf_surveys/locale/fr/LC_MESSAGES/django.mo
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.230770 django-form-surveys-2.0.0/djf_surveys/locale/id/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.246770 django-form-surveys-2.0.0/djf_surveys/locale/id/LC_MESSAGES/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5908 2023-05-15 09:18:04.000000 django-form-surveys-2.0.0/djf_surveys/locale/id/LC_MESSAGES/django.mo
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.250770 django-form-surveys-2.0.0/djf_surveys/migrations/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3775 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0001_initial.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      860 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0002_auto_20220330_1033.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      553 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0003_auto_20220330_1036.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      850 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0004_auto_20220330_1112.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      377 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0005_auto_20220404_1518.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      451 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0006_survey_private_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      895 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0007_auto_20220525_1126.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0008_auto_20220721_0935.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      784 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0009_auto_20220803_0927.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8956 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0010_model_translation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      662 2022-12-26 04:31:54.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0011_alter_question_key.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      611 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/mixin.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7182 2023-04-17 04:11:38.000000 django-form-surveys-2.0.0/djf_surveys/models.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.230770 django-form-surveys-2.0.0/djf_surveys/static/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.230770 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.250770 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/css/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      321 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/css/rating.css
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   356448 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/css/tailwindcss-3.3.1.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   455935 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/css/tailwindcss-plugin-3.3.1.js
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.254770 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/images/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2962 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/images/star-border.png
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2729 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/images/star-fill.png
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.230770 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.254770 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/css/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   198463 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      121 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css.map
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.270770 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   270873 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   783041 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js.map
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12217 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50339 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js.map
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   425275 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  1151819 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js.map
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   539120 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  1929935 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js.map
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7140 2023-05-12 08:30:24.000000 django-form-surveys-2.0.0/djf_surveys/summary.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.234770 django-form-surveys-2.0.0/djf_surveys/templates/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.278770 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.282770 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1761 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7165 2023-05-12 07:25:35.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/form_preview.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1132 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/master.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      702 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/question_form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       45 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/question_form_v2.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1790 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/summary.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1490 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/survey_list.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4237 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/answer_list.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.282770 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/buttons/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      292 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/buttons/add_button.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      343 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/buttons/delete_button.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      309 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/buttons/edit_button.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      457 2022-12-02 18:18:26.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/buttons/share_button.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.286770 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1638 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/alert.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      326 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/alert_js.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2955 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/card_list_answer.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2779 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/card_list_survey.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      347 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/empty_state.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3324 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/header_nav.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3622 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/modal_choice_field_type.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3073 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/modal_delete.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/modal_delete_js.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3552 2023-05-12 07:21:46.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/pagination.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      968 2023-05-12 07:05:05.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/search_form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      570 2023-05-12 07:05:05.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/section_welcome.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      557 2022-12-02 18:18:26.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/share_link_button_js.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      557 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/star_border.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/star_fill.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      889 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/detail_result.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2014 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      792 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/master.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/survey_list.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.286770 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      247 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/attrs_exclude_id.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      538 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      364 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/datepicker.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5069 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/inline_choices.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/radio_option.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1767 2023-03-15 09:08:50.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/star_rating.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.290770 django-form-surveys-2.0.0/djf_surveys/templatetags/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templatetags/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      509 2023-03-15 09:08:50.000000 django-form-surveys-2.0.0/djf_surveys/templatetags/djf_survey_tags.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      396 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/tests.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      799 2022-12-02 18:18:26.000000 django-form-surveys-2.0.0/djf_surveys/urls.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3722 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      514 2023-05-12 08:31:40.000000 django-form-surveys-2.0.0/djf_surveys/validators.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8190 2022-12-26 03:50:09.000000 django-form-surveys-2.0.0/djf_surveys/views.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1096 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/widgets.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-15 09:18:06.290770 django-form-surveys-2.0.0/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3085 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/setup.py
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.573810 django-form-surveys-2.0.1/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1059 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/LICENSE
+-rw-r--r--   0 irfanpule   (501) staff       (20)      158 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/MANIFEST.in
+-rw-r--r--   0 irfanpule   (501) staff       (20)     6504 2023-05-22 01:52:39.573669 django-form-surveys-2.0.1/PKG-INFO
+-rw-r--r--   0 irfanpule   (501) staff       (20)     5256 2023-05-15 09:11:47.000000 django-form-surveys-2.0.1/README.md
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.542648 django-form-surveys-2.0.1/django_form_surveys.egg-info/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     6504 2023-05-22 01:52:39.000000 django-form-surveys-2.0.1/django_form_surveys.egg-info/PKG-INFO
+-rw-r--r--   0 irfanpule   (501) staff       (20)     4778 2023-05-22 01:52:39.000000 django-form-surveys-2.0.1/django_form_surveys.egg-info/SOURCES.txt
+-rw-r--r--   0 irfanpule   (501) staff       (20)        1 2023-05-22 01:52:39.000000 django-form-surveys-2.0.1/django_form_surveys.egg-info/dependency_links.txt
+-rw-r--r--   0 irfanpule   (501) staff       (20)        1 2023-05-02 07:50:06.000000 django-form-surveys-2.0.1/django_form_surveys.egg-info/not-zip-safe
+-rw-r--r--   0 irfanpule   (501) staff       (20)       17 2023-05-22 01:52:39.000000 django-form-surveys-2.0.1/django_form_surveys.egg-info/requires.txt
+-rw-r--r--   0 irfanpule   (501) staff       (20)      101 2023-05-22 01:52:39.000000 django-form-surveys-2.0.1/django_form_surveys.egg-info/top_level.txt
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.545716 django-form-surveys-2.0.1/djf_surveys/
+-rw-r--r--   0 irfanpule   (501) staff       (20)       81 2023-05-22 01:37:30.000000 django-form-surveys-2.0.1/djf_surveys/__init__.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      977 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/admin.py
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.546159 django-form-surveys-2.0.1/djf_surveys/admins/
+-rw-r--r--   0 irfanpule   (501) staff       (20)        0 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/admins/__init__.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1387 2023-05-22 00:55:51.000000 django-form-surveys-2.0.1/djf_surveys/admins/urls.py
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.546658 django-form-surveys-2.0.1/djf_surveys/admins/v2/
+-rw-r--r--   0 irfanpule   (501) staff       (20)        0 2023-05-22 00:58:51.000000 django-form-surveys-2.0.1/djf_surveys/admins/v2/__init__.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      710 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/admins/v2/forms.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3812 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/admins/v2/views.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     8232 2023-05-12 09:00:06.000000 django-form-surveys-2.0.1/djf_surveys/admins/views.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1650 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/app_settings.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      194 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/apps.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      315 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/context_processors.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     6449 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/forms.py
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.539821 django-form-surveys-2.0.1/djf_surveys/locale/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.539606 django-form-surveys-2.0.1/djf_surveys/locale/en/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.546877 django-form-surveys-2.0.1/djf_surveys/locale/en/LC_MESSAGES/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     5632 2023-05-15 09:15:54.000000 django-form-surveys-2.0.1/djf_surveys/locale/en/LC_MESSAGES/django.mo
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.539742 django-form-surveys-2.0.1/djf_surveys/locale/fr/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.547024 django-form-surveys-2.0.1/djf_surveys/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     6132 2023-05-15 09:15:54.000000 django-form-surveys-2.0.1/djf_surveys/locale/fr/LC_MESSAGES/django.mo
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.539875 django-form-surveys-2.0.1/djf_surveys/locale/id/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.547282 django-form-surveys-2.0.1/djf_surveys/locale/id/LC_MESSAGES/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     5908 2023-05-15 09:15:54.000000 django-form-surveys-2.0.1/djf_surveys/locale/id/LC_MESSAGES/django.mo
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.550335 django-form-surveys-2.0.1/djf_surveys/migrations/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3775 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/migrations/0001_initial.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      860 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/migrations/0002_auto_20220330_1033.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      553 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/migrations/0003_auto_20220330_1036.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      850 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/migrations/0004_auto_20220330_1112.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      377 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/migrations/0005_auto_20220404_1518.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      451 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/migrations/0006_survey_private_response.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      895 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/migrations/0007_auto_20220525_1126.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      520 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/migrations/0008_auto_20220721_0935.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      784 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/migrations/0009_auto_20220803_0927.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     8956 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/migrations/0010_model_translation.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      662 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/migrations/0011_alter_question_key.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)        0 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/migrations/__init__.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      611 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/mixin.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     7182 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/models.py
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.540103 django-form-surveys-2.0.1/djf_surveys/static/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.540320 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.551340 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/css/
+-rw-r--r--   0 irfanpule   (501) staff       (20)      321 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/css/rating.css
+-rw-r--r--   0 irfanpule   (501) staff       (20)   356448 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/css/tailwindcss-3.3.1.js
+-rw-r--r--   0 irfanpule   (501) staff       (20)   455935 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/css/tailwindcss-plugin-3.3.1.js
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.552217 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/images/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     2962 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/images/star-border.png
+-rw-r--r--   0 irfanpule   (501) staff       (20)     2729 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/images/star-fill.png
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.540452 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.552916 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/css/
+-rw-r--r--   0 irfanpule   (501) staff       (20)   198463 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css
+-rw-r--r--   0 irfanpule   (501) staff       (20)      121 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css.map
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.564375 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/
+-rw-r--r--   0 irfanpule   (501) staff       (20)   270873 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js
+-rw-r--r--   0 irfanpule   (501) staff       (20)   783041 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js.map
+-rw-r--r--   0 irfanpule   (501) staff       (20)    12217 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js
+-rw-r--r--   0 irfanpule   (501) staff       (20)    50339 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js.map
+-rw-r--r--   0 irfanpule   (501) staff       (20)   425275 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js
+-rw-r--r--   0 irfanpule   (501) staff       (20)  1151819 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js.map
+-rw-r--r--   0 irfanpule   (501) staff       (20)   539120 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js
+-rw-r--r--   0 irfanpule   (501) staff       (20)  1929935 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js.map
+-rw-r--r--   0 irfanpule   (501) staff       (20)     7140 2023-05-12 09:00:06.000000 django-form-surveys-2.0.1/djf_surveys/summary.py
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.540587 django-form-surveys-2.0.1/djf_surveys/templates/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.567530 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.568734 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/admins/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1761 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/admins/form.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     7165 2023-05-12 09:00:06.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/admins/form_preview.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1132 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/admins/master.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      702 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/admins/question_form.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)       45 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/admins/question_form_v2.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1790 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/admins/summary.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1490 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/admins/survey_list.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     4237 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/answer_list.html
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.569315 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/buttons/
+-rw-r--r--   0 irfanpule   (501) staff       (20)      292 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/buttons/add_button.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      343 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/buttons/delete_button.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      309 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/buttons/edit_button.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      457 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/buttons/share_button.html
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.572256 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1638 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/alert.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      326 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/alert_js.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     2955 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/card_list_answer.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     2779 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/card_list_survey.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      347 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/empty_state.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3324 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/header_nav.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3622 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/modal_choice_field_type.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3073 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/modal_delete.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      777 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/modal_delete_js.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3552 2023-05-12 09:00:06.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/pagination.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      968 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/search_form.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      570 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/section_welcome.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      557 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/share_link_button_js.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      557 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/star_border.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)        0 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/star_fill.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      889 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/detail_result.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     2014 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/form.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      792 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/master.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1189 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/survey_list.html
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.573141 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/widgets/
+-rw-r--r--   0 irfanpule   (501) staff       (20)      247 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/widgets/attrs_exclude_id.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      538 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      364 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/widgets/datepicker.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     5069 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/widgets/inline_choices.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)      520 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/widgets/radio_option.html
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1767 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/widgets/star_rating.html
+drwxr-xr-x   0 irfanpule   (501) staff       (20)        0 2023-05-22 01:52:39.573422 django-form-surveys-2.0.1/djf_surveys/templatetags/
+-rw-r--r--   0 irfanpule   (501) staff       (20)        0 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/templatetags/__init__.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      509 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/templatetags/djf_survey_tags.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      396 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/tests.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      799 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/urls.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3722 2023-05-12 07:00:04.000000 django-form-surveys-2.0.1/djf_surveys/utils.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)      514 2023-05-12 09:00:06.000000 django-form-surveys-2.0.1/djf_surveys/validators.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     8190 2022-12-26 03:54:38.000000 django-form-surveys-2.0.1/djf_surveys/views.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)     1096 2023-05-15 09:14:45.000000 django-form-surveys-2.0.1/djf_surveys/widgets.py
+-rw-r--r--   0 irfanpule   (501) staff       (20)       38 2023-05-22 01:52:39.573855 django-form-surveys-2.0.1/setup.cfg
+-rw-r--r--   0 irfanpule   (501) staff       (20)     3070 2023-05-22 01:39:07.000000 django-form-surveys-2.0.1/setup.py
```

### Comparing `django-form-surveys-2.0.0/LICENSE` & `django-form-surveys-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/PKG-INFO` & `django-form-surveys-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-form-surveys
-Version: 2.0.0
+Version: 2.0.1
 Summary: A simple Django app to conduct Web-based survey
 Home-page: https://irfanpule.github.io/django-form-surveys
 Author: irfanpule
 Author-email: irfan.pule2@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-form-surveys-2.0.0/README.md` & `django-form-surveys-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/django_form_surveys.egg-info/PKG-INFO` & `django-form-surveys-2.0.1/django_form_surveys.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-form-surveys
-Version: 2.0.0
+Version: 2.0.1
 Summary: A simple Django app to conduct Web-based survey
 Home-page: https://irfanpule.github.io/django-form-surveys
 Author: irfanpule
 Author-email: irfan.pule2@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `django-form-surveys-2.0.0/django_form_surveys.egg-info/SOURCES.txt` & `django-form-surveys-2.0.1/django_form_surveys.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 django_form_surveys.egg-info/PKG-INFO
 django_form_surveys.egg-info/SOURCES.txt
-django_form_surveys.egg-info/SOURCES.txt.py
 django_form_surveys.egg-info/dependency_links.txt
-django_form_surveys.egg-info/dependency_links.txt.py
 django_form_surveys.egg-info/not-zip-safe
 django_form_surveys.egg-info/requires.txt
-django_form_surveys.egg-info/requires.txt.py
 django_form_surveys.egg-info/top_level.txt
-django_form_surveys.egg-info/top_level.txt.py
 djf_surveys/__init__.py
 djf_surveys/admin.py
 djf_surveys/app_settings.py
 djf_surveys/apps.py
 djf_surveys/context_processors.py
 djf_surveys/forms.py
 djf_surveys/mixin.py
@@ -26,14 +22,17 @@
 djf_surveys/utils.py
 djf_surveys/validators.py
 djf_surveys/views.py
 djf_surveys/widgets.py
 djf_surveys/admins/__init__.py
 djf_surveys/admins/urls.py
 djf_surveys/admins/views.py
+djf_surveys/admins/v2/__init__.py
+djf_surveys/admins/v2/forms.py
+djf_surveys/admins/v2/views.py
 djf_surveys/locale/en/LC_MESSAGES/django.mo
 djf_surveys/locale/fr/LC_MESSAGES/django.mo
 djf_surveys/locale/id/LC_MESSAGES/django.mo
 djf_surveys/migrations/0001_initial.py
 djf_surveys/migrations/0002_auto_20220330_1033.py
 djf_surveys/migrations/0003_auto_20220330_1036.py
 djf_surveys/migrations/0004_auto_20220330_1112.py
```

### Comparing `django-form-surveys-2.0.0/djf_surveys/admin.py` & `django-form-surveys-2.0.1/djf_surveys/admin.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/admins/urls.py` & `django-form-surveys-2.0.1/djf_surveys/admins/urls.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 urlpatterns = [
     path('', admin_views.AdminSurveyListView.as_view(), name='admin_survey'),
     path('create/survey/', admin_views.AdminCrateSurveyView.as_view(), name='admin_create_survey'),
     path('edit/survey/<str:slug>/', admin_views.AdminEditSurveyView.as_view(), name='admin_edit_survey'),
     path('delete/survey/<str:slug>/', admin_views.AdminDeleteSurveyView.as_view(), name='admin_delete_survey'),
     path('forms/<str:slug>/', admin_views.AdminSurveyFormView.as_view(), name='admin_forms_survey'),
-    path('question/add/<int:pk>/<int:type_field>', admin_views_v2.AdminCreateQuestionView.as_view(), name='admin_create_question'),
+    path('question/add/<int:pk>/<int:type_field>', admin_views_v2.AdminCreateQuestionView.as_view(),
+         name='admin_create_question'),
     path('question/edit/<int:pk>/', admin_views_v2.AdminUpdateQuestionView.as_view(), name='admin_edit_question'),
     path('question/delete/<int:pk>/', admin_views.AdminDeleteQuestionView.as_view(), name='admin_delete_question'),
     path('question/ordering/', admin_views.AdminChangeOrderQuestionView.as_view(), name='admin_change_order_question'),
     path('download/survey/<str:slug>/', admin_views.DownloadResponseSurveyView.as_view(), name='admin_download_survey'),
     path('summary/survey/<str:slug>/', admin_views.SummaryResponseSurveyView.as_view(), name='admin_summary_survey'),
 ]
```

### Comparing `django-form-surveys-2.0.0/djf_surveys/admins/views.py` & `django-form-surveys-2.0.1/djf_surveys/admins/views.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/app_settings.py` & `django-form-surveys-2.0.1/djf_surveys/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/forms.py` & `django-form-surveys-2.0.1/djf_surveys/forms.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/locale/en/LC_MESSAGES/django.mo` & `django-form-surveys-2.0.1/djf_surveys/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/locale/fr/LC_MESSAGES/django.mo` & `django-form-surveys-2.0.1/djf_surveys/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/locale/id/LC_MESSAGES/django.mo` & `django-form-surveys-2.0.1/djf_surveys/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/migrations/0001_initial.py` & `django-form-surveys-2.0.1/djf_surveys/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/migrations/0002_auto_20220330_1033.py` & `django-form-surveys-2.0.1/djf_surveys/migrations/0002_auto_20220330_1033.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/migrations/0003_auto_20220330_1036.py` & `django-form-surveys-2.0.1/djf_surveys/migrations/0003_auto_20220330_1036.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/migrations/0004_auto_20220330_1112.py` & `django-form-surveys-2.0.1/djf_surveys/migrations/0004_auto_20220330_1112.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/migrations/0007_auto_20220525_1126.py` & `django-form-surveys-2.0.1/djf_surveys/migrations/0007_auto_20220525_1126.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/migrations/0008_auto_20220721_0935.py` & `django-form-surveys-2.0.1/djf_surveys/migrations/0008_auto_20220721_0935.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/migrations/0009_auto_20220803_0927.py` & `django-form-surveys-2.0.1/djf_surveys/migrations/0009_auto_20220803_0927.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/migrations/0010_model_translation.py` & `django-form-surveys-2.0.1/djf_surveys/migrations/0010_model_translation.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/migrations/0011_alter_question_key.py` & `django-form-surveys-2.0.1/djf_surveys/migrations/0011_alter_question_key.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/mixin.py` & `django-form-surveys-2.0.1/djf_surveys/mixin.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/models.py` & `django-form-surveys-2.0.1/djf_surveys/models.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/css/tailwindcss-3.3.1.js` & `django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/css/tailwindcss-3.3.1.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/css/tailwindcss-plugin-3.3.1.js` & `django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/css/tailwindcss-plugin-3.3.1.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/images/star-border.png` & `django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/images/star-border.png`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/images/star-fill.png` & `django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/images/star-fill.png`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css` & `django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js` & `django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js.map` & `django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js.map`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js` & `django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js.map` & `django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js.map`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js` & `django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js.map` & `django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js.map`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js` & `django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js.map` & `django-form-surveys-2.0.1/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js.map`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/summary.py` & `django-form-surveys-2.0.1/djf_surveys/summary.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/form.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/admins/form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/form_preview.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/admins/form_preview.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/master.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/admins/master.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/question_form.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/admins/question_form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/summary.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/admins/summary.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/survey_list.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/admins/survey_list.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/answer_list.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/answer_list.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/alert.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/alert.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/card_list_answer.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/card_list_answer.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/card_list_survey.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/card_list_survey.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/header_nav.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/header_nav.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/modal_choice_field_type.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/modal_choice_field_type.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/modal_delete.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/modal_delete.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/modal_delete_js.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/modal_delete_js.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/pagination.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/pagination.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/search_form.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/search_form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/section_welcome.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/section_welcome.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/share_link_button_js.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/share_link_button_js.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/star_border.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/components/star_border.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/detail_result.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/detail_result.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/form.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/master.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/master.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/survey_list.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/survey_list.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/inline_choices.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/widgets/inline_choices.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/radio_option.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/widgets/radio_option.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/star_rating.html` & `django-form-surveys-2.0.1/djf_surveys/templates/djf_surveys/widgets/star_rating.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/urls.py` & `django-form-surveys-2.0.1/djf_surveys/urls.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/utils.py` & `django-form-surveys-2.0.1/djf_surveys/utils.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/validators.py` & `django-form-surveys-2.0.1/djf_surveys/validators.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/views.py` & `django-form-surveys-2.0.1/djf_surveys/views.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/djf_surveys/widgets.py` & `django-form-surveys-2.0.1/djf_surveys/widgets.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-2.0.0/setup.py` & `django-form-surveys-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import re
 import sys
 from io import open
 
-from setuptools import find_packages, setup
+from setuptools import setup
 
 
 def read(f):
     return open(f, 'r', encoding='utf-8').read()
 
 
 def get_version(package):
```

