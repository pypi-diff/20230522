# Comparing `tmp/nonebot-plugin-clock-0.8.8.tar.gz` & `tmp/nonebot-plugin-clock-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nonebot-plugin-clock-0.8.8.tar", last modified: Fri Apr 14 05:16:16 2023, max compression
+gzip compressed data, was "dist/nonebot-plugin-clock-0.9.tar", last modified: Mon May 22 02:05:53 2023, max compression
```

## Comparing `nonebot-plugin-clock-0.8.8.tar` & `nonebot-plugin-clock-0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/
--rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.8/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.8.8/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     1462 2023-04-13 03:19:28.000000 nonebot-plugin-clock-0.8.8/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock/
--rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock/Clock.py
--rw-r--r--   0 mac        (501) staff       (20)     6182 2023-04-13 09:30:23.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1972 2023-04-14 05:16:05.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock/database.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)      303 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      370 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       21 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/nonebot_plugin_clock.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.8.8/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-04-14 05:16:16.000000 nonebot-plugin-clock-0.8.8/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      552 2023-04-14 05:15:40.000000 nonebot-plugin-clock-0.8.8/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-22 02:05:53.000000 nonebot-plugin-clock-0.9/
+-rw-r--r--   0 mac        (501) staff       (20)     1067 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.9/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)       42 2023-04-12 10:33:21.000000 nonebot-plugin-clock-0.9/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)      301 2023-05-22 02:05:53.000000 nonebot-plugin-clock-0.9/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     1462 2023-04-13 03:19:28.000000 nonebot-plugin-clock-0.9/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-22 02:05:53.000000 nonebot-plugin-clock-0.9/nonebot_plugin_clock/
+-rw-r--r--   0 mac        (501) staff       (20)     1766 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.9/nonebot_plugin_clock/Clock.py
+-rw-r--r--   0 mac        (501) staff       (20)     6246 2023-05-22 01:15:52.000000 nonebot-plugin-clock-0.9/nonebot_plugin_clock/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     2046 2023-05-22 02:00:59.000000 nonebot-plugin-clock-0.9/nonebot_plugin_clock/database.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-22 02:05:53.000000 nonebot-plugin-clock-0.9/nonebot_plugin_clock.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)      301 2023-05-22 02:05:53.000000 nonebot-plugin-clock-0.9/nonebot_plugin_clock.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      370 2023-05-22 02:05:53.000000 nonebot-plugin-clock-0.9/nonebot_plugin_clock.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-22 02:05:53.000000 nonebot-plugin-clock-0.9/nonebot_plugin_clock.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-05-22 02:05:53.000000 nonebot-plugin-clock-0.9/nonebot_plugin_clock.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)       21 2023-05-22 02:05:53.000000 nonebot-plugin-clock-0.9/nonebot_plugin_clock.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       85 2023-04-12 07:04:41.000000 nonebot-plugin-clock-0.9/requirements.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-05-22 02:05:53.000000 nonebot-plugin-clock-0.9/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      550 2023-05-22 02:05:24.000000 nonebot-plugin-clock-0.9/setup.py
```

### Comparing `nonebot-plugin-clock-0.8.8/LICENSE` & `nonebot-plugin-clock-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.8/README.md` & `nonebot-plugin-clock-0.9/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.8/nonebot_plugin_clock/Clock.py` & `nonebot-plugin-clock-0.9/nonebot_plugin_clock/Clock.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-clock-0.8.8/nonebot_plugin_clock/__init__.py` & `nonebot-plugin-clock-0.9/nonebot_plugin_clock/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,54 @@
 import re
 
 from datetime import datetime, timedelta
 from nonebot.permission import SUPERUSER
-from nonebot import on_command, on_regex ,get_bot, get_driver
-from nonebot.adapters.onebot.v11.bot import Bot
-from nonebot.adapters.onebot.v11.event import Event
-from nonebot.adapters.onebot.v11.message import Message, MessageSegment
-from nonebot.params import CommandArg
+from nonebot import on_command, on_regex ,get_bot, get_driver, require
 from nonebot.typing import T_State
