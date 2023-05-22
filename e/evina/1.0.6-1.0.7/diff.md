# Comparing `tmp/evina-1.0.6.tar.gz` & `tmp/evina-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\evina-1.0.6.tar", last modified: Sun May  7 16:06:11 2023, max compression
+gzip compressed data, was "evina-1.0.7.tar", last modified: Mon May 22 09:58:45 2023, max compression
```

## Comparing `evina-1.0.6.tar` & `evina-1.0.7.tar`

### file list

```diff
@@ -1,27 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 16:06:11.386566 evina-1.0.6/
--rw-rw-rw-   0        0        0     1083 2023-05-02 16:19:36.000000 evina-1.0.6/LICENSE
--rw-rw-rw-   0        0        0       47 2023-05-07 06:53:08.000000 evina-1.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0       90 2023-05-07 16:06:11.384567 evina-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1349 2023-05-02 16:19:36.000000 evina-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 16:06:11.251625 evina-1.0.6/evina/
--rw-rw-rw-   0        0        0       90 2023-05-07 06:53:08.000000 evina-1.0.6/evina/__init__.py
--rw-rw-rw-   0        0        0      720 2023-05-07 06:53:08.000000 evina-1.0.6/evina/alipan.py
--rw-rw-rw-   0        0        0     4991 2023-05-07 16:05:10.000000 evina-1.0.6/evina/config.py
-drwxrwxrwx   0        0        0        0 2023-05-07 16:06:11.381574 evina-1.0.6/evina/disposition/
--rw-rw-rw-   0        0        0        0 2023-05-07 06:53:08.000000 evina-1.0.6/evina/disposition/__init__.py
--rw-rw-rw-   0        0        0     1135 2023-05-07 13:48:35.000000 evina-1.0.6/evina/disposition/config.conf
--rw-rw-rw-   0        0        0      101 2023-05-07 06:53:08.000000 evina-1.0.6/evina/disposition/evina.conf
--rw-rw-rw-   0        0        0    14673 2023-05-07 15:32:16.000000 evina-1.0.6/evina/douyin.py
--rw-rw-rw-   0        0        0    10237 2023-05-07 15:35:33.000000 evina-1.0.6/evina/douyu.py
--rw-rw-rw-   0        0        0     1641 2023-05-07 15:59:50.000000 evina-1.0.6/evina/evina.py
--rw-rw-rw-   0        0        0      955 2023-05-05 16:33:43.000000 evina-1.0.6/evina/replacement.py
--rw-rw-rw-   0        0        0     1342 2023-05-07 06:53:08.000000 evina-1.0.6/evina/ssh.py
-drwxrwxrwx   0        0        0        0 2023-05-07 16:06:11.362649 evina-1.0.6/evina.egg-info/
--rw-rw-rw-   0        0        0       90 2023-05-07 16:06:11.000000 evina-1.0.6/evina.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2023-05-07 16:06:11.000000 evina-1.0.6/evina.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 16:06:11.000000 evina-1.0.6/evina.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-07 16:06:11.000000 evina-1.0.6/evina.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       37 2023-05-07 16:06:11.000000 evina-1.0.6/evina.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-07 16:06:11.000000 evina-1.0.6/evina.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 16:06:11.386566 evina-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      477 2023-05-07 16:05:59.000000 evina-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:58:44.964893 evina-1.0.7/
+-rw-rw-rw-   0        0        0      187 2023-05-22 09:58:44.958913 evina-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2023-05-02 16:19:36.000000 evina-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 09:58:44.851011 evina-1.0.7/evina/
+-rw-rw-rw-   0        0        0       90 2023-05-07 06:53:08.000000 evina-1.0.7/evina/__init__.py
+-rw-rw-rw-   0        0        0      720 2023-05-07 06:53:08.000000 evina-1.0.7/evina/alipan.py
+-rw-rw-rw-   0        0        0     5740 2023-05-22 08:58:35.000000 evina-1.0.7/evina/config.py
+-rw-rw-rw-   0        0        0    14557 2023-05-22 08:58:48.000000 evina-1.0.7/evina/douyin.py
+-rw-rw-rw-   0        0        0     9388 2023-05-22 08:58:56.000000 evina-1.0.7/evina/douyu.py
+-rw-rw-rw-   0        0        0     1461 2023-05-22 08:59:28.000000 evina-1.0.7/evina/evina.py
+-rw-rw-rw-   0        0        0      980 2023-05-22 08:59:44.000000 evina-1.0.7/evina/replacement.py
+-rw-rw-rw-   0        0        0     1342 2023-05-07 06:53:08.000000 evina-1.0.7/evina/ssh.py
+drwxrwxrwx   0        0        0        0 2023-05-22 09:58:44.950919 evina-1.0.7/evina.egg-info/
+-rw-rw-rw-   0        0        0      187 2023-05-22 09:58:44.000000 evina-1.0.7/evina.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-22 09:58:44.000000 evina-1.0.7/evina.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 09:58:44.000000 evina-1.0.7/evina.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-22 09:58:44.000000 evina-1.0.7/evina.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2023-05-22 09:58:44.000000 evina-1.0.7/evina.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-22 09:58:44.000000 evina-1.0.7/evina.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 09:58:44.965890 evina-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      477 2023-05-22 09:00:51.000000 evina-1.0.7/setup.py
```

### Comparing `evina-1.0.6/README.md` & `evina-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `evina-1.0.6/evina/alipan.py` & `evina-1.0.7/evina/alipan.py`

 * *Files identical despite different names*

