# Comparing `tmp/tgbox-1.1.1.tar.gz` & `tmp/tgbox-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgbox-1.1.1.tar", last modified: Thu Mar 23 22:43:07 2023, max compression
+gzip compressed data, was "tgbox-1.2.tar", last modified: Mon May 22 20:45:52 2023, max compression
```

## Comparing `tgbox-1.1.1.tar` & `tgbox-1.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-03-23 22:43:07.552712 tgbox-1.1.1/
--rw-r--r--   0 non       (1000) non       (1000)       32 2021-12-13 19:32:05.000000 tgbox-1.1.1/MANIFEST.in
--rw-r--r--   0 non       (1000) non       (1000)     7761 2023-03-23 22:43:07.552712 tgbox-1.1.1/PKG-INFO
--rw-r--r--   0 non       (1000) non       (1000)     5715 2023-03-21 16:22:09.000000 tgbox-1.1.1/README.rst
--rw-r--r--   0 non       (1000) non       (1000)       38 2023-03-23 22:43:07.552712 tgbox-1.1.1/setup.cfg
--rw-r--r--   0 non       (1000) non       (1000)     1752 2023-03-23 22:37:41.000000 tgbox-1.1.1/setup.py
-drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-03-23 22:43:07.544711 tgbox-1.1.1/tgbox/
--rw-r--r--   0 non       (1000) non       (1000)      614 2023-03-23 22:37:41.000000 tgbox-1.1.1/tgbox/__init__.py
-drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-03-23 22:43:07.548711 tgbox-1.1.1/tgbox/api/
--rw-r--r--   0 non       (1000) non       (1000)       78 2023-03-21 15:56:42.000000 tgbox-1.1.1/tgbox/api/__init__.py
--rw-r--r--   0 non       (1000) non       (1000)     7382 2023-03-21 15:56:42.000000 tgbox-1.1.1/tgbox/api/db.py
--rw-r--r--   0 non       (1000) non       (1000)    72115 2023-03-21 15:56:42.000000 tgbox-1.1.1/tgbox/api/local.py
--rw-r--r--   0 non       (1000) non       (1000)    63939 2023-03-21 15:56:42.000000 tgbox-1.1.1/tgbox/api/remote.py
--rw-r--r--   0 non       (1000) non       (1000)    18595 2023-03-21 15:56:42.000000 tgbox-1.1.1/tgbox/api/utils.py
--rw-r--r--   0 non       (1000) non       (1000)     6068 2023-03-21 15:56:42.000000 tgbox-1.1.1/tgbox/crypto.py
--rw-r--r--   0 non       (1000) non       (1000)     3507 2023-03-21 15:56:42.000000 tgbox-1.1.1/tgbox/defaults.py
--rw-r--r--   0 non       (1000) non       (1000)     2097 2023-03-21 15:56:42.000000 tgbox-1.1.1/tgbox/errors.py
--rw-r--r--   0 non       (1000) non       (1000)    14566 2023-03-21 15:56:42.000000 tgbox-1.1.1/tgbox/fastelethon.py
--rw-r--r--   0 non       (1000) non       (1000)    20090 2023-03-21 15:56:42.000000 tgbox-1.1.1/tgbox/keys.py
-drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-03-23 22:43:07.548711 tgbox-1.1.1/tgbox/other/
--rw-r--r--   0 non       (1000) non       (1000)    13796 2023-03-21 15:56:42.000000 tgbox-1.1.1/tgbox/other/tgbox_logo.png
--rw-r--r--   0 non       (1000) non       (1000)    13116 2021-11-20 20:57:53.000000 tgbox-1.1.1/tgbox/other/words.txt
--rw-r--r--   0 non       (1000) non       (1000)    15930 2023-03-21 15:56:42.000000 tgbox-1.1.1/tgbox/tools.py
-drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-03-23 22:43:07.548711 tgbox-1.1.1/tgbox.egg-info/
--rw-r--r--   0 non       (1000) non       (1000)     7761 2023-03-23 22:43:05.000000 tgbox-1.1.1/tgbox.egg-info/PKG-INFO
--rw-r--r--   0 non       (1000) non       (1000)      438 2023-03-23 22:43:05.000000 tgbox-1.1.1/tgbox.egg-info/SOURCES.txt
--rw-r--r--   0 non       (1000) non       (1000)        1 2023-03-23 22:43:05.000000 tgbox-1.1.1/tgbox.egg-info/dependency_links.txt
--rw-r--r--   0 non       (1000) non       (1000)      163 2023-03-23 22:43:05.000000 tgbox-1.1.1/tgbox.egg-info/requires.txt
--rw-r--r--   0 non       (1000) non       (1000)        6 2023-03-23 22:43:05.000000 tgbox-1.1.1/tgbox.egg-info/top_level.txt
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-05-22 20:45:52.798249 tgbox-1.2/
+-rw-r--r--   0 non       (1000) non       (1000)       32 2023-05-13 15:05:38.000000 tgbox-1.2/MANIFEST.in
+-rw-r--r--   0 non       (1000) non       (1000)     7710 2023-05-22 20:45:52.798249 tgbox-1.2/PKG-INFO
+-rw-r--r--   0 non       (1000) non       (1000)     5723 2023-05-13 15:05:38.000000 tgbox-1.2/README.rst
+-rw-r--r--   0 non       (1000) non       (1000)       38 2023-05-22 20:45:52.798249 tgbox-1.2/setup.cfg
+-rw-r--r--   0 non       (1000) non       (1000)     2134 2023-05-22 20:43:54.000000 tgbox-1.2/setup.py
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-05-22 20:45:52.790248 tgbox-1.2/tgbox/
+-rw-r--r--   0 non       (1000) non       (1000)     1428 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/__init__.py
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-05-22 20:45:52.794248 tgbox-1.2/tgbox/api/
+-rw-r--r--   0 non       (1000) non       (1000)       78 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/api/__init__.py
+-rw-r--r--   0 non       (1000) non       (1000)     9285 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/api/db.py
+-rw-r--r--   0 non       (1000) non       (1000)   104193 2023-05-21 15:40:55.000000 tgbox-1.2/tgbox/api/local.py
+-rw-r--r--   0 non       (1000) non       (1000)    79976 2023-05-21 15:43:36.000000 tgbox-1.2/tgbox/api/remote.py
+-rw-r--r--   0 non       (1000) non       (1000)    20759 2023-05-14 15:15:11.000000 tgbox-1.2/tgbox/api/utils.py
+-rw-r--r--   0 non       (1000) non       (1000)     6266 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/crypto.py
+-rw-r--r--   0 non       (1000) non       (1000)     3744 2023-05-21 15:21:29.000000 tgbox-1.2/tgbox/defaults.py
+-rw-r--r--   0 non       (1000) non       (1000)     2097 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/errors.py
+-rw-r--r--   0 non       (1000) non       (1000)    14575 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/fastelethon.py
+-rw-r--r--   0 non       (1000) non       (1000)    19962 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/keys.py
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-05-22 20:45:52.794248 tgbox-1.2/tgbox/other/
+-rw-r--r--   0 non       (1000) non       (1000)    13796 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/other/tgbox_logo.png
+-rw-r--r--   0 non       (1000) non       (1000)    13116 2023-05-13 15:05:38.000000 tgbox-1.2/tgbox/other/words.txt
+-rw-r--r--   0 non       (1000) non       (1000)    19278 2023-05-22 18:58:07.000000 tgbox-1.2/tgbox/tools.py
+-rw-r--r--   0 non       (1000) non       (1000)       16 2023-05-22 19:12:12.000000 tgbox-1.2/tgbox/version.py
+drwxr-xr-x   0 non       (1000) non       (1000)        0 2023-05-22 20:45:52.794248 tgbox-1.2/tgbox.egg-info/
+-rw-r--r--   0 non       (1000) non       (1000)     7710 2023-05-22 20:45:52.000000 tgbox-1.2/tgbox.egg-info/PKG-INFO
+-rw-r--r--   0 non       (1000) non       (1000)      455 2023-05-22 20:45:52.000000 tgbox-1.2/tgbox.egg-info/SOURCES.txt
+-rw-r--r--   0 non       (1000) non       (1000)        1 2023-05-22 20:45:52.000000 tgbox-1.2/tgbox.egg-info/dependency_links.txt
+-rw-r--r--   0 non       (1000) non       (1000)      172 2023-05-22 20:45:52.000000 tgbox-1.2/tgbox.egg-info/requires.txt
+-rw-r--r--   0 non       (1000) non       (1000)        6 2023-05-22 20:45:52.000000 tgbox-1.2/tgbox.egg-info/top_level.txt
```

### Comparing `tgbox-1.1.1/PKG-INFO` & `tgbox-1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,94 +1,88 @@
 Metadata-Version: 2.1
 Name: tgbox
-Version: 1.1.1
+Version: 1.2
 Summary: Encrypted cloud storage API based on a Telegram API
 Home-page: https://github.com/NonProjects/tgbox
 Author: NonProjects
 Author-email: thenonproton@pm.me
 License: LGPL-2.1
-Download-URL: https://github.com/NonProjects/tgbox/archive/refs/tags/v1.1.1.tar.gz
+Download-URL: https://github.com/NonProjects/tgbox/archive/refs/tags/v1.2.tar.gz
 Description: TGBOX: encrypted cloud storage based on Telegram
         ================================================
-        .. image:: https://readthedocs.org/projects/tgbox/badge/?version=latest
+        .. epigraph::
+                | This repository contains a set of classes and functions used to manage TGBOX.
+                | Try the `tgbox-cli <https://github.com/NotStatilko/tgbox-cli>`__  if you're interested in working implementation!
         
         .. code-block:: python
         
-                from tgbox.api import (
-                    TelegramClient,
-                    make_remotebox,
-                    make_localbox
-                )
                 from asyncio import run as asyncio_run
-                from tgbox.keys import Phrase, make_basekey
                 from getpass import getpass # Hidden input
         
-                # Phone number linked to your Telegram account
-                PHONE_NUMBER = '+10000000000'
+                from tgbox.api import TelegramClient, make_remotebox, make_localbox
+                from tgbox.keys import Phrase, make_basekey
         
                 # This two will not work. Get your own at https://my.telegram.org
                 API_ID, API_HASH = 1234567, '00000000000000000000000000000000'
+                # Simple progress callback to track upload/download state
+                PROGRESS_CALLBACK = lambda c,t: print(round(c/t*100),'%')
         
                 async def main():
+                    phone = input('Phone number: ')
+        
                     tc = TelegramClient(
-                        phone_number = PHONE_NUMBER,
+                        phone_number = phone,
                         api_id = API_ID,
                         api_hash = API_HASH
                     )
-                    await tc.connect() # Connecting with Telegram
+                    await tc.connect() # Connecting to Telegram
                     await tc.send_code() # Requesting login code
         
-                    await tc.log_in(
-                        code = int(input('Code: ')),
-                        password = getpass('Pass: ')
-                    )
-                    # Generating your passphrase
-                    p = Phrase.generate()
-                    print(p.phrase.decode())
+                    code = int(input('Login code: '))
+                    password = getpass('Your password: ')
+        
+                    # Login to your Telegram account
+                    await tc.log_in(password, code)
+        
+                    # Generate and show your Box phrase
+                    print(phrase := Phrase.generate())
         
                     # WARNING: This will use 1GB of RAM for a
                     # couple of seconds. See help(make_basekey)
-                    basekey = make_basekey(p)
+                    basekey = make_basekey(phrase)
+        
+                    erb = await make_remotebox(tc) # Make EncryptedRemoteBox
+                    dlb = await make_localbox(erb, basekey) # Make DecryptedLocalBox
+                    drb = await erb.decrypt(dlb=dlb) # Obtain DecryptedRemoteBox
+        
+                    # Write a file path to upload to your Box
+                    file_to_upload = input('File to upload (path): ')
         
-                    # Make EncryptedRemoteBox
-                    erb = await make_remotebox(tc)
-                    # Make DecryptedLocalBox
-                    dlb = await make_localbox(erb, basekey)
-                    # Obtain DecryptedRemoteBox
-                    drb = await erb.decrypt(dlb=dlb)
-        
-                    # CATTRS is a File's CustomAttributes. You
-                    # can specify any you want. Here we will add
-                    # a "comment" attr with a true statement :^)
-                    cattrs = {'comment': b'Cats are cool B-)'}
-        
-                    # Preparing file for upload. This will return a PreparedFile object
-                    pf = await dlb.prepare_file(open('cats.png','rb'), cattrs=cattrs)
-        
-                    # Uploading PreparedFile to the RemoteBox
-                    # and return DecryptedRemoteBoxFile
-                    drbf = await drb.push_file(pf)
+                    # Preparing for upload. Will return a PreparedFile object
+                    pf = await dlb.prepare_file(open(file_to_upload,'rb'))
+                    # Uploading PreparedFile to Remote and getting DecryptedRemoteBoxFile
+                    drbf = await drb.push_file(pf, progress_callback=PROGRESS_CALLBACK)
         
-                    # Retrieving some info from the RemoteBoxFile
+                    # Retrieving some info from the RemoteBox file
                     print('File size:', drbf.size, 'bytes')
                     print('File name:', drbf.file_name)
         
                     # You can also access all information about
                     # the RemoteBoxFile you need from the LocalBox
                     dlbf = await dlb.get_file(drbf.id)
         
+                    print('File size:', dlbf.size, 'bytes')
                     print('File path:', dlbf.file_path)
-                    print('Custom Attributes:', dlbf.cattrs)
         
-                    # Downloading file back.
-                    await drbf.download()
+                    # Downloading your [already uploaded] file from Remote.
+                    await drbf.download(progress_callback=PROGRESS_CALLBACK)
         
                     # Close all connections
                     # after work was done
-                    await erb.done()
+                    await drb.done()
                     await dlb.done()
         
                 asyncio_run(main())
         
         Motivation
         ----------
         
@@ -117,15 +111,14 @@
            cd tgbox && python3 -m pip install .[doc] # Install with doc
            cd docs && make html && firefox _build/html/index.html
         
         Third party & thanks to
         -----------------------
         - `⭐️ <https://github.com/NonProjects/tgbox/stargazers>`__ **Stargazers!**
         - `Sphinx_rtd_theme <https://github.com/readthedocs/sphinx_rtd_theme>`__ (`MIT <https://github.com/readthedocs/sphinx_rtd_theme/blob/master/LICENSE>`__)
-        - `Regex <https://github.com/mrabarnett/mrab-regex>`__ (`LICENSE <https://github.com/mrabarnett/mrab-regex/blob/hg/LICENSE.txt>`__)
         - `Aiosqlite <https://github.com/omnilib/aiosqlite>`__ (`MIT <https://github.com/omnilib/aiosqlite/blob/main/LICENSE>`__)
         - `Telethon <https://github.com/LonamiWebs/Telethon>`__ (`MIT <https://github.com/LonamiWebs/Telethon/blob/master/LICENSE>`__)
         - `Ecdsa <https://github.com/tlsfuzzer/python-ecdsa>`__ (`LICENSE <https://github.com/tlsfuzzer/python-ecdsa/blob/master/LICENSE>`__)
         - `Filetype <https://github.com/h2non/filetype.py>`__ (`MIT <https://github.com/h2non/filetype.py/blob/master/LICENSE>`__)
         - `Cryptg <https://github.com/cher-nov/cryptg>`__ (`LICENSE <https://github.com/cher-nov/cryptg/blob/master/LICENSE.txt>`__)
         - `Cryptography <https://github.com/pyca/cryptography>`__ (`LICENSE <https://github.com/pyca/cryptography/blob/main/LICENSE>`__)
         
@@ -137,15 +130,15 @@
 Keywords: Telegram,Cloud-Storage,Cloud,API,Asyncio,Non-official
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Archiving :: Backup
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
 Provides-Extra: fast
```

### Comparing `tgbox-1.1.1/README.rst` & `tgbox-1.2/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,85 +1,79 @@
 TGBOX: encrypted cloud storage based on Telegram
 ================================================
-.. image:: https://readthedocs.org/projects/tgbox/badge/?version=latest
+.. epigraph::
+        | This repository contains a set of classes and functions used to manage TGBOX.
+        | Try the `tgbox-cli <https://github.com/NotStatilko/tgbox-cli>`__  if you're interested in working implementation!
 
 .. code-block:: python
 
-        from tgbox.api import (
-            TelegramClient,
-            make_remotebox,
-            make_localbox
-        )
         from asyncio import run as asyncio_run
-        from tgbox.keys import Phrase, make_basekey
         from getpass import getpass # Hidden input
 