-from nonebot import require
+from nonebot.matcher import Matcher
+from nonebot.params import CommandArg
+from nonebot.adapters.onebot.v11.bot import Bot
+from nonebot.adapters.onebot.v11 import MessageEvent, GroupMessageEvent, Message
+
+
+
 
 from .database import db
 from .Clock import Clock
 
 scheduler = require('nonebot_plugin_apscheduler').scheduler
 
 WHITELIST = getattr(get_driver().config, 'clock_white_list', [])
 BLACKLIST = getattr(get_driver().config, 'clock_black_list', [])
 CLOCK_DATA = {}
 
-async def CLOCK_RULE(event: Event) -> bool:
+
+del_clock_qq = on_command('删除闹钟', block=True)
+add_clock_qq = on_command('添加闹钟', aliases={'设置闹钟',}, block=True)
+
+async def CLOCK_RULE(bot: Bot, event: MessageEvent) -> bool:
     
+    ret = await SUPERUSER(bot, event)
+    if ret: return True
+
     # 黑名单优先判定
     if BLACKLIST:
         return event.user_id not in BLACKLIST
     
     if WHITELIST:
         if event.sender.role == "member" and event.user_id not in WHITELIST:
             return False
         
     return True
 
-
+def get_event_info( event: MessageEvent ):
+    if isinstance(event, GroupMessageEvent):
+        return ('group', event.group_id)
+    else:
+        return ('private', event.user_id)
 
 def create_clock_scheduler(clock):
     '''
     创建闹钟任务
     '''
     CLOCK_DATA[clock.id] = clock
 
@@ -101,48 +114,43 @@
             m = f'0{m}' if len(m)==1 else m
             t = f'{h}:{m}'
 
     return t
         
 
 # 创建闹钟
-add_clock_qq = on_command('添加闹钟', aliases={'设置闹钟',})
 @add_clock_qq.handle()
-async def _(bot: Bot, event: Event, state: T_State, messages: Message = CommandArg()):
+async def _(matcher: Matcher, bot: Bot, event: MessageEvent, state: T_State, messages: Message = CommandArg()):
     
     messages = str(messages).split(' ', 1)
 
     if len(messages) < 2:
-        await add_clock_qq.finish(message="添加格式为: “添加闹钟 时间 内容”")
+        await matcher.finish(message="添加格式为: “添加闹钟 时间 内容”")
 
     time_ = get_time(messages[0])
     if not time_:
-        await add_clock_qq.finish(message="时间格式错误")
+        await matcher.finish(message="时间格式错误")
 
     state['time'] = time_
-    state['type'] = 'private'
-    state['user'] = event.user_id
+    state['type'], state['user'] = get_event_info(event)
     state['content'] = messages[1] if messages[1] else '⏰'
 
-    if 'group' in event.get_event_name():
-        res1 = await SUPERUSER(bot, event)
-        res2 = await CLOCK_RULE(event)
-        if not (res1 or res2):
-            await add_clock_qq.finish(message="你没有该权限哦～")
-        state['type'] = 'group'
-        state['user'] = event.group_id
+    if state['type'] == 'group':
 
-    
+        ret = await CLOCK_RULE(bot, event)
+        if not ret:
+            await matcher.finish(message="你没有该权限哦～")
 
 
-@add_clock_qq.got('ones', prompt="⏰不重复, 设置为每日输入[Y/y]\n设置周几 如周一周三输入[13]\n设置某天，如圣诞输入 [12.25]")
-async def _(bot: Bot, event: Event, state: T_State):
+
+@add_clock_qq.got('ones', prompt="⏰设置不重复输入[N/n]\n⏰设置为每日输入[Y/y]\n⏰设置周几 如周一周三输入[13]\n⏰设置某天，如圣诞输入 [12.25]")
+async def _(matcher: Matcher, state: T_State):
 
     state['ones'] = str(state['ones'])
-    ones = 0 if state['ones'] in ['Y', 'y'] else 1
+    ones = 0 if state['ones'] in ['Y', 'y'] else 1 # Y,y之外的非数字 都设置一次性
     month, day = 0, 0
     week = ''
 
     if state['ones'].isdigit():
         week = state['ones']
         ones = 0
 
@@ -158,27 +166,25 @@
         'week' : week,
         'day' : day,
         'month' : month
     }
        
     add_clock(**data)
     ones_ = {1:'不重复', 0:'重复'}
-    await add_clock_qq.finish(message=f"[{ones_[ones]}]添加成功～")
+    await matcher.finish(message=f"[{ones_[ones]}]添加成功～")
 
 
 
 
 # # 查看闹钟
 check = on_regex("^(查看闹钟|提醒事项|闹钟|⏰)$" ,block=True)
 @check.handle()
