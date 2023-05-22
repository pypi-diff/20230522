# Comparing `tmp/plotguy-1.0.7.tar.gz` & `tmp/plotguy-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plotguy-1.0.7.tar", last modified: Fri May  5 07:13:11 2023, max compression
+gzip compressed data, was "plotguy-1.0.8.tar", last modified: Mon May 22 04:50:39 2023, max compression
```

## Comparing `plotguy-1.0.7.tar` & `plotguy-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-05 07:13:11.752160 plotguy-1.0.7/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-05-05 07:13:11.751918 plotguy-1.0.7/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.0.7/README.md
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-05 07:13:11.750527 plotguy-1.0.7/plotguy/
--rw-r--r--   0 cmw        (501) staff       (20)    24678 2023-05-05 07:11:41.000000 plotguy-1.0.7/plotguy/__init__.py
--rw-r--r--   0 cmw        (501) staff       (20)    16762 2023-02-28 03:04:57.000000 plotguy-1.0.7/plotguy/aggregate.py
--rw-r--r--   0 cmw        (501) staff       (20)    63231 2023-04-18 03:28:10.000000 plotguy-1.0.7/plotguy/components.py
--rw-r--r--   0 cmw        (501) staff       (20)    37694 2023-04-18 03:32:08.000000 plotguy-1.0.7/plotguy/equity_curves.py
--rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.0.7/plotguy/signals.py
-drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-05 07:13:11.751639 plotguy-1.0.7/plotguy.egg-info/
--rw-r--r--   0 cmw        (501) staff       (20)      353 2023-05-05 07:13:11.000000 plotguy-1.0.7/plotguy.egg-info/PKG-INFO
--rw-r--r--   0 cmw        (501) staff       (20)      279 2023-05-05 07:13:11.000000 plotguy-1.0.7/plotguy.egg-info/SOURCES.txt
--rw-r--r--   0 cmw        (501) staff       (20)        1 2023-05-05 07:13:11.000000 plotguy-1.0.7/plotguy.egg-info/dependency_links.txt
--rw-r--r--   0 cmw        (501) staff       (20)      131 2023-05-05 07:13:11.000000 plotguy-1.0.7/plotguy.egg-info/requires.txt
--rw-r--r--   0 cmw        (501) staff       (20)        8 2023-05-05 07:13:11.000000 plotguy-1.0.7/plotguy.egg-info/top_level.txt
--rw-r--r--   0 cmw        (501) staff       (20)       38 2023-05-05 07:13:11.752237 plotguy-1.0.7/setup.cfg
--rw-r--r--   0 cmw        (501) staff       (20)      832 2023-05-05 07:12:29.000000 plotguy-1.0.7/setup.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-22 04:50:39.982116 plotguy-1.0.8/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-05-22 04:50:39.981868 plotguy-1.0.8/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)        9 2022-09-09 02:08:10.000000 plotguy-1.0.8/README.md
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-22 04:50:39.980836 plotguy-1.0.8/plotguy/
+-rw-r--r--   0 cmw        (501) staff       (20)    24547 2023-05-21 22:31:41.000000 plotguy-1.0.8/plotguy/__init__.py
+-rw-r--r--   0 cmw        (501) staff       (20)    16839 2023-05-22 01:04:41.000000 plotguy-1.0.8/plotguy/aggregate.py
+-rw-r--r--   0 cmw        (501) staff       (20)    64059 2023-05-22 04:48:36.000000 plotguy-1.0.8/plotguy/components.py
+-rw-r--r--   0 cmw        (501) staff       (20)    37762 2023-05-22 04:38:48.000000 plotguy-1.0.8/plotguy/equity_curves.py
+-rw-r--r--   0 cmw        (501) staff       (20)    11123 2023-04-18 03:30:27.000000 plotguy-1.0.8/plotguy/signals.py
+drwxr-xr-x   0 cmw        (501) staff       (20)        0 2023-05-22 04:50:39.981695 plotguy-1.0.8/plotguy.egg-info/
+-rw-r--r--   0 cmw        (501) staff       (20)      353 2023-05-22 04:50:39.000000 plotguy-1.0.8/plotguy.egg-info/PKG-INFO
+-rw-r--r--   0 cmw        (501) staff       (20)      279 2023-05-22 04:50:39.000000 plotguy-1.0.8/plotguy.egg-info/SOURCES.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        1 2023-05-22 04:50:39.000000 plotguy-1.0.8/plotguy.egg-info/dependency_links.txt
+-rw-r--r--   0 cmw        (501) staff       (20)      131 2023-05-22 04:50:39.000000 plotguy-1.0.8/plotguy.egg-info/requires.txt
+-rw-r--r--   0 cmw        (501) staff       (20)        8 2023-05-22 04:50:39.000000 plotguy-1.0.8/plotguy.egg-info/top_level.txt
+-rw-r--r--   0 cmw        (501) staff       (20)       38 2023-05-22 04:50:39.982164 plotguy-1.0.8/setup.cfg
+-rw-r--r--   0 cmw        (501) staff       (20)      832 2023-05-22 04:49:57.000000 plotguy-1.0.8/setup.py
```

### Comparing `plotguy-1.0.7/plotguy/__init__.py` & `plotguy-1.0.8/plotguy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         save_name += f'{key}={str(para)}&'
 
     return save_name
 
 
 def path_reference_code(save_name):
