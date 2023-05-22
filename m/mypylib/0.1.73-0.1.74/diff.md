# Comparing `tmp/mypylib-0.1.73.tar.gz` & `tmp/mypylib-0.1.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypylib-0.1.73.tar", last modified: Wed May 17 12:30:57 2023, max compression
+gzip compressed data, was "mypylib-0.1.74.tar", last modified: Mon May 22 15:57:12 2023, max compression
```

## Comparing `mypylib-0.1.73.tar` & `mypylib-0.1.74.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-17 12:30:57.699808 mypylib-0.1.73/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-05-17 12:30:57.699568 mypylib-0.1.73/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.73/README.md
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-17 12:30:57.696797 mypylib-0.1.73/mypylib/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.73/mypylib/MP_shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    46835 2023-05-17 12:29:59.000000 mypylib-0.1.73/mypylib/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.73/mypylib/binance_copy_bot.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.73/mypylib/binance_copy_bot_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.73/mypylib/chdbif.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.73/mypylib/crypto.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.73/mypylib/finmind.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.73/mypylib/libexcel.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)    24302 2023-05-17 12:28:48.000000 mypylib-0.1.73/mypylib/mvp.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.73/mypylib/mytest.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.73/mypylib/option_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.73/mypylib/shioaji_history_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.73/mypylib/shioaji_kline.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.73/mypylib/shioaji_ticks.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.73/mypylib/sjtools.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.73/mypylib/tLineNotify.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     7316 2023-05-17 12:26:48.000000 mypylib-0.1.73/mypylib/ti.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-17 12:30:57.698763 mypylib-0.1.73/mypylib/tmpDevelopment/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.73/mypylib/tmpDevelopment/__init__.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.73/mypylib/tmpDevelopment/warrant_test.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.73/mypylib/tplaysound.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8467 2023-01-12 13:51:57.000000 mypylib-0.1.73/mypylib/tredis.py
--rw-r--r--   0 chenwei-ting   (501) staff       (20)     8184 2023-04-11 13:54:33.000000 mypylib-0.1.73/mypylib/warrant.py
-drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-17 12:30:57.698247 mypylib-0.1.73/mypylib.egg-info/
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-05-17 12:30:57.000000 mypylib-0.1.73/mypylib.egg-info/PKG-INFO
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      654 2023-05-17 12:30:57.000000 mypylib-0.1.73/mypylib.egg-info/SOURCES.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-05-17 12:30:57.000000 mypylib-0.1.73/mypylib.egg-info/dependency_links.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-05-17 12:30:57.000000 mypylib-0.1.73/mypylib.egg-info/top_level.txt
--rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-05-17 12:30:57.699892 mypylib-0.1.73/setup.cfg
--rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.73/setup.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-22 15:57:12.892549 mypylib-0.1.74/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-05-22 15:57:12.892310 mypylib-0.1.74/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3740 2022-08-12 06:28:20.000000 mypylib-0.1.74/README.md
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-22 15:57:12.890273 mypylib-0.1.74/mypylib/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3184 2022-07-20 06:07:23.000000 mypylib-0.1.74/mypylib/MP_shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    46940 2023-05-22 15:56:47.000000 mypylib-0.1.74/mypylib/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7105 2022-07-25 06:39:45.000000 mypylib-0.1.74/mypylib/binance_copy_bot.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     6342 2022-07-15 14:28:35.000000 mypylib-0.1.74/mypylib/binance_copy_bot_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3421 2022-08-01 06:21:06.000000 mypylib-0.1.74/mypylib/chdbif.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1083 2022-09-13 02:48:34.000000 mypylib-0.1.74/mypylib/crypto.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     5093 2022-08-12 06:28:16.000000 mypylib-0.1.74/mypylib/finmind.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    87196 2022-06-02 06:59:21.000000 mypylib-0.1.74/mypylib/libexcel.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)    24314 2023-05-22 15:55:11.000000 mypylib-0.1.74/mypylib/mvp.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1255 2022-06-26 10:52:11.000000 mypylib-0.1.74/mypylib/mytest.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     3588 2022-06-12 10:26:49.000000 mypylib-0.1.74/mypylib/option_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      778 2022-06-02 06:59:21.000000 mypylib-0.1.74/mypylib/shioaji_history_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2490 2023-04-11 13:54:33.000000 mypylib-0.1.74/mypylib/shioaji_kline.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1312 2022-06-02 06:59:21.000000 mypylib-0.1.74/mypylib/shioaji_ticks.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7649 2023-04-18 13:50:52.000000 mypylib-0.1.74/mypylib/sjtools.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1464 2022-09-05 05:47:59.000000 mypylib-0.1.74/mypylib/tLineNotify.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     7316 2023-05-17 12:26:48.000000 mypylib-0.1.74/mypylib/ti.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-22 15:57:12.891915 mypylib-0.1.74/mypylib/tmpDevelopment/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        0 2022-07-16 06:27:26.000000 mypylib-0.1.74/mypylib/tmpDevelopment/__init__.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     1074 2022-07-16 07:09:42.000000 mypylib-0.1.74/mypylib/tmpDevelopment/warrant_test.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     2543 2023-04-27 13:08:02.000000 mypylib-0.1.74/mypylib/tplaysound.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8467 2023-01-12 13:51:57.000000 mypylib-0.1.74/mypylib/tredis.py
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)     8184 2023-04-11 13:54:33.000000 mypylib-0.1.74/mypylib/warrant.py
+drwxr-xr-x   0 chenwei-ting   (501) staff       (20)        0 2023-05-22 15:57:12.891359 mypylib-0.1.74/mypylib.egg-info/
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      373 2023-05-22 15:57:12.000000 mypylib-0.1.74/mypylib.egg-info/PKG-INFO
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      654 2023-05-22 15:57:12.000000 mypylib-0.1.74/mypylib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        1 2023-05-22 15:57:12.000000 mypylib-0.1.74/mypylib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)        8 2023-05-22 15:57:12.000000 mypylib-0.1.74/mypylib.egg-info/top_level.txt
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)       38 2023-05-22 15:57:12.892668 mypylib-0.1.74/setup.cfg
+-rw-r--r--   0 chenwei-ting   (501) staff       (20)      846 2022-06-29 14:27:00.000000 mypylib-0.1.74/setup.py
```

### Comparing `mypylib-0.1.73/README.md` & `mypylib-0.1.74/README.md`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/MP_shioaji_ticks.py` & `mypylib-0.1.74/mypylib/MP_shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/__init__.py` & `mypylib-0.1.74/mypylib/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import requests
 
 ssl._create_default_https_context = ssl._create_unverified_context
 from termcolor import cprint
 from inspect import currentframe
 
-__version__ = '0.1.73'
+__version__ = '0.1.74'
 
 __info__ = {
     '2022/01/04: 0.1.18 加入 __info__。',
     '2022/01/04: 0.1.18 Carey修改 MVP的部分。',
     '2022/01/05: 0.1.19 add check_place_cover 預防漲停鎖住',
     '2022/01/06: 0.1.20 add get_stock_future_data(). 用來抓取每天股票期貨資料',
     '2022/01/06: 0.1.20 add get_stock_future_snapshot(). 用來抓每天股票、股票期貨漲停、跌停價格',
@@ -61,15 +61,16 @@
     '2023/02/13: 0.1.66 Move toggle_btn_off and toggle_btn_on here ',
     '2023/02/23: 0.1.67 get_new_warrant_list() 元富修改網站，封鎖 read_html()',
     '2023/03/15: 0.1.68 修正一些宣告',
     '2023/04/11: 0.1.69 換成shioaji 1.0 API',
     '2023/04/18: 0.1.70 Market() 增加 ask bid information',
     '2023/04/27: 0.1.71 tplaysound 減少buffer音量以免很吵',
     '2023/05/10: 0.1.72 改用shioaji API',
-    '2023/05/17: 0.1.73 shioaji 1.0 改 Mmvp.py & ti.py'
+    '2023/05/17: 0.1.73 shioaji 1.0 改 Mmvp.py & ti.py',
+    '2023/05/22: 0.1.74 mvp() 不繼承 base class。因為shioaji升級的關係。先可以跑再說'
 
 }
 
 request_headers = {
     'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_10_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/39.0.2171.95 Safari/537.36'
 }
```

