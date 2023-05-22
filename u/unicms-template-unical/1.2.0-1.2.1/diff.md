# Comparing `tmp/unicms_template_unical-1.2.0.tar.gz` & `tmp/unicms_template_unical-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicms_template_unical-1.2.0.tar", last modified: Tue Apr 11 09:19:33 2023, max compression
+gzip compressed data, was "unicms_template_unical-1.2.1.tar", last modified: Mon May 22 07:36:33 2023, max compression
```

## Comparing `unicms_template_unical-1.2.0.tar` & `unicms_template_unical-1.2.1.tar`

### file list

```diff
@@ -1,213 +1,214 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.515947 unicms_template_unical-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-11 09:19:33.515947 unicms_template_unical-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 09:19:33.515947 unicms_template_unical-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.483947 unicms_template_unical-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.487947 unicms_template_unical-1.2.0/src/unicms_template_unical/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.483947 unicms_template_unical-1.2.0/src/unicms_template_unical/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.483947 unicms_template_unical-1.2.0/src/unicms_template_unical/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.487947 unicms_template_unical-1.2.0/src/unicms_template_unical/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    22153 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.483947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.487947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/css/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.487947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/css/colors/
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/css/colors/unicms_exbriner.css
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/css/colors/unicms_unical.css
--rw-r--r--   0 runner    (1001) docker     (123)     9944 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/css/unicms_unical.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.487947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    43664 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.491947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/addressbook.svg
--rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/agenda.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/alert-red.svg
--rw-r--r--   0 runner    (1001) docker     (123)   130694 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/banner_1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/chi.png
--rw-r--r--   0 runner    (1001) docker     (123)    17329 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/dimes.svg
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/en.png
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/esp.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.491947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/favicon/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/favicon/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/favicon/favicon-32x32.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.495947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/ar.svg
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/en.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/es.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/eu.svg
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/fr.svg
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/it.svg
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/pt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/ru.svg
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/zh.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/ita.png
--rw-r--r--   0 runner    (1001) docker     (123)   312996 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/library1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo1.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_back.svg
--rw-r--r--   0 runner    (1001) docker     (123)    32050 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_presta.svg
--rw-r--r--   0 runner    (1001) docker     (123)    42300 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_unical_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_white.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.495947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/HRS4R.svg
--rw-r--r--   0 runner    (1001) docker     (123)    24514 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/ctc.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25799 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/demacs.svg
--rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/desf.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dfssn.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/diam.svg
--rw-r--r--   0 runner    (1001) docker     (123)    27886 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dibest.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dices.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28422 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dimeg.svg
--rw-r--r--   0 runner    (1001) docker     (123)    31883 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dimes.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22720 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dinci.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25608 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/discag.svg
--rw-r--r--   0 runner    (1001) docker     (123)    25944 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dispes.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23078 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/disu.svg
--rw-r--r--   0 runner    (1001) docker     (123)   106385 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/eu_funded.svg
--rw-r--r--   0 runner    (1001) docker     (123)    23410 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/eu_funded_white.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/exbriner.png
--rw-r--r--   0 runner    (1001) docker     (123)    20713 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/fis.svg
--rw-r--r--   0 runner    (1001) docker     (123)   473786 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/master_ges.png
--rw-r--r--   0 runner    (1001) docker     (123)   356948 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/news1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   441153 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/news2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   422058 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/news3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   126770 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/ponte-bucci-1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   508364 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/unical_banner.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    23187 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/unical_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.499947 unicms_template_unical-1.2.0/src/unicms_template_unical/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/js/external_link_new_tab.js
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/static/js/unicms_api_utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.499947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/500.html
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.499947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/base_v_original.html
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/error-page.html
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/unical_api_list.html
--rw-r--r--   0 runner    (1001) docker     (123)    32264 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/unicms_unical.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.507947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_3_level_page.html
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_3_level_page_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_contact.html
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_contact_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_buttons_childs.html
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_buttons_other_items.html
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs.html
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_collapse_other_items.html
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_@.html
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_arrow.html
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_chat.html
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_document.html
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_main.html
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_side.html
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_side_other_items.html
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_side_other_parent_same_level.html
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_to_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_2.html
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_alert.html
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_box_1.html
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_full_view_light.html
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_full_view_only_text.html
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_links.html
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_card.html
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards.html
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2_home.html
--rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html
--rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3_home.html
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4.html
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4_home.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.483947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.507947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_1/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_1/center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_1/right_spaced.html
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_1/section_center_alternative.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.507947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_2/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_2/center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_2/right_spaced.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.507947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_3/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_3/center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/grid/section_3/right_spaced.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.507947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/inits/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/inits/brython-init.html
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/loading-jumbo.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.511947 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department.html
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_ctc.html
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_demacs.html
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_desf.html
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dfssn.html
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_diam.html
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dibest.html
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dices.html
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dimeg.html
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dimes.html
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dinci.html
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_discag.html
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dispes.html
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_disu.html
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_fis.html
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/master_ges.html
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/multi_language.html
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/opendata.html
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/portale_home_v_original.html
--rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/project_exbriner.html
--rw-r--r--   0 runner    (1001) docker     (123)    15513 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/publication_list.html
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/publication_view.html
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/publication_view_hero_original.html
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/unical.html
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/unical_center_top_ab_a_double.html
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/unical_main_center_alternative.html
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/unical_right_spaced.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.511947 unicms_template_unical-1.2.0/src/unicms_template_unical/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-11 09:19:21.000000 unicms_template_unical-1.2.0/src/unicms_template_unical/templatetags/unicms_template_unical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 09:19:33.511947 unicms_template_unical-1.2.0/unicms_template_unical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-04-11 09:19:33.000000 unicms_template_unical-1.2.0/unicms_template_unical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11989 2023-04-11 09:19:33.000000 unicms_template_unical-1.2.0/unicms_template_unical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 09:19:33.000000 unicms_template_unical-1.2.0/unicms_template_unical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-11 09:19:33.000000 unicms_template_unical-1.2.0/unicms_template_unical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 09:19:33.000000 unicms_template_unical-1.2.0/unicms_template_unical.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.980769 unicms_template_unical-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-22 07:36:33.980769 unicms_template_unical-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 07:36:33.980769 unicms_template_unical-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.932769 unicms_template_unical-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.940769 unicms_template_unical-1.2.1/src/unicms_template_unical/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.932769 unicms_template_unical-1.2.1/src/unicms_template_unical/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.932769 unicms_template_unical-1.2.1/src/unicms_template_unical/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.940769 unicms_template_unical-1.2.1/src/unicms_template_unical/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    23781 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.936769 unicms_template_unical-1.2.1/src/unicms_template_unical/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.940769 unicms_template_unical-1.2.1/src/unicms_template_unical/static/css/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.940769 unicms_template_unical-1.2.1/src/unicms_template_unical/static/css/colors/
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/css/colors/unicms_exbriner.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/css/colors/unicms_unical.css
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/css/unicms_exbriner.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/css/unicms_unical.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.940769 unicms_template_unical-1.2.1/src/unicms_template_unical/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    43664 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.948769 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/addressbook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    10243 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/agenda.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/alert-red.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   130694 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/banner_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/chi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17329 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/dimes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/en.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/esp.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.948769 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/favicon/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/favicon/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/favicon/favicon-32x32.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.952769 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/flags/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/flags/ar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/flags/en.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/flags/es.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/flags/eu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/flags/fr.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/flags/it.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/flags/pt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/flags/ru.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/flags/zh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/ita.png
+-rw-r--r--   0 runner    (1001) docker     (123)   312996 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/library1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    27664 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logo1.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logo_back.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    32050 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logo_presta.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    42300 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logo_unical_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logo_white.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.956769 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/HRS4R.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    24514 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/ctc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25799 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/demacs.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    27889 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/desf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28678 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/dfssn.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23742 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/diam.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    27886 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/dibest.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25693 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/dices.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28422 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/dimeg.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    31883 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/dimes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22720 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/dinci.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25608 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/discag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    25944 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/dispes.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23078 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/disu.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   106385 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/eu_funded.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    23410 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/eu_funded_white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/exbriner.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20713 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/fis.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   473786 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/master_ges.png
+-rw-r--r--   0 runner    (1001) docker     (123)   356948 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/news1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   441153 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/news2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   422058 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/news3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   126770 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/ponte-bucci-1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   508364 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/unical_banner.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    23187 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/unical_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.956769 unicms_template_unical-1.2.1/src/unicms_template_unical/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/js/external_link_new_tab.js
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/static/js/unicms_api_utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.956769 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.956769 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/bases/
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/bases/base_v_original.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/bases/error-page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/bases/unical_api_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32078 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/bases/unicms_unical.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.972769 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_3_level_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_3_level_page_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_contact.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_contact_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_buttons_childs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_buttons_other_items.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_collapse_item_childs_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_collapse_other_items.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_@.html
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_arrow.html
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_chat.html
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_document.html
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_side.html
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_side_other_items.html
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_side_other_parent_same_level.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_to_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_alert.html
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_box_1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_full_view_light.html
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_full_view_only_text.html
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_links.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_card.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3_home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4_home.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.936769 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/grid/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.972769 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/grid/section_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/grid/section_1/center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/grid/section_1/right_spaced.html
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/grid/section_1/section_center_alternative.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.972769 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/grid/section_2/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/grid/section_2/center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/grid/section_2/right_spaced.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.972769 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/grid/section_3/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/grid/section_3/center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/grid/section_3/right_spaced.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.972769 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/inits/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/inits/brython-init.html
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/loading-jumbo.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.976769 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_ctc.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_demacs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_desf.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_dfssn.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_diam.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_dibest.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_dices.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_dimeg.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_dimes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_dinci.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_discag.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_dispes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_disu.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_fis.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/master_ges.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/multi_language.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/opendata.html
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/portale_home_v_original.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/project_exbriner.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15513 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/publication_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/publication_view.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/publication_view_hero_original.html
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/unical.html
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/unical_center_top_ab_a_double.html
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/unical_main_center_alternative.html
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/unical_right_spaced.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.976769 unicms_template_unical-1.2.1/src/unicms_template_unical/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-22 07:36:21.000000 unicms_template_unical-1.2.1/src/unicms_template_unical/templatetags/unicms_template_unical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 07:36:33.980769 unicms_template_unical-1.2.1/unicms_template_unical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-22 07:36:33.000000 unicms_template_unical-1.2.1/unicms_template_unical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-05-22 07:36:33.000000 unicms_template_unical-1.2.1/unicms_template_unical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 07:36:33.000000 unicms_template_unical-1.2.1/unicms_template_unical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-22 07:36:33.000000 unicms_template_unical-1.2.1/unicms_template_unical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 07:36:33.000000 unicms_template_unical-1.2.1/unicms_template_unical.egg-info/top_level.txt
```

### Comparing `unicms_template_unical-1.2.0/LICENSE` & `unicms_template_unical-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/PKG-INFO` & `unicms_template_unical-1.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicms_template_unical
-Version: 1.2.0
+Version: 1.2.1
 Summary: uniCMS Unical Template based on Bootstrap Italia
 Home-page: https://github.com/UniversitaDellaCalabria/unicms-template-unical
 Author: Giuseppe De Marco, Francesco Filicetti
 Author-email: giuseppe.demarco@unical.it, francesco.filicetti@unical.it
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `unicms_template_unical-1.2.0/setup.py` & `unicms_template_unical-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  twine upload dist/*
 
 SRC_FOLDER = 'src'
 PKG_NAME = 'unicms_template_unical'
 
 setup(
     name=PKG_NAME,
-    version='1.2.0',
+    version='1.2.1',
 
     packages=[PKG_NAME],
     package_dir={PKG_NAME: f"{SRC_FOLDER}/{PKG_NAME}"},
 
     package_data={PKG_NAME: [i.replace(f'{SRC_FOLDER}/{PKG_NAME}/', '')
                                    for i in glob(f'{SRC_FOLDER}/{PKG_NAME}/**',
                                                  recursive=True)]
```

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo` & `unicms_template_unical-1.2.1/src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,20 +1,20 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2022-08-23 11:38+0200\n"
+"PO-Revision-Date: 2023-04-11 15:36+0200\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 3.1.1\n"
+"X-Generator: Poedit 3.2.2\n"
 
 msgid "Accessibility and performance"
 msgstr "Accessibilità e prestazioni"
 
 msgid "Accomodation - Socrates Residence"
 msgstr "Accomodation - Residenza Socrates"
 
