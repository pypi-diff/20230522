# Comparing `tmp/zoom-python-client-0.0.4.tar.gz` & `tmp/zoom-python-client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoom-python-client-0.0.4.tar", last modified: Mon May 15 13:06:26 2023, max compression
+gzip compressed data, was "zoom-python-client-0.0.5.tar", last modified: Mon May 22 10:10:00 2023, max compression
```

## Comparing `zoom-python-client-0.0.4.tar` & `zoom-python-client-0.0.5.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.176268 zoom-python-client-0.0.4/
--rw-r--r--   0 rene       (501) staff       (20)       49 2022-09-06 12:27:11.000000 zoom-python-client-0.0.4/.coveragerc
--rw-r--r--   0 rene       (501) staff       (20)       65 2023-05-04 14:58:03.000000 zoom-python-client-0.0.4/.env.sample
--rw-r--r--   0 rene       (501) staff       (20)      137 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/.flake8
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.051737 zoom-python-client-0.0.4/.github/
--rw-r--r--   0 rene       (501) staff       (20)     2918 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/.github/CONTRIBUTING.md
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.055312 zoom-python-client-0.0.4/.github/workflows/
--rw-r--r--   0 rene       (501) staff       (20)     2325 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 rene       (501) staff       (20)      246 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/.github/workflows/pre-commit.yaml
--rw-r--r--   0 rene       (501) staff       (20)      776 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/.github/workflows/python-tests.yml
--rw-r--r--   0 rene       (501) staff       (20)     3086 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/.gitignore
--rw-r--r--   0 rene       (501) staff       (20)      634 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 rene       (501) staff       (20)       14 2022-09-05 07:24:11.000000 zoom-python-client-0.0.4/.tool-versions
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.056193 zoom-python-client-0.0.4/.vscode/
--rw-r--r--   0 rene       (501) staff       (20)      475 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/.vscode/settings.json
--rw-r--r--   0 rene       (501) staff       (20)    35149 2023-05-04 09:49:35.000000 zoom-python-client-0.0.4/LICENSE
--rw-r--r--   0 rene       (501) staff       (20)     3211 2023-05-15 13:06:26.174545 zoom-python-client-0.0.4/PKG-INFO
--rw-r--r--   0 rene       (501) staff       (20)     2632 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/README.md
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.059547 zoom-python-client-0.0.4/example/
--rw-r--r--   0 rene       (501) staff       (20)        0 2022-09-06 14:27:54.000000 zoom-python-client-0.0.4/example/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      355 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/example/get_meeting_livestream.py
--rw-r--r--   0 rene       (501) staff       (20)      317 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/example/get_user.py
--rw-r--r--   0 rene       (501) staff       (20)      630 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/example/get_user_meetings.py
--rw-r--r--   0 rene       (501) staff       (20)      938 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/example/set_meeting_livestream.py
--rw-r--r--   0 rene       (501) staff       (20)     1269 2023-05-15 13:06:17.000000 zoom-python-client-0.0.4/pyproject.toml
--rw-r--r--   0 rene       (501) staff       (20)      153 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/pytest.ini
--rw-r--r--   0 rene       (501) staff       (20)      145 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/requirements.dev.txt
--rw-r--r--   0 rene       (501) staff       (20)       63 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/requirements.txt
--rw-r--r--   0 rene       (501) staff       (20)       38 2023-05-15 13:06:26.176509 zoom-python-client-0.0.4/setup.cfg
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.060304 zoom-python-client-0.0.4/tests/
--rw-r--r--   0 rene       (501) staff       (20)        0 2022-09-05 07:32:56.000000 zoom-python-client-0.0.4/tests/__init__.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.061711 zoom-python-client-0.0.4/tests/utils/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/utils/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      176 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/utils/test_logger.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.065896 zoom-python-client-0.0.4/tests/zoom_python_client/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      405 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/base_test_case.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.066956 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/__init__.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.069114 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/meeting_livestreams/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/meeting_livestreams/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     3980 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/meeting_livestreams/test_meeting_livestreams_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.072170 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/meetings/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/meetings/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1200 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/meetings/test_meetings_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.074080 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/users/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/users/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1193 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/users/test_users_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.075453 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/webinar_livestreams/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/webinar_livestreams/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     3980 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/webinar_livestreams/test_webinar_livestreams_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.076894 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/webinars/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/webinars/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      748 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/client_components/webinars/test_webinars_component.py
--rw-r--r--   0 rene       (501) staff       (20)     1792 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/test_api_client.py
--rw-r--r--   0 rene       (501) staff       (20)     1757 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/test_zoom_api_client.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.078220 zoom-python-client-0.0.4/tests/zoom_python_client/utils/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/utils/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      185 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/utils/test_file_system.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.080638 zoom-python-client-0.0.4/tests/zoom_python_client/zoom_auth_api/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/zoom_auth_api/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1897 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/tests/zoom_python_client/zoom_auth_api/test_zoom_auth_api_client.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.034344 zoom-python-client-0.0.4/venv/
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.093753 zoom-python-client-0.0.4/venv/bin/
--rwxr-xr-x   0 rene       (501) staff       (20)      649 2023-05-15 12:44:10.000000 zoom-python-client-0.0.4/venv/bin/rst2html.py
--rwxr-xr-x   0 rene       (501) staff       (20)      771 2023-05-15 12:44:10.000000 zoom-python-client-0.0.4/venv/bin/rst2html4.py
--rwxr-xr-x   0 rene       (501) staff       (20)     1106 2023-05-15 12:44:10.000000 zoom-python-client-0.0.4/venv/bin/rst2html5.py
--rwxr-xr-x   0 rene       (501) staff       (20)      848 2023-05-15 12:44:10.000000 zoom-python-client-0.0.4/venv/bin/rst2latex.py
--rwxr-xr-x   0 rene       (501) staff       (20)      671 2023-05-15 12:44:10.000000 zoom-python-client-0.0.4/venv/bin/rst2man.py
--rwxr-xr-x   0 rene       (501) staff       (20)      837 2023-05-15 12:44:10.000000 zoom-python-client-0.0.4/venv/bin/rst2odt.py
--rwxr-xr-x   0 rene       (501) staff       (20)     2193 2023-05-15 12:44:10.000000 zoom-python-client-0.0.4/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 rene       (501) staff       (20)      656 2023-05-15 12:44:10.000000 zoom-python-client-0.0.4/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 rene       (501) staff       (20)      692 2023-05-15 12:44:10.000000 zoom-python-client-0.0.4/venv/bin/rst2s5.py
--rwxr-xr-x   0 rene       (501) staff       (20)      928 2023-05-15 12:44:10.000000 zoom-python-client-0.0.4/venv/bin/rst2xetex.py
--rwxr-xr-x   0 rene       (501) staff       (20)      657 2023-05-15 12:44:10.000000 zoom-python-client-0.0.4/venv/bin/rst2xml.py
--rwxr-xr-x   0 rene       (501) staff       (20)      725 2023-05-15 12:44:10.000000 zoom-python-client-0.0.4/venv/bin/rstpep2html.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.097945 zoom-python-client-0.0.4/zoom_python_client/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.4/zoom_python_client/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     2401 2023-05-08 09:39:49.000000 zoom-python-client-0.0.4/zoom_python_client/api_client.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.113522 zoom-python-client-0.0.4/zoom_python_client/client_components/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.4/zoom_python_client/client_components/__init__.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.129033 zoom-python-client-0.0.4/zoom_python_client/client_components/meeting_livestreams/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.4/zoom_python_client/client_components/meeting_livestreams/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1722 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.145388 zoom-python-client-0.0.4/zoom_python_client/client_components/meetings/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.4/zoom_python_client/client_components/meetings/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      624 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/zoom_python_client/client_components/meetings/meetings_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.147115 zoom-python-client-0.0.4/zoom_python_client/client_components/users/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.4/zoom_python_client/client_components/users/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1286 2023-05-04 14:58:03.000000 zoom-python-client-0.0.4/zoom_python_client/client_components/users/users_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.157828 zoom-python-client-0.0.4/zoom_python_client/client_components/webinar_livestreams/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.4/zoom_python_client/client_components/webinar_livestreams/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     1583 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.159323 zoom-python-client-0.0.4/zoom_python_client/client_components/webinars/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.4/zoom_python_client/client_components/webinars/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      401 2023-05-04 14:58:03.000000 zoom-python-client-0.0.4/zoom_python_client/client_components/webinars/webinars_component.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.161279 zoom-python-client-0.0.4/zoom_python_client/utils/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.4/zoom_python_client/utils/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)      221 2023-05-04 14:58:03.000000 zoom-python-client-0.0.4/zoom_python_client/utils/file_system.py
--rw-r--r--   0 rene       (501) staff       (20)      731 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/zoom_python_client/utils/logger.py
--rw-r--r--   0 rene       (501) staff       (20)     5030 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/zoom_python_client/zoom_api_client.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.169350 zoom-python-client-0.0.4/zoom_python_client/zoom_auth_api/
--rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.4/zoom_python_client/zoom_auth_api/__init__.py
--rw-r--r--   0 rene       (501) staff       (20)     2816 2023-05-15 13:04:54.000000 zoom-python-client-0.0.4/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py
--rw-r--r--   0 rene       (501) staff       (20)      817 2023-05-04 14:58:03.000000 zoom-python-client-0.0.4/zoom_python_client/zoom_client_interface.py
-drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-15 13:06:26.112759 zoom-python-client-0.0.4/zoom_python_client.egg-info/
--rw-r--r--   0 rene       (501) staff       (20)     3211 2023-05-15 13:06:25.000000 zoom-python-client-0.0.4/zoom_python_client.egg-info/PKG-INFO
--rw-r--r--   0 rene       (501) staff       (20)     3309 2023-05-15 13:06:26.000000 zoom-python-client-0.0.4/zoom_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 rene       (501) staff       (20)        1 2023-05-15 13:06:25.000000 zoom-python-client-0.0.4/zoom_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 rene       (501) staff       (20)      192 2023-05-15 13:06:25.000000 zoom-python-client-0.0.4/zoom_python_client.egg-info/requires.txt
--rw-r--r--   0 rene       (501) staff       (20)       29 2023-05-15 13:06:25.000000 zoom-python-client-0.0.4/zoom_python_client.egg-info/top_level.txt
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.120776 zoom-python-client-0.0.5/
+-rw-r--r--   0 rene       (501) staff       (20)       49 2022-09-06 12:27:11.000000 zoom-python-client-0.0.5/.coveragerc
+-rw-r--r--   0 rene       (501) staff       (20)       65 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/.env.sample
+-rw-r--r--   0 rene       (501) staff       (20)      137 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.flake8
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.008241 zoom-python-client-0.0.5/.github/
+-rw-r--r--   0 rene       (501) staff       (20)     2918 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.github/CONTRIBUTING.md
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.013650 zoom-python-client-0.0.5/.github/workflows/
+-rw-r--r--   0 rene       (501) staff       (20)     2325 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 rene       (501) staff       (20)      246 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.github/workflows/pre-commit.yaml
+-rw-r--r--   0 rene       (501) staff       (20)      776 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.github/workflows/python-tests.yml
+-rw-r--r--   0 rene       (501) staff       (20)     3086 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.gitignore
+-rw-r--r--   0 rene       (501) staff       (20)      634 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 rene       (501) staff       (20)       14 2022-09-05 07:24:11.000000 zoom-python-client-0.0.5/.tool-versions
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.015264 zoom-python-client-0.0.5/.vscode/
+-rw-r--r--   0 rene       (501) staff       (20)      475 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/.vscode/settings.json
+-rw-r--r--   0 rene       (501) staff       (20)    35149 2023-05-04 09:49:35.000000 zoom-python-client-0.0.5/LICENSE
+-rw-r--r--   0 rene       (501) staff       (20)     3211 2023-05-22 10:10:00.120063 zoom-python-client-0.0.5/PKG-INFO
+-rw-r--r--   0 rene       (501) staff       (20)     2632 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/README.md
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.021841 zoom-python-client-0.0.5/example/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2022-09-06 14:27:54.000000 zoom-python-client-0.0.5/example/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)      355 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/example/get_meeting_livestream.py
+-rw-r--r--   0 rene       (501) staff       (20)      317 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/example/get_user.py
+-rw-r--r--   0 rene       (501) staff       (20)      630 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/example/get_user_meetings.py
+-rw-r--r--   0 rene       (501) staff       (20)      938 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/example/set_meeting_livestream.py
+-rw-r--r--   0 rene       (501) staff       (20)     1269 2023-05-22 10:08:43.000000 zoom-python-client-0.0.5/pyproject.toml
+-rw-r--r--   0 rene       (501) staff       (20)      153 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/pytest.ini
+-rw-r--r--   0 rene       (501) staff       (20)      145 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/requirements.dev.txt
+-rw-r--r--   0 rene       (501) staff       (20)       63 2023-05-22 10:08:43.000000 zoom-python-client-0.0.5/requirements.txt
+-rw-r--r--   0 rene       (501) staff       (20)       38 2023-05-22 10:10:00.121046 zoom-python-client-0.0.5/setup.cfg
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.023390 zoom-python-client-0.0.5/tests/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2022-09-05 07:32:56.000000 zoom-python-client-0.0.5/tests/__init__.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.024782 zoom-python-client-0.0.5/tests/utils/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/utils/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)      176 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/utils/test_logger.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.031434 zoom-python-client-0.0.5/tests/zoom_python_client/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)      405 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/base_test_case.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.033934 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/__init__.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.036425 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/meeting_livestreams/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/meeting_livestreams/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     3980 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/meeting_livestreams/test_meeting_livestreams_component.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.039542 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/meetings/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/meetings/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     1200 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/meetings/test_meetings_component.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.046503 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/users/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/users/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     1193 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/users/test_users_component.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.049817 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/webinar_livestreams/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/webinar_livestreams/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     3980 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/webinar_livestreams/test_webinar_livestreams_component.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.053669 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/webinars/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/webinars/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)      748 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/client_components/webinars/test_webinars_component.py
+-rw-r--r--   0 rene       (501) staff       (20)     1792 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/test_api_client.py
+-rw-r--r--   0 rene       (501) staff       (20)     1757 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/test_zoom_api_client.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.056331 zoom-python-client-0.0.5/tests/zoom_python_client/utils/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/utils/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)      185 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/utils/test_file_system.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.058652 zoom-python-client-0.0.5/tests/zoom_python_client/zoom_auth_api/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/zoom_auth_api/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     1897 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/tests/zoom_python_client/zoom_auth_api/test_zoom_auth_api_client.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:09:59.976798 zoom-python-client-0.0.5/venv/
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.080321 zoom-python-client-0.0.5/venv/bin/
+-rwxr-xr-x   0 rene       (501) staff       (20)      649 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2html.py
+-rwxr-xr-x   0 rene       (501) staff       (20)      771 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2html4.py
+-rwxr-xr-x   0 rene       (501) staff       (20)     1106 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2html5.py
+-rwxr-xr-x   0 rene       (501) staff       (20)      848 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2latex.py
+-rwxr-xr-x   0 rene       (501) staff       (20)      671 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2man.py
+-rwxr-xr-x   0 rene       (501) staff       (20)      837 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2odt.py
+-rwxr-xr-x   0 rene       (501) staff       (20)     2193 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 rene       (501) staff       (20)      656 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 rene       (501) staff       (20)      692 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2s5.py
+-rwxr-xr-x   0 rene       (501) staff       (20)      928 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 rene       (501) staff       (20)      657 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rst2xml.py
+-rwxr-xr-x   0 rene       (501) staff       (20)      725 2023-05-15 12:44:10.000000 zoom-python-client-0.0.5/venv/bin/rstpep2html.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.086321 zoom-python-client-0.0.5/zoom_python_client/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     2401 2023-05-08 09:39:49.000000 zoom-python-client-0.0.5/zoom_python_client/api_client.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.092756 zoom-python-client-0.0.5/zoom_python_client/client_components/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/__init__.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.095579 zoom-python-client-0.0.5/zoom_python_client/client_components/meeting_livestreams/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/meeting_livestreams/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     1722 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.100113 zoom-python-client-0.0.5/zoom_python_client/client_components/meetings/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/meetings/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)      624 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/meetings/meetings_component.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.103139 zoom-python-client-0.0.5/zoom_python_client/client_components/users/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/users/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     1286 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/users/users_component.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.105756 zoom-python-client-0.0.5/zoom_python_client/client_components/webinar_livestreams/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/webinar_livestreams/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     1583 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.108782 zoom-python-client-0.0.5/zoom_python_client/client_components/webinars/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/webinars/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)      401 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/client_components/webinars/webinars_component.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.115703 zoom-python-client-0.0.5/zoom_python_client/utils/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/utils/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)      221 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/utils/file_system.py
+-rw-r--r--   0 rene       (501) staff       (20)      731 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/zoom_python_client/utils/logger.py
+-rw-r--r--   0 rene       (501) staff       (20)     5030 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/zoom_python_client/zoom_api_client.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.118693 zoom-python-client-0.0.5/zoom_python_client/zoom_auth_api/
+-rw-r--r--   0 rene       (501) staff       (20)        0 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/zoom_auth_api/__init__.py
+-rw-r--r--   0 rene       (501) staff       (20)     2816 2023-05-15 13:04:54.000000 zoom-python-client-0.0.5/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py
+-rw-r--r--   0 rene       (501) staff       (20)      817 2023-05-04 14:58:03.000000 zoom-python-client-0.0.5/zoom_python_client/zoom_client_interface.py
+drwxr-xr-x   0 rene       (501) staff       (20)        0 2023-05-22 10:10:00.091885 zoom-python-client-0.0.5/zoom_python_client.egg-info/
+-rw-r--r--   0 rene       (501) staff       (20)     3211 2023-05-22 10:09:59.000000 zoom-python-client-0.0.5/zoom_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 rene       (501) staff       (20)     3309 2023-05-22 10:09:59.000000 zoom-python-client-0.0.5/zoom_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 rene       (501) staff       (20)        1 2023-05-22 10:09:59.000000 zoom-python-client-0.0.5/zoom_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 rene       (501) staff       (20)      192 2023-05-22 10:09:59.000000 zoom-python-client-0.0.5/zoom_python_client.egg-info/requires.txt
+-rw-r--r--   0 rene       (501) staff       (20)       29 2023-05-22 10:09:59.000000 zoom-python-client-0.0.5/zoom_python_client.egg-info/top_level.txt
```

### Comparing `zoom-python-client-0.0.4/.github/CONTRIBUTING.md` & `zoom-python-client-0.0.5/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/.github/workflows/codeql-analysis.yml` & `zoom-python-client-0.0.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/.github/workflows/python-tests.yml` & `zoom-python-client-0.0.5/.github/workflows/python-tests.yml`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/.gitignore` & `zoom-python-client-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/.pre-commit-config.yaml` & `zoom-python-client-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/LICENSE` & `zoom-python-client-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/PKG-INFO` & `zoom-python-client-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoom-python-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Zoom API client for Python
 Author-email: Rene Fernandez <rene.fernandez@cern.ch>
 Project-URL: Homepage, https://github.com/cern-vc/zoom-python-client
 Project-URL: Bug Tracker, https://github.com/cern-vc/zoom-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `zoom-python-client-0.0.4/README.md` & `zoom-python-client-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/example/get_user_meetings.py` & `zoom-python-client-0.0.5/example/get_user_meetings.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/example/set_meeting_livestream.py` & `zoom-python-client-0.0.5/example/set_meeting_livestream.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/pyproject.toml` & `zoom-python-client-0.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zoom-python-client"