### Comparing `mypylib-0.1.73/mypylib/binance_copy_bot.py` & `mypylib-0.1.74/mypylib/binance_copy_bot.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/binance_copy_bot_test.py` & `mypylib-0.1.74/mypylib/binance_copy_bot_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/chdbif.py` & `mypylib-0.1.74/mypylib/chdbif.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/crypto.py` & `mypylib-0.1.74/mypylib/crypto.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/finmind.py` & `mypylib-0.1.74/mypylib/finmind.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/libexcel.py` & `mypylib-0.1.74/mypylib/libexcel.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/mvp.py` & `mypylib-0.1.74/mypylib/mvp.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,30 +7,32 @@
 
 matplotlib.use('PS')
 import matplotlib.pyplot as plt
 import gc
 import plotly.express as px
 
 
-class mvp(Base_Technical_Indicator):
+class mvp:
     class w:
         stop_trading_already = 'stop trading already'
 
     def __init__(self, symbol='', date='', period_seconds=10, volume_burst=1000.0, volume_lot=1000.0, volume_moving=1000.0, yesterday_close=0.0, volume_burst_30s=1000.0, volume_lot_30s=1000.0,
                  rule=1):
         cprint(f'MVP: symbol: {symbol}, '
                f'date: {date}, '
                f'period second: {period_seconds}, '
                f'volume burst: {volume_burst}, '
                f'volume burst_30s: {volume_burst_30s}, '
                f'volume lot: {volume_lot}, '
                f'volume moving: {volume_moving}',
                'yellow')
 