-async def _(bot: Bot, event: Event):
-
-    uid = event.group_id if 'group' in event.get_event_name() else event.user_id 
-
+async def _(matcher: Matcher, event: MessageEvent):
 
+    _, uid = get_event_info(event)
     def check_(msg: str) -> str:
 
         message = ""
         for m in Message(msg):
             if m.type == 'at':
                 message += f"@{m.data['qq']}"
             else:
@@ -188,29 +194,27 @@
     clock_msg = []
     for id in CLOCK_DATA:
         clock = CLOCK_DATA[id]
         if clock.user == uid:
             clock_msg.append(check_(clock.get_info()))
 
     if clock_msg:
-        await bot.send(event, message= Message('\n'.join(clock_msg)))
+        await matcher.finish(message= Message('\n'.join(clock_msg)))
     else:
-        await bot.send(event, message='目前没有闹钟')
+        await matcher.finish(message='目前没有闹钟')
     
 
 
 # 删除闹钟
-del_ = on_command('删除闹钟', block=True)
-@del_.handle()
-async def _(bot: Bot, event: Event, ids = CommandArg()):
-    ids = str(ids).split()
-    
-    if ids:
-        uid = event.group_id if 'group' in event.get_event_name() else event.user_id 
-        task = [[],[]]
-        for id in ids:
-            id = int(id)
-            if del_clock(id, uid):
-                task[0].append(id) # succeed
-            else:
-                task[1].append(id) # fail
-        await del_.finish(message=f'删除闹钟{task[0]}'+ f'\n不存在的id{task[1]}' if task[1] else '')
+@del_clock_qq.handle()
+async def _(matcher: Matcher, event: MessageEvent, ids = CommandArg()):
+
+    _, uid = get_event_info(event)
+    task = [[],[]]
+
+    for id in str(ids).split():
+        id = int(id)
+        if del_clock(id, uid):
+            task[0].append(id) # succeed
+        else:
+            task[1].append(id) # fail
+    await matcher.finish(message=f'删除闹钟{task[0]}'+ f'\n不存在的id{task[1]}' if task[1] else '')
```

### Comparing `nonebot-plugin-clock-0.8.8/nonebot_plugin_clock/database.py` & `nonebot-plugin-clock-0.9/nonebot_plugin_clock/database.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-
 import os
 import sqlite3
+from nonebot.log import logger
+
 from .Clock import Clock
 
 TABLE = "CLOCKS"
 db_ = os.path.dirname(__file__) + '/data.sqlite'
-
+logger.info(f"CLOCK DB: {db_}")
 
 if not os.path.exists(db_):
     
     conn = sqlite3.connect(db_)
 
     c = conn.cursor()
     try:
@@ -20,17 +21,17 @@
             content VARCHAR(20),
             month INTEGER,
             day INTEGER,
             week VARCHAR(7),
             c_time TIME,
             ones INTEGER NOT NULL);
         ''')
-        print('create db')
+        logger.info('create db')
     except:
-        print('create db fail ...')
+        logger.info('create db fail ...')
 
     conn.commit()
     conn.close()
     
 
 class DB:
     def __init__(self, db, table):
@@ -64,11 +65,11 @@
         '''
         #DataFrame(data = data, columns=['id', 'type', 'uid', 'note', 'time', 'omes'])
         return self.execute(f"SELECT * FROM {self.table};")
 
         
     def new_id(self):
         res = self.execute(f"SELECT max(id) FROM {self.table};")
-        return res[0][0] + 1 if res[0][0] else 0
+        return res[0][0] + 1 if res[0][0] else 1
 
 
 db = DB(db_, TABLE)
```

### Comparing `nonebot-plugin-clock-0.8.8/setup.py` & `nonebot-plugin-clock-0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding: utf-8
 
 from setuptools import setup
 requirements = [r.strip() for r in open("requirements.txt", 'r', encoding='utf-8').readlines()]
 
 setup(
     name='nonebot-plugin-clock',
-    version='0.8.8',
+    version='0.9',
     author='Zeta',
     author_email='',
     long_description="https://github.com/Zeta-qixi/nonebot-plugin-clock",
     license="MIT Licence",
     url='https://github.com/Zeta-qixi/nonebot-plugin-clock/',
     description='nonebot_plugin about clock',
     packages=['nonebot_plugin_clock'],
```

