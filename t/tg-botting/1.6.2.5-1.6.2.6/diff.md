# Comparing `tmp/tg-botting-1.6.2.5.tar.gz` & `tmp/tg-botting-1.6.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg-botting-1.6.2.5.tar", last modified: Tue May 16 20:30:24 2023, max compression
+gzip compressed data, was "tg-botting-1.6.2.6.tar", last modified: Mon May 22 16:44:22 2023, max compression
```

## Comparing `tg-botting-1.6.2.5.tar` & `tg-botting-1.6.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 20:30:24.800221 tg-botting-1.6.2.5/
--rw-rw-rw-   0        0        0      920 2023-05-16 20:30:24.799225 tg-botting-1.6.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      930 2022-12-06 14:18:03.000000 tg-botting-1.6.2.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-16 20:30:24.800221 tg-botting-1.6.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1447 2023-05-16 20:29:58.000000 tg-botting-1.6.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:30:24.794840 tg-botting-1.6.2.5/tg_botting/
--rw-rw-rw-   0        0        0    30186 2023-05-16 20:29:55.000000 tg-botting-1.6.2.5/tg_botting/bot.py
--rw-rw-rw-   0        0        0      976 2023-01-11 17:39:26.000000 tg-botting-1.6.2.5/tg_botting/cog.py
--rw-rw-rw-   0        0        0      995 2022-12-13 21:08:58.000000 tg-botting-1.6.2.5/tg_botting/generals.py
--rw-rw-rw-   0        0        0    15742 2023-05-13 19:27:53.000000 tg-botting-1.6.2.5/tg_botting/objects.py
--rw-rw-rw-   0        0        0       38 2022-12-13 21:06:01.000000 tg-botting-1.6.2.5/tg_botting/user_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 20:30:24.798226 tg-botting-1.6.2.5/tg_botting.egg-info/
--rw-rw-rw-   0        0        0      920 2023-05-16 20:30:24.000000 tg-botting-1.6.2.5/tg_botting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-16 20:30:24.000000 tg-botting-1.6.2.5/tg_botting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 20:30:24.000000 tg-botting-1.6.2.5/tg_botting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-16 20:30:24.000000 tg-botting-1.6.2.5/tg_botting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-16 20:30:24.000000 tg-botting-1.6.2.5/tg_botting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 16:44:22.235522 tg-botting-1.6.2.6/
+-rw-rw-rw-   0        0        0      920 2023-05-22 16:44:22.235522 tg-botting-1.6.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      930 2022-12-06 14:18:03.000000 tg-botting-1.6.2.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 16:44:22.235522 tg-botting-1.6.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1447 2023-05-22 16:05:50.000000 tg-botting-1.6.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:44:22.229538 tg-botting-1.6.2.6/tg_botting/
+-rw-rw-rw-   0        0        0    30372 2023-05-22 16:43:44.000000 tg-botting-1.6.2.6/tg_botting/bot.py
+-rw-rw-rw-   0        0        0      976 2023-01-11 17:39:26.000000 tg-botting-1.6.2.6/tg_botting/cog.py
+-rw-rw-rw-   0        0        0      995 2022-12-13 21:08:58.000000 tg-botting-1.6.2.6/tg_botting/generals.py
+-rw-rw-rw-   0        0        0    15742 2023-05-13 19:27:53.000000 tg-botting-1.6.2.6/tg_botting/objects.py
+-rw-rw-rw-   0        0        0       38 2022-12-13 21:06:01.000000 tg-botting-1.6.2.6/tg_botting/user_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:44:22.234525 tg-botting-1.6.2.6/tg_botting.egg-info/
+-rw-rw-rw-   0        0        0      920 2023-05-22 16:44:22.000000 tg-botting-1.6.2.6/tg_botting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-22 16:44:22.000000 tg-botting-1.6.2.6/tg_botting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:44:22.000000 tg-botting-1.6.2.6/tg_botting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-22 16:44:22.000000 tg-botting-1.6.2.6/tg_botting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 16:44:22.000000 tg-botting-1.6.2.6/tg_botting.egg-info/top_level.txt
```

### Comparing `tg-botting-1.6.2.5/PKG-INFO` & `tg-botting-1.6.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 1.6.2.5
+Version: 1.6.2.6
 Summary: python library for easy creation of a telegram bot.
 Home-page: https://github.com/2sweetheart2/tg_botting/tree/master
 Author: Sweetie (Roma Fomkin)
 Author-email: <2004sweetheart2004@gmail.com>
 Keywords: python,bot,tg,tg bot,telegram,telegram bot,botting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `tg-botting-1.6.2.5/README.md` & `tg-botting-1.6.2.6/README.md`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.2.5/setup.py` & `tg-botting-1.6.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.6.2.5'