-        super().__init__(symbol, date, period_seconds=period_seconds)
+        # super().__init__(symbol, date, period_seconds=period_seconds)
+
+        self.symbol = symbol
 
         self.rule = rule
 
         # Percentage
         self.percentage_trigger_and_down_tolerance = 0.99
 
         # MVP index
@@ -70,38 +72,38 @@
         self.mvp_tmp = {'ts': [],
                         'close': [],
                         'volume': []
                         }
 
     def period_accumulate(self, tick: Tick):
         # print(f'acc: {tick.ts} {tick.close} {tick.volume}')
-        super().period_accumulate(tick)
+        # super().period_accumulate(tick)
 
         self.mvp_tmp['ts'].append(tick.datetime)
         self.mvp_tmp['close'].append(tick.close)
         self.mvp_tmp['volume'].append(tick.volume)
         self.volume_current = sum(self.mvp_tmp['volume'])
         if self.price_open == 0:
             self.price_open = tick.close
 
     def period_calculate(self, tick: Tick):
         # print(f'cal: {tick.ts} {tick.close} {tick.volume}')
-        super().period_calculate(tick)
+        # super().period_calculate(tick)
 
         self.add_mvp_index()
 
         self.mvp_tmp['ts'].clear()
         self.mvp_tmp['close'].clear()
         self.mvp_tmp['volume'].clear()
 
     def push(self, tick: Tick):
         if self.bool_stop_trading_already:
             return
 
-        super().push(tick)
+        # super().push(tick)
 
     def check_place_cover(self, tick: Tick, price) -> bool:
         index = self.mvp_index.shape[0] - 1
         cur_mvp = self.mvp_index.iloc[index]
         pre1_mvp = self.mvp_index.iloc[index - 1]
         pre2_mvp = self.mvp_index.iloc[index - 3]
         ts = cur_mvp['ts']
```

### Comparing `mypylib-0.1.73/mypylib/mytest.py` & `mypylib-0.1.74/mypylib/mytest.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/option_test.py` & `mypylib-0.1.74/mypylib/option_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/shioaji_history_ticks.py` & `mypylib-0.1.74/mypylib/shioaji_history_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/shioaji_kline.py` & `mypylib-0.1.74/mypylib/shioaji_kline.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/shioaji_ticks.py` & `mypylib-0.1.74/mypylib/shioaji_ticks.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/sjtools.py` & `mypylib-0.1.74/mypylib/sjtools.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/tLineNotify.py` & `mypylib-0.1.74/mypylib/tLineNotify.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/ti.py` & `mypylib-0.1.74/mypylib/ti.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/tmpDevelopment/warrant_test.py` & `mypylib-0.1.74/mypylib/tmpDevelopment/warrant_test.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/tplaysound.py` & `mypylib-0.1.74/mypylib/tplaysound.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/tredis.py` & `mypylib-0.1.74/mypylib/tredis.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib/warrant.py` & `mypylib-0.1.74/mypylib/warrant.py`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/mypylib.egg-info/SOURCES.txt` & `mypylib-0.1.74/mypylib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypylib-0.1.73/setup.py` & `mypylib-0.1.74/setup.py`

 * *Files identical despite different names*