-        # Phone number linked to your Telegram account
-        PHONE_NUMBER = '+10000000000'
+        from tgbox.api import TelegramClient, make_remotebox, make_localbox
+        from tgbox.keys import Phrase, make_basekey
 
         # This two will not work. Get your own at https://my.telegram.org
         API_ID, API_HASH = 1234567, '00000000000000000000000000000000'
+        # Simple progress callback to track upload/download state
+        PROGRESS_CALLBACK = lambda c,t: print(round(c/t*100),'%')
 
         async def main():
+            phone = input('Phone number: ')
+
             tc = TelegramClient(
-                phone_number = PHONE_NUMBER,
+                phone_number = phone,
                 api_id = API_ID,
                 api_hash = API_HASH
             )
-            await tc.connect() # Connecting with Telegram
+            await tc.connect() # Connecting to Telegram
             await tc.send_code() # Requesting login code
 
-            await tc.log_in(
-                code = int(input('Code: ')),
-                password = getpass('Pass: ')
-            )
-            # Generating your passphrase
-            p = Phrase.generate()
-            print(p.phrase.decode())
+            code = int(input('Login code: '))
+            password = getpass('Your password: ')
+
+            # Login to your Telegram account
+            await tc.log_in(password, code)
+
+            # Generate and show your Box phrase
+            print(phrase := Phrase.generate())
 
             # WARNING: This will use 1GB of RAM for a
             # couple of seconds. See help(make_basekey)
-            basekey = make_basekey(p)
+            basekey = make_basekey(phrase)
+
+            erb = await make_remotebox(tc) # Make EncryptedRemoteBox
+            dlb = await make_localbox(erb, basekey) # Make DecryptedLocalBox
+            drb = await erb.decrypt(dlb=dlb) # Obtain DecryptedRemoteBox
+
+            # Write a file path to upload to your Box
+            file_to_upload = input('File to upload (path): ')
 
-            # Make EncryptedRemoteBox
-            erb = await make_remotebox(tc)
-            # Make DecryptedLocalBox
-            dlb = await make_localbox(erb, basekey)
-            # Obtain DecryptedRemoteBox
-            drb = await erb.decrypt(dlb=dlb)
-
-            # CATTRS is a File's CustomAttributes. You
-            # can specify any you want. Here we will add
-            # a "comment" attr with a true statement :^)
-            cattrs = {'comment': b'Cats are cool B-)'}
-
-            # Preparing file for upload. This will return a PreparedFile object
-            pf = await dlb.prepare_file(open('cats.png','rb'), cattrs=cattrs)
-
-            # Uploading PreparedFile to the RemoteBox
-            # and return DecryptedRemoteBoxFile
-            drbf = await drb.push_file(pf)
+            # Preparing for upload. Will return a PreparedFile object
+            pf = await dlb.prepare_file(open(file_to_upload,'rb'))
+            # Uploading PreparedFile to Remote and getting DecryptedRemoteBoxFile
+            drbf = await drb.push_file(pf, progress_callback=PROGRESS_CALLBACK)
 
-            # Retrieving some info from the RemoteBoxFile
+            # Retrieving some info from the RemoteBox file
             print('File size:', drbf.size, 'bytes')
             print('File name:', drbf.file_name)
 
             # You can also access all information about
             # the RemoteBoxFile you need from the LocalBox
             dlbf = await dlb.get_file(drbf.id)
 
+            print('File size:', dlbf.size, 'bytes')
             print('File path:', dlbf.file_path)
-            print('Custom Attributes:', dlbf.cattrs)
 
-            # Downloading file back.
-            await drbf.download()
+            # Downloading your [already uploaded] file from Remote.
+            await drbf.download(progress_callback=PROGRESS_CALLBACK)
 
             # Close all connections
             # after work was done
-            await erb.done()
+            await drb.done()
             await dlb.done()
 
         asyncio_run(main())
 
 Motivation
 ----------
 
@@ -108,15 +102,14 @@
    cd tgbox && python3 -m pip install .[doc] # Install with doc
    cd docs && make html && firefox _build/html/index.html
 
 Third party & thanks to
 -----------------------
 - `⭐️ <https://github.com/NonProjects/tgbox/stargazers>`__ **Stargazers!**
 - `Sphinx_rtd_theme <https://github.com/readthedocs/sphinx_rtd_theme>`__ (`MIT <https://github.com/readthedocs/sphinx_rtd_theme/blob/master/LICENSE>`__)
-- `Regex <https://github.com/mrabarnett/mrab-regex>`__ (`LICENSE <https://github.com/mrabarnett/mrab-regex/blob/hg/LICENSE.txt>`__)
 - `Aiosqlite <https://github.com/omnilib/aiosqlite>`__ (`MIT <https://github.com/omnilib/aiosqlite/blob/main/LICENSE>`__)
 - `Telethon <https://github.com/LonamiWebs/Telethon>`__ (`MIT <https://github.com/LonamiWebs/Telethon/blob/master/LICENSE>`__)
 - `Ecdsa <https://github.com/tlsfuzzer/python-ecdsa>`__ (`LICENSE <https://github.com/tlsfuzzer/python-ecdsa/blob/master/LICENSE>`__)
 - `Filetype <https://github.com/h2non/filetype.py>`__ (`MIT <https://github.com/h2non/filetype.py/blob/master/LICENSE>`__)
 - `Cryptg <https://github.com/cher-nov/cryptg>`__ (`LICENSE <https://github.com/cher-nov/cryptg/blob/master/LICENSE.txt>`__)
 - `Cryptography <https://github.com/pyca/cryptography>`__ (`LICENSE <https://github.com/pyca/cryptography/blob/main/LICENSE>`__)
```

### Comparing `tgbox-1.1.1/setup.py` & `tgbox-1.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,69 @@
 from setuptools import setup
+from ast import literal_eval
+from sys import version_info
+
+
+CURRENT_PYTHON = version_info[:2]
+REQUIRED_PYTHON = (3, 8)
+
+if CURRENT_PYTHON < REQUIRED_PYTHON:
+    raise RuntimeError('The \'tgbox\' library require Python v3.8+')
+
+
+with open('tgbox/version.py', encoding='utf-8') as f:
+    version = literal_eval(f.read().split('=',1)[1].strip())
 
 setup(
     name             = 'tgbox',
     packages         = ['tgbox', 'tgbox.api'],
-    version          = '1.1.1',
+    version          = version,
     license          = 'LGPL-2.1',
     description      = 'Encrypted cloud storage API based on a Telegram API',
     long_description = open('README.rst', encoding='utf-8').read(),
     author           = 'NonProjects',
     author_email     = 'thenonproton@pm.me',
     url              = 'https://github.com/NonProjects/tgbox',
-    download_url     = 'https://github.com/NonProjects/tgbox/archive/refs/tags/v1.1.1.tar.gz',
+    download_url     = f'https://github.com/NonProjects/tgbox/archive/refs/tags/v{version}.tar.gz',
 
     long_description_content_type='text/x-rst',
 
     package_data = {
         'tgbox': ['tgbox/other'],
     },
     include_package_data = True,
 
     install_requires = [
-        'aiosqlite==0.17.0',
-        'telethon==1.25.4',
-        'ecdsa==0.16.1',
-        'filetype==1.0.8',
+        'aiosqlite==0.18.0',
+        'telethon==1.28.2',
+        'ecdsa==0.18.0',
+        'filetype==1.2.0',
         'pysocks==1.7.1'
     ],
     keywords = [
         'Telegram', 'Cloud-Storage', 'Cloud',
         'API', 'Asyncio', 'Non-official'
     ],
     extras_require = {
         'fast': [
             'cryptography',
-            'cryptg==0.3.1',
-            'regex==2022.8.17'
+            'cryptg==0.4.0'
         ],
-        'doc': ['sphinx-rtd-theme==1.0.0']
+        'doc': [
+            'sphinx-rtd-theme==1.2.0',
+            'sphinxcontrib-jquery==4.1'
+        ]
     },
     classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Topic :: Security :: Cryptography',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: System :: Archiving :: Backup',
         'License :: OSI Approved :: GNU General Public License v2 (GPLv2)',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9'
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+
     ]
 )
```

### Comparing `tgbox-1.1.1/tgbox/api/db.py` & `tgbox-1.2/tgbox/api/db.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """This module stores wrappers around Tgbox SQL DB."""
 
+import logging
+
 from typing import (
     Optional, Union,
     AsyncGenerator
 )
 from os import PathLike
 from pathlib import Path
 
@@ -14,36 +16,39 @@
     DEF_NO_FOLDER, DEF_UNK_FOLDER,
 )
 from ..errors import PathIsDirectory
 from ..tools import anext
 
 __all__ = ['SqlTableWrapper', 'TgboxDB', 'TABLES']
 
