# Comparing `tmp/morpheus-mail-0.0.5.tar.gz` & `tmp/morpheus-mail-1.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/morpheus-mail-0.0.5.tar", last modified: Thu Oct  4 12:35:45 2018, max compression
+gzip compressed data, was "morpheus-mail-1.0.17.tar", last modified: Mon May 22 15:21:18 2023, max compression
```

## Comparing `morpheus-mail-0.0.5.tar` & `morpheus-mail-1.0.17.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-04 12:35:45.000000 morpheus-mail-0.0.5/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3832 2018-10-04 12:34:07.000000 morpheus-mail-0.0.5/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     1376 2018-10-04 12:34:07.000000 morpheus-mail-0.0.5/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-04 12:35:45.000000 morpheus-mail-0.0.5/morpheus/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-04 12:35:45.000000 morpheus-mail-0.0.5/morpheus/app/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-04 12:35:45.000000 morpheus-mail-0.0.5/morpheus/app/render/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6808 2018-10-04 12:34:07.000000 morpheus-mail-0.0.5/morpheus/app/render/main.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       69 2018-10-04 12:34:07.000000 morpheus-mail-0.0.5/morpheus/app/render/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-10-04 12:35:45.000000 morpheus-mail-0.0.5/morpheus_mail.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)        9 2018-10-04 12:35:45.000000 morpheus-mail-0.0.5/morpheus_mail.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-10-04 12:35:45.000000 morpheus-mail-0.0.5/morpheus_mail.egg-info/zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2018-10-04 12:35:45.000000 morpheus-mail-0.0.5/morpheus_mail.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1122 2018-10-04 12:35:45.000000 morpheus-mail-0.0.5/morpheus_mail.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-10-04 12:35:45.000000 morpheus-mail-0.0.5/morpheus_mail.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      304 2018-10-04 12:35:45.000000 morpheus-mail-0.0.5/morpheus_mail.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      455 2018-10-04 12:35:45.000000 morpheus-mail-0.0.5/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1122 2018-10-04 12:35:45.000000 morpheus-mail-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:18.687962 morpheus-mail-1.0.17/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-22 15:21:18.687962 morpheus-mail-1.0.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:18.683962 morpheus-mail-1.0.17/morpheus_mail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-22 15:21:18.000000 morpheus-mail-1.0.17/morpheus_mail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-22 15:21:18.000000 morpheus-mail-1.0.17/morpheus_mail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:21:18.000000 morpheus-mail-1.0.17/morpheus_mail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-22 15:21:18.000000 morpheus-mail-1.0.17/morpheus_mail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 15:21:18.000000 morpheus-mail-1.0.17/morpheus_mail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:21:18.000000 morpheus-mail-1.0.17/morpheus_mail.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-22 15:21:18.687962 morpheus-mail-1.0.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:18.683962 morpheus-mail-1.0.17/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:18.683962 morpheus-mail-1.0.17/src/render/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/src/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/src/render/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:21:18.683962 morpheus-mail-1.0.17/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/tests/test_aux.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31782 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/tests/test_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/tests/test_render.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/tests/test_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-22 15:20:08.000000 morpheus-mail-1.0.17/tests/test_user_display.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `morpheus-mail-0.0.5/setup.py` & `morpheus-mail-1.0.17/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 from setuptools import setup
 
+from src.version import VERSION
+
 setup(
     name='morpheus-mail',
-    version='0.0.5',
+    version=str(VERSION),
     description='Email rendering engine from morpheus',
     long_description="""
-Note: this only installs the rendering logic for `morpheus <https://github.com/tutorcruncher/morpheus>`_ 
+Note: this only installs the rendering logic for `morpheus <https://github.com/tutorcruncher/morpheus>` \
 for testing and email preview.
 