### Comparing `evina-1.0.6/evina/config.py` & `evina-1.0.7/evina/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,52 +17,67 @@
 from evina import replacement
 
 
 class Conf:
     def __init__(self) -> None:
         replacement.DotEnv._get_stream = replacement.ReplaceMent.new_get_stream
         conf_file = os.path.join(
-            os.path.abspath(os.path.join(os.path.dirname(__file__))),
-            'disposition', 'config.conf')
+            os.path.join(os.environ.get('HOME'), '.evina', 'config.conf'))
+        if not os.path.exists(conf_file):
+            logger.error(
+                ' 未发现配置文件 config.conf | 请输入: wget -O ~/.evina/config.conf https://raw.githubusercontent.com/Softcute-Ezong/type/main/evina/config.conf'
+            )
+            sys.exit()
         evina_file = os.path.join(
-            os.path.abspath(os.path.join(os.path.dirname(__file__))),
-            'disposition', 'evina.conf')
+            os.path.join(os.environ.get('HOME'), '.evina', 'evina.conf'))
+        if not os.path.exists(evina_file):
+            logger.error(
+                ' 未发现配置文件 evina.conf | 请输入: wget -O ~/.evina/evina.conf https://raw.githubusercontent.com/Softcute-Ezong/type/main/evina/evina.conf'
+            )
+            sys.exit()
 
         parse = argparse.ArgumentParser()
         parse.add_argument('--start', '-s', nargs=1, help='选择需要录制的平台。')
         parse.add_argument('--url', '-u', nargs='*', help='需要录制的直播间URL/ID。')
         parse.add_argument('--name', '-n', nargs='*', help='自定义文件夹名称')
         self.arg = parse.parse_args()
 
-        self.default = Dynaconf(envvar_prefix='evina',
-                                load_dotenv=True,
-                                dotenv_path=conf_file,
-                                dotenv_override=False)
-
         self.conf = Dynaconf(envvar_prefix='evina',
                              load_dotenv=True,
                              dotenv_path=conf_file,
                              dotenv_override=True)
 
         self.evina_douyu = Dynaconf(envvar_prefix='douyu',
                                     load_dotenv=True,
                                     dotenv_path=evina_file,
                                     dotenv_override=True)
 
         self.evina_douyin = Dynaconf(envvar_prefix='douyin',
                                      load_dotenv=True,
                                      dotenv_path=evina_file,
                                      dotenv_override=True)