-    reference_code = str(zlib.crc32(bytes(save_name, 'UTF-8')))[:6]
+    reference_code = str(zlib.crc32(bytes(save_name, 'UTF-8')))[:8]
     return reference_code
 
 
 def generate_filepath(para_combination, folder=''):
     file_format = para_combination['file_format']
 
     if not file_format == 'parquet':
@@ -202,24 +202,18 @@
     manager_list = mp.Manager().list()  # To save the result with index number
 
     cal_performance_list = []
     for para_combination in all_para_combination:
         para_combination['risk_free_rate'] = risk_free_rate
         cal_performance_list.append((para_combination, manager_list))
 
-    a = datetime.datetime.now()
-
     pool = mp.Pool(processes=number_of_core)
     pool.map(mp_cal_performance, cal_performance_list)
     pool.close()
 
-    b = datetime.datetime.now()
-    t = b - a
-    print('Process time:', t.total_seconds(), 's')
-
     pd.DataFrame(list(manager_list)).to_csv('backtest_result.csv')
 
 
 def plot_signal_analysis(py_filename, output_folder, start_date, end_date, para_dict, signal_settings):
     app = signals.Signals(py_filename, output_folder, start_date, end_date, para_dict, generate_filepath,
                           signal_settings)
```

### Comparing `plotguy-1.0.7/plotguy/aggregate.py` & `plotguy-1.0.8/plotguy/aggregate.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,19 +236,23 @@
                     df_csv = pd.read_parquet(path)  # Daraframe that may not be daily
                 else:
                     df_csv = pd.read_csv(path, index_col=0)
 
                 df_csv['date'] = pd.to_datetime(df_csv['date'], format='%Y-%m-%d')
                 df_csv = df_csv.set_index('date')
 
+                # print(df_csv)
+
                 if (intraday or summary):
                     df = plotguy.resample_summary_to_daily(para_combination=para_combination[i],folder=folders[i])
                 else:
                     df = df_csv
 
+                df = df.set_index('date')
+
                 df_current = pd.DataFrame()
                 if normalized_boolean:
                     df_current[f'{folders[i]}_{pys[i]}_{i}'] = df['equity_value'] / (df['equity_value'].iloc[0] / 100000)
                 else:
                     df_current[f'{folders[i]}_{pys[i]}_{i}'] = df['equity_value']
                 df_current.index = df.index
                 dfs.append(df_current.copy())
@@ -326,14 +330,15 @@
 
             total_dict['annualized_return'] = annualized_return
             total_dict['annualized_std'] = annualized_std
             total_dict['annualized_sr'] = annualized_sr
 
             start_date_year = df_all_curves.loc[df_all_curves.index[0], 'date'].year
             end_date_year = df_all_curves.loc[df_all_curves.index[-1], 'date'].year
+
             year_list = list(range(start_date_year, end_date_year + 1))
 
 
             # Performance by year
             df_year = pd.DataFrame()
             df_year['equity_value'] = df_all_curves['Aggregate_Equity'].copy()
             df_year['date'] = df_agg.index.copy()
```

### Comparing `plotguy-1.0.7/plotguy/components.py` & `plotguy-1.0.8/plotguy/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     def __init__(self,number_of_curves):
         self.sort_method_dropdown = html.Div(
             dbc.Select(id='sort_method',
                        placeholder="Select Sorting Method",
                        value=f'Top Net Profit',
                        options=[{'label': f'Top {number_of_curves} Net Profit', 'value': 'Top Net Profit'},
                                 {'label': f'Top {number_of_curves} Return-BaH % Difference', 'value': 'Top Return to BaH Ratio'},
-                                {'label': f'Top {number_of_curves} Net Profit/MDD', 'value': 'Top Net Profit to MDD'}, ],
+                                {'label': f'Top {number_of_curves} Sharp Ratio', 'value': 'Top Sharp Ratio'}, ],
                        style={'border-radius': '5px', 'font-size': '12px', }),
             style={'padding-left': '15px', 'width': '235px'})
 
 
     def empty_line_chart(self):
         chart_bg = self.chart_bg
         fig_line = px.line()