@@ -50,14 +50,17 @@
 
 msgid "Certified email"
 msgstr "Posta certificata"
 
 msgid "Chinese"
 msgstr "Cinese"
 
+msgid "Close"
+msgstr "Chiudi"
+
 msgid "Code of ethics and conduct"
 msgstr "Codice etico e di comportamento"
 
 msgid "Convention Center"
 msgstr "Centro Congressi"
 
 msgid "Cookies and consent methods"
@@ -285,17 +288,14 @@
 
 msgid "SPID / UniCal ID"
 msgstr "Accesso SPID / UniCal ID"
 
 msgid "Search"
 msgstr "Cerca"
 
-msgid "Services for disabled and dyslexic students"
-msgstr "Studenti con disabilità, DSA e BES"
-
 msgid "Share on"
 msgstr "Condividi su"
 
 msgid "Sitemap"
 msgstr "Mappa del sito"
 
 msgid "Spinoff / Patent Showcase"
@@ -306,20 +306,23 @@
 
 msgid "Staff services"
 msgstr "Servizi per il personale"
 
 msgid "State examinations"
 msgstr "Esami di Stato"
 
-msgid "Strategic plan 2020/2022"
-msgstr "Piano strategico 2020/2022"
+msgid "Strategic plan 2023/2025"
+msgstr "Piano strategico 2023/2025"
 
 msgid "Students webmail"
 msgstr "Webmail studenti"
 
+msgid "Students with disabilities/LDS"
+msgstr "Studenti con disabilità/DSA"
+
 msgid "Study activities catalogue"
 msgstr "Catalogo degli insegnamenti"
 
 msgid "Support"
 msgstr "Supporto"
 
 msgid "Teacher training courses"
