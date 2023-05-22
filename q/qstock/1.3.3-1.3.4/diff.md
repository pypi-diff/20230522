# Comparing `tmp/qstock-1.3.3.tar.gz` & `tmp/qstock-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qstock-1.3.3.tar", last modified: Tue Dec  6 09:51:01 2022, max compression
+gzip compressed data, was "qstock-1.3.4.tar", last modified: Mon May 22 07:05:00 2023, max compression
```

## Comparing `qstock-1.3.3.tar` & `qstock-1.3.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2022-12-06 09:51:01.374484 qstock-1.3.3/
--rw-rw-rw-   0        0        0       78 2022-11-01 14:56:44.000000 qstock-1.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2248 2022-12-06 09:51:01.374484 qstock-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     1970 2022-11-04 08:02:12.000000 qstock-1.3.3/README.rst
-drwxrwxrwx   0        0        0        0 2022-12-06 09:51:01.344477 qstock-1.3.3/qstock/
--rw-rw-rw-   0        0        0     1063 2022-07-26 08:59:56.000000 qstock-1.3.3/qstock/LICENSE
--rw-rw-rw-   0        0        0     1125 2022-10-10 08:33:46.000000 qstock-1.3.3/qstock/README.md
--rw-rw-rw-   0        0        0      794 2022-11-02 12:55:38.000000 qstock-1.3.3/qstock/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-06 09:51:01.359480 qstock-1.3.3/qstock/backtest/
--rw-rw-rw-   0        0        0      174 2022-11-01 14:34:14.000000 qstock-1.3.3/qstock/backtest/__init__.py
--rw-rw-rw-   0        0        0    15199 2022-10-10 15:03:36.000000 qstock-1.3.3/qstock/backtest/turtle.py
--rw-rw-rw-   0        0        0     8409 2022-11-02 12:15:26.000000 qstock-1.3.3/qstock/backtest/vec_backtest.py
-drwxrwxrwx   0        0        0        0 2022-12-06 09:51:01.367482 qstock-1.3.3/qstock/data/
--rw-rw-rw-   0        0        0      142 2022-11-06 03:47:12.000000 qstock-1.3.3/qstock/data/__init__.py
--rw-rw-rw-   0        0        0   241609 2022-12-04 13:58:48.000000 qstock-1.3.3/qstock/data/demjson.py
--rw-rw-rw-   0        0        0    33641 2022-11-06 03:47:12.000000 qstock-1.3.3/qstock/data/fundamental.py
--rw-rw-rw-   0        0        0    13207 2022-12-06 08:20:23.000000 qstock-1.3.3/qstock/data/industry.py
--rw-rw-rw-   0        0        0    12910 2022-12-04 14:28:04.000000 qstock-1.3.3/qstock/data/macro.py
--rw-rw-rw-   0        0        0    19008 2022-11-06 03:47:12.000000 qstock-1.3.3/qstock/data/money.py
--rw-rw-rw-   0        0        0    12299 2022-11-06 03:47:12.000000 qstock-1.3.3/qstock/data/news.py
--rw-rw-rw-   0        0        0    39664 2022-11-06 03:47:12.000000 qstock-1.3.3/qstock/data/ths.js
--rw-rw-rw-   0        0        0    52411 2022-12-06 08:43:17.000000 qstock-1.3.3/qstock/data/trade.py
--rw-rw-rw-   0        0        0    27327 2022-11-06 04:32:16.000000 qstock-1.3.3/qstock/data/tsdata.py
--rw-rw-rw-   0        0        0    18609 2022-12-05 02:56:58.000000 qstock-1.3.3/qstock/data/util.py
-drwxrwxrwx   0        0        0        0 2022-12-06 09:51:01.371482 qstock-1.3.3/qstock/plot/
--rw-rw-rw-   0        0        0      557 2022-10-10 15:03:36.000000 qstock-1.3.3/qstock/plot/__init__.py
--rw-rw-rw-   0        0        0    20279 2022-11-01 13:32:52.000000 qstock-1.3.3/qstock/plot/chart_plot.py
--rw-rw-rw-   0        0        0    12692 2022-11-04 05:44:12.000000 qstock-1.3.3/qstock/plot/data_plot.py
-drwxrwxrwx   0        0        0        0 2022-12-06 09:51:01.373485 qstock-1.3.3/qstock/stock/
--rw-rw-rw-   0        0        0      169 2022-10-27 12:40:14.000000 qstock-1.3.3/qstock/stock/__init__.py
--rw-rw-rw-   0        0        0     1587 2022-11-02 12:14:26.000000 qstock-1.3.3/qstock/stock/stock_pool.py
--rw-rw-rw-   0        0        0    15174 2022-12-06 09:39:43.000000 qstock-1.3.3/qstock/stock/ths_em_pool.py
-drwxrwxrwx   0        0        0        0 2022-12-06 09:51:01.357480 qstock-1.3.3/qstock.egg-info/
--rw-rw-rw-   0        0        0     2248 2022-12-06 09:51:01.000000 qstock-1.3.3/qstock.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      714 2022-12-06 09:51:01.000000 qstock-1.3.3/qstock.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-06 09:51:01.000000 qstock-1.3.3/qstock.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      163 2022-12-06 09:51:01.000000 qstock-1.3.3/qstock.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-12-06 09:51:01.000000 qstock-1.3.3/qstock.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-12-06 09:51:01.374484 qstock-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0      879 2022-12-06 09:49:43.000000 qstock-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:05:00.696017 qstock-1.3.4/
+-rw-rw-rw-   0        0        0       78 2022-11-01 14:56:44.000000 qstock-1.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2124 2023-05-22 07:05:00.680384 qstock-1.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1846 2023-05-22 06:55:29.000000 qstock-1.3.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-22 07:05:00.539744 qstock-1.3.4/qstock/
+-rw-rw-rw-   0        0        0     1063 2022-07-26 08:59:56.000000 qstock-1.3.4/qstock/LICENSE
+-rw-rw-rw-   0        0        0     1125 2022-10-10 08:33:46.000000 qstock-1.3.4/qstock/README.md
+-rw-rw-rw-   0        0        0      845 2023-05-22 07:02:04.000000 qstock-1.3.4/qstock/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:05:00.586641 qstock-1.3.4/qstock/backtest/
+-rw-rw-rw-   0        0        0      174 2022-11-01 14:34:14.000000 qstock-1.3.4/qstock/backtest/__init__.py
+-rw-rw-rw-   0        0        0    15199 2022-10-10 15:03:36.000000 qstock-1.3.4/qstock/backtest/turtle.py
+-rw-rw-rw-   0        0        0     8409 2022-11-02 12:15:26.000000 qstock-1.3.4/qstock/backtest/vec_backtest.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:05:00.649145 qstock-1.3.4/qstock/data/
+-rw-rw-rw-   0        0        0      142 2022-12-06 12:18:32.000000 qstock-1.3.4/qstock/data/__init__.py
+-rw-rw-rw-   0        0        0   241609 2022-12-06 12:18:32.000000 qstock-1.3.4/qstock/data/demjson.py
+-rw-rw-rw-   0        0        0    33718 2022-12-07 01:31:36.000000 qstock-1.3.4/qstock/data/fundamental.py
+-rw-rw-rw-   0        0        0    13207 2022-12-06 12:18:32.000000 qstock-1.3.4/qstock/data/industry.py
+-rw-rw-rw-   0        0        0    12910 2022-12-06 12:18:32.000000 qstock-1.3.4/qstock/data/macro.py
+-rw-rw-rw-   0        0        0    19008 2022-12-06 12:18:32.000000 qstock-1.3.4/qstock/data/money.py
+-rw-rw-rw-   0        0        0    11720 2022-12-07 06:36:28.000000 qstock-1.3.4/qstock/data/news.py
+-rw-rw-rw-   0        0        0    39664 2022-12-06 12:18:32.000000 qstock-1.3.4/qstock/data/ths.js
+-rw-rw-rw-   0        0        0    52500 2023-02-06 12:10:12.000000 qstock-1.3.4/qstock/data/trade.py
+-rw-rw-rw-   0        0        0    18609 2022-12-06 12:18:32.000000 qstock-1.3.4/qstock/data/util.py
+-rw-rw-rw-   0        0        0     7869 2023-05-05 13:05:53.000000 qstock-1.3.4/qstock/data/wencai.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:05:00.664766 qstock-1.3.4/qstock/plot/
+-rw-rw-rw-   0        0        0      557 2022-10-10 15:03:36.000000 qstock-1.3.4/qstock/plot/__init__.py
+-rw-rw-rw-   0        0        0    20279 2022-11-01 13:32:52.000000 qstock-1.3.4/qstock/plot/chart_plot.py
+-rw-rw-rw-   0        0        0    12692 2022-11-04 05:44:12.000000 qstock-1.3.4/qstock/plot/data_plot.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:05:00.680384 qstock-1.3.4/qstock/stock/
+-rw-rw-rw-   0        0        0      169 2022-10-27 12:40:14.000000 qstock-1.3.4/qstock/stock/__init__.py
+-rw-rw-rw-   0        0        0     1587 2022-11-02 12:14:26.000000 qstock-1.3.4/qstock/stock/stock_pool.py
+-rw-rw-rw-   0        0        0    15174 2022-12-06 09:39:43.000000 qstock-1.3.4/qstock/stock/ths_em_pool.py
+drwxrwxrwx   0        0        0        0 2023-05-22 07:05:00.571009 qstock-1.3.4/qstock.egg-info/
+-rw-rw-rw-   0        0        0     2124 2023-05-22 07:05:00.000000 qstock-1.3.4/qstock.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      714 2023-05-22 07:05:00.000000 qstock-1.3.4/qstock.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 07:05:00.000000 qstock-1.3.4/qstock.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      163 2023-05-22 07:05:00.000000 qstock-1.3.4/qstock.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-22 07:05:00.000000 qstock-1.3.4/qstock.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 07:05:00.696017 qstock-1.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-05-22 06:57:13.000000 qstock-1.3.4/setup.py
```

### Comparing `qstock-1.3.3/PKG-INFO` & `qstock-1.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: qstock
-Version: 1.3.3
+Version: 1.3.4
 Summary: Quantitative finance and stock analysis using Python
 Home-page: https://github.com/tkfy920/qstock
 Author: Jinyi Zhang
 Author-email: 723195276@qq.com
 License: MIT Licence
 Keywords: pip,qstock
 Platform: any
 
 qstock由“Python金融量化”公众号开发，试图打造成个人量化投研分析开源库，目前包括数据获取（data）、可视化(plot)、选股(stock)和量化回测（backtest）四个模块。其中数据模块（data）数据来源于东方财富网、同花顺、新浪财经等网上公开数据，数据爬虫部分参考了现有金融数据包tushare、akshare和efinance。qstock致力于为用户提供更加简洁和规整化的金融市场数据接口。可视化模块基于plotly.express和pyecharts包，为用户提供基于web的交互图形简单操作接口；选股模块提供了同花顺的技术选股和公众号策略选股，包括RPS、MM趋势、财务指标、资金流模型等，回测模块为大家提供向量化（基于pandas）和基于事件驱动的基本框架和模型。