-
-        replacement.Auth._EMAIL_USER = self.default.settings.email_user
-        replacement.Auth._EMAIL_PASSWORD = self.default.settings.email_password
-        email_host = self.default.settings.email_user.split('@')[1].split('.')
-        replacement.Auth._EMAIL_HOST = 'smtp.{}.{}'.format(
-            email_host[0], email_host[1])
-        Aligo(email=(self.default.settings.email_user, '阿里云盘登录二维码验证'))
+        if self.conf.settings.email_user == 'XXXXXX':
+            logger.error(
+                " 未配置验证邮箱 | 修改 config.conf EVINA_SETTINGS__EMAIL_USER = 'XXXXXX'"
+            )
+            sys.exit()
+        if self.conf.settings.email_password == 'XXXXXX':
+            logger.error(
+                " 未配置邮箱 SMTP | 修改 config.conf EVINA_SETTINGS__EMAIL_PASSWORD = 'XXXXXX'"
+            )
+            sys.exit()
+        email_host = self.conf.settings.email_user.split('@')[1].split('.')
+        email_config = replacement.EMailConfig(
+            email=self.conf.settings.email_user,
+            host='smtp.{}.{}'.format(email_host[0], email_host[1]),
+            port=465,
+            password=self.conf.settings.email_password,
+            user=self.conf.settings.email_user,
+            content='阿里云盘登录二维码验证')
+        Aligo(email=email_config)
 
 
 class Arg(Conf):
     def __init__(self) -> None:
         super().__init__()
         if self.arg.start != None:
             self.start = self.arg.start[0]
```

### Comparing `evina-1.0.6/evina/douyin.py` & `evina-1.0.7/evina/douyin.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,22 +22,21 @@
 import requests
 from evina import ssh
 from faker import Faker
 from loguru import logger
 
 
 class Douyin:
-    def __init__(self, name, settings, default_settings, uid=None):
+    def __init__(self, name, settings, uid=None):
         logger.info('线程创建成功 | 线程名 - {} | PID - {}'.format(
             threading.current_thread().name,
             threading.current_thread().ident))
         self.name = name
         self.settings = settings
-        self.default_settings = default_settings
-        self.open = self.default_settings.open
+        self.open = self.settings.open
         self.ua = Faker(locale="zh_CN").user_agent()
 
         if uid == None:
             sys.exit()
         if uid.endswith('/'):
             uid = uid.rsplit('/', 1)[0]
         uid = uid.rsplit('/', 1)
@@ -87,16 +86,16 @@
             for key, value in flv_pull_url.items():
                 flv_list.append(value)
             hls_pull_url_map = stream_url['hls_pull_url_map']
             for key, value in hls_pull_url_map.items():
                 m3u8_list.append(value)
             list = flv_list + m3u8_list
             time = datetime.datetime.now().ctime().replace(':', '-')