+logger = logging.getLogger(__name__)
+
 TABLES = {
     'BOX_DATA': (
         ('BOX_CHANNEL_ID', 'BLOB NOT NULL'),
         ('BOX_CR_TIME', 'BLOB NOT NULL'),
         ('BOX_SALT', 'BLOB NOT NULL'),
         ('MAINKEY', 'BLOB'),
         ('SESSION', 'BLOB NOT NULL'),
         ('API_ID', 'BLOB NOT NULL'),
         ('API_HASH', 'BLOB NOT NULL'),
+        ('FAST_SYNC_LAST_EVENT_ID', 'BLOB')
     ),
     'FILES': (
         ('ID', 'INTEGER PRIMARY KEY'),
         ('UPLOAD_TIME', 'BLOB NOT NULL'),
         ('PPATH_HEAD', 'BLOB NOT NULL'),
         ('FILEKEY', 'BLOB'),
         ('FINGERPRINT', 'BLOB'),
         ('METADATA', 'BLOB NOT NULL'),
         ('UPDATED_METADATA', 'BLOB')
     ),
     'PATH_PARTS': (
         ('ENC_PART', 'BLOB NOT NULL'),
-        ('PART_ID', 'BLOB NOT NULL'),
+        ('PART_ID', 'BLOB NOT NULL PRIMARY KEY'),
         ('PARENT_PART_ID', 'BLOB'),
     ),
     'DEFAULTS': (                            # Default value
         ('METADATA_MAX', 'INTEGER NOT NULL', int(Limits.METADATA_MAX)),
         ('FILE_PATH_MAX', 'INTEGER NOT NULL', int(Limits.FILE_PATH_MAX)),
 
         ('DOWNLOAD_PATH', 'TEXT NOT NULL', str(DOWNLOAD_PATH)),
@@ -65,63 +70,78 @@
     @property
     def table_name(self) -> str:
         """Returns table name"""
         return self._table_name
 
     async def count_rows(self) -> int:
         """Execute ``SELECT count(*) from TABLE_NAME``"""
+
+        logger.debug(f'SELECT count(*) FROM {self._table_name}')
+
         cursor = await self._aiosql_conn.execute(
             f'SELECT count(*) FROM {self._table_name}'
         )
         return (await cursor.fetchone())[0]
 
-    # TODO: Auto add FROM <TABLE_NAME> for select
-    #       and INSERT INTO <TABLE_NAME> for insert
     async def select(self, sql_tuple: Optional[tuple] = None) -> AsyncGenerator:
         """
         If ``sql_tuple`` isn't specified, then will be used
         ``(SELECT * FROM TABLE_NAME, ())`` statement.
         """
         if not sql_tuple:
             sql_tuple = (f'SELECT * FROM {self._table_name}',())
 
+        logger.debug(f'self._aiosql_conn.execute(*{sql_tuple})')
+
         cursor = await self._aiosql_conn.execute(*sql_tuple)
         async for row in cursor: yield row
 
     async def select_once(self, sql_tuple: Optional[tuple] = None) -> tuple:
         """
         Will return first row which match the ``sql_tuple``,
         see ``select()`` method for ``sql_tuple`` details.
         """
         return await anext(self.select(sql_tuple=sql_tuple))
 
     async def insert(
             self, *args, sql_statement: Optional[str] = None,
-            commit: bool=True) -> None:
+            commit: bool=True, ignore: bool=False) -> None:
         """
         If ``sql_statement`` isn't specified, then will be used
         ``INSERT INTO TABLE_NAME values (...)``.
 
         This method doesn't check if you insert correct data
         or correct amount of it, you should know DB structure.
+
+        If ``ignore`` specified, will be used ``INSERT OR IGNORE``
+        instead of ``INSERT`` to silently ignore errors.
         """
+        insert_ = 'INSERT OR IGNORE' if ignore else 'INSERT'
+
         if not sql_statement:
             sql_statement = (
-                f'INSERT INTO {self._table_name} values ('
+                f'{insert_} INTO {self._table_name} values ('
                 + ('?,' * len(args))[:-1] + ')'
             )
+        logger.debug(f'self._aiosql_conn.execute({sql_statement}, {args})')
         await self._aiosql_conn.execute(sql_statement, args)
-        if commit: await self._aiosql_conn.commit()
+        if commit:
+            logger.debug('self._aiosql_conn.commit()')
+            await self._aiosql_conn.commit()
 
     async def execute(self, sql_tuple: tuple, commit: bool=True):
+        logger.debug(f'self._aiosql_conn.execute(*{sql_tuple})')
         result = await self._aiosql_conn.execute(*sql_tuple)
-        if commit: await self._aiosql_conn.commit()
+        if commit:
+            logger.debug('self._aiosql_conn.commit()')
+            await self._aiosql_conn.commit()
         return result # Returns Cursor object
 
     async def commit(self) -> None:
+        logger.info('SqlTableWrapper._aiosql_conn.commit()')
         await self._aiosql_conn.commit()
 
 class TgboxDB:
     def __init__(self, db_path: Union[PathLike, str]):
         """
         Arguments:
             db_path (``PathLike``, ``str``):
@@ -130,44 +150,59 @@
         if isinstance(db_path, PathLike):
             self._db_path = db_path
         else:
             self._db_path = Path(db_path)
 
         self._aiosql_db = None
         self._aiosql_db_is_closed = None
+        self._initialized = False
+
         self._name = self._db_path.name
 
         if self._db_path.is_dir():
             raise PathIsDirectory('Path is directory.')
 
     @property
     def name(self) -> str:
+        """Returns TgboxDB name"""
         return self._name
 
     @property
     def db_path(self) -> PathLike:
+        """Returns path to TgboxDB file"""
         return self._db_path
 
     @property
+    def initialized(self) -> bool:
+        """Will return True if TgboxDB is initialized"""
+        return self._initialized
+
+    @property
     def closed(self) -> bool:
         """
         This method will return ``None`` if DB wasn't opened,
         False if it's still opened, True if it's was closed.
         """
         return self._aiosql_db_is_closed
 
     @staticmethod
     async def create(db_path: Union[str, PathLike]) -> 'TgboxDB':
+        """Will initialize TgboxDB"""
         return await TgboxDB(db_path).init()
 
     async def close(self) -> None:
+        """Will close TgboxDB"""
+        logger.info(f'{self._db_path} @ self._aiosql_db.close()')
         await self._aiosql_db.close()
         self._aiosql_db_is_closed = True
 
     async def init(self) -> 'TgboxDB':
+        logger.debug(f'tgbox.api.db.TgboxDB.init("{self._db_path}")')
+
+        logger.info(f'Opening SQLite connection to {self._db_path}')
         self._aiosql_db = await aiosqlite.connect(self._db_path)
 
         for table, data in TABLES.items():
             try:
                 columns = ', '.join((f'{i[0]} {i[1]}' for i in data))
                 await self._aiosql_db.execute(
                     f'CREATE TABLE {table} ({columns})'
@@ -177,38 +212,52 @@
                         f'INSERT INTO {table} VALUES ('
                         + ('?,' * len(data))[:-1] + ')'
                     )
                     await self._aiosql_db.execute(
                         sql_statement, [i[2] for i in data]
                     )
             except aiosqlite.OperationalError: # Table exists
+                # The code below will update TgboxDB schema if it's outdated
                 table_columns = await self._aiosql_db.execute(
                     f'PRAGMA table_info({table})'
                 )
                 table_columns = set((i[1] for i in await table_columns.fetchall()))
                 required_columns = set((i[0] for i in data))
 
                 if table_columns != required_columns:
+                    logger.info(f'TgboxDB {self._db_path} seems outdated. Updating...')
                     table_columns &= required_columns
 
+                    logger.debug(f'CREATE TABLE "updated!{table}" ({columns})')
+
                     await self._aiosql_db.execute(
                         f'CREATE TABLE "updated!{table}" ({columns})'
                     )
                     table_columns_str = ', '.join(table_columns)
+
+                    logger.debug(
+                        f"""INSERT INTO "updated!{table}" ({table_columns_str}) """
+                        f"""SELECT {table_columns_str} FROM {table}"""
+                    )
                     await self._aiosql_db.execute(
                         f"""INSERT INTO "updated!{table}" ({table_columns_str}) """
                         f"""SELECT {table_columns_str} FROM {table}"""
                     )
+                    logger.debug(f'DROP TABLE {table}')
                     await self._aiosql_db.execute(f'DROP TABLE {table}')
+
+                    logger.debug(f'ALTER TABLE "updated!{table}" RENAME TO {table}')
                     await self._aiosql_db.execute(
                         f'ALTER TABLE "updated!{table}" RENAME TO {table}'
                     )
+        logger.info('TgboxDB._aiosql_conn.commit()')
         await self._aiosql_db.commit()
         self._aiosql_db_is_closed = False
 
         tables = await self._aiosql_db.execute(
             "SELECT name FROM sqlite_master WHERE type='table'"
         )
         for table in (await tables.fetchall()):
             setattr(self, table[0], SqlTableWrapper(self._aiosql_db, table[0]))
 
+        self._initialized = True
         return self
```

### Comparing `tgbox-1.1.1/tgbox/api/remote.py` & `tgbox-1.2/tgbox/api/remote.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,89 @@
 """Module with API functions and classes for RemoteBox."""
 
+import logging
+
 from typing import (
     BinaryIO, Union, NoReturn, Callable,
     AsyncGenerator, List, Dict, Optional
 )
 from pathlib import Path
+from asyncio import gather, sleep
 
 from os import PathLike
+from traceback import format_exc
 
 from base64 import (
     urlsafe_b64encode,
     urlsafe_b64decode
 )
 from asyncio import iscoroutinefunction
 
+from telethon.utils import resolve_id
 from telethon.tl.custom.file import File
-from telethon.tl.functions.messages import EditChatAboutRequest
 
+from telethon.tl.functions.messages import (
+    EditChatAboutRequest, SearchRequest
+)
 from telethon.errors import (
     ChatAdminRequiredError,
     MediaCaptionTooLongError,
+    MessageNotModifiedError,
     AuthKeyUnregisteredError,
     FilePartsInvalidError
 )
 from telethon.tl.functions.channels import (
     CreateChannelRequest, EditPhotoRequest,
     GetFullChannelRequest, DeleteChannelRequest
 )
 from telethon.tl.types import (
-    Channel, Message, PeerChannel
+    Channel, Message, PeerChannel,
+    InputMessagesFilterDocument
 )
-from telethon import events
-
 from ..crypto import get_rnd_bytes
 from ..crypto import AESwState as AES
 
 from ..keys import (
     make_mainkey, make_sharekey, MainKey,
     ShareKey, ImportKey, FileKey, BaseKey,
     make_filekey, make_requestkey, RequestKey
 )
 from ..defaults import (
-    Limits, PREFIX, DEF_UNK_FOLDER,
     VERBYTE, BOX_IMAGE_PATH, DEF_TGBOX_NAME,
+    Limits, PREFIX, DEF_UNK_FOLDER, UploadLimits,
     REMOTEBOX_PREFIX, DEF_NO_FOLDER, DOWNLOAD_PATH
 )
 from ..fastelethon import upload_file, download_file
 
 from ..errors import (
     NotEnoughRights, NotATgboxFile, IncorrectKey,
     NotInitializedError, RemoteBoxInaccessible,
     LimitExceeded, NotImported, AESError, RemoteFileNotFound,
     NoPlaceLeftForMetadata, SessionUnregistered
 )
 from ..tools import (
     int_to_bytes, bytes_to_int, SearchFilter, OpenPretender,
-    pad_request_size, PackedAttributes, prbg, anext
+    pad_request_size, PackedAttributes, prbg, anext,
+    make_safe_file_path
 )
 from .utils import (
-    TelegramClient, RemoteBoxDefaults,
-    DefaultsTableWrapper, search_generator
+    TelegramClient, TelegramVirtualFile,
+    RemoteBoxDefaults, DefaultsTableWrapper,
+    search_generator
 )
 __all__ = [
     'make_remotebox',
     'get_remotebox',
     'EncryptedRemoteBox',
     'DecryptedRemoteBox',
     'EncryptedRemoteBoxFile',
     'DecryptedRemoteBoxFile',
 ]
+logger = logging.getLogger(__name__)
+
 async def make_remotebox(
         tc: TelegramClient,
         box_name: Optional[str] = DEF_TGBOX_NAME,
         rb_prefix: Optional[str] = REMOTEBOX_PREFIX,
         box_image: Optional[Union[PathLike, str]] = BOX_IMAGE_PATH,
         box_salt: Optional[bytes] = None) -> 'EncryptedRemoteBox':
     """
@@ -104,24 +115,28 @@
     """
     if box_salt and len(box_salt) != 32:
         raise ValueError('BoxSalt bytelength != 32')
 
     box_salt = urlsafe_b64encode(
         box_salt if box_salt else get_rnd_bytes()
     )
+    box_salt = box_salt.decode()
+
     channel_name = rb_prefix + box_name
 
+    logger.info(f'Making RemoteBox {channel_name} ({box_salt[:12]}...)')
+
     channel = (await tc(CreateChannelRequest(
         channel_name, '', megagroup=False))).chats[0]
 
     if box_image:
         box_image = await tc.upload_file(open(box_image,'rb'))
         await tc(EditPhotoRequest(channel, box_image))
 
-    await tc(EditChatAboutRequest(channel, box_salt.decode()))
+    await tc(EditChatAboutRequest(channel, box_salt))
     return EncryptedRemoteBox(channel, tc)
 
 async def get_remotebox(
         dlb: Optional['DecryptedLocalBox'] = None,
         tc: Optional['TelegramClient'] = None,
         entity: Optional[Union[int, str, PeerChannel]] = None,
         proxy: Optional[Union[tuple, list, dict]] = None)\
@@ -151,41 +166,52 @@
         proxy (tuple, list, dict, optional):
             An iterable consisting of the proxy info. If connection
             is one of MTProxy, then it should contain MTProxy credentials:
             ('hostname', port, 'secret'). Otherwise, it’s meant to store
             function parameters for PySocks, like (type, 'hostname', port).
             See https://github.com/Anorov/PySocks#usage-1 for more info.
     """
-    if tc: account = tc
+    if tc:
+        account = tc
 
     elif tc and not entity:
         raise ValueError('entity must be specified with tc')
     else:
         account = TelegramClient(
             session=dlb._session,
             api_id=dlb._api_id,
             api_hash=dlb._api_hash,
             proxy=proxy
         )
         await account.connect()
+
+    if dlb:
+        logger.info(
+            f'''Getting RemoteBox ID{dlb._box_channel_id} '''
+            f'''with the {dlb._tgbox_db._db_path} LocalBox'''
+        )
+    else:
+        logger.info(f'Getting RemoteBox ({entity}) with TelegramClient')
     try:
         entity = entity if entity else PeerChannel(dlb._box_channel_id)
         channel_entity = await account.get_entity(entity)
     except AuthKeyUnregisteredError:
         raise SessionUnregistered(
             '''Session was disconnected. Change it with '''
             '''DecryptedLocalBox.replace_session method.'''
         ) from None
     except ValueError:
         # ValueError: Could not find the input entity for PeerChannel
         raise RemoteBoxInaccessible(RemoteBoxInaccessible.__doc__) from None
 
     if not dlb:
+        logger.debug('DLB is NOT specified, return EncryptedRemoteBox')
         return EncryptedRemoteBox(channel_entity, account)
     else:
+        logger.debug('DLB is specified, return DecryptedRemoteBox')
         return await EncryptedRemoteBox(
             channel_entity, account).decrypt(dlb=dlb)
 
 class EncryptedRemoteBox:
     """
     *RemoteBox* is a remote cloud storage. You can
     upload files and download them later.
@@ -211,15 +237,15 @@
         from asyncio import run as asyncio_run
 
         PHONE_NUMBER = '+10000000000' # Your phone number
         API_ID = 1234567 # Your own API_ID: my.telegram.org
         API_HASH = '00000000000000000000000000000000' # Your own API_HASH
 
         async def main():
-            # Connecting and logging to Telegram
+            # Connect and sign-in to Telegram
             tc = TelegramClient(
                 phone_number = PHONE_NUMBER,
                 api_id = API_ID,
                 api_hash = API_HASH
             )
             await tc.connect()
             await tc.send_code()
@@ -252,25 +278,28 @@
 
             defaults (``DefaultsTableWrapper``, ``RemoteBoxDefaults``):
                 Class with a default values/constants we will use.
         """
         self._tc = tc
 
         self._box_channel = box_channel
-        self._box_channel_id = box_channel.id
+        self._box_channel_id = resolve_id(box_channel.id)[0]
 
         self._box_salt = None
         # We can't use await in __init__, so
         # you should await get_box_salt firstly.
         self._box_name = None
         # Similar to box_salt, await get_box_name.
 
         if defaults:
+            logger.debug('ERB: Found custom defaults, will try to use it')
             self._defaults = defaults
         else:
+            logger.debug('ERB: Custom defaults is not present')
+
             self._defaults = RemoteBoxDefaults(
                 METADATA_MAX = Limits.METADATA_MAX,
                 FILE_PATH_MAX = Limits.FILE_PATH_MAX,
                 DEF_UNK_FOLDER = DEF_UNK_FOLDER,
                 DEF_NO_FOLDER = DEF_NO_FOLDER,
                 DOWNLOAD_PATH = DOWNLOAD_PATH
             )
@@ -281,25 +310,14 @@
 
     def __eq__(self, other) -> bool:
         return all((
             isinstance(other, self.__class__),
             self._box_channel_id == other.box_channel_id
         ))
     @property
-    def event(self) -> events.NewMessage:
-        """
-        Will return ``events.NewMessage`` for
-        ``Channel`` of this *RemoteBox*.
-
-        You can use it in Telethon's decorator,
-        see *"Events Reference"* in Telethon Docs.
-        """
-        return events.NewMessage(chats=self.box_channel_id)
-
-    @property
     def defaults(self) -> Union[DefaultsTableWrapper, RemoteBoxDefaults]:
         """
         Will return ``DefaultsTableWrapper`` if
         ``dlb`` was specified or ``RemoteBoxDefaults``
         with arguments from the ``defaults`` module if wasn't.
         """
         return self._defaults
@@ -324,14 +342,34 @@
         async for msg in self._tc.iter_messages(self._box_channel):
             if not msg:
                 continue
             if msg.document:
                 return msg.id
         return 0
 
+    async def get_files_total(self) -> int:
+        """Returns a total number of files in this *RemoteBox"""
+
+        search = await self._tc(SearchRequest(
+            peer = self._box_channel,
+            filter = InputMessagesFilterDocument(),
+
+            q = '',
+            min_date = None,
+            max_date = None,
+
+            offset_id = 0,
+            add_offset = 0,
+            limit = 0,
+            max_id = 0,
+            min_id = 0,
+            hash = 0
+        ))
+        return search.count
+
     async def get_box_salt(self) -> bytes:
         """
         Returns BoxSalt. Will be cached
         after first method call.
         """
         if not self._box_salt:
             full_rq = await self._tc(GetFullChannelRequest(channel=self._box_channel))
@@ -341,15 +379,15 @@
 
     async def get_box_name(self):
         """
         Returns name of ``RemoteBox``.
         Will be cached after first method call.
         """
         if not self._box_name:
-            entity = await self._tc.get_entity(self._box_channel_id)
+            entity = await self._tc.get_entity(self._box_channel)
             self._box_name = entity.title.split(': ')[1]
         return self._box_name
 
     async def file_exists(self, id: int) -> bool:
         """
         Returns ``True`` if file with specified ``id``
         exists in RemoteBox. ``False`` otherwise.
@@ -418,18 +456,22 @@
                 If specified, returns file that method can't
                 decrypt (if imported) as ``EncryptedRemoteBoxFile``.
 
             cache_preview (``bool``, optional):
                 Cache preview in returned by method
                 RemoteBoxFiles or not. ``True`` by default.
         """
+        logger.info(f'Getting file ID{id} from the RemoteBox ID{self._box_channel_id}')
+
         if hasattr(self, '_mainkey') and not key:
+            logger.debug('self have _mainkey, will try to return DecryptedRemoteBoxFile')
             key = self._mainkey # pylint: disable=no-member
 
         if hasattr(self, '_dlb'):
+            logger.debug('self have _dlb, will try to return DecryptedRemoteBoxFile')
             dlb = self._dlb # pylint: disable=no-member
 
         file_iter = self.files(
             key, dlb=dlb, decrypt=decrypt,
             ids=id, cache_preview=cache_preview,
             return_imported_as_erbf=return_imported_as_erbf,
             ignore_errors=ignore_errors
@@ -438,25 +480,30 @@
             return await anext(file_iter)
         # If there is no file by ``id``.
         except StopAsyncIteration:
             return None
 
     async def files(
             self, key: Optional[Union[MainKey, FileKey]] = None,
-            dlb: Optional['DecryptedLocalBox'] = None, *,
+            dlb: Optional['DecryptedLocalBox'] = None,
+            *,
             ignore_errors: bool=True,
             return_imported_as_erbf: bool=False,
             limit: Optional[int] = None,
-            offset_id: int=0, max_id: int=0,
-            min_id: int=0, add_offset: int=0,
+            offset_id: int=0,
+            max_id: int=0,
+            min_id: int=0,
+            add_offset: int=0,
             search: Optional[str] = None,
             from_user: Optional[Union[str, int]] = None,
             wait_time: Optional[float] = None,
             ids: Optional[Union[int, List[int]]] = None,
-            reverse: bool=False, decrypt: bool=True,
+            reverse: bool=False,
+            decrypt: bool=True,
+            timeout: int=15,
             cache_preview: bool=True,
             erase_encrypted_metadata: bool=True) -> AsyncGenerator[
                 Union['EncryptedRemoteBoxFile',
                       'DecryptedRemoteBoxFile'],
                 None
             ]:
         """
@@ -547,111 +594,201 @@
                 If set to ``True``, the remote files will be returned in reverse
                 order (from oldest to newest, instead of the default newest
                 to oldest). This also means that the meaning of ``offset_id``
                 parameter is reversed, although ``offset_id`` still be exclusive.
                 ``min_id`` becomes equivalent to ``offset_id`` instead of being ``max_id``
                 as well since files are returned in ascending order.
 
+            timeout (``int``, optional):
+                How many seconds generator will sleep at every 1000 file.
+                By default it's 15 seconds. Don't use too low timeouts,
+                you will receive FloodWaitError otherwise (TGBOX).
+
             decrypt (``bool``, optional):
                 Returns ``DecryptedRemoteBoxFile`` if ``True`` (default),
                 ``EncryptedRemoteBoxFile`` otherwise.
 
             cache_preview (``bool``, optional):
                 Cache preview in yielded by generator
                 RemoteBoxFiles or not. ``True`` by default.
 
             erase_encrypted_metadata (``bool``, optional):
                 Will remove metadata from the parent
                 ``EncryptedRemoteBoxFile`` after decryption
                 to save more RAM if ``True``. You can call
                 ``.init()`` method on it to load it again.
         """
+        logger.info(f'*RemoteBox.files generator started, ids={ids}')
+
+        if key:
+            logger.debug('Custom key specified, will try to use it to decrypt files')
+
         if hasattr(self, '_mainkey') and not key:
+            logger.debug('self have _mainkey, will try to yield DecryptedRemoteBoxFile')
             key = self._mainkey # pylint: disable=no-member
 
         if hasattr(self, '_dlb'):
+            logger.debug('self have _dlb, will try to yield DecryptedRemoteBoxFile')
             dlb = self._dlb # pylint: disable=no-member
 
         if decrypt and not any((key, dlb)):
             raise ValueError(
                 'You need to specify key or dlb to be able to decrypt.'
             )
         key = key if (key or not dlb) else dlb._mainkey
 
         it_messages = self._tc.iter_messages(
             self._box_channel, limit=limit, offset_id=offset_id,
             max_id=max_id, min_id=min_id, add_offset=add_offset,
             search=search, from_user=from_user, wait_time=wait_time,
             ids=ids, reverse=reverse
         )
-        async for m in it_messages:
-            if not m and ignore_errors:
-                continue
-
-            elif not m and not ignore_errors:
-                raise RemoteFileNotFound('One of requsted by you file doesn\'t exist')
-
-            if m.document:
-                if not decrypt:
-                    rbf = await EncryptedRemoteBoxFile(
+        async def rbf_wrapper(m):
+            if not m or not m.document:
+                return
+
+            if not decrypt:
+                logger.debug(
+                    '''Decryption is disabled, will try to '''
+                    '''yield EncryptedRemoteBoxFile''')
+                try:
+                    return await EncryptedRemoteBoxFile(
                         m, self._tc, cache_preview=cache_preview,
                         defaults=self._defaults).init()
-                else:
+
+                except NotATgboxFile:
+                    logger.debug(
+                       f'''Document: {m.file.name[:12]}...(ID{m.id}) '''
+                        '''is not a TGBOX file, skipping.'''
+                    )
+                    return
+
+            logger.debug(
+                '''Decryption is enabled, will try to '''
+                '''yield DecryptedRemoteBoxFile''')
+            try:
+                return await EncryptedRemoteBoxFile(
+                    m, self._tc, cache_preview=cache_preview,
+                    defaults=self._defaults).decrypt(
+                        key, erase_encrypted_metadata)
+
+            except Exception as e: # In case of imported file
+                logger.debug(
+                    '''Failed to decrypt EncryptedRemoteBoxFile '''
+                   f'''(ID{m.id}), it seems that file is imported/'''
+                   f'''non-TGBOX [{e}]'''
+                )
+                if return_imported_as_erbf and not dlb:
+                    logger.debug(
+                        '''return_imported_as_erbf is True & DLB '''
+                        '''is not specified, so will return ERBF''')
                     try:
-                        rbf = await EncryptedRemoteBoxFile(
+                        return await EncryptedRemoteBoxFile(
                             m, self._tc, cache_preview=cache_preview,
-                            defaults=self._defaults).decrypt(
-                                key, erase_encrypted_metadata)
+                            defaults=self._defaults).init()
 
-                    except Exception as e: # In case of imported file
-                        if return_imported_as_erbf and not dlb:
-                            rbf = await EncryptedRemoteBoxFile(
-                                m, self._tc, cache_preview=cache_preview,
-                                defaults=self._defaults).init()
-
-                        elif ignore_errors and not dlb:
-                            continue
-
-                        elif not ignore_errors and not dlb:
-                            raise IncorrectKey(
-                                'File is imported. Specify dlb?') from None
-                        elif dlb:
-                            # We try to fetch FileKey of imported file from DLB.
-                            dlb_file = await dlb.get_file(m.id, cache_preview=False)
-
-                            # If we haven't imported this file to DLB
-                            if not dlb_file:
-                                if return_imported_as_erbf:
-                                    rbf = await EncryptedRemoteBoxFile(
-                                        m, self._tc, cache_preview=cache_preview,
-                                        defaults=self._defaults).init()
-
-                                elif ignore_errors:
-                                    continue
-                                else:
-                                    raise NotImported(
-                                        """You don\'t have FileKey for this file. """
-                                        """Set to True ``return_imported_as_erbf``?"""
-                                    ) from None
-                            else:
-                                # We already imported file, so have FileKey
-                                rbf = await EncryptedRemoteBoxFile(
+                    except NotATgboxFile:
+                        logger.debug(
+                           f'''Document: {m.file.name[:12]}...(ID{m.id}) '''
+                            '''is not a TGBOX file, skipping.'''
+                        )
+                        return
+
+                elif ignore_errors and not dlb:
+                    logger.debug(
+                        '''return_imported_as_erbf is False & DLB '''
+                        '''is not specified, ignore_errors is True '''
+                        '''so we will continue iteration for other.'''
+                    )
+                    return
+
+                elif not ignore_errors and not dlb:
+                    raise IncorrectKey(
+                        'File is imported. Try to specify dlb?') from None
+
+                elif dlb:
+                    logger.debug('DLB is specified, will try to fetch FileKey from it.')
+                    # We try to fetch FileKey of imported file from DLB.
+                    dlb_file = await dlb.get_file(m.id, cache_preview=False)
+
+                    # If we haven't imported this file to DLB
+                    if not dlb_file:
+                        if return_imported_as_erbf:
+                            try:
+                                logger.debug(
+                                   f'''DLB is specified, but FileKey to {m.id} is not '''
+                                    '''present in it. return_imported_as_erbf is True, '''
+                                    '''so we will return ERBF.'''
+                                )
+                                return await EncryptedRemoteBoxFile(
                                     m, self._tc, cache_preview=cache_preview,
-                                    defaults=self._defaults).decrypt(dlb_file._filekey)
+                                    defaults=self._defaults).init()
+
+                            except NotATgboxFile:
+                                logger.debug(
+                                   f'''Document: {m.file.name[:12]}...(ID{m.id}) '''
+                                    '''is not a TGBOX file, skipping.'''
+                                )
+                                return
+
+                        elif ignore_errors:
+                            logger.debug(
+                               f'''DLB is specified, but FileKey to ID{m.id} is not '''
+                                '''present in it. return_imported_as_erbf is False, '''
+                                '''so we will skip it and continue iteration.'''
+                            )
+                            return
                         else:
-                            raise e # Unknown Exception
-                yield rbf
+                            raise NotImported(
+                                """You don\'t have FileKey for this file. """
+                                """Set to True ``return_imported_as_erbf``?"""
+                            ) from None
+                    else:
+                        # We already imported file, so DLB contains a FileKey
+                        return await EncryptedRemoteBoxFile(
+                            m, self._tc, cache_preview=cache_preview,
+                            defaults=self._defaults).decrypt(dlb_file._filekey)
+
+        processed_messages = 0
+        while True:
+            # Sleep `timeout` seconds every 1000 files
+            if processed_messages and processed_messages % 1000 == 0:
+                logger.debug(f'Sleep {timeout=} seconds...')
+                await sleep(timeout)
+
+            logger.debug('Receiving the new chunk of messages...')
+
+            messages_chunk = []
+            for _ in range(100):
+                try:
+                    messages_chunk.append(rbf_wrapper(await anext(it_messages)))
+                except StopAsyncIteration:
+                    break
+
+            processed_messages += len(messages_chunk)
+            logger.debug(f'Chunk length = {len(messages_chunk)}')
+
+            if not messages_chunk:
+                break
+
+            for drbf in (drbfiles := await gather(*messages_chunk)):
+                if drbf: yield drbf
 
     async def search_file(
             self,
             sf: SearchFilter,
             mainkey: Optional[MainKey] = None,
             dlb: Optional['DecryptedLocalBox'] = None,
-            cache_preview: bool=True) ->\
-            AsyncGenerator[Union['EncryptedRemoteBoxFile', 'DecryptedRemoteBoxFile'], None]:
+            cache_preview: bool=True,
+            return_imported_as_erbf: bool=False,
+            reverse: bool=True) -> AsyncGenerator[
+                Union[
+                    'EncryptedRemoteBoxFile',
+                    'DecryptedRemoteBoxFile'
+                ], None]:
         """
         This method used to search for files in your ``RemoteBox``.
 
         Arguments:
             sf (``SearchFilter``):
                 ``SearchFilter`` with kwargs you like.
 
@@ -661,20 +798,31 @@
             dlb (``DecryptedLocalBox``, optional):
                 LocalBox associated with this ``RemoteBox``. We
                 will take ``MainKey`` from it.
 
             cache_preview (``bytes``, optional):
                 Will cache preview in file object if ``True``.
 
+            return_imported_as_erbf (``bool``, optional):
+                If specified, will yield files that generator can't
+                decrypt (imported) as ``EncryptedRemoteBoxFile``.
+
+            reverse (``bool``, optional):
+                If set to ``True`` (by default), the remote files
+                will be returned in reverse order (from oldest to
+                newest, instead of the default newest to oldest).
+
         .. note::
             - If ``dlb`` and ``mainkey`` not specified, then method\
-            will search on ``EncryptedRemoteBoxFile``.
+            will search only for ``EncryptedRemoteBoxFile``.
             - You may ignore this kwargs if you call this\
             method on ``DecryptedRemoteBox`` class.
         """
+        logger.info(f'Searching for files with {sf}')
+
         if hasattr(self, '_mainkey'):
             mainkey = self._mainkey
 
         if hasattr(self, '_dlb'):
             dlb = self._dlb
 
         min_id = sf.in_filters['min_id'][-1] if sf.in_filters['min_id'] else 0
@@ -683,16 +831,17 @@
 
         it_messages = self.files(
             key=mainkey,
             dlb=dlb,
             ids=ids,
             min_id=min_id,
             max_id=max_id,
-            reverse=True,
-            cache_preview=cache_preview
+            reverse=reverse,
+            cache_preview=cache_preview,
+            return_imported_as_erbf = return_imported_as_erbf
         )
         sgen = search_generator(
             sf, lb=dlb,
             it_messages=it_messages,
             cache_preview=cache_preview
         )
         async for file in sgen:
@@ -710,52 +859,143 @@
                 PreparedFile to upload. You should recieve
                 it via ``DecryptedLocalBox.prepare_file``.
 
             progress_callback (``Callable[[int, int], None]``, optional):
                 A callback function accepting two parameters:
                 (downloaded_bytes, total).
         """
+        logger.info(f'Pushing {pf.file} to RemoteBox ID{pf.dlb._box_channel_id}...')
+
+        me = await self._tc.get_me()
+
+        if me.premium and pf.filesize > UploadLimits.PREMIUM:
+            raise LimitExceeded(
+                f'''Max allowed filesize for you is {UploadLimits.PREMIUM} '''
+                f'''bytes, your file is {pf.filesize} bytes in size.'''
+            )
+        if not me.premium and pf.filesize > UploadLimits.DEFAULT:
+            raise LimitExceeded(
+                f'''Max allowed filesize for you is {UploadLimits.DEFAULT} '''
+                f'''bytes, your file is {pf.filesize} bytes in size.'''
+            )
         # Last 16 bytes of metadata is IV
         aes_state = AES(pf.filekey, pf.metadata[-16:])
 
         oe = OpenPretender(pf.file, aes_state, pf.filesize)
         oe.concat_metadata(pf.metadata)
         try:
-            ifile = await upload_file(
-                self._tc, oe,
-                file_name=urlsafe_b64encode(pf.filesalt).decode(),
+            # Here we will use fast upload function
+            try:
+                ifile = await upload_file(
+                    self._tc, oe,
+                    file_name=urlsafe_b64encode(pf.filesalt).decode(),
+                    part_size_kb=512, file_size=pf.filesize,
+                    progress_callback=progress_callback
+                )
+            except FilePartsInvalidError:
+                raise LimitExceeded('Your file is too big to upload')
+
+        except Exception as e:
+            # If some error was found during uploading then it's
+            # probably because of fast "upload_file(...)" from
+            # the custom fastelethon module. We will try to
+            # use the slow upload from the Telethon library
+            logger.warning(f'Fast upload FAILED, falling to SLOW!\n{format_exc()}')
+
+            ifile = await self._tc.upload_file(
+                oe, file_name=urlsafe_b64encode(pf.filesalt).decode(),
                 part_size_kb=512, file_size=pf.filesize,
                 progress_callback=progress_callback
             )
-        except FilePartsInvalidError:
-            raise LimitExceeded('Your file is too big to upload')
         try:
             file_message = await self._tc.send_file(
                 self._box_channel, file=ifile,
-                silent=False, force_document=True
+                silent=False, force_document=True,
+                caption = '<This caption must be removed>'
             )
         except ChatAdminRequiredError:
             box_name = await self.get_box_name()
             raise NotEnoughRights(
                 '''You don\'t have enough privileges to upload '''
                f'''files to remote {box_name}. Ask for it or '''
                 '''use this box as read only.'''
             ) from None
 
+        # We will set and remove caption only for
+        # "Recent Actions" admin log. We can make
+        # a quick synchronization with its help.
+        await self._tc.edit_message(
+            entity = self._box_channel,
+            message = file_message, text = ''
+        )
         pf.set_file_id(file_message.id)
         pf.set_upload_time(int(file_message.date.timestamp()))
 
         await pf.dlb._make_local_file(pf)
 
         erbf = await EncryptedRemoteBoxFile(
             file_message, self._tc,
             defaults=self._defaults).init()
 
         return await erbf.decrypt(pf.dlb._mainkey)
 
+    async def delete_files(
+            self,
+
+            *rbf: Union[
+                'EncryptedRemoteBoxFile',
+                'DecryptedRemoteBoxFile'
+            ],
+            rbf_ids: Optional[list] = None,
+
+            lb: Optional[
+                Union[
+                    'tgbox.api.local.EncryptedLocalBox',
+                    'tgbox.api.local.DecryptedLocalBox'
+                ]
+            ] = None) -> None:
+        """
+        A function to remove a bunch of remote files
+        at once. You need to have some admin rights.
+
+        Arguments:
+            rbf (``EncryptedRemoteBoxFile``, ``DecryptedRemoteBoxFile``, asterisk):
+                ``(Encrypted|Decrypted)RemoteBoxFile(s)`` to remove.
+
+            rbf_ids (``list``, optional):
+                You can specify ids instead of RemoteBox file
+                objects. However, ``rbf`` is preferred here.
+
+            lb (``EncryptedLocalBox``, ``DecryptedLocalBox``, optional):
+                You can specify a *LocalBox* associated
+                with current *RemoteBox* to also remove
+                all specified files in *LocalBox* too.
+
+        .. note::
+            If you want to delete files only from
+            your LocalBox then you can use the
+            same method on your LocalBoxFile.
+        """
+        rbf_ids = rbf_ids if rbf_ids else []
+        rbf_ids.extend(rbf_.id for rbf_ in rbf)
+
+        logger.info(f'Removing {len(rbf_ids)} remote files...')
+
+        rm_result = await self._tc.delete_messages(
+            entity = self._box_channel,
+            message_ids = rbf_ids
+        )
+        if not rm_result[0].pts_count:
+            raise NotEnoughRights(
+                '''You don\'t have enough rights to delete '''
+                '''files from this RemoteBox.'''
+            )
+        if lb:
+            await lb.delete_files(lbf_ids=rbf_ids)
+
     async def get_requestkey(self, basekey: BaseKey) -> RequestKey:
         """
         Returns ``RequestKey`` for this *RemoteBox*.
         You should use this method if you want
         to decrypt other's ``RemoteBox``.
 
         Arguments:
@@ -878,29 +1118,38 @@
 
         self._box_salt = erb._box_salt
         self._box_name = erb._box_name
 
         self._dlb = dlb
 
         if self._dlb:
+            logger.debug('DecryptedRemoteBox is decrypted with the DLB')
             self._mainkey = self._dlb._mainkey
             self._defaults = self._dlb._defaults
         else:
             if not key:
                 raise ValueError('Must be specified at least key or dlb')
 
             if isinstance(key, (MainKey, ImportKey)):
+                logger.debug('DecryptedRemoteBox is decrypted with the MainKey')
                 self._mainkey = MainKey(key.key)
             elif isinstance(key, BaseKey):
+                logger.debug('DecryptedRemoteBox is decrypted with the BaseKey->MainKey')
                 self._mainkey = make_mainkey(key, self._box_salt)
             else:
                 raise IncorrectKey('key is not Union[MainKey, ImportKey, BaseKey]')
 
             self._defaults = erb._defaults
 
+    @staticmethod
+    async def decrypt() -> NoReturn:
+        raise AttributeError(
+            """This function was inherited from ``EncryptedRemoteBox`` """
+            """and cannot be used on ``DecryptedRemoteBox``."""
+        )
     async def get_sharekey(self, reqkey: Optional[RequestKey] = None) -> ShareKey:
         """
         Returns ``ShareKey`` for this Box.
         You should use this method if you want
         to share your ``RemoteBox`` with other people.
 
         Arguments:
@@ -985,14 +1234,15 @@
 
         self._sender = sended_file.post_author
 
         self._tc = tc
         self._cache_preview = cache_preview
 
         self._upload_time = int(self._message.date.timestamp())
+        self._box_channel = sended_file.chat
         self._box_channel_id = sended_file.peer_id.channel_id
         self._file_size = self._file.size
         self._file_file_name = self._file.name
 
         self._file_iv = None
         self._file_salt = None
         self._box_salt = None
@@ -1002,22 +1252,25 @@
 
         if self._message.fwd_from:
             self._imported = True
         else:
             self._imported = False
 
         if defaults is None:
+            logger.debug('ERBF: Custom defaults is not present')
+
             self._defaults = RemoteBoxDefaults(
                 METADATA_MAX = Limits.METADATA_MAX,
                 FILE_PATH_MAX = Limits.FILE_PATH_MAX,
                 DEF_UNK_FOLDER = DEF_UNK_FOLDER,
                 DEF_NO_FOLDER = DEF_NO_FOLDER,
                 DOWNLOAD_PATH = DOWNLOAD_PATH,
             )
         else:
+            logger.debug('ERBF: Found custom defaults, will try to use it')
             self._defaults = defaults
 
     def __hash__(self) -> int:
         if not self.initialized:
             raise NotInitializedError(
                 'Must be initialized before hashing'
             )
@@ -1103,29 +1356,39 @@
 
     @property
     def file(self) -> File:
         """Returns Telethon's ``File`` object."""
         return self._file
 
     @property
+    def message(self) -> Message:
+        """Returns Telethon's ``Message`` object."""
+        return self._message
+
+    @property
     def file_size(self) -> int:
         """Returns size of the ``File`` from ``Message`` object."""
         return self._file_size
 
     @property
     def file_file_name(self) -> bytes:
         """Returns *remote file* name."""
         return self._file_file_name
 
     @property
     def box_channel_id(self) -> int:
-        """Returns ID of the Box Channel."""
+        """Returns ID of the RemoteBox ``Channel``."""
         return self._box_channel_id
 
     @property
+    def box_channel(self) -> Channel:
+        """Returns RemoteBox ``Channel`` object."""
+        return self._box_channel
+
+    @property
     def prefix(self) -> Union[bytes, None]:
         """Returns file prefix or ``None`` if not initialized"""
         return self._prefix
 
     def __raise_initialized(self) -> NoReturn:
         if not self.initialized:
             raise NotInitializedError('RemoteBoxFile must be initialized.')
@@ -1139,21 +1402,25 @@
 
         Arguments:
             verify_prefix (``bool``, optional):
                 If ``True``, will check that file has a
                 ``defaults.PREFIX`` in metadata, and if
                 not, will raise a ``NotATgboxFile`` exception.
         """
+        logger.info(f'Initializing EncryptedRemoteBoxFile (ID{self._id})...')
+
         if isinstance(self._defaults, DefaultsTableWrapper):
             if not self._defaults.initialized:
                 await self._defaults.init()
 
         # 3 is amount of bytes to which we pack metadata length
         request_amount = len(PREFIX) + len(VERBYTE) + 3
 
+        logger.debug(f'base_data request_amount is {request_amount} bytes')
+
         async for base_data in self._tc.iter_download(
             self._message.document, request_size=pad_request_size(request_amount)):
                 base_data = base_data[:request_amount]
 
                 self._prefix = bytes(base_data[:len(PREFIX)])
                 self._version_byte = bytes(base_data[len(PREFIX):len(PREFIX)+1])
 
@@ -1172,30 +1439,40 @@
                 # in the total metadata bytesize.
                 metadata_size += 16
                 break
 
         if metadata_size > self._defaults.METADATA_MAX:
             raise LimitExceeded(f'{metadata_size=} > {self._defaults.METADATA_MAX=}')
 
+        logger.debug(f'metadata_size is {metadata_size} bytes')
+
+        if metadata_size <= 1048576:
+            metadata_size_padded = pad_request_size(metadata_size)
+        else:
+            metadata_size_padded = metadata_size
+
+        logger.debug(f'metadata_size_padded is {metadata_size_padded} bytes')
+
         iter_down = self._tc.iter_download(
             file = self._message.document,
             offset = request_amount,
-            request_size = pad_request_size(metadata_size)
+            request_size = metadata_size_padded
         )
         async for metadata in iter_down:
             m = self._prefix + self._version_byte
             m += int_to_bytes(metadata_size,3)
             self._metadata = m + bytes(metadata[:metadata_size])
             break
 
         parsedm = PackedAttributes.unpack(self._metadata[len(m):-16])
 
         if 'file_fingerprint' in parsedm:
             self._fingerprint = parsedm['file_fingerprint']
         else:
+            # For backward compatibility only
             self._fingerprint = b''
 
         self._file_salt = parsedm['file_salt']
         self._box_salt = parsedm['box_salt']
         self._file_iv = self._metadata[-16:]
 
         self._initialized = True
@@ -1209,16 +1486,18 @@
         undone. You need to have rights for this action.
 
         .. note::
             If you want to delete file only from
             your LocalBox then you can use the
             same ``delete()`` method on your LocalBoxFile.
         """
+        logger.debug(f'Removing file ID{self._id} from ID{self._box_channel_id}')
+
         rm_result = await self._tc.delete_messages(
-            self._box_channel_id, [self._id]
+            self._box_channel, [self._id]
         )
         if not rm_result[0].pts_count:
             raise NotEnoughRights(
                 '''You don\'t have enough rights to delete '''
                 '''file from this RemoteBox.'''
             )
     def get_requestkey(self, mainkey: MainKey) -> RequestKey:
@@ -1252,14 +1531,15 @@
                 Will remove metadata from the parent
                 ``EncryptedRemoteBoxFile`` after decryption
                 to save more RAM if ``True``. You can call
                 ``.init()`` method on it to load it again.
         """
         if not self.initialized:
             await self.init()
+
         return await DecryptedRemoteBoxFile(self, key).init(
             erase_encrypted_metadata=erase_encrypted_metadata)
 
 class DecryptedRemoteBoxFile(EncryptedRemoteBoxFile):
     """
     This class represents decrypted remote file.
     You can retrieve all metadata info from properties.
@@ -1321,16 +1601,18 @@
         self._file = erbf._file
         self._sender = erbf._sender
 
         self._tc = erbf._tc
         self._defaults = erbf._defaults
         self._cache_preview = erbf._cache_preview
 
-        self._box_salt = erbf._box_salt
+        self._box_channel = erbf._box_channel
         self._box_channel_id = erbf._box_channel_id
+
+        self._box_salt = erbf._box_salt
         self._file_size = erbf._file_size
         self._fingerprint = erbf._fingerprint
 
         self._upload_time, self._size = erbf._upload_time, None
         self._file_iv, self._file_salt = erbf._file_iv, erbf._file_salt
         self._cattrs, self._file_path = None, None
         self._duration, self._version_byte = None, erbf._version_byte
@@ -1387,14 +1669,18 @@
 
     @property
     def file_path(self) -> Union[Path, None]:
         """Returns file path or ``None`` if not initialized."""
         return self._file_path
 
     def set_file_path(self, file_path: Path) -> None:
+        """
+        Will change self._file_path to file_path.
+        In most cases you don't need to use this
+        """
         self._file_path = file_path
 
     @property
     def file_name(self) -> Union[str, None]:
         """Returns file name or ``None`` if not initialized."""
         return self._file_name
 
@@ -1416,14 +1702,20 @@
         """
         return self._residual_metadata
 
     def __raise_initialized(self) -> NoReturn:
         if not self._initialized:
             raise NotInitializedError('RemoteBoxFile must be initialized.')
 
+    @staticmethod
+    async def decrypt() -> NoReturn:
+        raise AttributeError(
+            """This function was inherited from ``EncryptedRemoteBoxFile`` """
+            """and cannot be used on ``DecryptedRemoteBoxFile``."""
+        )
     async def init(
             self, cache_preview: bool=True,
             erase_encrypted_metadata: Optional[bool] = True
         ) -> 'DecryptedRemoteBoxFile':
         """
         This method will decrypt and parse metadata from
         the EncryptedRemoteBoxFile.
@@ -1437,78 +1729,112 @@
         If ERBFI wasn't initialized, this
         method will init it.
 
         If ``cache_preview`` was disabled in the
         parent class then you can set similar kwarg
         here to ``True`` and method will save it.
         """
+        logger.debug(f'Initializing DRBF ID({self._id})...')
+
         if not self._erbf._initialized:
             await self._erbf.init()
 
         cache_preview = cache_preview if cache_preview else self._cache_preview
         pattr_offset = len(PREFIX) + len(VERBYTE) + 3
 
+        logger.debug('Unpacking Public part of RBF metadata...')
+
         unpacked_metadata = PackedAttributes.unpack(
             bytes(self._erbf._metadata[pattr_offset:-16])
         )
         self._file_pos = len(self._erbf._metadata)
+        logger.debug(f'Actual encrypted filedata position: {self._file_pos}')
+
+        logger.debug('Unpacking Secret part of RBF metadata...')
 
         secret_metadata = AES(self._filekey).decrypt(
             unpacked_metadata['secret_metadata']
         )
         secret_metadata = PackedAttributes.unpack(secret_metadata)
 
         if not secret_metadata: # secret_metadata can't be empty dict
             raise AESError('Metadata wasn\'t decrypted correctly. Incorrect key?')
 
         if cache_preview:
+            logger.debug('cache_preview is True, DRBF preview will be saved.')
             self._preview = secret_metadata['preview']
         else:
+            logger.debug('cache_preview is False, DRBF preview won\'t be saved.')
             secret_metadata.pop('preview')
             self._preview = b''
 
         self._duration = bytes_to_int(secret_metadata['duration'])
         self._size = bytes_to_int(secret_metadata['file_size'])
         self._file_name = secret_metadata['file_name'].decode()
         self._cattrs = PackedAttributes.unpack(secret_metadata['cattrs'])
         self._mime = secret_metadata['mime'].decode()
 
         if self._mainkey:
+            logger.debug('Decrypting efile_path with the MainKey')
             self._file_path = AES(self._mainkey).decrypt(
                 secret_metadata['efile_path']
             )
             self._file_path = Path(self._file_path.decode())
         else:
+            logger.warning(
+               f'''We can\'t decrypt real file path of ID{self._id} because '''
+                '''MainKey is not present. Try to decrypt EncryptedRemoteBoxFile '''
+                '''with MainKey to fix this. Setting to DEF_NO_FOLDER...'''
+            )
             self._file_path = self._defaults.DEF_NO_FOLDER
 
         for attr in self.__required_metadata:
             secret_metadata.pop(attr)
 
         self._residual_metadata = secret_metadata
 
         if self._message.message:
             try:
                 edited_metadata = AES(self._filekey).decrypt(
                     urlsafe_b64decode(self._message.message)
                 )
                 edited_metadata = PackedAttributes.unpack(edited_metadata)
+                logger.debug(f'Updates to metadata for ID{self._id} found. Applying...')
 
                 for k,v in tuple(edited_metadata.items()):
                     if k in self.__required_metadata:
-                        setattr(self, f'_{k}', v)
+                        if k == 'cattrs':
+                            setattr(self, f'_{k}', PackedAttributes.unpack(v))
+
+                        elif k == 'efile_path':
+                            if self._mainkey:
+                                file_path = AES(self._mainkey).decrypt(v)
+                                self._file_path = Path(file_path.decode())
+                            else:
+                                logger.debug(
+                                    '''Updated metadata contains efile_path, but '''
+                                    '''this DecryptedRemoteBoxFile wasn\'t '''
+                                    '''decrypted with MainKey, so we will ignore it'''
+                                )
+                        else:
+                            # str attributes
+                            if k in ('mime', 'file_name'):
+                                setattr(self, f'_{k}', v.decode())
+                            else:
+                                setattr(self, f'_{k}', v)
                     else:
                         self._residual_metadata[k] = v
 
                     del edited_metadata[k]
 
-            except (TypeError, ValueError):
-                # Caption is not an updated metadata.
-                # TODO: Log this in future.
-                pass
-
+            except Exception:
+                logger.debug(
+                    f'''Updates to metadata for ID{self._id} failed. '''
+                    f'''Traceback:\n{format_exc()}'''
+                )
         self._initialized = True
 
         if erase_encrypted_metadata:
             self._erbf._initialized = False
             self._erbf._metadata = None
 
         return self
@@ -1556,84 +1882,127 @@
 
             progress_callback (``Callable[[int, int], None]``, optional):
                 A callback function accepting two parameters:
                 (downloaded_bytes, total).
         """
         self.__raise_initialized()
 
+        logger.info(f'Downloading DRBF (ID{self._id})...')
+
         if decrypt:
             aws = AES(self._filekey, self._file_iv)
 
         if outfile is None:
             outfile = self._defaults.DOWNLOAD_PATH
 
         if isinstance(outfile, (str, PathLike)):
             outfile = Path(outfile)
-            outfile.mkdir(exist_ok=True)
+            outfile.mkdir(exist_ok=True, parents=True)
 
             path = self._defaults.DEF_UNK_FOLDER if hide_folder else self._file_path
             # The first '/' symbol in '/home/non/' is also path part,
             # so we need to create a folders like / -> home -> non,
-            # however, Linux (and i believe all Unix) OS doesn't allow
+            # however, Linux (and i believe all UNIX) OS doesn't allow
             # to use a '/' symbol in filename, so instead of / we use
             # a '@' while creating path. You can refer to it as root.
-            path = str(self._defaults.DEF_NO_FOLDER if not path else path)
             #
-            if path.startswith('/'):
-                path = str(Path('@', path.lstrip('/')))
+            # In Windows paths [i.e C:\Users\user] the first path
+            # part (anchor) is 'C:\\'. We will remove all but
+            # letter to prevent strange behaviour on Windows
             #
+            # The make_safe_file_path() func do this for us
+            path = make_safe_file_path(path)
+
             if hide_name:
                 name = prbg(16).hex() + Path(self._file_name).suffix
             else:
                 name = self._file_name
 
             outfile = Path(outfile, path, name.lstrip('/'))
             outfile.parent.mkdir(exist_ok=True, parents=True)
+
             outfile = open(outfile,'wb')
 
         elif isinstance(outfile, BinaryIO) or hasattr(outfile, 'write'):
             pass # We already can write
         else:
             raise TypeError('outfile not Union[BinaryIO, str, PathLike].')
 
-        iter_down = download_file(
-            client = self._tc,
-            location = self._message.document,
-            request_size = request_size,
-        )
-        buffered, offset, total = b'', self._file_pos, 0
-        async for chunk in iter_down:
-            if buffered:
-                buffered += chunk
-                chunk = buffered[:request_size]
-                buffered = buffered[request_size:]
-            else:
-                buffered += chunk[offset:]
-                offset = None; continue
-
-            chunk = aws.decrypt(chunk, unpad=False) if decrypt else chunk
-            outfile.write(chunk)
+        logger.debug(f'outfile is {outfile}')
 
-            if progress_callback:
-                total += len(chunk)
-                if iscoroutinefunction(progress_callback):
-                    await progress_callback(total, self._file_size)
+        use_slow_download_switch = 0
+        while True:
+            try:
+                # By default we will try to download file via the
+                # fast "download_file" coroutine from fastelethon
+                # module. If it fails, the "use_slow_download_switch"
+                # will be incremented and this code will be switched
+                # to the default "iter_download" from TelegramClient;
+                # If it will fail too, -- we will raise an error.
+                if use_slow_download_switch == 0:
+                    iter_down = download_file(
+                        client = self._tc,
+                        location = self._message.document,
+                        request_size = request_size,
+                    )
                 else:
-                    progress_callback(total, self._file_size)
+                    # Switch to the default slow method
+                    iter_down = self._tc.iter_download(
+                        self._message.document,
+                        request_size=request_size
+                    )
+                buffered, offset, total = b'', self._file_pos, 0
+                async for chunk in iter_down:
+                    if buffered:
+                        buffered += chunk
+                        chunk = buffered[:request_size]
+                        buffered = buffered[request_size:]
+                    else:
+                        buffered += chunk[offset:]
+                        offset = None; continue
+
+                    chunk = aws.decrypt(chunk, unpad=False) if decrypt else chunk
+                    outfile.write(chunk)
+
+                    if progress_callback:
+                        total += len(chunk)
+                        logger.debug(
+                            f'''ID{self._id}: Downloaded {self._file_size} '''
+                            f'''from the {total} bytes'''
+                        )
+                        if iscoroutinefunction(progress_callback):
+                            await progress_callback(total, self._file_size)
+                        else:
+                            progress_callback(total, self._file_size)
+
+                if buffered:
+                    logger.debug(f'ID{self._id}: Writing the last buffered bytes...')
+                    outfile.write(aws.decrypt(buffered, unpad=True) if decrypt else chunk)
+
+                    if progress_callback:
+                        if iscoroutinefunction(progress_callback):
+                            await progress_callback(
+                                self._file_size, self._file_size)
+                        else:
+                            progress_callback(
+                                self._file_size, self._file_size)
 
-        if buffered:
-            outfile.write(aws.decrypt(buffered, unpad=True) if decrypt else chunk)
+                break # Download is successfull so we can exit this loop
 
-            if progress_callback:
-                if iscoroutinefunction(progress_callback):
-                    await progress_callback(
-                        self._file_size, self._file_size)
+            except Exception as e:
+                if use_slow_download_switch < 1:
+                    use_slow_download_switch += 1
+                    logger.warning(
+                        '''Fast download FAILED. Trying to use SLOW. '''
+                       f'''Traceback:\n{format_exc()}''')
+                    continue
                 else:
-                    progress_callback(
-                        self._file_size, self._file_size)
+                    logger.error('Fast & Slow download methods failed')
+                    raise e
+
         return outfile
 
     async def update_metadata(
             self, changes: Dict[str, Union[bytes, None]],
             dlb: Optional['DecryptedLocalBox'] = None
         ):
         """This method will "update" file metadata attributes
@@ -1668,84 +2037,102 @@
 
         .. note::
             - Your LocalBox will NOT know about this update,
               so you should specify here ``dlb`` (is better way)
               or await the ``refresh_metadata`` method on the
               ``DecryptedLocalBoxFile`` with the same ID.
 
-            - Not a *default* metadata (like file_name, mime, etc)
+            - Not a *default* metadata (default is file_name, mime, etc)
               will be placed to the ``residual_metadata`` property dict.
 
             - There is a file caption (and so updated metadata)
               limit: 1KB and 2KB for a Premium Telegram users.
 
-            - You can replace file's path by specifying a
-              ``file_path`` key with appropriate value. Also,
-              you **will need** to specify a ``DecryptedLocalBox``
+            - You can replace file's path by specifying a ``file_path``
+              key with appropriate path (str/bytes). Also, you
+              **will need** to specify a ``DecryptedLocalBox``
               as ``dlb`` so we can create a new *LocalBoxDirectory*
               from your path. Without it you will get a ``ValueError``
         """
         if 'efile_path' in changes:
             raise ValueError('The "changes" should not contain efile_path')
 
         if 'file_path' in changes and not dlb:
             raise ValueError('You can\'t change file_path without specifying dlb!')
+
+        current_changes = changes.copy()
+
+        logger.debug(f'Applying changes {current_changes} to the ID{self._id}...')
         try:
             message_caption = urlsafe_b64decode(self._message.message)
             updates = AES(self._filekey).decrypt(message_caption)
             updates = PackedAttributes.unpack(updates)
         except (ValueError, TypeError):
             updates = {}
 
-        new_file_path = changes.pop('file_path', None)
+        new_file_path = current_changes.pop('file_path', None)
+        if isinstance(new_file_path, bytes):
+            new_file_path = new_file_path.decode()
 
         if new_file_path:
             directory = await dlb._make_local_path(Path(new_file_path))
 
             await dlb._tgbox_db.FILES.execute((
                 'UPDATE FILES SET PPATH_HEAD=? WHERE ID=?',
                 (directory.part_id, self._id)
             ))
-            efile_path = AES(self._mainkey).encrypt(str(new_file_path).encode())
-            changes['efile_path'] = efile_path
+            efile_path = AES(dlb._mainkey).encrypt(new_file_path.encode())
+            current_changes['efile_path'] = efile_path
+
+        # If new_file_path is empty string then it's should be
+        # a request to remove updated file_path attribute
+        # from the RemoteBox file and restore default
+        if new_file_path is not None:
+            updates.pop('efile_path', None)
 
-        updates.update(changes)
+        updates.update(current_changes)
 
         for k,v in tuple(updates.items()):
             if not v:
                 del updates[k]
 
                 if k in self._residual_metadata:
                     del self._residual_metadata[k]
 
-        updates_packed = PackedAttributes.pack(**updates)
-        updates_encrypted = AES(self._filekey).encrypt(updates_packed)
+        if updates:
+            updates_packed = PackedAttributes.pack(**updates)
+            updates_encrypted = AES(self._filekey).encrypt(updates_packed)
+            updates_encoded = urlsafe_b64encode(updates_encrypted).decode()
+        else:
+            updates_encoded = ''
         try:
-            await self._message.edit(
-                urlsafe_b64encode(updates_encrypted).decode()
-            )
+            await self._message.edit(updates_encoded)
         except MediaCaptionTooLongError:
             raise NoPlaceLeftForMetadata(NoPlaceLeftForMetadata.__doc__) from None
         except ChatAdminRequiredError:
             raise NotEnoughRights(NotEnoughRights.__doc__) from None
-
+        except MessageNotModifiedError as e:
+            logger.debug(
+                '''Updates wasn\'t commited to your RemoteBox '''
+               f'''because of MessageNotModifiedError: {e}'''
+            )
         for k,v in tuple(updates.items()):
             if k in self.__required_metadata:
                 if k == 'cattrs':
                     setattr(self, f'_{k}', PackedAttributes.unpack(v))
                 elif k == 'efile_path':
                     self._file_path = new_file_path
                 else:
                     setattr(self, f'_{k}', v)
             else:
                 self._residual_metadata[k] = v
 
         if dlb:
-            dlbfi = await dlb.get_file(self._id)
-            await dlbfi.refresh_metadata(_updated_metada=updates_encrypted)
+            dlbf = await dlb.get_file(self._id)
+            await dlbf.refresh_metadata(_updated_metadata=updates_encoded)
 
     def get_sharekey(self, reqkey: Optional[RequestKey] = None) -> ShareKey:
         """
         Returns ``ShareKey`` for this file. You should
         use this method if you want to share this
         file with other people.
```

### Comparing `tgbox-1.1.1/tgbox/api/utils.py` & `tgbox-1.2/tgbox/api/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,50 @@
-"""Module with all API utils."""
+"""Module with utils for api package."""
+
+import logging
 
 from typing import (
     BinaryIO, Optional,
     Union, AsyncGenerator
 )
 from os import PathLike
 from dataclasses import dataclass
+from re import search as re_search
 from base64 import urlsafe_b64encode
 
 from telethon.tl.custom.file import File
 from telethon.sessions import StringSession
 
 from telethon.tl.types import Photo, Document
 from telethon.tl.types.auth import SentCode
 
 from telethon import TelegramClient as TTelegramClient
 from telethon.errors import SessionPasswordNeededError
 from telethon.tl.functions.auth import ResendCodeRequest
 
-try:
-    from regex import search as re_search
-except ImportError:
-    from re import search as re_search
 
 from ..defaults import VERSION
-from ..tools import anext, SearchFilter
 from ..fastelethon import download_file
+from ..tools import anext, SearchFilter, _TypeList
 
 from .db import TABLES, TgboxDB
 
 __all__ = [
     'search_generator',
     'DirectoryRoot',
     'PreparedFile',
     'TelegramClient',
     'DefaultsTableWrapper',
     'RemoteBoxDefaults'
 ]
+logger = logging.getLogger(__name__)
+
 class TelegramClient(TTelegramClient):
     """
-    A little extend to the ``telethon.TelegramClient``.
+    A little extension to the ``telethon.TelegramClient``.
 
     This class inherits Telethon's TelegramClient and support
     all features that has ``telethon.TelegramClient``.
 
     Typical usage:
 
     .. code-block:: python
@@ -69,14 +70,16 @@
                 code = int(input('Code: ')),
                 password = getpass('Pass: ')
             )
             erb = await make_remotebox(tc)
 
         asyncio_run(main())
     """
+    __version__ = VERSION
+
     def __init__(
             self, api_id: int, api_hash: str,
             phone_number: Optional[str] = None,
             session: Optional[Union[str, StringSession]] = None,
             **kwargs) -> None:
         """
         .. note::
@@ -110,26 +113,27 @@
             raise ValueError(
                 'You should specify at least ``session`` or ``phone_number``.'
             )
         super().__init__(
             StringSession(session),
             api_id, api_hash, **kwargs
         )
-        self.__version__ = VERSION
         self._api_id, self._api_hash = api_id, api_hash
         self._phone_number = phone_number
 
     async def send_code(self, force_sms: Optional[bool]=False) -> SentCode:
         """
         Sends the Telegram code needed to login to the given phone number.
 
         Arguments:
             force_sms (``bool``, optional):
                 Whether to force sending as SMS.
         """
+        logger.info(f'Sending login code to {self._phone_number}...')
+
         return await self.send_code_request(
             self._phone_number, force_sms=force_sms
         )
     async def log_in(
             self, password: Optional[str] = None,
             code: Optional[Union[int,str]] = None) -> None:
         """
@@ -143,17 +147,25 @@
 
             code (``int``, optional):
                 The code that Telegram sent you after calling
                 ``TelegramClient.send_code()`` method.
         """
         if not await self.is_user_authorized():
             try:
+                logger.info(f'Trying to sign-in with {self._phone_number} and {code} code..')
                 await self.sign_in(self._phone_number, code)
             except SessionPasswordNeededError:
+                logger.info(
+                    '''Log-in without 2FA password failed. '''
+                   f'''Trying to sign-in with {self._phone_number}, '''
+                   f'''password and {code} code..'''
+                )
                 await self.sign_in(password=password)
+        else:
+            logger.debug(f'User {self._phone_number} is already authorized.')
 
     async def resend_code(self, sent_code: SentCode) -> SentCode:
         """
         Will send you login code again. This can be used to
         force Telegram send you SMS or Call to dictate code.
 
         Arguments:
@@ -165,17 +177,63 @@
 
         .. code-block:: python
 
             tc = tgbox.api.TelegramClient(...)
             sent_code = await tc.send_code()
             sent_code = await tc.resend_code(sent_code)
         """
+        logger.info(f'Resending login code to {self._phone_number}...')
         return await self(ResendCodeRequest(
             self._phone_number, sent_code.phone_code_hash)
         )
+
+class TelegramVirtualFile:
+    """
+    You can use this class for re-upload to RemoteBox
+    files that already was uploaded to any other
+    Telegram chat. Wrap it over ``Document`` and
+    specify in the ``DecryptedLocalBox.prepare_file``
+    """
+    def __init__(self, document: Union[Photo, Document], tc: TelegramClient):
+        self.tc = tc
+        self.document = document
+
+        file = File(document)
+
+        self.name = file.name
+        self.size = file.size
+        self.mime = file.mime_type
+
+        self.duration = file.duration\
+            if file.duration else 0
+
+        self._downloader = None
+
+    async def get_preview(self, quality: int=1) -> bytes:
+        if hasattr(self.document,'sizes')\
+            and not self.document.sizes:
+                return b''
+
+        if hasattr(self.document,'thumbs')\
+            and not self.document.thumbs:
+                return b''
+
+        return await self.tc.download_media(
+            message = self.document,
+            thumb = quality, file = bytes
+        )
+    async def read(self, size: int=-1) -> bytes:
+        """Will return <= 512KiB of data. 'size' ignored"""
+        if not self._downloader:
+            self._downloader = download_file(
+                self.tc, self.document
+            )
+        chunk = await anext(self._downloader)
+        return chunk
+
 @dataclass
 class PreparedFile:
     """
     This dataclass store data needed for upload
     by ``DecryptedRemoteBox.push_file`` in future.
 
     Usually it's only for internal use.
@@ -203,49 +261,96 @@
     Type used to specify that you want to
     access absolute local directory root.
 
     This class doesn't have any methods,
     please use it only for ``lbd.iterdir``
     """
 
-# TODO: Improve SearchFilter
 async def search_generator(
         sf: SearchFilter, it_messages: Optional[AsyncGenerator] = None,
         lb: Optional['tgbox.api.local.DecryptedLocalBox'] = None,
         cache_preview: bool = True) -> AsyncGenerator:
     """
     Generator used to search for files in dlb and rb. It's
-    only for internal use, and you shouldn't use it in your
+    only for internal use and you shouldn't use it in your
     own projects.
 
     If file is exported from other RemoteBox and was imported to your
     LocalBox, then you can specify ``dlb`` as ``lb``. AsyncGenerator
     will try to get ``FileKey`` and decrypt ``EncryptedRemoteBoxFile``.
     Otherwise imported file will be ignored.
     """
     in_func = re_search if sf.in_filters['re'] else lambda p,s: p in s
 
     if it_messages:
         iter_from = it_messages
+
+    elif any((sf.in_filters['scope'], sf.ex_filters['scope'])):
+        if not sf.in_filters['scope']:
+            lbf = await anext(lb.files(), None)
+            if not lbf: return # Local doesn't have files
+
+        async def scope_generator(scope: Union[str, list]):
+            scope = scope if scope else DirectoryRoot
+            scope = scope if isinstance(scope, _TypeList) else [scope]
+
+            for current_scope in scope:
+                if current_scope is DirectoryRoot:
+                    iterdir = lbf.directory.iterdir(ppid=current_scope)
+
+                elif hasattr(current_scope, '_part_id'):
+                    iterdir = current_scope.iterdir()
+
+                else:
+                    iterdir = await lb.get_directory(current_scope)
+                    if not iterdir:
+                        return
+                    iterdir = iterdir.iterdir()
+
+                async for content in iterdir:
+                    if hasattr(content, '_part_id'):
+                        # This is DecryptedLocalBoxDirectory
+                        if str(content) in sf.ex_filters['scope']:
+                            continue # This directory is excluded
+
+                        async for dlbf in scope_generator(content):
+                            yield dlbf # This is DecryptedLocalBoxFile
+                    else:
+                        yield content # This is DecryptedLocalBoxFile
+
+        iter_from = scope_generator(sf.in_filters['scope'])
     else:
-        min_id = sf.in_filters['min_id'][-1] if sf.in_filters['min_id'] else None
-        max_id = sf.in_filters['max_id'][-1] if sf.in_filters['max_id'] else None
-        iter_from = lb.files(min_id=min_id, max_id=max_id, cache_preview=cache_preview)
+        min_id = sf.in_filters['min_id'][-1]\
+            if sf.in_filters['min_id'] else None
+
+        max_id = sf.in_filters['max_id'][-1]\
+            if sf.in_filters['max_id'] else None
+
+        iter_from = lb.files(
+            min_id = min_id,
+            max_id = max_id,
+            ids = sf.in_filters['id'],
+            cache_preview = cache_preview
+        )
 
     if not iter_from:
         raise ValueError('At least it_messages or lb must be specified.')
 
     async for file in iter_from:
         if hasattr(file, '_message'): # *RemoteBoxFile
             file_size = file.file_size
-            file_path = file.file_path if file.file_path else ''
-        elif hasattr(file, '_tgbox_db'): # *LocalBoxFile
+
+            if hasattr(file, 'file_path') and file.file_path:
+                file_path = str(file.file_path)
+            else:
+                file_path = ''
+
+        elif hasattr(file, '_lb'): # *LocalBoxFile
             file_size = file.size
-            await file.directory.lload(full=True)
-            file_path = str(file.directory)
+            file_path = str(file.file_path) if file.file_path else ''
         else:
             continue
 
         # We will use it as flags, the first
         # is for 'include', the second is for
         # 'exclude'. Both should be True to
         # match SearchFilter filters.
@@ -411,78 +516,20 @@
             else:
                 if filter['verbyte']:
                     if indx == 0:
                         yield_result[indx] = False
                         break
 
         if all(yield_result):
+            logger.debug(f'SearchFilter matched ID{file.id}')
             yield file
         else:
+            logger.debug(f'SearchFilter mismatch ID{file.id} [{yield_result}]')
             continue
 
-class _TelegramVirtualFile:
-    """
-    We use this class for re-upload to RemoteBox
-    files that already was uploaded to any other
-    Telegram chat. That's only for internal use.
-    """
-    def __init__(
-            self, document: Union[Photo, Document],
-            session: StringSession,
-            api_id: int, api_hash: str):
-
-        self.downloader = None
-        self.document = document
-
-        self.tc = TelegramClient(
-            session=session,
-            api_id=api_id,
-            api_hash=api_hash
-        )
-        self.tc = self.tc.connect()
-        self._client_initialized = False
-
-        file = File(document)
-
-        self.name = file.name
-        self.size = file.size
-        self.mime = file.mime_type
-
-        self.duration = file.duration\
-            if file.duration else 0
-
-    async def get_preview(self, quality: int=1) -> bytes:
-        if not self._client_initialized:
-            self.tc = await self.tc # connect
-            self._client_initialized = True
-
-        if hasattr(self.document,'sizes')\
-            and not self.document.sizes:
-                return b''
-
-        if hasattr(self.document,'thumbs')\
-            and not self.document.thumbs:
-                return b''
-
-        return await self.tc.download_media(
-            message = self.document,
-            thumb = quality, file = bytes
-        )
-    async def read(self, size: int) -> bytes:
-        if not self._client_initialized:
-            self.tc = await self.tc
-            self._client_initialized = True
-
-        if not self.downloader:
-            self.downloader = download_file(
-                self.tc, self.document
-            )
-        chunk = await anext(self.downloader)
-        return chunk
-
 class DefaultsTableWrapper:
     """
     This little class will wrap around the
     DEFAULTS table of TGBOX DB and will
     fetch all contents of it.
 
     You can await the ``change`` coroutine
@@ -499,14 +546,18 @@
 
     @property
     def initialized(self) -> bool:
         return self._initialized
 
     async def init(self) -> 'DefaultsTableWrapper':
         """Fetch the defaults and initialize"""
+        logger.debug(
+            '''Initializing DefaultsTableWrapper for '''
+           f'''{self._tgbox_db._db_path} LocalBox'''
+        )
         if self._tgbox_db.closed:
             await self._tgbox_db.init()
 
         defaults = await self._tgbox_db.DEFAULTS.select_once()
         for default, value in zip(TABLES['DEFAULTS'], defaults):
             setattr(self, default[0], value)
 
@@ -553,14 +604,16 @@
                 ... # Some code was omited here
                 # Change the default download path
                 dlb.defaults.change('DOWNLOAD_PATH', 'Downloads')
 
             asyncio_run(main())
         """
         getattr(self, key) # Vetrify that Key exist
+
+        logger.info(f'Changing defaults | UPDATE DEFAULTS SET {key}={value}')
         await self._tgbox_db.DEFAULTS.execute((
             f'UPDATE DEFAULTS SET {key}=?', (value,)
         ))
 
 @dataclass
 class RemoteBoxDefaults:
     METADATA_MAX: int
```

### Comparing `tgbox-1.1.1/tgbox/crypto.py` & `tgbox-1.2/tgbox/crypto.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 """This module stores all cryptography used in API."""
 
+import logging
+
+logger = logging.getLogger(__name__)
+
 from os import urandom
 from typing import Union, Optional
 
 from pyaes.util import (
     append_PKCS7_padding,
     strip_PKCS7_padding
 )
 from .errors import ModeInvalid
 try:
     from cryptography.hazmat.primitives.ciphers\
         import Cipher, algorithms, modes
     FAST_ENCRYPTION = True
+    logger.info('Fast cryptography library was found.')
 except ModuleNotFoundError:
     # We can use PyAES if there is no cryptography library.
     # PyAES is much slower. You can use it for quick tests.
     from pyaes import AESModeOfOperationCBC
     FAST_ENCRYPTION = False
+    logger.warning('Fast cryptography library was NOT found. ')
 try:
     # Check if cryptg is installed.
     from cryptg import __name__ as _
     del _
     FAST_TELETHON = True
 except ModuleNotFoundError:
     FAST_TELETHON = False
@@ -46,15 +52,15 @@
                 AES encryption/decryption Key.
 
             iv (``bytes``):
                 AES Initialization Vector.
         """
         key = key.key if hasattr(key, 'key') else key
 
-        self._aes_state = AESModeOfOperationCBC(
+        self._aes_state = AESModeOfOperationCBC( # pylint: disable=E0601
             key = bytes(key), iv = bytes(iv)
         )
         self.__mode = None # encrypt mode is 1 and decrypt is 2
 
     @staticmethod
     def __convert_memoryview(data: Union[bytes, memoryview]) -> bytes:
         # PyAES doesn't support memoryview, convert to bytes
```

### Comparing `tgbox-1.1.1/tgbox/defaults.py` & `tgbox-1.2/tgbox/defaults.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """This module stores API defaults."""
 
+import logging
+
 from enum import IntEnum
 from pathlib import Path
-from . import __version__
-
 try:
     from sys import _MEIPASS
 except ImportError:
     _MEIPASS = None
 
+from .version import VERSION
+
 __all__ = [
     'Limits',
+    'UploadLimits',
     'Scrypt',
     'VERSION',
     'VERBYTE',
     'DEF_TGBOX_NAME',
     'REMOTEBOX_PREFIX',
     'DEF_NO_FOLDER',
     'DEF_UNK_FOLDER',
@@ -22,26 +25,33 @@
     'BOX_IMAGE_PATH',
     'WORDS_PATH',
     'FFMPEG',
     'ABSPATH',
     'DOWNLOAD_PATH',
     'PYINSTALLER_DATA'
 ]
+logger = logging.getLogger(__name__)
+
 class Limits(IntEnum):
     """Default TGBOX API limits"""
     # We store metadata size in three bytes, but
     # by default it's size is limited to 1MB. You
     # can set it up to the 256^3-1, but to share
     # your files with other people they should have
     # a METADATA_MAX that >= than yours.
     METADATA_MAX: int=1000000
     # Max FILE_PATH length on Linux
     # is 4096 bytes (4KiB).
     FILE_PATH_MAX: int=4096
 
+class UploadLimits(IntEnum):
+    """Telegram filesize limits"""
+    DEFAULT = 2000000000
+    PREMIUM = 4000000000
+
 class Scrypt(IntEnum):
     """Default Scrypt KDF configuration"""
     # See https://en.wikipedia.org/wiki/Scrypt for base info about Scrypt
     # -------------------------------------------------------------------
     # This salt affects basekeys, you can change it to protect your RemoteBox
     # from bruteforcing, but be sure to backup your own salt, because if you
     # lose it, then it will be impossible to recover your decryption key for Tgbox.
@@ -57,15 +67,14 @@
     N:     int=2**20
     R:     int=8
     P:     int=1
 
 # Path that will be used to save downloaded files.
 DOWNLOAD_PATH: Path=Path('DownloadsTGBOX')
 
-VERSION: str=__version__
 VERBYTE: bytes=b'\x01'
 
 DEF_TGBOX_NAME:   str='TGBOX'
 REMOTEBOX_PREFIX: str=f'{DEF_TGBOX_NAME}[{VERBYTE.hex()}]: '
 
 DEF_NO_FOLDER:  Path=Path('NO_FOLDER')
 DEF_UNK_FOLDER: Path=Path('UNKNOWN_FOLDER')
@@ -88,14 +97,15 @@
 # or extract duration. It will be added to
 # your resulted executable.
 #
 # https://www.ffmpeg.org/download.html#build-windows
 #
 for file in _other.iterdir():
     if file.name == 'ffmpeg.exe':
+        logger.info(f'FFMPEG found in {str(_other)}, we will use it')
         FFMPEG = _other / 'ffmpeg.exe'
 
 # By default, PyInstaller will not grab files
 # from 'other' folder. To resolve this error
 # you will need to manually add it to .spec file.
 #
 # See
```

### Comparing `tgbox-1.1.1/tgbox/errors.py` & `tgbox-1.2/tgbox/errors.py`

 * *Files identical despite different names*

### Comparing `tgbox-1.1.1/tgbox/fastelethon.py` & `tgbox-1.2/tgbox/fastelethon.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Copied from Mautrix-Telegram
     github.com/tulir/mautrix-telegram/
 
 Copied again from Painor GitHub
     gist.github.com/painor/7e74de80ae0c819d3e9abcf9989a8dd6
 
 | This file was patched for TGBOX project (github.com/NonProjects/tgbox)
-| and may not work as you expected in your libraries.
+| and may not work as you expect in your code.
 
 Big thanks to all contributors of this module.
 """
 
 import os
 import math
 import asyncio
@@ -48,15 +48,15 @@
     InputFileBig, InputFile
 )
 from telethon.tl.functions.upload import (
     GetFileRequest,
     SaveFilePartRequest,
     SaveBigFilePartRequest
 )