```

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po` & `unicms_template_unical-1.2.1/src/unicms_template_unical/locale/it/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: \n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-08-23 11:36+0200\n"
-"PO-Revision-Date: 2022-08-23 11:38+0200\n"
+"POT-Creation-Date: 2023-04-11 15:31+0200\n"
+"PO-Revision-Date: 2023-04-11 15:36+0200\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 3.1.1\n"
+"X-Generator: Poedit 3.2.2\n"
 
 #: templates/404.html:6
 msgid "Error 404"
 msgstr "Errore 404"
 
 #: templates/404.html:10
 msgid "Page or Resource not found"
@@ -54,39 +54,40 @@
 msgstr "Error 500"
 
 #: templates/500.html:10
 msgid "This service has encourrend and unexpected error"
 msgstr "Questo servizio ha riscontrato un errore imprevisto"
 
 #: templates/bases/base_v_original.html:32
-#: templates/bases/unicms_unical.html:69 templates/bases/unicms_unical.html:84
-#: templates/bases/unicms_unical.html:89 templates/bases/unicms_unical.html:96
-#: templates/bases/unicms_unical.html:541 templates/pages/department.html:33
+#: templates/bases/unicms_unical.html:59 templates/bases/unicms_unical.html:74
+#: templates/bases/unicms_unical.html:79 templates/bases/unicms_unical.html:86
+#: templates/bases/unicms_unical.html:528 templates/pages/department.html:33
 #: templates/pages/department.html:141 templates/pages/opendata.html:33
+#: templates/pages/project_exbriner.html:44
 msgid "University of Calabria"
 msgstr "Università della Calabria"
 
 #: templates/bases/base_v_original.html:37
-#: templates/bases/unicms_unical.html:55
+#: templates/bases/unicms_unical.html:45
 msgid "Official University of Calabria website"
 msgstr "Sito istituzionale dell'Università della Calabria"
 
 #: templates/bases/base_v_original.html:77
-#: templates/bases/unicms_unical.html:160
-#: templates/bases/unicms_unical.html:161
-#: templates/bases/unicms_unical.html:166
-#: templates/bases/unicms_unical.html:167
+#: templates/bases/unicms_unical.html:150
+#: templates/bases/unicms_unical.html:151
+#: templates/bases/unicms_unical.html:156
+#: templates/bases/unicms_unical.html:157
 msgid "Address book"
 msgstr "Rubrica"
 
 #: templates/bases/base_v_original.html:82
-#: templates/bases/unicms_unical.html:132
-#: templates/bases/unicms_unical.html:135
-#: templates/bases/unicms_unical.html:144
-#: templates/bases/unicms_unical.html:150
+#: templates/bases/unicms_unical.html:122
+#: templates/bases/unicms_unical.html:125
+#: templates/bases/unicms_unical.html:134
+#: templates/bases/unicms_unical.html:140
 #: templates/blocks/unical_media_collection_searchbox.html:30
 #: templates/blocks/unical_media_collection_searchbox.html:50
 #: templates/pages/publication_list.html:142
 msgid "Search"
 msgstr "Cerca"
 
 #: templates/bases/base_v_original.html:107
@@ -125,364 +126,368 @@
 msgid "previous"
 msgstr "precedente"
 
 #: templates/bases/unical_api_list.html:60
 msgid "next"
 msgstr "successiva"
 
-#: templates/bases/unicms_unical.html:73 templates/bases/unicms_unical.html:93
-#: templates/bases/unicms_unical.html:100
+#: templates/bases/unicms_unical.html:63 templates/bases/unicms_unical.html:83
+#: templates/bases/unicms_unical.html:90
 msgid "HRS4R"
 msgstr ""
 
-#: templates/bases/unicms_unical.html:239
-#: templates/bases/unicms_unical.html:240
+#: templates/bases/unicms_unical.html:229
+#: templates/bases/unicms_unical.html:230
 #: templates/pages/multi_language.html:19
 #: templates/pages/multi_language.html:20
 msgid "Chinese"
 msgstr "Cinese"
 
-#: templates/bases/unicms_unical.html:242
-#: templates/bases/unicms_unical.html:243
+#: templates/bases/unicms_unical.html:232
+#: templates/bases/unicms_unical.html:233
 #: templates/pages/multi_language.html:22
 #: templates/pages/multi_language.html:23
 msgid "French"
 msgstr "Francese"
 
-#: templates/bases/unicms_unical.html:245
-#: templates/bases/unicms_unical.html:246
+#: templates/bases/unicms_unical.html:235
+#: templates/bases/unicms_unical.html:236
 #: templates/pages/multi_language.html:25
 #: templates/pages/multi_language.html:26
 msgid "Portuguese"
 msgstr "Portoghese"
 
-#: templates/bases/unicms_unical.html:248
-#: templates/bases/unicms_unical.html:249
+#: templates/bases/unicms_unical.html:238
+#: templates/bases/unicms_unical.html:239
 #: templates/pages/multi_language.html:28
 #: templates/pages/multi_language.html:29
 msgid "Espanol"
 msgstr "Spagnolo"
 
-#: templates/bases/unicms_unical.html:251
-#: templates/bases/unicms_unical.html:252
+#: templates/bases/unicms_unical.html:241
+#: templates/bases/unicms_unical.html:242
 #: templates/pages/multi_language.html:31
 #: templates/pages/multi_language.html:32
 msgid "Arabic"
 msgstr "Arabo"
 
-#: templates/bases/unicms_unical.html:254
-#: templates/bases/unicms_unical.html:255
+#: templates/bases/unicms_unical.html:244
+#: templates/bases/unicms_unical.html:245
 #: templates/pages/multi_language.html:34
 #: templates/pages/multi_language.html:35
 msgid "Russian"
 msgstr "Russo"
 
-#: templates/bases/unicms_unical.html:270
+#: templates/bases/unicms_unical.html:257
 msgid "Main menu"
 msgstr ""
 
-#: templates/bases/unicms_unical.html:275
+#: templates/bases/unicms_unical.html:262
 msgid "Show/Hide menu"
 msgstr ""
 
-#: templates/bases/unicms_unical.html:290
-#, fuzzy
-#| msgid "close"
+#: templates/bases/unicms_unical.html:277
 msgid "Close"
-msgstr "chiudi"
+msgstr "Chiudi"
 
-#: templates/bases/unicms_unical.html:377
-#: templates/bases/unicms_unical.html:378
+#: templates/bases/unicms_unical.html:364
+#: templates/bases/unicms_unical.html:365
 msgid "UniCal for students"
 msgstr "UniCal per gli studenti"
 
-#: templates/bases/unicms_unical.html:383
+#: templates/bases/unicms_unical.html:370
 msgid "Prospective students, Enrolled and Graduates"
 msgstr "Futuri studenti, iscritti e laureati"
 
-#: templates/bases/unicms_unical.html:384
+#: templates/bases/unicms_unical.html:371
 msgid "Educational offer"
 msgstr "Offerta formativa"
 
-#: templates/bases/unicms_unical.html:385
+#: templates/bases/unicms_unical.html:372
 msgid "Study activities catalogue"
 msgstr "Catalogo degli insegnamenti"
 
-#: templates/bases/unicms_unical.html:386
+#: templates/bases/unicms_unical.html:373
 msgid "Enroll, study and graduate"
 msgstr "Iscriversi, studiare e laurearsi"
 
-#: templates/bases/unicms_unical.html:387
+#: templates/bases/unicms_unical.html:374
 msgid "Right to study"
 msgstr "Diritto allo studio"
 
-#: templates/bases/unicms_unical.html:388
+#: templates/bases/unicms_unical.html:375
 msgid "Orientation"
 msgstr "Orientamento"
 
-#: templates/bases/unicms_unical.html:389
-msgid "Services for disabled and dyslexic students"
-msgstr "Studenti con disabilità, DSA e BES"
+#: templates/bases/unicms_unical.html:376
+msgid "Students with disabilities/LDS"
+msgstr "Studenti con disabilità/DSA"
 
-#: templates/bases/unicms_unical.html:390
+#: templates/bases/unicms_unical.html:377
 msgid "Psychological counseling"
 msgstr "Counselling psicologico"
 
-#: templates/bases/unicms_unical.html:391
+#: templates/bases/unicms_unical.html:378
 msgid "Career Service / Job Placement"
 msgstr "Career Service - Job Placement"
 
-#: templates/bases/unicms_unical.html:392
+#: templates/bases/unicms_unical.html:379
 msgid "International agreements and networks"
 msgstr "Accordi e network internazionali"
 
-#: templates/bases/unicms_unical.html:393
+#: templates/bases/unicms_unical.html:380
 msgid "Teacher training courses"
 msgstr "Formazione degli insegnanti"
 
-#: templates/bases/unicms_unical.html:394
+#: templates/bases/unicms_unical.html:381
 msgid "State examinations"
 msgstr "Esami di Stato"
 
-#: templates/bases/unicms_unical.html:403
-#: templates/bases/unicms_unical.html:404
+#: templates/bases/unicms_unical.html:390
+#: templates/bases/unicms_unical.html:391
 msgid "UniCal online"
 msgstr "UniCal online"
 
-#: templates/bases/unicms_unical.html:409 templates/pages/department.html:110
-#: templates/pages/department_dinci.html:91
+#: templates/bases/unicms_unical.html:396 templates/pages/department.html:110
+#: templates/pages/department_dinci.html:86
 msgid "Online front-office"
 msgstr "Front-office online"
 
-#: templates/bases/unicms_unical.html:410 templates/pages/department.html:111
-#: templates/pages/department_dinci.html:92
+#: templates/bases/unicms_unical.html:397 templates/pages/department.html:111
+#: templates/pages/department_dinci.html:87
 msgid "Online ticket"
 msgstr "Ticket online"
 
-#: templates/bases/unicms_unical.html:411
+#: templates/bases/unicms_unical.html:398
 msgid "ITC Services"
 msgstr "Servizi online ICT"
 
-#: templates/bases/unicms_unical.html:412
+#: templates/bases/unicms_unical.html:399
 msgid "Wi-Fi Services"
 msgstr "Servizi Wi-Fi"
 
-#: templates/bases/unicms_unical.html:413
+#: templates/bases/unicms_unical.html:400
 msgid "Students webmail"
 msgstr "Webmail studenti"
 
-#: templates/bases/unicms_unical.html:414
+#: templates/bases/unicms_unical.html:401
 msgid "Employees webmail"
 msgstr "Webmail dipendenti"
 
-#: templates/bases/unicms_unical.html:415
+#: templates/bases/unicms_unical.html:402
 msgid "SPID / UniCal ID"
 msgstr "Accesso SPID / UniCal ID"
 
-#: templates/bases/unicms_unical.html:416
+#: templates/bases/unicms_unical.html:403
 msgid "Online Taxes / PagoPA"
 msgstr "Tasse online / PagoPA"
 
-#: templates/bases/unicms_unical.html:417
+#: templates/bases/unicms_unical.html:404
 msgid "Exam reservations - ESSE3"
 msgstr "Prenotazioni esami - ESSE3"
 
-#: templates/bases/unicms_unical.html:418
+#: templates/bases/unicms_unical.html:405
 msgid "ESSE3PA"
 msgstr ""
 
-#: templates/bases/unicms_unical.html:419
+#: templates/bases/unicms_unical.html:406
 msgid "e-Learning platform"
 msgstr "Piattaforma e-Learning"
 
-#: templates/bases/unicms_unical.html:420
+#: templates/bases/unicms_unical.html:407
 msgid "Web Radio"
 msgstr ""
 
-#: templates/bases/unicms_unical.html:421
+#: templates/bases/unicms_unical.html:408
 msgid "Online Magazine"
 msgstr "Magazine online"
 
-#: templates/bases/unicms_unical.html:430
-#: templates/bases/unicms_unical.html:431
+#: templates/bases/unicms_unical.html:417
+#: templates/bases/unicms_unical.html:418
 msgid "Living on Campus"
 msgstr "Vivere il campus"
 
-#: templates/bases/unicms_unical.html:436
+#: templates/bases/unicms_unical.html:423
 msgid "Departments"
 msgstr "Dipartimenti"
 
-#: templates/bases/unicms_unical.html:437
+#: templates/bases/unicms_unical.html:424
 msgid "Campus residences"
 msgstr "Quartieri Centro Residenziale"
 
-#: templates/bases/unicms_unical.html:438
+#: templates/bases/unicms_unical.html:425
 msgid "Canteen services"
 msgstr "Servizio mensa"
 
-#: templates/bases/unicms_unical.html:439
+#: templates/bases/unicms_unical.html:426
 msgid "Libraries"
 msgstr "Biblioteche"
 
-#: templates/bases/unicms_unical.html:440
+#: templates/bases/unicms_unical.html:427
 msgid "Museum hub"
 msgstr "Sistema Museale"
 
-#: templates/bases/unicms_unical.html:441
+#: templates/bases/unicms_unical.html:428
 msgid "Theaters and cinemas"
 msgstr "Teatri e Cinema"
 
-#: templates/bases/unicms_unical.html:442
+#: templates/bases/unicms_unical.html:429
 msgid "Language Centre"
 msgstr "Centro Linguistico"
 
-#: templates/bases/unicms_unical.html:443
+#: templates/bases/unicms_unical.html:430
 msgid "Health Center"
 msgstr "Centro Sanitario - Emergenze"
 
-#: templates/bases/unicms_unical.html:444
+#: templates/bases/unicms_unical.html:431
 msgid "Sports Center"
 msgstr "Centro Sportivo"
 
-#: templates/bases/unicms_unical.html:445
+#: templates/bases/unicms_unical.html:432
 msgid "Convention Center"
 msgstr "Centro Congressi"
 
-#: templates/bases/unicms_unical.html:446
+#: templates/bases/unicms_unical.html:433
 msgid "Infants Center"
 msgstr "Polo d’Infanzia"
 
-#: templates/bases/unicms_unical.html:447
+#: templates/bases/unicms_unical.html:434
 msgid "Accomodation - Socrates Residence"
 msgstr "Accomodation - Residenza Socrates"
 
-#: templates/bases/unicms_unical.html:448
+#: templates/bases/unicms_unical.html:435
 msgid "Territory info"
 msgstr "Info territorio"
 
-#: templates/bases/unicms_unical.html:457
-#: templates/bases/unicms_unical.html:458
+#: templates/bases/unicms_unical.html:444
+#: templates/bases/unicms_unical.html:445
 msgid "Transparent UniCal"
 msgstr "UniCal trasparente"
 
-#: templates/bases/unicms_unical.html:463
+#: templates/bases/unicms_unical.html:450
 msgid "Organization"
 msgstr "Organizzazione"
 
-#: templates/bases/unicms_unical.html:464 templates/pages/department.html:123
+#: templates/bases/unicms_unical.html:451 templates/pages/department.html:123
 msgid "Transparent administration"
 msgstr "Amministrazione trasparente"
 
-#: templates/bases/unicms_unical.html:465
-msgid "Strategic plan 2020/2022"
-msgstr "Piano strategico 2020/2022"
+#: templates/bases/unicms_unical.html:452
+msgid "Strategic plan 2023/2025"
+msgstr "Piano strategico 2023/2025"
 
-#: templates/bases/unicms_unical.html:466
+#: templates/bases/unicms_unical.html:453
 msgid "Governing bodies"
 msgstr "Organi di Governo"
 
-#: templates/bases/unicms_unical.html:467
+#: templates/bases/unicms_unical.html:454
 msgid "Official register of the University"
 msgstr "Albo ufficiale di Ateneo"
 
-#: templates/bases/unicms_unical.html:468
+#: templates/bases/unicms_unical.html:455
 msgid "Quality Assurance System"
 msgstr "Sistema di Assicurazione della Qualità"
 
-#: templates/bases/unicms_unical.html:469
+#: templates/bases/unicms_unical.html:456
 msgid "Trusted Advisor of the University"
 msgstr "Consigliera di fiducia dell’Ateneo"
 
-#: templates/bases/unicms_unical.html:470
+#: templates/bases/unicms_unical.html:457
 msgid "Code of ethics and conduct"
 msgstr "Codice etico e di comportamento"
 
-#: templates/bases/unicms_unical.html:471
+#: templates/bases/unicms_unical.html:458
 msgid "Spinoff / Patent Showcase"
 msgstr "Vetrina Spinoff / Brevetti"
 
-#: templates/bases/unicms_unical.html:472
+#: templates/bases/unicms_unical.html:459
 msgid "Fundraising, donations, 5x1000"
 msgstr "Fundraising, donazioni, 5x1000"
 
-#: templates/bases/unicms_unical.html:496
-#: templates/bases/unicms_unical.html:548 templates/pages/department.html:148
+#: templates/bases/unicms_unical.html:483
+#: templates/bases/unicms_unical.html:535 templates/pages/department.html:148
 msgid "Certified email"
 msgstr "Posta certificata"
 
-#: templates/bases/unicms_unical.html:497
+#: templates/bases/unicms_unical.html:484
 msgid "Electronic invoicing"
 msgstr "Fatturazione elettronica"
 
-#: templates/bases/unicms_unical.html:498
+#: templates/bases/unicms_unical.html:485
 msgid "Web editor / Contacts"
 msgstr "Redazione web / Contatti"
 
-#: templates/bases/unicms_unical.html:499 templates/pages/department.html:124
+#: templates/bases/unicms_unical.html:486 templates/pages/department.html:124
+#: templates/pages/master_ges.html:60
 msgid "Accessibility and performance"
 msgstr "Accessibilità e prestazioni"
 
-#: templates/bases/unicms_unical.html:507 templates/pages/department.html:125
+#: templates/bases/unicms_unical.html:494 templates/pages/department.html:125
+#: templates/pages/master_ges.html:58
 msgid "Data protection / GDPR"
 msgstr "Protezione dati - GDPR"
 
-#: templates/bases/unicms_unical.html:508 templates/pages/department.html:126
+#: templates/bases/unicms_unical.html:495 templates/pages/department.html:126
+#: templates/pages/master_ges.html:59
 msgid "Cookies and consent methods"
 msgstr "Cookie e modalità di consenso"
 
-#: templates/bases/unicms_unical.html:509 templates/pages/department.html:127
+#: templates/bases/unicms_unical.html:496 templates/pages/department.html:127
+#: templates/pages/master_ges.html:70
 msgid "Legal notes"
 msgstr "Note legali"
 
-#: templates/bases/unicms_unical.html:510
+#: templates/bases/unicms_unical.html:497 templates/pages/master_ges.html:71
 msgid "Credits"
 msgstr "Crediti"
 
-#: templates/bases/unicms_unical.html:518
+#: templates/bases/unicms_unical.html:505
 msgid "Phishing: how to protect yourself"
 msgstr "Phishing: Come proteggersi"
 
-#: templates/bases/unicms_unical.html:519
+#: templates/bases/unicms_unical.html:506
 msgid "Web access statistics"
 msgstr "Statistiche accessi web"
 
-#: templates/bases/unicms_unical.html:520
+#: templates/bases/unicms_unical.html:507
 msgid "User Guide - UniCMS"
 msgstr "Guida d’uso - UniCMS"
 
-#: templates/bases/unicms_unical.html:521
+#: templates/bases/unicms_unical.html:508
 msgid "Intranet area"
 msgstr "Area intranet"
 
-#: templates/bases/unicms_unical.html:528
+#: templates/bases/unicms_unical.html:515
 msgid "RSS feeds"
 msgstr "Feed RSS"
 
-#: templates/bases/unicms_unical.html:529
+#: templates/bases/unicms_unical.html:516
 msgid "Alumni"
 msgstr "Sezione Alumni"
 
-#: templates/bases/unicms_unical.html:530
+#: templates/bases/unicms_unical.html:517
 msgid "Identity / Logo section"
 msgstr "Sezione identità / Logo"
 
-#: templates/bases/unicms_unical.html:531 templates/pages/department.html:128
+#: templates/bases/unicms_unical.html:518 templates/pages/department.html:128
 msgid "Sitemap"
 msgstr "Mappa del sito"
 
 #: templates/blocks/unical_carousel_hero_slider.html:15
 #: templates/blocks/unical_publication_notices_v1_carousel_home.html:68
 #: templates/blocks/unical_publications_cards_carousel.html:135
+#: templates/blocks/unical_publications_cards_carousel_v2.html:234
 #: templates/pages/publication_list.html:88
 msgid "Previous"
 msgstr "Precedente"
 
 #: templates/blocks/unical_carousel_hero_slider.html:23
 #: templates/blocks/unical_publication_notices_v1_carousel_home.html:76
 #: templates/blocks/unical_publications_cards_carousel.html:143
+#: templates/blocks/unical_publications_cards_carousel_v2.html:242
 #: templates/pages/publication_list.html:94
 msgid "Next"
 msgstr "Successivo"
 
 #: templates/blocks/unical_media_collection_searchbox.html:117
 msgid "No items here"
 msgstr "Nessun risultato prodotto"
@@ -535,32 +540,39 @@
 #: templates/blocks/unical_publication_notices_v1_carousel.html:28
 #: templates/blocks/unical_publication_notices_v1_carousel_home.html:19
 #: templates/blocks/unical_publication_notices_v1_carousel_home.html:45
 #: templates/blocks/unical_publications_card.html:34
 #: templates/blocks/unical_publications_cards.html:53
 #: templates/blocks/unical_publications_cards_carousel.html:45
 #: templates/blocks/unical_publications_cards_carousel.html:104
+#: templates/blocks/unical_publications_cards_carousel_v2.html:78
+#: templates/blocks/unical_publications_cards_carousel_v2.html:138
+#: templates/blocks/unical_publications_cards_carousel_v2.html:203
 #: templates/blocks/unical_publications_cards_mosaic.html:77
 #: templates/blocks/unical_publications_cards_mosaic.html:164
 #: templates/blocks/unical_publications_cards_mosaic_v2.html:71
 #: templates/blocks/unical_publications_cards_mosaic_v3.html:73
 #: templates/blocks/unical_publications_cards_mosaic_v3.html:159
+#: templates/blocks/unical_publications_cards_mosaic_v4.html:43
 #: templates/pages/publication_list.html:186
 #: templates/pages/publication_view.html:70
 #: templates/pages/publication_view_hero_original.html:58
 msgid "Published"
 msgstr "Pubblicato"
 
 #: templates/blocks/unical_publication_notices_v1.html:43
 #: templates/blocks/unical_publications_cards.html:81
 #: templates/blocks/unical_publications_cards.html:84
 #: templates/blocks/unical_publications_cards_carousel.html:157
 #: templates/blocks/unical_publications_cards_carousel_home.html:16
+#: templates/blocks/unical_publications_cards_carousel_v2.html:256
+#: templates/blocks/unical_publications_cards_carousel_v2_home.html:16
 #: templates/blocks/unical_publications_cards_mosaic.html:197
 #: templates/blocks/unical_publications_cards_mosaic_v3.html:193
+#: templates/blocks/unical_publications_cards_mosaic_v4.html:76
 msgid "Go to all news"
 msgstr "Vai a tutte le notizie"
 
 #: templates/blocks/unical_publication_notices_v1_carousel.html:49
 #: templates/blocks/unical_publication_notices_v1_carousel_home.html:90
 msgid "Go to all notices"
 msgstr "Vai a tutti gli avvisi"
@@ -585,19 +597,19 @@
 msgid "Staff services"
 msgstr "Servizi per il personale"
 
 #: templates/pages/department.html:100 templates/pages/department_ctc.html:52
 msgid "Documents, announcements and competitions"
 msgstr "Documenti, bandi e concorsi"
 
-#: templates/pages/department.html:112 templates/pages/department_dinci.html:93
+#: templates/pages/department.html:112 templates/pages/department_dinci.html:88
 msgid "Smart Campus"
 msgstr ""
 
-#: templates/pages/department.html:113 templates/pages/department_dinci.html:94
+#: templates/pages/department.html:113 templates/pages/department_dinci.html:89
 msgid "Unical Life"
 msgstr ""
 
 #: templates/pages/department_ctc.html:29
 msgid "Department of Chemistry and Chemical Technologies"
 msgstr ""
 
@@ -610,14 +622,15 @@
 msgstr "Area riservata"
 
 #: templates/pages/department_demacs.html:29
 msgid "Department of Mathematics and Computer Science"
 msgstr ""
 
 #: templates/pages/department_desf.html:29
+#: templates/pages/project_exbriner.html:106
 msgid "Department of Economics, Statistics and Finance"
 msgstr ""
 
 #: templates/pages/department_dfssn.html:29
 msgid "Department of Pharmacy and Health and Nutrition Sciences"
 msgstr ""
 
@@ -629,23 +642,27 @@
 msgid "Department of Biology, Ecology and Earth Sciences"
 msgstr ""
 
 #: templates/pages/department_dices.html:29
 msgid "Cepartment of Culture, Edication and Society"
 msgstr ""
 
+#: templates/pages/department_dimeg.html:29
+msgid "Department of Mechanical, Energy and Management Engineering"
+msgstr ""
+
 #: templates/pages/department_dimes.html:29
 msgid "Department of Computer Engineering, Modeling, Electronics and Systems"
 msgstr ""
 
-#: templates/pages/department_dinci.html:35
+#: templates/pages/department_dinci.html:30
 msgid "Department of Civil Engineering"
 msgstr ""
 
-#: templates/pages/department_dinci.html:90
+#: templates/pages/department_dinci.html:85
 msgid "ELEANOR"
 msgstr ""
 
 #: templates/pages/department_discag.html:29
 msgid "Department of Business and Legal Sciences"
 msgstr ""
 
@@ -657,14 +674,32 @@
 msgid "Department of Humanities"
 msgstr "Dipartimento di Studi Umanistici"
 
 #: templates/pages/department_fis.html:29
 msgid "Physics Department"
 msgstr "Dipartimento di Fisica"
 
+#: templates/pages/master_ges.html:46
+#, fuzzy
+#| msgid "Transparent UniCal"
+msgid "Portale UniCal"
+msgstr "UniCal trasparente"
+
+#: templates/pages/master_ges.html:47
+msgid "Portale DIMEG"
+msgstr ""
+
+#: templates/pages/master_ges.html:48
+msgid "Master e Alta Formazione"
+msgstr ""
+
+#: templates/pages/master_ges.html:82
+msgid "Manager di impianti ed eventi sportivi complessi"
+msgstr ""
+
 #: templates/pages/multi_language.html:13
 #: templates/pages/multi_language.html:14
 #: templates/pages/multi_language.html:16
 #: templates/pages/multi_language.html:17
 msgid "Italian"
 msgstr "Italiano"
 
@@ -680,14 +715,20 @@
 msgid "Preferences"
 msgstr "Preferenze"
 
 #: templates/pages/portale_home_v_original.html:47
 msgid "I agree"
 msgstr "Accetto"
 
+#: templates/pages/project_exbriner.html:25
+msgid ""
+"EXBRINER Project (Horizon Europe/Marie Skłodowska-Curie Actions/Doctoral "
+"Networks, call: HORIZON-MSCA-2021-DN-01)"
+msgstr ""
+
 #: templates/pages/publication_list.html:51
 msgid "Back to all news"
 msgstr "Torna a tutte le notizie"
 
 #: templates/pages/publication_list.html:88
 #: templates/pages/publication_list.html:94
 msgid "Page"
@@ -724,14 +765,17 @@
 msgid "Published in"
 msgstr "Pubblicato in"
 
 #: templates/pages/publication_view_hero_original.html:85
 msgid "It might interest you"
 msgstr "Potrebbe interessarti"
 
+#~ msgid "Services for disabled and dyslexic students"
+#~ msgstr "Studenti con disabilità, DSA e BES"
+
 #~ msgid "Teaching catalog"
 #~ msgstr "Catologo insegnamenti"
 
 #~ msgid "Language"
 #~ msgstr "Lingua"
 
 #~ msgid "Contacts"
```

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/css/colors/unicms_exbriner.css` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/css/colors/unicms_exbriner.css`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     }
 }
 
 /**
  * Footer Main
  */
 .it-footer-main{
-    background: var(--dark_grey_unical);
+    background: var(--bordeaux_unical);
 }
 
 /**
  * Footer Small Prints
  */
 .it-footer-small-prints{
     background: var(--bordeaux_unical);
@@ -160,39 +160,20 @@
     background-color: var(--bordeaux_unical);
     border-color: var(--bordeaux_unical);
 }
 .form-check [type=radio]:checked+label::before {
     border-color: var(--bordeaux_unical);
 }
 