@@ -429,16 +429,16 @@
 
         return filter_button
 
 
     def sort_method_df(self, sort_method, result_df, number_of_curves):
         if sort_method == 'Top Net Profit':
             df_sorted = result_df.sort_values(by='net_profit', ascending=False).head(number_of_curves).copy()
-        elif sort_method == 'Top Net Profit to MDD':
-            df_sorted = result_df.sort_values(by='net_profit_to_mdd', ascending=False).head(number_of_curves).copy()
+        elif sort_method == 'Top Sharp Ratio':
+            df_sorted = result_df.sort_values(by='annualized_sr', ascending=False).head(number_of_curves).copy()
         elif sort_method == 'Top Return to BaH Ratio':
             df_sorted = result_df.sort_values(by='return_to_bah', ascending=False).head(number_of_curves).copy()
         else:
             df_sorted = result_df.copy()
 
         df_sorted = df_sorted.reset_index(drop=True)
 
@@ -739,19 +739,21 @@
 
         save_path = plotguy.generate_filepath(para_combination=para_combination)
         if file_format == 'parquet':
             df_backtest = pd.read_parquet(save_path)  # Daraframe that may not be daily
         else:
             df_backtest = pd.read_csv(save_path, index_col=0)  # Daraframe that may not be daily
 
+
         df_csv = df_backtest.copy()
         df_chart = self.prepare_df_chart(df_csv)
 
         df_signal = df_chart.copy()
-        df_signal = df_signal.dropna(subset=['action'])
+        df_signal = df_signal.dropna(subset=['action'])  # for csv
+        df_signal = df_signal.loc[df_signal['action'] != '']  # for parquet
         df_signal = df_signal.reset_index()
         signal_open_date = []
         signal_open_close = []
         signal_close_date = []
         signal_close_close = []
         signal_close_reason = []
 
@@ -806,16 +808,18 @@
 
         df_signal_final = pd.DataFrame()
         df_signal_final['open_date'] = open_date
         df_signal_final['open_close'] = open_close
         df_signal_final['close_date'] = close_date
         df_signal_final['close_close'] = close_close
         df_signal_final['close_reason'] = close_reason
-        df_signal_final['pctchange'] = ((df_signal_final['close_close'] - df_signal_final['open_close']) /
-                                        df_signal_final['open_close']) * 100
+        df_signal_final['pctchange'] = (((df_signal_final['close_close'] - df_signal_final['open_close']) /
+                                        df_signal_final['open_close']) * 100)
+
+
         df_signal_final.open_close = df_signal_final.open_close.round(2)
         df_signal_final.close_close = df_signal_final.close_close.round(2)
         df_signal_final.pctchange = df_signal_final.pctchange.round(2)
 
         # print(df_signal_final)
 
         hover_template = "<br>".join([
@@ -827,14 +831,16 @@
             "Pct Change: %{customdata[5]}%",
         ])
 
 
         title = ''
         para_dict = para_combination['para_dict']
         for key in para_dict:
+            if len(title) > 100:
+                title = title + '<br>'
             title = title + f'{key}:{para_combination[key]} '
 
         # Count number of subchart
         subchart_count = 0
         try:
             fig = settings['subchart_1']
             subchart_count += 1
@@ -847,15 +853,15 @@
         if subchart_count == 0: row_height = [1]
         if subchart_count == 1: row_height = [0.85,0.15]
         if subchart_count == 2: row_height = [0.7,0.15,0.15]
 
         fig_line = make_subplots(rows=subchart_count+1, cols=1,
                                  row_heights=row_height,shared_xaxes=True)
 