-log: logging.Logger = logging.getLogger("telethon")
+logger: logging.Logger = logging.getLogger(__name__)
 
 TypeLocation = Union[
     Document, Photo, InputDocumentFileLocation,
     InputPeerPhotoFileLocation,
     InputFileLocation, InputPhotoFileLocation
 ]
 class DownloadSender:
@@ -130,15 +130,15 @@
     async def next(self, data: bytes) -> None:
         if self.previous:
             await self.previous
         self.previous = self.loop.create_task(self._next(data))
 
     async def _next(self, data: bytes) -> None:
         self.request.bytes = data
-        log.debug(f"Sending file part {self.request.file_part}/{self.part_count}"
+        logger.debug(f"Sending file part {self.request.file_part}/{self.part_count}"
                   f" with {len(data)} bytes")
         await self.client._call(self.sender, self.request)
         self.request.file_part += self.stride
 
     async def disconnect(self) -> None:
         if self.previous:
             await self.previous
@@ -244,15 +244,15 @@
     async def _create_sender(self) -> MTProtoSender:
         dc = await self.client._get_dc(self.dc_id)
         sender = MTProtoSender(self.auth_key, loggers=self.client._log)
         await sender.connect(self.client._connection(dc.ip_address, dc.port, dc.id,
                                                      loggers=self.client._log,
                                                      proxy=self.client._proxy))
         if not self.auth_key:
-            log.debug(f"Exporting auth to DC {self.dc_id}")
+            logger.debug(f"Exporting auth to DC {self.dc_id}")
             auth = await self.client(ExportAuthorizationRequest(self.dc_id))
             self.client._init_request.query = ImportAuthorizationRequest(id=auth.id,
                                                                          bytes=auth.bytes)
             req = InvokeWithLayerRequest(LAYER, self.client._init_request)
             await sender.send(req)
             self.auth_key = sender.auth_key
         return sender
@@ -280,15 +280,15 @@
             connection_count: Optional[int] = None
             ) -> AsyncGenerator[bytes, None]:
 
         connection_count = connection_count or self._get_connection_count(file_size)
         part_size = (part_size_kb or utils.get_appropriated_part_size(file_size)) * 1024
         part_count = math.ceil(file_size / part_size)
 