-/**
- * Section muted
- */
-.section.section-muted {
-    background-color: #f7f7f7;
-}
-
-a {
-    color: #B01717;
-}
-
-a:hover, a:active {
-    color: #6f0b0a;
-}
-
 /** only visited **/
 a.no-color,
 ol.breadcrumb a  {
     color: var(--dark_grey_unical);
 }
 
-.background-yellow {
-    background: #ffed00;
-}
-
 .background-white {
     background: var(--white);
 }
 
 .background-light-grey {
     background: var(--light_grey);
     color: var(--dark_grey_unical);
@@ -372,7 +353,20 @@
 .it-footer-main h4 a {
     border-bottom: 1px solid var(--bordeaux_unical);
 }
 
 input.top-input::placeholder {
     color: var(--bordeaux_unical);
 }
+
+/**
+ * custom
+ */
+.it-header-wrapper .it-nav-wrapper .it-header-navbar-wrapper {
+    background: var(--bordeaux_unical);
+}
+
+@media (min-width: 992px){
+    .menu-wrapper li.megamenu a.nav-link {
+        color: var(--white) !important;
+    }
+}
```

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/css/colors/unicms_unical.css` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/css/colors/unicms_unical.css`

 * *Files 7% similar despite different names*

```diff
@@ -366,14 +366,27 @@
 .it-hero-wrapper .it-hero-text-wrapper h2.unical-hero-heading,
 .it-hero-wrapper .it-hero-text-wrapper h3.unical-hero-heading,
 .it-hero-wrapper .it-hero-text-wrapper h4.unical-hero-heading {
     background: #fff;
     color: var(--bordeaux_unical);
 }
 
-.it-footer-main h4 a {
+.it-footer-main h4 span {
     border-bottom: 1px solid var(--bordeaux_unical);
 }
 
 input.top-input::placeholder {
     color: #fff;
 }
+
+.navbar .navbar-collapsable .navbar-nav li a.nav-link {
+    color: #000;
+}
+
+.nav-tabs .nav-link .icon {
+    fill: var(--dark_grey);
+}
+
+.nav-tabs .nav-link.active .icon,
+.nav-tabs .nav-link .icon:hover {
+    fill: var(--bordeaux_unical);
+}
```

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/css/unicms_unical.css` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/css/unicms_unical.css`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,14 @@
 .custom-unical .card-wrapper {
   padding-bottom: 16px;
 }
 .it-carousel-wrapper.custom-unical .owl-carousel .owl-dots {
   display: none;
 }
 .navbar .navbar-collapsable .navbar-nav li a.nav-link {
-  color: #000;
   border-bottom: none !important;
 }
 .it-carousel-wrapper .owl-stage-outer {
   padding-top: 0px;
   padding-bottom: 0;
 }
 /** * Main Menu */
@@ -334,14 +333,18 @@
   .it-hero-wrapper.unical-hero-wrapper-slim .it-hero-text-wrapper.unical-hero-text-wrapper {
     padding: 20px 26px;
   }
 }
 .it-footer-main {
   font-size: 15px;
 }
+.it-footer-main h4 span {
+    font-size: 16px;
+    text-transform: uppercase;
+}
 @media (max-width: 991px) {
   .it-footer-main .link-list-wrapper ul li a {
     padding: 24px 0;
   }
 }
 /** Owl CLS fix */
 .owl-carousel {
```

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/addressbook.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/addressbook.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/agenda.jpg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/agenda.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/alert-red.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/alert-red.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/banner_1.jpg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/banner_1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/chi.png` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/chi.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/dimes.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/dimes.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/en.png` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/en.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/esp.png` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/esp.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/ar.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/flags/ar.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/en.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/flags/en.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/es.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/flags/es.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/eu.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/flags/eu.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/flags/zh.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/flags/zh.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/ita.png` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/ita.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/library1.jpg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/library1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo.png` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo1.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logo1.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_back.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logo_back.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_presta.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logo_presta.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_unical_white.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logo_unical_white.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logo_white.png` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logo_white.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/HRS4R.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/HRS4R.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/ctc.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/ctc.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/demacs.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/demacs.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/desf.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/desf.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dfssn.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/dfssn.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/diam.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/diam.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dibest.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/dibest.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dices.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/dices.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dimeg.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/dimeg.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dimes.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/dimes.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dinci.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/dinci.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/discag.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/discag.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/dispes.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/dispes.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/disu.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/disu.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/eu_funded.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/eu_funded.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/eu_funded_white.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/eu_funded_white.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/exbriner.png` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/exbriner.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/fis.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/fis.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/logos/master_ges.png` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/logos/master_ges.png`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/news1.jpg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/news1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/news2.jpg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/news2.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/news3.jpg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/news3.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/ponte-bucci-1.jpg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/ponte-bucci-1.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/unical_banner.jpg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/unical_banner.jpg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/unical_logo.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/unical_logo.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg` & `unicms_template_unical-1.2.1/src/unicms_template_unical/static/images/unical_logo_bullet_white.svg`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/404.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/404.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/base_v_original.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/bases/base_v_original.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/error-page.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/bases/error-page.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/unical_api_list.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/bases/unical_api_list.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/bases/unicms_unical.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/bases/unicms_unical.html`

 * *Files 1% similar despite different names*

```diff
@@ -354,43 +354,43 @@
 {% block footer_menu_section %}
 <section>
     <div class="row" style="padding-top: 20px;">
 
         {% block first_column %}
         <div class="col-lg-3 col-sm-6 pb-2">
             <h4>
-                <a href="#" title="{% trans 'UniCal for students' %}">
+                <span>
                     {% trans 'UniCal for students' %}
-                </a>
+                </span>
             </h4>
             <div class="link-list-wrapper">
                 <ul class="footer-list link-list clearfix">
                     <li><a class="list-item" href="/campus/servizi/" title="{% trans 'Prospective students, Enrolled and Graduates' %}">{% trans 'Prospective students, Enrolled and Graduates' %}</a></li>
                     <li><a class="list-item" href="/didattica/offerta-formativa/" title="{% trans 'Educational offer' %}">{% trans 'Educational offer' %}</a></li>
                     <li><a class="list-item" href="/didattica/offerta-formativa/catalogo/" title="{% trans 'Study activities catalogue' %}">{% trans 'Study activities catalogue' %}</a></li>
                     <li><a class="list-item" href="/didattica/iscriversi-studiare-laurearsi/" title="{% trans 'Enroll, study and graduate' %}">{% trans 'Enroll, study and graduate' %}</a></li>
                     <li><a class="list-item" href="/didattica/diritto-allo-studio/" title="{% trans 'Right to study' %}">{% trans 'Right to study' %}</a></li>
                     <li><a class="list-item" href="/didattica/orientamento/" title="{% trans 'Orientation' %}">{% trans 'Orientation' %}</a></li>
-                    <li><a class="list-item" href="/didattica/diritto-allo-studio/servizi-per-studenti-con-disabilita-e-dsa/" title="{% trans 'Services for disabled and dyslexic students' %}">{% trans 'Services for disabled and dyslexic students' %}</a></li>
+                    <li><a class="list-item" href="/didattica/diritto-allo-studio/servizi-per-studenti-con-disabilita-e-dsa/" title="{% trans 'Students with disabilities/LDS' %}">{% trans 'Students with disabilities/LDS' %}</a></li>
                     <li><a class="list-item" href="/didattica/orientamento/counselling/" title="{% trans 'Psychological counseling' %}">{% trans 'Psychological counseling' %}</a></li>
                     <li><a class="list-item" href="http://careerservices.unical.it/" target="_blank" rel="noopener noreferrer" title="{% trans 'Career Service / Job Placement' %}">{% trans 'Career Service / Job Placement' %}</a></li>
                     <li><a class="list-item" href="/internazionale/studiare-all-estero/accordi-e-reti/accordi-internazionali/" title="{% trans 'International agreements and networks' %}">{% trans 'International agreements and networks' %}</a></li>
                     <li><a class="list-item" href="/didattica/offerta-formativa/formazione-insegnanti/" title="{% trans 'Teacher training courses' %}">{% trans 'Teacher training courses' %}</a></li>
                     <li><a class="list-item" href="/didattica/offerta-formativa/esami-di-stato/" title="{% trans 'State examinations' %}">{% trans 'State examinations' %}</a></li>
                 </ul>
             </div>
         </div>
         {% endblock first_column %}
 
         {% block second_column %}
         <div class="col-lg-3 col-sm-6 pb-2">
             <h4>
-                <a href="#" title="{% trans 'UniCal online' %}">
+                <span>
                     {% trans 'UniCal online' %}
-                </a>
+                </span>
             </h4>
             <div class="link-list-wrapper">
                 <ul class="footer-list link-list clearfix">
                     <li><a class="list-item" href="/front-office/" title="{% trans 'Online front-office' %}">{% trans 'Online front-office' %}</a></li>
                     <li><a class="list-item" href="https://ticket.unical.it/" target="_blank" rel="noopener noreferrer" title="{% trans 'Online ticket' %}">{% trans 'Online ticket' %}</a></li>
                     <li><a class="list-item" href="/servizi-ict" title="{% trans 'ITC Services' %}">{% trans 'ITC Services' %}</a></li>
                     <li><a class="list-item" href="/servizi-ict/servizi-digitali-studenti/accesso-wifi-ateneo/" title="{% trans 'Wi-Fi Services' %}">{% trans 'Wi-Fi Services' %}</a></li>
@@ -407,17 +407,17 @@
             </div>
         </div>
         {% endblock second_column %}
 
         {% block third_column %}
         <div class="col-lg-3 col-sm-6 pb-2">
             <h4>
-                <a href="#" title="{% trans 'Living on Campus' %}">
+                <span>
                     {% trans 'Living on Campus' %}
-                </a>
+                </span>
             </h4>
             <div class="link-list-wrapper">
                 <ul class="footer-list link-list clearfix">
                     <li><a class="list-item" href="/organizzazione/strutture/dipartimenti/" title="{% trans 'Departments' %}">{% trans 'Departments' %}</a></li>
                     <li><a class="list-item" href="/campus/vivere-il-campus/quartieri/" title="{% trans 'Campus residences' %}">{% trans 'Campus residences' %}</a></li>
                     <li><a class="list-item" href="/campus/vivere-il-campus/servizio-mensa/" title="{% trans 'Canteen services' %}">{% trans 'Canteen services' %}</a></li>
                     <li><a class="list-item" href="/campus/vivere-il-campus/biblioteche/" title="{% trans 'Libraries' %}">{% trans 'Libraries' %}</a></li>
@@ -434,23 +434,23 @@
             </div>
         </div>
         {% endblock third_column %}
 
         {% block fourth_column %}
         <div class="col-lg-3 col-sm-6 pb-2">
             <h4>
-                <a href="#" title="{% trans 'Transparent UniCal' %}">
+                <span>
                     {% trans 'Transparent UniCal' %}
-                </a>
+                </span>
             </h4>
             <div class="link-list-wrapper">
                 <ul class="footer-list link-list clearfix">
                     <li><a class="list-item" href="/organizzazione/strutture/direzioni-aree/" title="{% trans 'Organization' %}">{% trans 'Organization' %}</a></li>
                     <li><a class="list-item" href="/organizzazione/chi-siamo/portale-trasparenza/" title="{% trans 'Transparent administration' %}">{% trans 'Transparent administration' %}</a></li>
-                    <li><a class="list-item" href="/organizzazione/chi-siamo/linee-strategiche/" title="{% trans 'Strategic plan 2020/2022' %}">{% trans 'Strategic plan 2020/2022' %}</a></li>
+                    <li><a class="list-item" href="/organizzazione/chi-siamo/linee-strategiche/" title="{% trans 'Strategic plan 2023/2025' %}">{% trans 'Strategic plan 2023/2025' %}</a></li>
                     <li><a class="list-item" href="/organizzazione/chi-siamo/organi/" title="{% trans 'Governing bodies' %}">{% trans 'Governing bodies' %}</a></li>
                     <li><a class="list-item" href="https://titulus-unical.cineca.it/albo/" target="_blank" rel="noopener noreferrer" title="{% trans 'Official register of the University' %}">{% trans 'Official register of the University' %}</a></li>
                     <li><a class="list-item" href="/organizzazione/chi-siamo/assicurazione-qualita/" title="{% trans 'Quality Assurance System' %}">{% trans 'Quality Assurance System' %}</a></li>
                     <li><a class="list-item" href="/consigliera-di-fiducia/" title="{% trans 'Trusted Advisor of the University' %}">{% trans 'Trusted Advisor of the University' %}</a></li>
                     <li><a class="list-item" href="/organizzazione/chi-siamo/organi/altri-organi-e-organismi/commissione-etica/" title="{% trans 'Code of ethics and conduct' %}">{% trans 'Code of ethics and conduct' %}</a></li>
                     <li><a class="list-item" href="/innovazione-societa/trasferimento-tecnologico/creazione-imprese-innovative/spin-off/" title="{% trans 'Spinoff / Patent Showcase' %}">{% trans 'Spinoff / Patent Showcase' %}</a></li>
                     <li><a class="list-item" href="/5x1000" title="{% trans 'Fundraising, donations, 5x1000' %}">{% trans 'Fundraising, donations, 5x1000' %}</a></li>
@@ -497,15 +497,15 @@
                         </div>
 
                         <div class="col-lg-3 col-sm-6">
                             <div class="link-list-wrapper">
                                 <ul class="footer-list link-list clearfix">
                                     <li><a class="list-item" href="/media/medias/2021/phishing.pdf" title="{% trans 'Phishing: how to protect yourself' %}">{% trans 'Phishing: how to protect yourself' %}</a></li>
                                     <li><a class="list-item" href="/statistiche-accessi-web" title="{% trans 'Web access statistics' %}">{% trans 'Web access statistics' %}</a></li>
-                                    <li><a class="list-item" href="/servizi-ict/servizi-digitali-utente/gestione-sito/" title="{% trans 'User Guide - UniCMS' %}">{% trans 'User Guide - UniCMS' %}</a></li>
+                                    <li><a class="list-item" href="/servizi-ict/servizi-digitali-per-il-personale/gestione-sito/" title="{% trans 'User Guide - UniCMS' %}">{% trans 'User Guide - UniCMS' %}</a></li>
                                     <li><a class="list-item" href="/editorial-board/" title="{% trans 'Intranet area' %}">{% trans 'Intranet area' %}</a></li>
                                 </ul>
                             </div>
                         </div>
                         <div class="col-lg-3 col-sm-6">
                             <div class="link-list-wrapper">
                                 <ul class="footer-list link-list clearfix">
```

#### html2text {}

```diff
@@ -62,62 +62,62 @@
     * __Twitter
     * __Linkedin
     * __Instagram
     * __Youtube
     * __Github
 {% endblock footer_top %}  {% block footer_menu_section %}
 {% block first_column %}
-*** {%_trans_'UniCal_for_students'_%} ***
+***  {% trans 'UniCal for students' %}  ***
     * {%_trans_'Prospective_students,_Enrolled_and_Graduates'_%}
     * {%_trans_'Educational_offer'_%}
     * {%_trans_'Study_activities_catalogue'_%}
     * {%_trans_'Enroll,_study_and_graduate'_%}
     * {%_trans_'Right_to_study'_%}
     * {%_trans_'Orientation'_%}
-    * {%_trans_'Services_for_disabled_and_dyslexic_students'_%}
+    * {%_trans_'Students_with_disabilities/LDS'_%}
     * {%_trans_'Psychological_counseling'_%}
     * {%_trans_'Career_Service_/_Job_Placement'_%}
     * {%_trans_'International_agreements_and_networks'_%}
     * {%_trans_'Teacher_training_courses'_%}
     * {%_trans_'State_examinations'_%}
 {% endblock first_column %} {% block second_column %}
-*** {%_trans_'UniCal_online'_%} ***
+***  {% trans 'UniCal online' %}  ***
     * {%_trans_'Online_front-office'_%}
     * {%_trans_'Online_ticket'_%}
     * {%_trans_'ITC_Services'_%}
     * {%_trans_'Wi-Fi_Services'_%}
     * {%_trans_'Students_webmail'_%}
     * {%_trans_'Employees_webmail'_%}
     * {%_trans_'SPID_/_UniCal_ID'_%}
     * {%_trans_'Online_Taxes_/_PagoPA'_%}
     * {%_trans_'Exam_reservations_-_ESSE3'_%}
     * {%_trans_'ESSE3PA'_%}
     * {%_trans_'e-Learning_platform'_%}
     * {%_trans_'Web_Radio'_%}
     * {%_trans_'Online_Magazine'_%}
 {% endblock second_column %} {% block third_column %}
-*** {%_trans_'Living_on_Campus'_%} ***
+***  {% trans 'Living on Campus' %}  ***
     * {%_trans_'Departments'_%}
     * {%_trans_'Campus_residences'_%}
     * {%_trans_'Canteen_services'_%}
     * {%_trans_'Libraries'_%}
     * {%_trans_'Museum_hub'_%}
     * {%_trans_'Theaters_and_cinemas'_%}
     * {%_trans_'Language_Centre'_%}
     * {%_trans_'Health_Center'_%}
     * {%_trans_'Sports_Center'_%}
     * {%_trans_'Convention_Center'_%}
     * {%_trans_'Infants_Center'_%}
     * {%_trans_'Accomodation_-_Socrates_Residence'_%}
     * {%_trans_'Territory_info'_%}
 {% endblock third_column %} {% block fourth_column %}
-*** {%_trans_'Transparent_UniCal'_%} ***
+***  {% trans 'Transparent UniCal' %}  ***
     * {%_trans_'Organization'_%}
     * {%_trans_'Transparent_administration'_%}
-    * {%_trans_'Strategic_plan_2020/2022'_%}
+    * {%_trans_'Strategic_plan_2023/2025'_%}
     * {%_trans_'Governing_bodies'_%}
     * {%_trans_'Official_register_of_the_University'_%}
     * {%_trans_'Quality_Assurance_System'_%}
     * {%_trans_'Trusted_Advisor_of_the_University'_%}
     * {%_trans_'Code_of_ethics_and_conduct'_%}
     * {%_trans_'Spinoff_/_Patent_Showcase'_%}
     * {%_trans_'Fundraising,_donations,_5x1000'_%}
```

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_carousel_cards.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_carousel_hero_slider_slim.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_carousel_to_page.html`

 * *Files 9% similar despite different names*

```diff
@@ -36,10 +36,10 @@
                 {% endfor %}
                 </div>
             </div>
             {% endif %}
         </div>
     </div>
     {% if not forloop.last %}
-    <hr class="my-4 bordeaux-unical-bg">
+    <hr class="my-4" style="color: var(--bordeaux_unical)">
     {% endif %}
 {% endfor %}
```

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_contact.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_contact.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_contact_v2.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_contact_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_media_collection_collapse.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_media_collection_items.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_media_collection_searchbox.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_buttons.html`

 * *Files 12% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         <a href="{{ link }}" class="no-color">
         {% endif %}
             {{ title }}
         {% if link %}
         </a>
         {% endif %}
     </h1>
-    <hr class="my-4 bordeaux-unical-bg">
+    <hr class="my-4" style="color: var(--bordeaux_unical)">
 </div>
 {% endif %}
 
 {% for item in items %}
 
     {% call obj=item method='link' request=request as link %}
 
@@ -31,8 +31,8 @@
                     {{ item.name }}
                     {% if item == current %}</b>{% endif %}
                 </h5>
         </span>
     </a>
 {% endfor %}
 
-<hr class="my-4 bordeaux-unical-bg">
+<hr class="my-4" style="color: var(--bordeaux_unical)">
```

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_collapse.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_collapse_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_grey_box_generic.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_main.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_main.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_main_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_secondary.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_side.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_side.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_sitemap.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_menu_to_page_with_publication.html`

 * *Files 8% similar despite different names*

```diff
@@ -66,12 +66,12 @@
             {% endfor %}
             </div>
         </div>
         {% endif %}
     </div>
 </div>
 {% if not forloop.last %}
-<hr class="my-4 bordeaux-unical-bg">
+<hr class="my-4" style="color: var(--bordeaux_unical)">
 {% endif %}
 {% endfor %}
```

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_page_publication_card_1_content.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_page_publication_card_2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_page_publication_collapse.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_page_publication_preview_1.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_page_publication_top.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_alert.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_alert.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_attachments.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_full_view.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publication_notices_v1_carousel_home.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_card.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_card.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_home_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2_home.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_carousel_v2_home.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v2.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v3.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/blocks/unical_publications_cards_mosaic_v4.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/loading-jumbo.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/loading-jumbo.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_ctc.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_ctc.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_demacs.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_demacs.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_desf.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_desf.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dfssn.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_dfssn.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_diam.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_diam.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dibest.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_dibest.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dices.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_dices.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dimeg.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_dimeg.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dimes.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_dimes.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dinci.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_dinci.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_discag.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_discag.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_dispes.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_dispes.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_disu.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_disu.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/department_fis.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/department_fis.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/master_ges.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/master_ges.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/multi_language.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/multi_language.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/opendata.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/opendata.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/portale_home_dipartimento_v3_dimes.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/portale_home_v_original.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/portale_home_v_original.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/project_exbriner.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/project_exbriner.html`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 {% block analytics_value %}
 {% endblock analytics_value %}
 
 {% block custom_style %}
 <link rel="shortcut icon" href="{% unicms_template_unical_static_path 'images/favicon/favicon-32x32.png' %}">
 <link rel="stylesheet" href="{% unicms_template_unical_static_path 'css/unicms_unical.css' %}" type="text/css">
+<link rel="stylesheet" href="{% unicms_template_unical_static_path 'css/unicms_exbriner.css' %}" type="text/css">
 <link rel="stylesheet" href="{% unicms_template_unical_static_path 'css/colors/unicms_exbriner.css' %}" type="text/css">
 {% endblock custom_style %}
 
 {% block page_meta_description %}{% if webpath.meta_description %}{{ webpath.meta_description }}{% else %}{% trans "EXBRINER Project (Horizon Europe/Marie Skłodowska-Curie Actions/Doctoral Networks, call: HORIZON-MSCA-2021-DN-01)" %}{% endif %}{% endblock page_meta_description %}
 {% block page_meta_keywords %}{% if webpath.meta_keywords %}{{ webpath.meta_keywords }}{% else %}ExBrineR{% endif %}{% endblock page_meta_keywords %}
 
 {% block header_slim_wrapper %}
```

#### html2text {}

```diff
@@ -1,14 +1,15 @@
 {% extends "department.html" %} {% load i18n %} {% load static %}  {% load
 unicms_carousels %} {% load unicms_contexts %} {% load unicms_menus %} {% load
 unicms_templates %} {% load unicms_pages %} {% load unicms_publications %} {%
 load unicms_template_unical %} {% block analytics_value %} {% endblock
 analytics_value %} {% block custom_style %}
 
 
+
  {% endblock custom_style %} {% block page_meta_description %}{% if
 webpath.meta_description %}{{ webpath.meta_description }}{% else %}{% trans
 "EXBRINER Project (Horizon Europe/Marie SkÅodowska-Curie Actions/Doctoral
 Networks, call: HORIZON-MSCA-2021-DN-01)" %}{% endif %}{% endblock
 page_meta_description %} {% block page_meta_keywords %}{% if
 webpath.meta_keywords %}{{ webpath.meta_keywords }}{% else %}ExBrineR{% endif
 %}{% endblock page_meta_keywords %} {% block header_slim_wrapper %} {%
```

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/publication_list.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/publication_list.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/publication_view.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/publication_view.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templates/pages/publication_view_hero_original.html` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templates/pages/publication_view_hero_original.html`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/src/unicms_template_unical/templatetags/unicms_template_unical.py` & `unicms_template_unical-1.2.1/src/unicms_template_unical/templatetags/unicms_template_unical.py`

 * *Files identical despite different names*

### Comparing `unicms_template_unical-1.2.0/unicms_template_unical.egg-info/PKG-INFO` & `unicms_template_unical-1.2.1/unicms_template_unical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicms-template-unical
-Version: 1.2.0
+Version: 1.2.1
 Summary: uniCMS Unical Template based on Bootstrap Italia
 Home-page: https://github.com/UniversitaDellaCalabria/unicms-template-unical
 Author: Giuseppe De Marco, Francesco Filicetti
 Author-email: giuseppe.demarco@unical.it, francesco.filicetti@unical.it
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `unicms_template_unical-1.2.0/unicms_template_unical.egg-info/SOURCES.txt` & `unicms_template_unical-1.2.1/unicms_template_unical.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 setup.py
 src/unicms_template_unical/__init__.py
 src/unicms_template_unical/apps.py
 src/unicms_template_unical/settings.py
 src/unicms_template_unical/locale/it/LC_MESSAGES/django.mo
 src/unicms_template_unical/locale/it/LC_MESSAGES/django.po
+src/unicms_template_unical/static/css/unicms_exbriner.css
 src/unicms_template_unical/static/css/unicms_unical.css
 src/unicms_template_unical/static/css/colors/unicms_exbriner.css
 src/unicms_template_unical/static/css/colors/unicms_unical.css
 src/unicms_template_unical/static/fonts/TitilliumWeb-Black.ttf
 src/unicms_template_unical/static/images/addressbook.svg
 src/unicms_template_unical/static/images/agenda.jpg
 src/unicms_template_unical/static/images/alert-red.svg
```