-qstock目前在pypi官网上发布，开源第一版本为1.1.0，目前更新至1.3.1.
+qstock目前在pypi官网上发布，开源第一版本为1.1.0，目前更新至1.3.4.
 
 读者直接“pip install qstock ”安装，或通过'pip install --upgrade qstock'进行更新。GitHub地址：https://github.com/tkfy920/qstock。
 
-目前部分策略选股和策略回测功能仅供知识星球会员使用，会员可在知识星球置顶帖子上上获取qstock-vip-1.3.1.tar.gz （强化版）安装包，将安装包放在工作路径下输入'pip install qstock-vip-1.3.1.tar.gz'进行离线安装。
+目前部分策略选股和策略回测功能仅供知识星球会员使用，会员可在知识星球置顶帖子上上获取qstock离线安装包。
 
 相关教程：
 
 【qstock开源了】数据篇之行情交易数据(https://mp.weixin.qq.com/s/p1lEsBVhrm5ej3YZl0BhOw)
 【qstock数据篇】行业概念板块与资金流(https://mp.weixin.qq.com/s/hj4yuqFDBidAeSRucz6TwQ)
 【qstock量化】数据篇之股票基本面数据(https://mp.weixin.qq.com/s/XznS8hFMEa47x1IElZXJaA)
 【qstock量化】数据篇之宏观指标和财经新闻文本(https://mp.weixin.qq.com/s/vq7BJUCdHMkcgJYjsErpYQ)
```

### Comparing `qstock-1.3.3/README.rst` & `qstock-1.3.4/qstock.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,27 @@
+Metadata-Version: 2.1
+Name: qstock
+Version: 1.3.4
+Summary: Quantitative finance and stock analysis using Python
+Home-page: https://github.com/tkfy920/qstock
+Author: Jinyi Zhang
+Author-email: 723195276@qq.com
+License: MIT Licence
+Keywords: pip,qstock
+Platform: any
+
 qstock由“Python金融量化”公众号开发，试图打造成个人量化投研分析开源库，目前包括数据获取（data）、可视化(plot)、选股(stock)和量化回测（backtest）四个模块。其中数据模块（data）数据来源于东方财富网、同花顺、新浪财经等网上公开数据，数据爬虫部分参考了现有金融数据包tushare、akshare和efinance。qstock致力于为用户提供更加简洁和规整化的金融市场数据接口。可视化模块基于plotly.express和pyecharts包，为用户提供基于web的交互图形简单操作接口；选股模块提供了同花顺的技术选股和公众号策略选股，包括RPS、MM趋势、财务指标、资金流模型等，回测模块为大家提供向量化（基于pandas）和基于事件驱动的基本框架和模型。
-qstock目前在pypi官网上发布，开源第一版本为1.1.0，目前更新至1.3.1.
+qstock目前在pypi官网上发布，开源第一版本为1.1.0，目前更新至1.3.4.
 
 读者直接“pip install qstock ”安装，或通过'pip install --upgrade qstock'进行更新。GitHub地址：https://github.com/tkfy920/qstock。
 
-目前部分策略选股和策略回测功能仅供知识星球会员使用，会员可在知识星球置顶帖子上上获取qstock-vip-1.3.1.tar.gz （强化版）安装包，将安装包放在工作路径下输入'pip install qstock-vip-1.3.1.tar.gz'进行离线安装。
+目前部分策略选股和策略回测功能仅供知识星球会员使用，会员可在知识星球置顶帖子上上获取qstock离线安装包。
 
 相关教程：
 
 【qstock开源了】数据篇之行情交易数据(https://mp.weixin.qq.com/s/p1lEsBVhrm5ej3YZl0BhOw)
 【qstock数据篇】行业概念板块与资金流(https://mp.weixin.qq.com/s/hj4yuqFDBidAeSRucz6TwQ)
 【qstock量化】数据篇之股票基本面数据(https://mp.weixin.qq.com/s/XznS8hFMEa47x1IElZXJaA)
 【qstock量化】数据篇之宏观指标和财经新闻文本(https://mp.weixin.qq.com/s/vq7BJUCdHMkcgJYjsErpYQ)
 【qstock量化】动态交互数据可视化(https://mp.weixin.qq.com/s/zmY4gsPDQ6xDDpC-fVBUPg)
         
-更多干货请关注微信公众号：Python金融量化
+更多干货请关注微信公众号：Python金融量化
```

### Comparing `qstock-1.3.3/qstock/LICENSE` & `qstock-1.3.4/qstock/LICENSE`

 * *Files identical despite different names*

### Comparing `qstock-1.3.3/qstock/README.md` & `qstock-1.3.4/qstock/README.md`

 * *Files identical despite different names*

### Comparing `qstock-1.3.3/qstock/__init__.py` & `qstock-1.3.4/qstock/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,17 @@
 ##行业、概念板块数据
 from qstock.data.industry import *
 #资金流向数据
 from qstock.data.money import *
 #宏观经济数据
 from qstock.data.macro import *
 
+#问财数据
+from qstock.data.wencai import *
+
 #可视化模块
 from qstock.plot.data_plot import *
 from qstock.plot.chart_plot import *
 
 #选股模块
 from qstock.stock.stock_pool import *
 from qstock.stock.ths_em_pool import *
```

### Comparing `qstock-1.3.3/qstock/backtest/turtle.py` & `qstock-1.3.4/qstock/backtest/turtle.py`

 * *Files identical despite different names*

### Comparing `qstock-1.3.3/qstock/backtest/vec_backtest.py` & `qstock-1.3.4/qstock/backtest/vec_backtest.py`

 * *Files identical despite different names*

### Comparing `qstock-1.3.3/qstock/data/demjson.py` & `qstock-1.3.4/qstock/data/demjson.py`

 * *Files identical despite different names*

### Comparing `qstock-1.3.3/qstock/data/fundamental.py` & `qstock-1.3.4/qstock/data/fundamental.py`

 * *Files 1% similar despite different names*

```diff
@@ -612,19 +612,23 @@
         r = requests.get(url, params=params)
         data_json = r.json()
         temp_df = pd.DataFrame(data_json["result"]["data"])
         df = pd.concat([df, temp_df], ignore_index=True)
 
     df.reset_index(inplace=True)
     df["index"] = range(1, len(df) + 1)
-    df.columns = ["序号","_","代码", "简称","_","公告日","报告日","_","预测指标",
-        "_","_","_","_","业绩变动","变动原因","预告类型","上年同期","_","_",
-        "_","_","变动幅度","预测数值","_","_",]
-    df = df[["代码","简称","预测指标","业绩变动","预测数值","变动幅度",
-            "变动原因","预告类型","上年同期","公告日",]]
+    
+    old_cols=['SECURITY_CODE', 'SECURITY_NAME_ABBR','NOTICE_DATE', 'REPORT_DATE', 
+              'PREDICT_FINANCE','PREDICT_CONTENT', 'CHANGE_REASON_EXPLAIN','PREDICT_TYPE',
+              'PREYEAR_SAME_PERIOD', 'INCREASE_JZ', 'FORECAST_JZ']
+    
+    new_cols=["代码","简称","预测指标","业绩变动","预测数值","变动幅度",
+            "变动原因","预告类型","上年同期","公告日"]
+    df=df.rename(columns=dict(zip(old_cols,new_cols)))[new_cols]
+    
     return df
 
 
 def stock_yjbb(date= "20200331"):
     """
     东方财富年报季报业绩报表
     http://data.eastmoney.com/bbsj/202003/yjbb.html
```

### Comparing `qstock-1.3.3/qstock/data/industry.py` & `qstock-1.3.4/qstock/data/industry.py`

 * *Files identical despite different names*

### Comparing `qstock-1.3.3/qstock/data/macro.py` & `qstock-1.3.4/qstock/data/macro.py`

 * *Files identical despite different names*

### Comparing `qstock-1.3.3/qstock/data/money.py` & `qstock-1.3.4/qstock/data/money.py`

 * *Files identical despite different names*

### Comparing `qstock-1.3.3/qstock/data/news.py` & `qstock-1.3.4/qstock/data/news.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 """
 Created on Fri Sep 30 22:05:59 2022
 
 @author: Jinyi Zhang
 """
 import re
 import pandas as pd
+import json
 import requests
 import time
+import signal
 import hashlib
 from datetime import datetime,timedelta
 from bs4 import BeautifulSoup
 from tqdm import tqdm
 import multitasking
+from func_timeout import func_set_timeout
+signal.signal(signal.SIGINT, multitasking.killall)
 
 ######新闻资讯数据
 def news_data(news_type=None,start=None,end=None,code=None):
     
     '''news_type:新闻类型：cctv'或'新闻联播'
     'js'或'金十数据'；'stock' 或'个股新闻'
     不输入参数，默认输出财联社电报新闻数据
@@ -156,15 +160,15 @@
     else:
         url = f"https://tv.cctv.com/lm/xwlb/day/{date}.shtml"
         res = requests.get(url)
         res.encoding = "utf-8"
         soup = BeautifulSoup(res.text, "lxml")
         page_url = [item.find("a")["href"] for item in soup.find_all("li")[1:]]
         
-    for page in tqdm(page_url, leave=True):
+    for page in page_url:
         try:
             r = requests.get(page, headers=headers)
             r.encoding = "utf-8"
             soup = BeautifulSoup(r.text, "lxml")
             if soup.find("h3"):
                 title = soup.find("h3").text
             else:
@@ -209,34 +213,39 @@
     '''获取某日期期间的所有新闻联播数据
     start:起始日期，如'20220930'
     end:结束日期，如'20221001'
     '''
     dates=get_dates(start,end)
     data_list=[]
     @multitasking.task
+    @func_set_timeout(5)
     def run(date):
         data = get_news_cctv(date)
         data_list.append(data)
         pbar.update()
     pbar = tqdm(total=len(dates))
     for date in dates:
-        run(date)
+        try:
+            run(date)
+        except:
+            continue
     multitasking.wait_for_tasks()
     # 转换为dataframe
     df = pd.concat(data_list, axis=0,ignore_index=True)
     return df
 
 def news_js(start,end):
     '''获取某日期期间的所有金十数据-市场快讯数据
     start:起始日期，如'20220930'
     end:结束日期，如'20221001'
     '''
     dates=get_dates(start,end)
     data_list=[]
     @multitasking.task
+    @func_set_timeout(5)
     def run(date):
         data = get_js_news(date)
         data_list.append(data)
         pbar.update()
     pbar = tqdm(total=len(dates))
     for date in dates:
         run(date)
@@ -298,49 +307,29 @@
     df.columns = ["datetime", "content"]
     df.sort_values(["datetime"], inplace=True)
     df.reset_index(inplace=True, drop=True)
     return df
 
 def stock_news(stock):
     """
-    东方财富-个股新闻-最近 20 条新闻
-    http://so.eastmoney.com/news/s?keyword=%E4%B8%AD%E5%9B%BD%E4%BA%BA%E5%AF%BF&pageindex=1&searchrange=8192&sortfiled=4
+    东方财富-个股新闻
     stock: 股票代码
     """
-    url = "http://searchapi.eastmoney.com//bussiness/Web/GetCMSSearchList"
+    url = "https://search-api-web.eastmoney.com/search/jsonp"
     params = {
-        "type": "8196",
-        "pageindex": "1",
-        "pagesize": "20",
-        "keyword": f"({stock})()",
-        "name": "zixun",
-        "_": "1608800267874",
+        "cb": "jQuery3510875346244069884_1668256937995",
+        "param": '{"uid":"",'
+        + f'"keyword":"{stock}"'
+        + ',"type":["cmsArticleWebOld"],"client":"web","clientType":"web","clientVersion":"curr","param":{"cmsArticleWebOld":{"searchScope":"default","sort":"default","pageIndex":1,"pageSize":100,"preTag":"<em>","postTag":"</em>"}}}',
+        "_": "1668256937996",
     }
-    headers = {
-        "Accept": "*/*",
-        "Accept-Encoding": "gzip, deflate",
-        "Accept-Language": "zh-CN,zh;q=0.9,en;q=0.8",
-        "Cache-Control": "no-cache",
-        "Connection": "keep-alive",
-        "Host": "searchapi.eastmoney.com",
-        "Pragma": "no-cache",
-        "Referer": "http://so.eastmoney.com/",
-        "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/87.0.4280.88 Safari/537.36",
-    }
-
-    data = requests.get(url, params=params, headers=headers).json()
-    df = pd.DataFrame(data["Data"])
-    df.columns = ["url","title","_","date","content",]
-    df['code'] = stock
-    df = df[["code","title","content","date","url",]]
-    df["title"] = (
-        df["title"].str.replace(r"\(<em>", "", regex=True).str.replace(r"</em>\)", "", regex=True))
-    df["content"] = (
-        df["content"].str.replace(r"\(<em>", "", regex=True).str.replace(r"</em>\)", "", regex=True)
-    )
-    df["content"] = (
-        df["content"].str.replace(r"<em>", "", regex=True).str.replace(r"</em>", "", regex=True)
+    res = requests.get(url, params=params)
+    data_text = res.text
+    data_json = json.loads(
+        data_text.strip("jQuery3510875346244069884_1668256937995(")[:-1]
     )
-    df["content"] = df["content"].str.replace(r"\u3000", "", regex=True)
-    df["content"] = df["content"].str.replace(r"\r\n", " ", regex=True)
-    df['date']= df['date'].apply(lambda s:s[:9])
-    return df[['code','title','content','date']]
+    df = pd.DataFrame(data_json["result"]["cmsArticleWebOld"])
+    df['title']=df['title'].apply(lambda s:re.sub('[\(<em></em>\<em></em>]','',s))
+    df['content']=df['content'].apply(lambda s:re.sub('[\(<em></em>\<em></em>]','',s))
+    df['code']=stock
+    df=df[['date','code','title','content','url']]
+    return df
```

### Comparing `qstock-1.3.3/qstock/data/ths.js` & `qstock-1.3.4/qstock/data/ths.js`

 * *Files identical despite different names*

### Comparing `qstock-1.3.3/qstock/data/trade.py` & `qstock-1.3.4/qstock/data/trade.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 @Date    ：2022/9/29 20:27 
 '''
 
 import json
 import re
 import signal
 import requests
+from retry import retry
 import pandas as pd
 import multitasking
 from tqdm import tqdm
 from func_timeout import func_set_timeout
 
 from jsonpath import jsonpath
 from datetime import datetime, timedelta
@@ -577,15 +578,16 @@
     if isinstance(code_list, str):
         code_list = [code_list]
     
     if end is None:
         end=latest_trade_date()
 
     @multitasking.task
-    @func_set_timeout(5)
+    #@retry(tries=3, delay=1)
+    @func_set_timeout(10)
     def run(code):
         try:
             temp = web_data(code, start, end, freq, fqt)
             temp[temp.name[0]]=temp.close
             data_list.append(temp[temp.name[0]])
             pbar.update()
         except:
@@ -614,15 +616,16 @@
     if end is None:
         end=latest_trade_date()
 
     data_list = []
     pbar = tqdm(total=len(code_list))
     
     @multitasking.task
-    @func_set_timeout(5)
+    #@retry(tries=3, delay=1)
+    @func_set_timeout(10)
     def run(code):
         data = web_data(code, start, end, freq, fqt)
         data_list.append(data)
         pbar.update()
     for code in code_list:
         run(code)
     multitasking.wait_for_tasks()
```

### Comparing `qstock-1.3.3/qstock/data/util.py` & `qstock-1.3.4/qstock/data/util.py`

 * *Files identical despite different names*

### Comparing `qstock-1.3.3/qstock/plot/__init__.py` & `qstock-1.3.4/qstock/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `qstock-1.3.3/qstock/plot/chart_plot.py` & `qstock-1.3.4/qstock/plot/chart_plot.py`

 * *Files identical despite different names*

### Comparing `qstock-1.3.3/qstock/plot/data_plot.py` & `qstock-1.3.4/qstock/plot/data_plot.py`

 * *Files identical despite different names*

### Comparing `qstock-1.3.3/qstock/stock/stock_pool.py` & `qstock-1.3.4/qstock/stock/stock_pool.py`

 * *Files identical despite different names*

### Comparing `qstock-1.3.3/qstock/stock/ths_em_pool.py` & `qstock-1.3.4/qstock/stock/ths_em_pool.py`

 * *Files identical despite different names*

### Comparing `qstock-1.3.3/qstock.egg-info/PKG-INFO` & `qstock-1.3.4/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,16 @@
-Metadata-Version: 2.1
-Name: qstock
-Version: 1.3.3
-Summary: Quantitative finance and stock analysis using Python
-Home-page: https://github.com/tkfy920/qstock
-Author: Jinyi Zhang
-Author-email: 723195276@qq.com
-License: MIT Licence
-Keywords: pip,qstock
-Platform: any
-
 qstock由“Python金融量化”公众号开发，试图打造成个人量化投研分析开源库，目前包括数据获取（data）、可视化(plot)、选股(stock)和量化回测（backtest）四个模块。其中数据模块（data）数据来源于东方财富网、同花顺、新浪财经等网上公开数据，数据爬虫部分参考了现有金融数据包tushare、akshare和efinance。qstock致力于为用户提供更加简洁和规整化的金融市场数据接口。可视化模块基于plotly.express和pyecharts包，为用户提供基于web的交互图形简单操作接口；选股模块提供了同花顺的技术选股和公众号策略选股，包括RPS、MM趋势、财务指标、资金流模型等，回测模块为大家提供向量化（基于pandas）和基于事件驱动的基本框架和模型。
-qstock目前在pypi官网上发布，开源第一版本为1.1.0，目前更新至1.3.1.
+qstock目前在pypi官网上发布，开源第一版本为1.1.0，目前更新至1.3.4.
 
 读者直接“pip install qstock ”安装，或通过'pip install --upgrade qstock'进行更新。GitHub地址：https://github.com/tkfy920/qstock。
 
-目前部分策略选股和策略回测功能仅供知识星球会员使用，会员可在知识星球置顶帖子上上获取qstock-vip-1.3.1.tar.gz （强化版）安装包，将安装包放在工作路径下输入'pip install qstock-vip-1.3.1.tar.gz'进行离线安装。
+目前部分策略选股和策略回测功能仅供知识星球会员使用，会员可在知识星球置顶帖子上上获取qstock离线安装包。
 
 相关教程：
 
 【qstock开源了】数据篇之行情交易数据(https://mp.weixin.qq.com/s/p1lEsBVhrm5ej3YZl0BhOw)
 【qstock数据篇】行业概念板块与资金流(https://mp.weixin.qq.com/s/hj4yuqFDBidAeSRucz6TwQ)
 【qstock量化】数据篇之股票基本面数据(https://mp.weixin.qq.com/s/XznS8hFMEa47x1IElZXJaA)
 【qstock量化】数据篇之宏观指标和财经新闻文本(https://mp.weixin.qq.com/s/vq7BJUCdHMkcgJYjsErpYQ)
 【qstock量化】动态交互数据可视化(https://mp.weixin.qq.com/s/zmY4gsPDQ6xDDpC-fVBUPg)
         
-更多干货请关注微信公众号：Python金融量化
+更多干货请关注微信公众号：Python金融量化
```

### Comparing `qstock-1.3.3/qstock.egg-info/SOURCES.txt` & `qstock-1.3.4/qstock.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 qstock/data/fundamental.py
 qstock/data/industry.py
 qstock/data/macro.py
 qstock/data/money.py
 qstock/data/news.py
 qstock/data/ths.js
 qstock/data/trade.py
-qstock/data/tsdata.py
 qstock/data/util.py
+qstock/data/wencai.py
 qstock/plot/__init__.py
 qstock/plot/chart_plot.py
 qstock/plot/data_plot.py
 qstock/stock/__init__.py
 qstock/stock/stock_pool.py
 qstock/stock/ths_em_pool.py
```

### Comparing `qstock-1.3.3/setup.py` & `qstock-1.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.rst", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='qstock',
-    version='1.3.3',
+    version='1.3.4',
     keywords=['pip','qstock'],
     description='Quantitative finance and stock analysis using Python',
     long_description=long_description,
     author='Jinyi Zhang',
     author_email='723195276@qq.com',
     url='https://github.com/tkfy920/qstock',
```