-        log.debug("Starting parallel download: "
+        logger.debug("Starting parallel download: "
                   f"{connection_count} {part_size} {part_count} {file!s}")
 
         await self._init_download(
             connection_count,
             file, part_count,
             part_size, offset=offset
         )
@@ -299,17 +299,17 @@
                 tasks.append(self.loop.create_task(sender.next()))
             for task in tasks:
                 data = await task
                 if not data:
                     break
                 yield data
                 part += 1
-                log.debug(f"Part {part} downloaded")
+                logger.debug(f"Part {part} downloaded")
 
-        log.debug("Parallel download finished, cleaning up connections")
+        logger.debug("Parallel download finished, cleaning up connections")
         await self._cleanup()
 
 
 parallel_transfer_locks: DefaultDict[int, asyncio.Lock] =\
     defaultdict(lambda: asyncio.Lock())
 
 async def stream_file(
```

### Comparing `tgbox-1.1.1/tgbox/keys.py` & `tgbox-1.2/tgbox/keys.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,34 +49,40 @@
 ]
 
 class Phrase:
     """This class represents passphrase"""
     def __init__(self, phrase: Union[bytes, str]):
         if isinstance(phrase, str):
             self._phrase = phrase.encode()
-        else:
+
+        elif isinstance(phrase, bytes):
             self._phrase = phrase
+        else:
+            raise TypeError('phrase must be Union[bytes, str]')
 
     def __repr__(self) -> str:
         return f'Phrase({repr(self._phrase)}) # at {hex(id(self))}'
 
+    def __str__(self) -> str:
+        return self._phrase.decode()
+
     def __hash__(self) -> int:
         # Without 22 hash of bytes will be equal to object's
         return hash((self._phrase,22))
 
     def __eq__(self, other) -> bool:
         return hash(self) == hash(other)
 
     @property
     def phrase(self) -> bytes:
         """Returns currrent raw phrase"""
         return self._phrase
 
     @classmethod
-    def generate(cls, words_count: int=12) -> 'Phrase':
+    def generate(cls, words_count: int=6) -> 'Phrase':
         """
         Generates passphrase
 
         Arguments:
             words_count (``int``, optional):
                 Words count in ``Phrase``.
         """
@@ -411,15 +417,16 @@
             encoding=Encoding.X962,
             format=PublicFormat.CompressedPoint)
     else:
         skey = SigningKey.from_string(
             sha256(key + salt).digest(),
             curve=SECP256k1, hashfunc=sha256
         )