-Everything else is excluded to avoid installing unnecessary packages. 
+Everything else is excluded to avoid installing unnecessary packages.
 """,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
         'Intended Audience :: Developers',
         'Intended Audience :: Information Technology',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: MIT License',
         'Operating System :: Unix',
         'Operating System :: POSIX :: Linux',
         'Topic :: Internet',
     ],
     author='Samuel Colvin',
     author_email='s@muelcolvin.com',
     url='https://github.com/tutorcruncher/morpheus',
     license='MIT',
-    packages=['morpheus.render'],
-    package_dir={'morpheus.render': 'morpheus/app/render'},
+    packages=['src.render'],
+    package_dir={'src.render': 'src/render'},
     python_requires='>=3.6',
     zip_safe=True,
     install_requires=[
         'chevron>=0.11.1',
         'libsass>=0.13.2',
         'misaka>=2.1.0',
+        'python_version>3',
     ],
 )
```

### Comparing `morpheus-mail-0.0.5/morpheus/app/render/main.py` & `morpheus-mail-1.0.17/src/render/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,59 @@
+from dataclasses import dataclass
+
+import chevron
 import logging
 import re
+import sass
 import secrets
 from base64 import urlsafe_b64encode
-from typing import Dict, NamedTuple
-
-import chevron
-import sass
 from chevron import ChevronError
 from misaka import HtmlRenderer, Markdown
+from typing import Dict
 
 markdown = Markdown(HtmlRenderer(flags=['hard-wrap']), extensions=['no-intra-emphasis'])
-logger = logging.getLogger('morpheus.render')
+logger = logging.getLogger('render')
 
 
-class MessageDef(NamedTuple):
+@dataclass
+class MessageDef:
     first_name: str
     last_name: str
     main_template: str
     mustache_partials: Dict[str, dict]
     macros: Dict[str, dict]
     subject_template: str
     context: dict
     headers: dict
 
 
-class EmailInfo(NamedTuple):
+@dataclass
+class EmailInfo:
     full_name: str
     subject: str
     html_body: str
     headers: dict
     shortened_link: list
 
 
 def _update_context(context, partials, macros):
     for k, v in context.items():
         if k.endswith('__md'):
             yield k[:-4], markdown(v)
         elif k.endswith('__sass'):
             yield k[:-6], sass.compile(string=v, output_style='compressed', precision=10).strip('\n')
         elif k.endswith('__render'):
-            v = chevron.render(
-                _apply_macros(v, macros),
-                data=context,
-                partials_dict=partials
-            )
+            v = chevron.render(_apply_macros(v, macros), data=context, partials_dict=partials)
             yield k[:-8], markdown(v)
 
 
 def _apply_macros(s, macros):
     if macros:
         for key, body in macros.items():
-            m = re.search('^(\S+)\((.*)\) *$', key)
+            m = re.search(r'^(\S+)\((.*)\) *$', key)
             if not m:
                 logger.warning('invalid macro "%s", skipping it', key)
                 continue
             name, arg_defs = m.groups()
             arg_defs = [a.strip(' ') for a in arg_defs.split('|') if a.strip(' ')]
 
             def replace_macro(m):
@@ -73,19 +72,15 @@
     re.compile(r'\.(?:png|jpg|bmp)$'),
     re.compile(r'^https?://maps.googleapis.com'),
     re.compile(r'^https?://maps.google.com'),
 ]
 
 
 def looks_like_link(s):
-    return (
-        isinstance(s, str) and
-        re.match('^https?://', s) and
-        not any(m.search(s) for m in SKIPPED_LINKS)
-    )
+    return isinstance(s, str) and re.match('^https?://', s) and not any(m.search(s) for m in SKIPPED_LINKS)
 
 
 def apply_short_links(context, click_url, click_random=30, backup_arg=False):
     shortened_link = []
     extra = {}
     for k, v in context.items():
         # TODO deal with unsubscribe links properly
@@ -111,72 +106,175 @@
     except ChevronError as e:
         logger.warning('invalid subject template: %s', e)
         subject = m.subject_template
 
     shortened_link = []
     if click_url:
         shortened_link = apply_short_links(m.context, click_url, click_random, backup_arg=True)
-    m.context.update(
-        email_subject=subject,
-        **dict(_update_context(m.context, m.mustache_partials, m.macros))
-    )
+    m.context.update(email_subject=subject, **dict(_update_context(m.context, m.mustache_partials, m.macros)))
     unsubscribe_link = m.context.get('unsubscribe_link')
     if unsubscribe_link:
         m.headers.setdefault('List-Unsubscribe', f'<{unsubscribe_link}>')
 
     return EmailInfo(
         full_name=full_name,
         subject=subject,
         html_body=chevron.render(
-            _apply_macros(m.main_template, m.macros),
-            data=m.context,
-            partials_dict=m.mustache_partials,
+            _apply_macros(m.main_template, m.macros), data=m.context, partials_dict=m.mustache_partials
         ),
         headers=m.headers,
         shortened_link=shortened_link,
     )
 
 
 BASIC_CHARACTERS = {
     # basic characters from https://support.messagebird.com/hc/en-us/articles/208739765-Which-special-
     # characters-count-as-two-characters-in-a-text-message- ordered and repeats removed!
-    ' ', '!', '"', '#', '$', '%', '&', "'", '(', ')', '*', '+', ',', '-', '.', '/',
-    '0', '1', '2', '3', '4', '5', '6', '7', '8', '9', ':', ';', '<', '=', '>', '?', '@',
-    'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U',
-    'V', 'W', 'X', 'Y', 'Z',
+    ' ',
+    '!',
+    '"',
+    '#',
+    '$',
+    '%',
+    '&',
+    "'",
+    '(',
+    ')',
+    '*',
+    '+',
+    ',',
+    '-',
+    '.',
+    '/',
+    '0',
+    '1',
+    '2',
+    '3',
+    '4',
+    '5',
+    '6',
+    '7',
+    '8',
+    '9',
+    ':',
+    ';',
+    '<',
+    '=',
+    '>',
+    '?',
+    '@',
+    'A',
+    'B',
+    'C',
+    'D',
+    'E',
+    'F',
+    'G',
+    'H',
+    'I',
+    'J',
+    'K',
+    'L',
+    'M',
+    'N',
+    'O',
+    'P',
+    'Q',
+    'R',
+    'S',
+    'T',
+    'U',
+    'V',
+    'W',
+    'X',
+    'Y',
+    'Z',
     '_',
-    'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u',
-    'v', 'w', 'x', 'y', 'z',
-    '¡', '£', '¤', '¥', '§', '¿', 'Ä', 'Å', 'Æ', 'Ç', 'É', 'Ñ', 'Ö', 'Ø', 'Ü', 'ß', 'à', 'ä', 'å', 'æ', 'è',
-    'é', 'ì', 'ñ', 'ò', 'ö', 'ø', 'ù', 'ü', 'Γ', 'Δ', 'Θ', 'Λ', 'Ξ', 'Π', 'Σ', 'Φ', 'Ψ', 'Ω',
+    'a',
+    'b',
+    'c',
+    'd',
+    'e',
+    'f',
+    'g',
+    'h',
+    'i',
+    'j',
+    'k',
+    'l',
+    'm',
+    'n',
+    'o',
+    'p',
+    'q',
+    'r',
+    's',
+    't',
+    'u',
+    'v',
+    'w',
+    'x',
+    'y',
+    'z',
+    '¡',
+    '£',
+    '¤',
+    '¥',
+    '§',
+    '¿',
+    'Ä',
+    'Å',
+    'Æ',
+    'Ç',
+    'É',
+    'Ñ',
+    'Ö',
+    'Ø',
+    'Ü',
+    'ß',
+    'à',
+    'ä',
+    'å',
+    'æ',
+    'è',
+    'é',
+    'ì',
+    'ñ',
+    'ò',
+    'ö',
+    'ø',
+    'ù',
+    'ü',
+    'Γ',
+    'Δ',
+    'Θ',
+    'Λ',
+    'Ξ',
+    'Π',
+    'Σ',
+    'Φ',
+    'Ψ',
+    'Ω',
     # special cases from https://support.messagebird.com/hc/en-gb/articles/200731072-In-which-charset-can-I-deliver-
     # SMS-messages-and-what-should-I-take-into-consideration- this is not an exhaustive list :(
-    'ç', '®'
+    'ç',
+    '®',
 }
 
 # from first link above
 # apparently messagebird call \n an extension character which differs from https://en.wikipedia.org/wiki/GSM_03.38
 # this might be because they replace \n with LF + CR which would constitute 2 characters
 EXTENSION_CHARACTERS = {'\n', '[', '\\', ']', '^', '{', '|', '}', '~', '€'}
 
 # from https://support.messagebird.com/hc/en-us/articles/208739745-How-long-is-1-SMS-Message-
-MULTIPART_LENGTHS = [
-    (1, 160),
-    (2, 306),
-    (3, 459),
-    (4, 612),
-    (5, 765),
-    (6, 918),
-    (7, 1071),
-    (8, 1224),
-    (9, 1377),
-]
+MULTIPART_LENGTHS = [(1, 160), (2, 306), (3, 459), (4, 612), (5, 765), (6, 918), (7, 1071), (8, 1224), (9, 1377)]
 
 
-class SmsLength(NamedTuple):
+@dataclass
+class SmsLength:
     length: int
     parts: int
 
 
 class MessageTooLong(ValueError):
     pass
```