+VERSION = '1.6.2.6'
 DESCRIPTION = 'python library for easy creation of a telegram bot.'
 LONG_DESCRIPTION = 'A package that allows you to create bots for telegram using its entire API.'
 
 setup(
     name="tg-botting",
     version=VERSION,
     url='https://github.com/2sweetheart2/tg_botting/tree/master',
```

### Comparing `tg-botting-1.6.2.5/tg_botting/bot.py` & `tg-botting-1.6.2.6/tg_botting/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import traceback
 from inspect import signature
 
 import aiohttp
 import pyrogram
 import requests
 from pyrogram import Client
+from pyrogram.errors import UsernameInvalid
 from pyrogram.errors.exceptions import bad_request_400
 
 from . import generals
 from .cog import Cog
 from .objects import Message, ChatActions, UserProfilePicture, CallbackQuery, Command, ChatPermission, \
     PromotePermission, PreCheckOutQuery, Chat, User
 
@@ -620,60 +621,65 @@
         for arg in args:
             try:
                 data.append(int(arg))
                 continue
             except:
                 pass
             if arg[0] == '@':
-                data.append(await User.load(arg,self))
+                try:
+                    data.append(await User.load(arg,self))
+                except UsernameInvalid:
+                    data.append(None)
                 continue
             data.append(arg)
         return data
 
     async def tupe_error(self,message, arg,need_type):
         type = need_type
         if need_type==int:
             type = 'число'
         elif need_type==str:
             type = 'строка'
         elif need_type==User:
             type = 'пользователь'
+
+        if isinstance(arg,User):
+            arg='пользователь'
         await message.reply(self.type_error_message.format(arg,type))
 
 
     async def dispatch(self, message):
         if self.has_prefix(message):
             ms = message.text.split()
             ms.pop(0)
             rs, c, from_aliases = self.search(' '.join(ms))
             if rs:
                 for i in range(c):
                     ms.pop(0)
                 args = await self.get_args(ms)
                 need_args = signature(rs.func)
                 put_args = []
-                minus = 1
                 na = dict(need_args.parameters)
                 if 'self' in na.keys():
                     na.pop('self')
                 try:
                     na.pop(list(na.keys())[0])
                 except:
                     print("ERROR: ",na,'\n','put_args: ',put_args,'\nargs: ',args,rs)
                 try:
                     for i in range(0,len(na)):
                         val = list(na.values())[i]
                         try:
                             if val.annotation != inspect.Parameter.empty:
-                                if not isinstance(args[i-minus],val.annotation):
-                                    return await self.tupe_error(message,args[i-minus],val.annotation)
+                                if not isinstance(args[i],val.annotation):
+                                    return await self.tupe_error(message,args[i],val.annotation)
                         except IndexError as e:
                             put_args.append(None)
                             continue
-                        put_args.append(args[i-minus])
+                        put_args.append(args[i])
                         ms.pop(0)
                 except:
                     print("ERROR2: ",na,'\n','put_args: ',put_args,'\nargs: ',args,rs)
 
                 message.text = ' '.join(ms)
                 setattr(message, 'texts', ms)
                 if len(self.chat_filter) > 0:
```

### Comparing `tg-botting-1.6.2.5/tg_botting/cog.py` & `tg-botting-1.6.2.6/tg_botting/cog.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.2.5/tg_botting/generals.py` & `tg-botting-1.6.2.6/tg_botting/generals.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.2.5/tg_botting/objects.py` & `tg-botting-1.6.2.6/tg_botting/objects.py`

 * *Files identical despite different names*

### Comparing `tg-botting-1.6.2.5/tg_botting.egg-info/PKG-INFO` & `tg-botting-1.6.2.6/tg_botting.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tg-botting
-Version: 1.6.2.5
+Version: 1.6.2.6
 Summary: python library for easy creation of a telegram bot.
 Home-page: https://github.com/2sweetheart2/tg_botting/tree/master
 Author: Sweetie (Roma Fomkin)
 Author-email: <2004sweetheart2004@gmail.com>
 Keywords: python,bot,tg,tg bot,telegram,telegram bot,botting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