-        vkey = skey.get_verifying_key()._compressed_encode()
+        vkey = skey.get_verifying_key()
+        vkey = vkey.to_string('compressed')
 
     return RequestKey(vkey)
 
 def make_sharekey(
      *, mainkey: Optional[MainKey] = None,
         requestkey: Optional[RequestKey] = None,
         box_salt: Optional[bytes] = None,
@@ -429,22 +436,23 @@
     """
     Function for making ShareKeys.
 
     .. note::
         You may want to know what is ``RequestKey`` before reading
         this. Please, run help on ``make_requestkey`` to get info.
 
-    Alice recieves ``RequestKey`` from Bob. But what she should do
+    Alice recieved ``RequestKey`` from Bob. But what she should do
     next? As reqkey is just EC-pubkey, she wants to make a shared
-    secret key. A makes her own privkey as B, with
-    ``sha256(mainkey + salt)`` & initializes ECDH with B pubkey
-    and her privkey. After this, A makes a shared secret, which
-    is 32-byte length AES-CBC key & encrypts her file/main key.
-    IV here is first 16 byte of ``sha256(requestkey)``. Then she
-    prepends her pubkey to the result and sends it to Bob.
+    secret key. A makes her own privkey as B, with ``sha256(mainkey
+    + sha256(salt + requestkey))`` & initializes ECDH with B pubkey
+    and her privkey. After this, A makes a hashed with SHA256
+    shared secret, which is 32-byte length AES-CBC key & encrypts
+    her file/main key. IV here is first 16 bytes of the
+    ``sha256(requestkey)``. Then she prepends her pubkey to
+    the resulted encrypted file/main key and sends it to Bob.
 
     With A pubkey, B can easily get the same shared secret and
     decrypt ``ShareKey`` to make the ``ImportKey``.
 
     The things will be much less complicated if Alice don't mind
     to share her File or Box with ALL peoples. Then she drops only
     her file or main key in raw. Simple is better than complex, after all.
@@ -488,16 +496,18 @@
                 """with requestkey."""
             )
         else:
             salt, key = box_salt, mainkey
     else:
         salt, key = file_salt, filekey
 
+    skey_salt = sha256(salt + requestkey.key).digest()
+
     if FAST_ENCRYPTION:
-        skey_data = int.from_bytes(sha256(key + salt).digest(), 'big')
+        skey_data = int.from_bytes(sha256(key + skey_salt).digest(), 'big')
         skey = ec.derive_private_key(skey_data, ec.SECP256K1())
 
         vkey = skey.public_key().public_bytes(
             encoding=Encoding.X962,
             format=PublicFormat.CompressedPoint
         )
         b_pubkey = ec.EllipticCurvePublicKey.from_encoded_point(
@@ -505,32 +515,31 @@
             data=requestkey.key
         )
         enc_key = skey.exchange(
             algorithm=ec.ECDH(),
             peer_public_key=b_pubkey)
     else:
         skey = SigningKey.from_string(
-            sha256(key + salt).digest(),
+            sha256(key + skey_salt).digest(),
             curve=SECP256k1, hashfunc=sha256
         )
-        vkey = skey.get_verifying_key()._compressed_encode()
+        vkey = skey.get_verifying_key()
+        vkey = vkey.to_string('compressed')
 
-        b_point = VerifyingKey._from_compressed(
+        b_pubkey = VerifyingKey.from_string(
             requestkey.key, curve=SECP256k1
         )
-        b_pubkey = VerifyingKey.from_public_point(
-            b_point, curve=SECP256k1, hashfunc=sha256
-        )
         ecdh = ECDH(
             curve=SECP256k1,
             private_key=skey,
             public_key=b_pubkey
         )
         enc_key = ecdh.generate_sharedsecret_bytes()
 
+    enc_key = sha256(enc_key).digest()
     iv = sha256(requestkey.key).digest()[:16]
 
     encrypted_key = AES(enc_key, iv).encrypt(
         key.key, pad=False, concat_iv=False
     )
     return ShareKey(encrypted_key + vkey)
 
@@ -570,53 +579,50 @@
 
     .. note::
         At least ``box_salt`` or ``file_salt`` must
         be specified in function.
     """
     if len(sharekey) == 32: # Key isn't encrypted.
         return ImportKey(sharekey.key)
-    else:
-        if not any((box_salt, file_salt)):
-            raise ValueError(
-                'At least box_salt or file_salt must be specified.'
-            )
-        else:
-            salt = box_salt if box_salt else file_salt
 
-            requestkey = make_requestkey(
-                key, box_salt=box_salt, file_salt=file_salt
-            )
-            if FAST_ENCRYPTION:
-                skey_data = int.from_bytes(sha256(key + salt).digest(), 'big')
-                skey = ec.derive_private_key(skey_data, ec.SECP256K1())
-
-                a_pubkey = ec.EllipticCurvePublicKey.from_encoded_point(
-                    curve=ec.SECP256K1(),
-                    data=sharekey[32:]
-                )
-                dec_key = skey.exchange(
-                    algorithm=ec.ECDH(),
-                    peer_public_key=a_pubkey)
-            else:
-                skey = SigningKey.from_string(
-                    sha256(key + salt).digest(),
-                    curve=SECP256k1, hashfunc=sha256
-                )
-                a_point = VerifyingKey._from_compressed(
-                    sharekey[32:], curve=SECP256k1
-                )
-                a_pubkey = VerifyingKey.from_public_point(
-                    a_point, curve=SECP256k1, hashfunc=sha256
-                )
-                ecdh = ECDH(
-                    curve=SECP256k1,
-                    private_key=skey,
-                    public_key=a_pubkey
-                )
-                dec_key = ecdh.generate_sharedsecret_bytes()
+    if not any((box_salt, file_salt)):
+        raise ValueError(
+            'At least box_salt or file_salt must be specified.'
+        )
+    salt = box_salt if box_salt else file_salt
 
-            iv = sha256(requestkey.key).digest()[:16]
+    requestkey = make_requestkey(
+        key, box_salt=box_salt, file_salt=file_salt
+    )
+    if FAST_ENCRYPTION:
+        skey_data = int.from_bytes(sha256(key + salt).digest(), 'big')
+        skey = ec.derive_private_key(skey_data, ec.SECP256K1())
 
-            decrypted_key = AES(dec_key, iv).decrypt(
-                sharekey[:32], unpad=False
-            )
-            return ImportKey(decrypted_key)
+        a_pubkey = ec.EllipticCurvePublicKey.from_encoded_point(
+            curve=ec.SECP256K1(),
+            data=sharekey[32:]
+        )
+        dec_key = skey.exchange(
+            algorithm=ec.ECDH(),
+            peer_public_key=a_pubkey)
+    else:
+        skey = SigningKey.from_string(
+            sha256(key + salt).digest(),
+            curve=SECP256k1, hashfunc=sha256
+        )
+        a_pubkey = VerifyingKey.from_string(
+            sharekey[32:], curve=SECP256k1
+        )
+        ecdh = ECDH(
+            curve=SECP256k1,
+            private_key=skey,
+            public_key=a_pubkey
+        )
+        dec_key = ecdh.generate_sharedsecret_bytes()
+
+    dec_key = sha256(dec_key).digest()
+    iv = sha256(requestkey.key).digest()[:16]
+
+    decrypted_key = AES(dec_key, iv).decrypt(
+        sharekey[:32], unpad=False
+    )
+    return ImportKey(decrypted_key)
```

### Comparing `tgbox-1.1.1/tgbox/other/tgbox_logo.png` & `tgbox-1.2/tgbox/other/tgbox_logo.png`

 * *Files identical despite different names*

### Comparing `tgbox-1.1.1/tgbox/other/words.txt` & `tgbox-1.2/tgbox/other/words.txt`

 * *Files identical despite different names*

### Comparing `tgbox-1.1.1/tgbox/tools.py` & `tgbox-1.2/tgbox/tools.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 """This module stores utils required by API."""
 
-try:
-    from regex import search as re_search
-except ImportError:
-    from re import search as re_search
-
 from asyncio import (
     iscoroutine, get_event_loop
 )
 from copy import deepcopy
 from pprint import pformat
 from hashlib import sha256
 from random import randrange
 
+from typing import (
+    BinaryIO, Optional, Dict,
+    Generator, Union
+)
 from subprocess import PIPE, run as subprocess_run
-from typing import BinaryIO, Optional, Dict, Generator
 
 from io import BytesIO
 from os import PathLike
-from pathlib import Path
 from functools import partial
+
+from re import search as re_search
 from os import remove as remove_file
 
+from platform import system as platform_system
+from pathlib import PureWindowsPath, Path
+
 from .errors import (
     ConcatError,
     PreviewImpossible,
     DurationImpossible
 )
 from .defaults import FFMPEG
 from .keys import FileKey, MainKey
@@ -36,17 +38,19 @@
     'SearchFilter',
     'OpenPretender',
     'PackedAttributes',
     'int_to_bytes',
     'bytes_to_int',
     'get_media_duration',
     'make_media_preview',
-    'ppart_id_generator'
+    'ppart_id_generator',
+    'make_general_path',
+    'guess_path_type',
+    'make_safe_file_path'
 ]