-            if 'FILE' in self.default_settings.keys() and self.default_settings.file != '':
-                file = os.path.join(self.default_settings.file, 'download', '抖音录播',
+            if 'FILE' in self.settings.keys() and self.settings.file != '':
+                file = os.path.join(self.settings.file, 'download', '抖音录播',
                                     name, time)
             else:
                 file = os.path.join(os.getcwd(), 'download', '抖音录播', name,
                                     time)
             ali_file = os.path.join('录播', '抖音录播', name,
                                     time).replace('\\', '/')
             if not os.path.exists(file):
@@ -112,25 +111,25 @@
                 logger.info('抖音直播间 - {} - {} | 已成功保存直播源地址到文件'.format(
                     name,
                     url.rsplit('/', 1)[1]))
             if self.open:
                 logger.info('抖音直播间 - {} - {} 开始录制'.format(
                     name,
                     url.rsplit('/', 1)[1]))
-                if self.default_settings.docker == False:
+                if self.settings.docker == False:
                     subout = subprocess.run(
                         "ffmpeg -i " + '"{}"'.format(list[0]) +
                         " -c:a copy -c:v copy -bsf:a aac_adtstoasc -threads {} -preset {} -f {}  -f segment -segment_time {} -strftime 1 "
                         .format(str(self.settings.thread),
                                 self.settings.preset, self.settings.scheme,
                                 str(self.settings.time)) +
                         '"{}"'.format(
                             os.path.join(file, '%Y-%m-%d-%H-%M-%S.ts')))
                     logger.info(subout)
-                if self.default_settings.docker == True:
+                if self.settings.docker == True:
                     ssh.Ssh(list[0], os.path.join(file,
                                                   '%Y-%m-%d-%H-%M-%S.ts'),
                             self.settings)
                     alipan.Backup(local_file=file, ali_file=ali_file)
                     shutil.rmtree(
                         os.path.join(
                             os.path.abspath(
```

### Comparing `evina-1.0.6/evina/douyu.py` & `evina-1.0.7/evina/douyu.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,29 +13,28 @@
 import re
 import shutil
 import subprocess
 import sys
 import threading
 import time
 
+from evina import alipan
 import requests
+from evina import ssh
 from faker import Faker
 from loguru import logger
 
-from evina import alipan, ssh
-
 
 class Douyu:
-    def __init__(self, rid, name, settings, default_settings):
+    def __init__(self, rid, name, settings):
         logger.info('线程创建成功 | 线程名 - {} | PID - {}'.format(
             threading.current_thread().name,
             threading.current_thread().ident))
         self.settings = settings
-        self.default_settings = default_settings
-        self.open = self.default_settings.open
+        self.open = self.settings.open
         self.name = name
         self.rid = rid
         self.ua = Faker(locale="zh_CN").user_agent()
         try:
             self.api()
         except:
             self.data = self.js()
@@ -50,16 +49,16 @@
         if self.response['state'] == 'SUCCESS':
             if self.name == None:
                 filename = self.response['Rendata']['data']['nickname']
             else:
                 filename = self.name
             # time = str(datetime.datetime.now().strftime('%Y-%m-%d-%H-%M-%S'))
             time = datetime.datetime.now().ctime().replace(':', '-')
-            if 'FILE' in self.default_settings.keys() and self.default_settings.file != '':
-                file = os.path.join(self.default_settings.file, 'download', '斗鱼录播',
+            if 'FILE' in self.settings.keys() and self.settings.file != '':
+                file = os.path.join(self.settings.file, 'download', '斗鱼录播',
                                     filename, time)
             else:
                 file = os.path.join(os.getcwd(), 'download', '斗鱼录播', filename,
                                     time)
             ali_file = os.path.join('录播', '斗鱼录播', filename,
                                     time).replace('\\', '/')
             if not os.path.exists(file):
@@ -71,25 +70,25 @@
             logger.info('斗鱼直播间 - {} | 源地址为 - {}'.format(self.rid, link))
             if self.open == False:
                 logger.info('斗鱼直播间 - {} - {} | 已成功保存直播源地址到文件'.format(
                     filename, self.rid))
 
             if self.open:
                 logger.info('斗鱼直播间 - {} - {} 开始录制'.format(filename, self.rid))
-                if self.default_settings.docker == False:
+                if self.settings.docker == False:
                     subout = subprocess.run(
                         "ffmpeg -i " + '"{}"'.format(link) +
                         " -c:a copy -c:v copy -bsf:a aac_adtstoasc -threads {} -preset {} -f {}  -f segment -segment_time {} -strftime 1 "
                         .format(str(self.settings.thread),
                                 self.settings.preset, self.settings.scheme,
                                 str(self.settings.time)) +
                         '"{}"'.format(
                             os.path.join(file, '%Y-%m-%d-%H-%M-%S.ts')))
                     logger.info(subout)
-                if self.default_settings.docker == True:
+                if self.settings.docker == True:
                     ssh.Ssh(link, os.path.join(file, '%Y-%m-%d-%H-%M-%S.ts'),
                             self.settings)
                     alipan.Backup(local_file=file, ali_file=ali_file)
                     shutil.rmtree(
                         os.path.join(
                             os.path.abspath(
                                 os.path.join(os.path.dirname(__file__), '..')),
@@ -99,34 +98,30 @@
         file = os.path.join(
             os.path.dirname(__file__),
             str(datetime.datetime.now()).replace(':', '-') + '.js')
         jstime = str(int(time.time()))
         did = '10000000000000000000000000001501'
         url = 'https://www.douyu.com/{}'.format(self.rid)
         response = requests.get(url=url)
-        try:
-            self.rid = re.findall(r'ROOM.room_id =(\d+)', response.text,
-                                  re.S)[0]
-        except:
-            self.rid = re.findall(r'ROOM.room_id = (\d+)', response.text,
-                                  re.S)[0]
+        try:self.rid = re.findall(r'ROOM.room_id =(\d+)', response.text, re.S)[0]
+        except:self.rid = re.findall(r'ROOM.room_id = (\d+)', response.text, re.S)[0]
         jsdate = re.findall(
             r'<script type="text/javascript">.*?var vdwdae325w_64we = .*?;(.*?)</script>',
             response.text, re.S)[0]
         # js = 'module.paths.push("D:/node/node_modules");const CryptoJS = require("crypto-js");' + jsdate + \
         #     "let arguments=process.argv.splice(2).join('').split(',');for(var i = 0; i < arguments.length; i++) {}console.log(ub98484234(arguments[0],arguments[1],arguments[2]))"
-        js = 'module.paths.push("{}");const CryptoJS = require("crypto-js");'.format(self.default_settings.node_modules) + jsdate + \
+        js = 'module.paths.push("{}");const CryptoJS = require("crypto-js");'.format(self.settings.node_modules) + jsdate + \
             "let arguments=process.argv.splice(2).join('').split(',');for(var i = 0; i < arguments.length; i++) {}console.log(ub98484234(arguments[0],arguments[1],arguments[2]))"
         js = js.replace(';', ';\n').replace('}', '}\n')
         f = open(file=file, mode='w', encoding='utf8')
         f.write(js)
         f.close()
         # thenum = os.popen('{} "{}" {},{},{}'.format(os.path.join('D:\\', 'node', 'node.exe'), file, self.rid, did, jstime)).read().replace('\n', '')
         thenum = os.popen(
-            '{} "{}" {},{},{}'.format(self.default_settings.nodejs, file, self.rid,
+            '{} "{}" {},{},{}'.format(self.settings.nodejs, file, self.rid,
                                       did, jstime)).read().replace('\n', '')
         dict = {
             'cdn': '',
             'rate': '-1',
             'iar': '1',
             'ive': '0',
             'hevc': '0',
@@ -153,59 +148,48 @@
             self.ua
         }
         response = requests.post(url=url, headers=headers, data=self.data)
         if response.status_code != 200:
             logger.info('斗鱼直播间 - {} | 暂未开播'.format(self.rid))
             sys.exit()
         data = json.loads(response.text)
-        if '房间未开播' in data.values():
-            logger.info('斗鱼直播间 - {} | 暂未开播'.format(self.rid))
-            sys.exit()
+        if '房间未开播' in data.values():logger.info('斗鱼直播间 - {} | 暂未开播'.format(self.rid));sys.exit()
         rtmp_url = data['data']['rtmp_url']
         rtmp_live = data['data']['rtmp_live']
         rea_rid = rtmp_live.split('?')[0]
         http = os.path.join(random.choice(['http://hdltc1.douyucdn.cn/live', 'http://hw-tct.douyucdn.cn/live']))  \
             + '/' + rea_rid
         if self.name == None:
             name = self.get_name()
         else:
             name = self.name
-        if 'FILE' in self.default_settings.keys() and self.default_settings.file != '':
-            file = os.path.join(self.default_settings.file, 'download', '斗鱼录播', name,
+        if 'FILE' in self.settings.keys() and self.settings.file != '':
+            file = os.path.join(self.settings.file, 'download', '斗鱼录播', name,
                                 time)
         else:
             file = os.path.join(os.getcwd(), 'download', '斗鱼录播', name, time)
         ali_file = os.path.join('录播', '斗鱼录播', name, time).replace('\\', '/')
         if not os.path.exists(file):
             os.makedirs(file)
         f = open(file=os.path.join(file, '直播源.txt'), mode='w', encoding='utf8')
         f.write(http)
         f.close()
         logger.info('斗鱼直播间 - {} - {} | 源地址为 - {}'.format(name, self.rid, http))
         if self.open == False:
             logger.info('已成功保存直播源地址到文件')
         if self.open:
             logger.info('斗鱼直播间 - {} - {} 开始录制'.format(name, self.rid))
-            if self.default_settings.docker == False:
-                subout = subprocess.run(
-                    "ffmpeg -i " + '"{}"'.format(http) +
-                    " -c:a copy -c:v copy -bsf:a aac_adtstoasc -threads {} -preset {} -f {}  -f segment -segment_time {} -strftime 1 "
-                    .format(str(self.settings.thread), self.settings.preset,
-                            self.settings.scheme, str(self.settings.time)) +
-                    '"{}"'.format(os.path.join(file, '%Y-%m-%d-%H-%M-%S.ts')))
-                logger.info(subout)
-            if self.default_settings.docker == True:
-                ssh.Ssh(http, os.path.join(file, '%Y-%m-%d-%H-%M-%S.ts'),
-                        self.settings)
-                alipan.Backup(local_file=file, ali_file=ali_file)
-                shutil.rmtree(
-                    os.path.join(
-                        os.path.abspath(
-                            os.path.join(os.path.dirname(__file__), '..')),
-                        'download', '斗鱼录播', name))
+            # os.system('ffmpeg -i "{}" -c:v copy -c:a copy "{}"'.format(link, file))
+            ssh.Ssh(http, os.path.join(file, '%Y-%m-%d-%H-%M-%S.ts'), self.settings)
+            alipan.Backup(local_file=file, ali_file=ali_file)
+            shutil.rmtree(
+                os.path.join(
+                    os.path.abspath(
+                        os.path.join(os.path.dirname(__file__), '..')),
+                    'download', '斗鱼录播', name))
 
     def get_name(self):
         url = 'https://www.douyu.com/betard/{}'.format(self.rid)
         headers = {
             'accept':
             'application/json, text/plain, */*',
             'accept-language':
```

### Comparing `evina-1.0.6/evina/evina.py` & `evina-1.0.7/evina/evina.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,40 +5,35 @@
 # @Author  : 橙橙橙心滴
 # @File    : check.py
 '''
 
 import threading
 import time
 
-from evina import douyin
-from evina import douyu
-
-from evina import config
+from evina import config, douyin, douyu
 
 
 class Evina(config.Arg, config.Env):
     def __init__(self) -> None:
 
         super().__init__()
         for start in self.dict:
             if start == 'douyu':
                 for url, name in self.dict[start].items():
                     if 'http' in url and not url.endswith('/'):
                         url = url.rsplit('/', 1)[1]
                     if not self.check(url):
                         threading.Thread(target=douyu.Douyu,
-                                         args=(url, name, self.conf.settings,
-                                               self.default.settings),
+                                         args=(url, name, self.conf.settings),
                                          name=url).start()
             if start == 'douyin':
                 for url, name in self.dict[start].items():
                     if not self.check(str(url)):
                         threading.Thread(target=douyin.Douyin,
-                                         args=(name, self.conf.settings,
-                                               self.default.settings, url),
+                                         args=(name, self.conf.settings, url),
                                          name=url).start()
 
     def check(self, name):
         for thread in threading.enumerate():
             if name == thread.name:
                 return True
         return False
```

### Comparing `evina-1.0.6/evina/replacement.py` & `evina-1.0.7/evina/replacement.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # @File    : replacement.py
 '''
 
 import io
 import os
 from contextlib import contextmanager
 
+from aligo import EMailConfig
 from aligo.core.Auth import Auth
 from dynaconf.vendor.dotenv.compat import StringIO
 from dynaconf.vendor.dotenv.main import DotEnv
 from loguru import logger
 
 
 class ReplaceMent:
@@ -29,10 +30,7 @@
                 yield B
         else:
             if A.verbose:
                 logger.info(
                     'Python-dotenv could not find configuration file %s.',
                     A.dotenv_path or '.env')
             yield StringIO('')
-
-
-
```

### Comparing `evina-1.0.6/evina/ssh.py` & `evina-1.0.7/evina/ssh.py`

 * *Files identical despite different names*