-        fig_line.update_layout(title = {'text': title , 'font': {'size': 12 }  })
+        fig_line.update_layout(title = {'text': title , 'font': {'size': 12 }, 'y':0.97,  })
         fig_line.update_xaxes(showline=True, zeroline=False, linecolor='white', gridcolor='rgba(0, 0, 0, 0)')
         fig_line.update_yaxes(showline=True, zeroline=False, linecolor='white', gridcolor='rgba(0, 0, 0, 0)')
         fig_line.add_trace(go.Scatter(mode='lines', hoverinfo='skip',
                                       x=df_chart['date'], y=df_chart['equity_value'],
                                       line=dict(color=line_colour, width=1), name='Strategy Equity'), row=1, col=1)
 
         hover_template_stock_price = "<br>".join([
@@ -1030,25 +1036,42 @@
         equity_curves = []
         for folder in folders:
             df_saved = pd.read_csv(f'{folder}/saved_strategies.csv')
             for i, row in df_saved.iterrows():
                 equity_path = f'{folder}/{row["path"]}'
 
                 dict = {}
+                # parameters = ast.literal_eval(row['para_combination'])
                 dict['para_combination'] = ast.literal_eval(row['para_combination'])
-                para_combination = dict['para_combination']
+                para_combination = ast.literal_eval(row['para_combination'])
+                dict['para_combination'] = para_combination
                 file_format = para_combination['file_format']
                 save_name = plotguy.filename_only(para_combination)
                 ref_code = plotguy.path_reference_code(save_name)
-                parameters = self.path_to_dict(equity_path, file_format )
+
+
+                # parameters = self.path_to_dict(equity_path, file_format)
+                parameters = {}
+                for element in save_name.split('&')[:-1]:
+                    key, content = element.split('=')
+                    if key == 'date':
+                        # parameters['date'] = f'{content[:8]} - {content[8:]}'
+                        parameters['startdate'], parameters['enddate'] = content[:8], content[8:]
+                    elif key == 'summary_mode':
+                        pass
+                    else:
+                        parameters[key] = content
 
                 dict['folder'] = folder
                 dict['py'] = parameters['file']
                 dict['path'] = equity_path
                 dict['parameters'] = parameters
+
+
+
                 dict['performance'] = {
                     'initial_capital': row['initial'],
                     'net_profit_to_mdd': row['net_profit_to_mdd'],
                     'net_profit': row['net_profit'],
                     'mdd_dollar': row['mdd_dollar'],
                     'mdd_pct': row['mdd_pct'],
                     'num_of_trade': row['num_of_trade'],
@@ -1056,16 +1079,18 @@
                     'return_on_capital': row['return_on_capital'],
                     'total_commission': row['total_commission'],
                     'sharp_ratio': row['sharp'],
                 }
                 dict['format'] = file_format
                 dict['ref'] = ref_code
 
+
                 start_date_year = datetime.datetime.strptime(parameters['startdate'], '%Y%m%d').year
                 end_date_year = datetime.datetime.strptime(parameters['enddate'], '%Y%m%d').year
+
                 year_list = list(range(start_date_year, end_date_year + 1))
                 for year in year_list:
                     dict['performance'][f'{year}'] = row[f'{year}']
                     dict['performance'][f'{year}'] = row[f'{year}']
                     dict['performance'][f'{year}_win_count'] = row[f'{year}_win_count']
 
                 equity_curves.append(dict)
@@ -1266,14 +1291,15 @@
         mdd_pct = "{:.0%}".format(total_dict['mdd_pct'])
 
         year_col = []
         year_count = []
         year_count_col = []
         year_win_rate_col = []
         year_return_col = []
+
         for year in year_list:
             year_col.append(html.Div(year))
             year_count.append(int(total_dict[f'{year}']))
             year_count_col.append(html.Div(int(total_dict[f'{year}'])))
             rate = total_dict[f'{year}_win_count']/total_dict[f'{year}']
             year_win_rate_col.append(html.Div( "{:.0%}".format(rate) ))
             year_return = total_dict[f'{year}_return']
```

### Comparing `plotguy-1.0.7/plotguy/equity_curves.py` & `plotguy-1.0.8/plotguy/equity_curves.py`

 * *Files 0% similar despite different names*

```diff
@@ -604,14 +604,15 @@
                     try:
                         self.num_of_win = round(int(df['num_of_trade'])*float(df['win_rate'])/100)
                     except:
                         self.num_of_win = '--'
                     self.return_on_capital = df['return_on_capital']
                     self.sharp = df['annualized_sr']
                     self.total_commission = df['total_commission']
+                    self.total_commission = df['total_commission']
                     year_count = []
                     year_win_count = []
                     for year in self.year_list:
                         if not df[f'{year}_win_rate'] == '--':
                             win_count = round(int(df[str(year)])*float(df[f'{year}_win_rate'])/100)
                         else:
                             win_count = 0
```

### Comparing `plotguy-1.0.7/plotguy/signals.py` & `plotguy-1.0.8/plotguy/signals.py`

 * *Files identical despite different names*

### Comparing `plotguy-1.0.7/setup.py` & `plotguy-1.0.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="plotguy",
-    version="1.0.7",
+    version="1.0.8",
     author="Plotguy Team",
     author_email="plotguy.info@gmail.com",
     description="Plotguy",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[         
         'pandas>=1.5.2',
```