-anext = lambda agen: agen.__anext__()
 
 class _TypeList:
     """
     This is cutted version of ``list()`` that
     checks type on ``.append(...)``.
 
     You can specify multiply types with
@@ -59,14 +63,17 @@
     def __init__(self, type_, *args):
         self.type = type_ if isinstance(type_, tuple) else (type_,)
         self.list = [self.__check_type(i) for i in args]
 
     def __bool__(self):
         return bool(self.list)
 
+    def __len__(self):
+        return len(self.list)
+
     def __iter__(self):
         for i in self.list:
             yield i
 
     def __getitem__(self, sl):
         return self.list[sl]
 
@@ -117,26 +124,48 @@
       match **all** of filters, **not** one of it.
 
     * The ``SearchFilter`` accepts ``list`` as kwargs \
       value. You can ``SearchFilter(id=[3,5,10])``.
 
     * The ``SearchFilter(**kwargs)`` will add all filters \
       to the **include**. Also use ``SearchFilter.include(...)`` \
-      & ``SearchFilter.exclude(...)`` methods after initializion.
+      & ``SearchFilter.exclude(...)`` methods after initialization.
 
     All filters:
+        * **scope** *str*: Define a path as search scope:
+            The *scope* is an absolute directory in which
+            we will search your file by other *filters*. By
+            default, the ``tgbox.api.utils.search_generator``
+            will search over the entire *LocalBox*. This can
+            be slow if you're have too many files.
+
+            **Example**: let's imagine that You're a Linux user which
+            share it's *Box* with the Windows user. In this case,
+            Your *LocalBox* will contain a path parts on the
+            ``'/'`` (Linux) and ``'C:\\'`` (Windows) roots. If You
+            know that some file was uploaded by Your friend,
+            then You can specify a ``scope='C:\\'`` to ignore
+            all files uploaded from the Linux machine. This
+            will significantly fasten the search process,
+            because almost all filters require to select
+            row from the LocalBox DB, decrypt Metadata and
+            compare its values with ones from ``SearchFilter``.
+
+            | !: The ``scope`` will be ignored on *RemoteBox* search.
+            | !: The ``min_id`` & ``max_id`` will be ignored if ``scope`` used.
+
         * **id** *integer*: File ID
 
         * **cattrs** *dict*: File CustomAttributes:
             To search for CATTRS you need to specify a dict.
 
             E.g: If *file* ``cattrs={b'comment': b'hi!'}``, then
             *filter* ``cattrs={b'comment': b'h'}`` will match.
 
-            By default, ``tgbox.tools.search_generator`` will
+            By default, ``tgbox.api.utils.search_generator`` will
             use an ``in``, like ``b'h' in b'hi!'``, but you
             can set a ``re`` flag to use regular expressions,
             so *filter* ``cattrs={b'comment': b'hi(.)'}`` will match.
 
         * **file_path** *pathlib.Path*, *str*
         * **file_name** *bytes*: File name
         * **file_salt** *bytes*: File salt
@@ -153,14 +182,15 @@
 
         * **mime**     *str*:  File mime type
         * **imported** *bool*: Yield only imported files
         * **re**       *bool*: re_search for every ``bytes``
     """
     def __init__(self, **kwargs):
         self.in_filters = {
+            'scope':     _TypeList(str),
             'cattrs':    _TypeList(dict),
             'file_path': _TypeList(str),
             'file_name': _TypeList(str),
             'file_salt': _TypeList((bytes,str)),
             'verbyte':   _TypeList(bytes),
             'id':        _TypeList(int),
             'min_id':    _TypeList(int),
@@ -449,14 +479,82 @@
 
     return int.to_bytes(int_, length, 'big', signed=signed)
 
 def bytes_to_int(bytes_: bytes, signed: Optional[bool] = False) -> int:
     """Converts bytes to int with Big byteorder."""
     return int.from_bytes(bytes_, 'big', signed=signed)
 
+def guess_path_type(path: Union[str, Path]) -> str:
+    """
+    This function will try to guess file path
+    type. It can be Windows-like or Unix-like
+
+    Returns 'windows' or 'unix'
+    """
+    if PureWindowsPath(path).drive:
+        return 'windows'
+    return 'unix'
+
+def make_general_path(path: Union[str, Path]) -> Path:
+    """
+    This function will make a valid
+    UNIX-like Path from the Windows-like
+    on the UNIX-like systems.
+    """
+    # Windows can support UNIX-like paths
+    if platform_system().lower() == 'windows':
+        return Path(path) if isinstance(path, str) else path
+
+    path = path if isinstance(path, str) else str(path)
+
+    if (win_path := PureWindowsPath(path)).drive:
+        return Path(*win_path.parts)
+
+    return Path(path)
+
+def make_safe_file_path(path: Union[str, Path]) -> Path:
+    """
+    This function will make a safe file path (a
+    file path that can be easily inserted into
+    another path). This is mostly for internal
+    purposes, i.e ``DecryptedRemoteBox.download()``
+
+    This function will make a
+        @/home/non/test from /home/non/test
+        C\\Users\\non\\test from C:\\Users\\non\\test
+
+    ...so this path can be easily inserted into
+    another, i.e DownloadsTGBOX/@/home/non/test
+
+    ``path`` *must* be absolute.
+    """
+    path_type = guess_path_type(path)
+    path = make_general_path(path)
+
+    if path_type == 'unix':
+        # /home/non -> @/home/non
+        if str(path)[0] == '/':
+            return Path(str(path).replace('/','@/',1))
+        else:
+            return Path(str(path).replace('\\','@\\',1))
+
+    elif path_type == 'windows':
+        # C:\Users\user -> C\Users\User
+        drive_letter = path.parts[0][0]
+        return Path(drive_letter, *path.parts[1:])
+
+async def anext(aiterator, default=...):
+    """Analogue to Python 3.10+ anext()"""
+    try:
+        return await aiterator.__anext__()
+    except StopAsyncIteration as e:
+        if default is not Ellipsis:
+            return default
+        raise e
+
 async def get_media_duration(file_path: str) -> int:
     """Returns video/audio duration with ffmpeg in seconds."""
     func = partial(subprocess_run,
         args=[FFMPEG, '-i', file_path],
         stdout=None, stderr=PIPE
     )
     try:
```

### Comparing `tgbox-1.1.1/tgbox.egg-info/PKG-INFO` & `tgbox-1.2/tgbox.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,94 +1,88 @@
 Metadata-Version: 2.1
 Name: tgbox
-Version: 1.1.1
+Version: 1.2
 Summary: Encrypted cloud storage API based on a Telegram API
 Home-page: https://github.com/NonProjects/tgbox
 Author: NonProjects
 Author-email: thenonproton@pm.me
 License: LGPL-2.1
-Download-URL: https://github.com/NonProjects/tgbox/archive/refs/tags/v1.1.1.tar.gz
+Download-URL: https://github.com/NonProjects/tgbox/archive/refs/tags/v1.2.tar.gz
 Description: TGBOX: encrypted cloud storage based on Telegram
         ================================================
-        .. image:: https://readthedocs.org/projects/tgbox/badge/?version=latest
+        .. epigraph::
+                | This repository contains a set of classes and functions used to manage TGBOX.
+                | Try the `tgbox-cli <https://github.com/NotStatilko/tgbox-cli>`__  if you're interested in working implementation!
         
         .. code-block:: python
         
-                from tgbox.api import (
-                    TelegramClient,
-                    make_remotebox,
-                    make_localbox
-                )
                 from asyncio import run as asyncio_run
-                from tgbox.keys import Phrase, make_basekey
                 from getpass import getpass # Hidden input
         
-                # Phone number linked to your Telegram account
-                PHONE_NUMBER = '+10000000000'
+                from tgbox.api import TelegramClient, make_remotebox, make_localbox
+                from tgbox.keys import Phrase, make_basekey
         
                 # This two will not work. Get your own at https://my.telegram.org
                 API_ID, API_HASH = 1234567, '00000000000000000000000000000000'
+                # Simple progress callback to track upload/download state
+                PROGRESS_CALLBACK = lambda c,t: print(round(c/t*100),'%')
         
                 async def main():
+                    phone = input('Phone number: ')
+        
                     tc = TelegramClient(
-                        phone_number = PHONE_NUMBER,
+                        phone_number = phone,
                         api_id = API_ID,
                         api_hash = API_HASH
                     )
-                    await tc.connect() # Connecting with Telegram
+                    await tc.connect() # Connecting to Telegram
                     await tc.send_code() # Requesting login code
         
-                    await tc.log_in(
-                        code = int(input('Code: ')),
-                        password = getpass('Pass: ')
-                    )
-                    # Generating your passphrase
-                    p = Phrase.generate()
-                    print(p.phrase.decode())
+                    code = int(input('Login code: '))
+                    password = getpass('Your password: ')
+        
+                    # Login to your Telegram account
+                    await tc.log_in(password, code)
+        
+                    # Generate and show your Box phrase
+                    print(phrase := Phrase.generate())
         
                     # WARNING: This will use 1GB of RAM for a
                     # couple of seconds. See help(make_basekey)
-                    basekey = make_basekey(p)
+                    basekey = make_basekey(phrase)
+        
+                    erb = await make_remotebox(tc) # Make EncryptedRemoteBox
+                    dlb = await make_localbox(erb, basekey) # Make DecryptedLocalBox
+                    drb = await erb.decrypt(dlb=dlb) # Obtain DecryptedRemoteBox
+        
+                    # Write a file path to upload to your Box
+                    file_to_upload = input('File to upload (path): ')
         
-                    # Make EncryptedRemoteBox
-                    erb = await make_remotebox(tc)
-                    # Make DecryptedLocalBox
-                    dlb = await make_localbox(erb, basekey)
-                    # Obtain DecryptedRemoteBox
-                    drb = await erb.decrypt(dlb=dlb)
-        
-                    # CATTRS is a File's CustomAttributes. You
-                    # can specify any you want. Here we will add
-                    # a "comment" attr with a true statement :^)
-                    cattrs = {'comment': b'Cats are cool B-)'}
-        
-                    # Preparing file for upload. This will return a PreparedFile object
-                    pf = await dlb.prepare_file(open('cats.png','rb'), cattrs=cattrs)
-        
-                    # Uploading PreparedFile to the RemoteBox
-                    # and return DecryptedRemoteBoxFile
-                    drbf = await drb.push_file(pf)
+                    # Preparing for upload. Will return a PreparedFile object
+                    pf = await dlb.prepare_file(open(file_to_upload,'rb'))
+                    # Uploading PreparedFile to Remote and getting DecryptedRemoteBoxFile
+                    drbf = await drb.push_file(pf, progress_callback=PROGRESS_CALLBACK)
         
-                    # Retrieving some info from the RemoteBoxFile
+                    # Retrieving some info from the RemoteBox file
                     print('File size:', drbf.size, 'bytes')
                     print('File name:', drbf.file_name)
         
                     # You can also access all information about
                     # the RemoteBoxFile you need from the LocalBox
                     dlbf = await dlb.get_file(drbf.id)
         
+                    print('File size:', dlbf.size, 'bytes')
                     print('File path:', dlbf.file_path)
-                    print('Custom Attributes:', dlbf.cattrs)
         
-                    # Downloading file back.
-                    await drbf.download()
+                    # Downloading your [already uploaded] file from Remote.
+                    await drbf.download(progress_callback=PROGRESS_CALLBACK)
         
                     # Close all connections
                     # after work was done
-                    await erb.done()
+                    await drb.done()
                     await dlb.done()
         
                 asyncio_run(main())
         
         Motivation
         ----------
         
@@ -117,15 +111,14 @@
            cd tgbox && python3 -m pip install .[doc] # Install with doc
            cd docs && make html && firefox _build/html/index.html
         
         Third party & thanks to
         -----------------------
         - `⭐️ <https://github.com/NonProjects/tgbox/stargazers>`__ **Stargazers!**
         - `Sphinx_rtd_theme <https://github.com/readthedocs/sphinx_rtd_theme>`__ (`MIT <https://github.com/readthedocs/sphinx_rtd_theme/blob/master/LICENSE>`__)
-        - `Regex <https://github.com/mrabarnett/mrab-regex>`__ (`LICENSE <https://github.com/mrabarnett/mrab-regex/blob/hg/LICENSE.txt>`__)
         - `Aiosqlite <https://github.com/omnilib/aiosqlite>`__ (`MIT <https://github.com/omnilib/aiosqlite/blob/main/LICENSE>`__)
         - `Telethon <https://github.com/LonamiWebs/Telethon>`__ (`MIT <https://github.com/LonamiWebs/Telethon/blob/master/LICENSE>`__)
         - `Ecdsa <https://github.com/tlsfuzzer/python-ecdsa>`__ (`LICENSE <https://github.com/tlsfuzzer/python-ecdsa/blob/master/LICENSE>`__)
         - `Filetype <https://github.com/h2non/filetype.py>`__ (`MIT <https://github.com/h2non/filetype.py/blob/master/LICENSE>`__)
         - `Cryptg <https://github.com/cher-nov/cryptg>`__ (`LICENSE <https://github.com/cher-nov/cryptg/blob/master/LICENSE.txt>`__)
         - `Cryptography <https://github.com/pyca/cryptography>`__ (`LICENSE <https://github.com/pyca/cryptography/blob/main/LICENSE>`__)
         
@@ -137,15 +130,15 @@
 Keywords: Telegram,Cloud-Storage,Cloud,API,Asyncio,Non-official
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Archiving :: Backup
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
 Provides-Extra: fast
```