-version = "0.0.4"
-dependencies = ["python-dotenv>=0.21.0", "requests>=2.26.0"]
+version = "0.0.5"
+dependencies = ["python-dotenv>=0.21.0", "requests>=2.23.0"]
 authors = [{ name = "Rene Fernandez", email = "rene.fernandez@cern.ch" }]
 description = "Zoom API client for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `zoom-python-client-0.0.4/tests/zoom_python_client/client_components/meeting_livestreams/test_meeting_livestreams_component.py` & `zoom-python-client-0.0.5/tests/zoom_python_client/client_components/meeting_livestreams/test_meeting_livestreams_component.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/tests/zoom_python_client/client_components/meetings/test_meetings_component.py` & `zoom-python-client-0.0.5/tests/zoom_python_client/client_components/meetings/test_meetings_component.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/tests/zoom_python_client/client_components/users/test_users_component.py` & `zoom-python-client-0.0.5/tests/zoom_python_client/client_components/users/test_users_component.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/tests/zoom_python_client/client_components/webinar_livestreams/test_webinar_livestreams_component.py` & `zoom-python-client-0.0.5/tests/zoom_python_client/client_components/webinar_livestreams/test_webinar_livestreams_component.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/tests/zoom_python_client/client_components/webinars/test_webinars_component.py` & `zoom-python-client-0.0.5/tests/zoom_python_client/client_components/webinars/test_webinars_component.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/tests/zoom_python_client/test_api_client.py` & `zoom-python-client-0.0.5/tests/zoom_python_client/test_api_client.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/tests/zoom_python_client/test_zoom_api_client.py` & `zoom-python-client-0.0.5/tests/zoom_python_client/test_zoom_api_client.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/tests/zoom_python_client/zoom_auth_api/test_zoom_auth_api_client.py` & `zoom-python-client-0.0.5/tests/zoom_python_client/zoom_auth_api/test_zoom_auth_api_client.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/venv/bin/rst2html.py` & `zoom-python-client-0.0.5/venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/venv/bin/rst2html4.py` & `zoom-python-client-0.0.5/venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/venv/bin/rst2html5.py` & `zoom-python-client-0.0.5/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/venv/bin/rst2latex.py` & `zoom-python-client-0.0.5/venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/venv/bin/rst2man.py` & `zoom-python-client-0.0.5/venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/venv/bin/rst2odt.py` & `zoom-python-client-0.0.5/venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/venv/bin/rst2odt_prepstyles.py` & `zoom-python-client-0.0.5/venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/venv/bin/rst2pseudoxml.py` & `zoom-python-client-0.0.5/venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/venv/bin/rst2s5.py` & `zoom-python-client-0.0.5/venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/venv/bin/rst2xetex.py` & `zoom-python-client-0.0.5/venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/venv/bin/rst2xml.py` & `zoom-python-client-0.0.5/venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/venv/bin/rstpep2html.py` & `zoom-python-client-0.0.5/venv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/zoom_python_client/api_client.py` & `zoom-python-client-0.0.5/zoom_python_client/api_client.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py` & `zoom-python-client-0.0.5/zoom_python_client/client_components/meeting_livestreams/meeting_livestreams_component.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/zoom_python_client/client_components/meetings/meetings_component.py` & `zoom-python-client-0.0.5/zoom_python_client/client_components/meetings/meetings_component.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/zoom_python_client/client_components/users/users_component.py` & `zoom-python-client-0.0.5/zoom_python_client/client_components/users/users_component.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py` & `zoom-python-client-0.0.5/zoom_python_client/client_components/webinar_livestreams/webinar_livestreams_component.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/zoom_python_client/utils/logger.py` & `zoom-python-client-0.0.5/zoom_python_client/utils/logger.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/zoom_python_client/zoom_api_client.py` & `zoom-python-client-0.0.5/zoom_python_client/zoom_api_client.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py` & `zoom-python-client-0.0.5/zoom_python_client/zoom_auth_api/zoom_auth_api_client.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/zoom_python_client/zoom_client_interface.py` & `zoom-python-client-0.0.5/zoom_python_client/zoom_client_interface.py`

 * *Files identical despite different names*

### Comparing `zoom-python-client-0.0.4/zoom_python_client.egg-info/PKG-INFO` & `zoom-python-client-0.0.5/zoom_python_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zoom-python-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Zoom API client for Python
 Author-email: Rene Fernandez <rene.fernandez@cern.ch>
 Project-URL: Homepage, https://github.com/cern-vc/zoom-python-client
 Project-URL: Bug Tracker, https://github.com/cern-vc/zoom-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `zoom-python-client-0.0.4/zoom_python_client.egg-info/SOURCES.txt` & `zoom-python-client-0.0.5/zoom_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

