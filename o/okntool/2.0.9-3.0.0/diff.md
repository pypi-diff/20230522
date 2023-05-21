# Comparing `tmp/okntool-2.0.9.tar.gz` & `tmp/okntool-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "okntool-2.0.9.tar", last modified: Mon Mar  6 21:00:11 2023, max compression
+gzip compressed data, was "okntool-3.0.0.tar", last modified: Sun May 21 23:05:28 2023, max compression
```

## Comparing `okntool-2.0.9.tar` & `okntool-3.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 21:00:11.187899 okntool-2.0.9/
--rw-rw-rw-   0        0        0    11558 2022-10-24 23:26:11.000000 okntool-2.0.9/LICENSE
--rw-rw-rw-   0        0        0      555 2023-03-06 21:00:11.186903 okntool-2.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     3270 2023-02-02 01:56:53.000000 okntool-2.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-03-06 21:00:11.170812 okntool-2.0.9/okntool/
--rw-rw-rw-   0        0        0        0 2022-10-24 23:28:13.000000 okntool-2.0.9/okntool/__init__.py
--rw-rw-rw-   0        0        0     5692 2023-01-31 23:54:34.000000 okntool-2.0.9/okntool/oknserver_graph_plot_config.json
--rw-rw-rw-   0        0        0    75283 2023-03-06 20:59:54.000000 okntool-2.0.9/okntool/okntool.py
-drwxrwxrwx   0        0        0        0 2023-03-06 21:00:11.185905 okntool-2.0.9/okntool.egg-info/
--rw-rw-rw-   0        0        0      555 2023-03-06 21:00:11.000000 okntool-2.0.9/okntool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-03-06 21:00:11.000000 okntool-2.0.9/okntool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 21:00:11.000000 okntool-2.0.9/okntool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-03-06 21:00:11.000000 okntool-2.0.9/okntool.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-03-06 20:59:57.000000 okntool-2.0.9/okntool.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2023-03-06 21:00:11.000000 okntool-2.0.9/okntool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-06 21:00:11.000000 okntool-2.0.9/okntool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-06 21:00:11.188897 okntool-2.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1078 2023-03-06 20:59:54.000000 okntool-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:05:28.780034 okntool-3.0.0/
+-rw-rw-rw-   0        0        0    11558 2023-02-13 22:18:47.000000 okntool-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0      555 2023-05-21 23:05:28.780034 okntool-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3270 2023-02-13 22:18:47.000000 okntool-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 23:05:28.770061 okntool-3.0.0/okntool/
+-rw-rw-rw-   0        0        0        0 2023-02-13 22:18:47.000000 okntool-3.0.0/okntool/__init__.py
+-rw-rw-rw-   0        0        0     5899 2023-05-21 22:27:11.000000 okntool-3.0.0/okntool/oknserver_graph_plot_config.json
+-rw-rw-rw-   0        0        0    77412 2023-05-21 23:00:52.000000 okntool-3.0.0/okntool/okntool.py
+drwxrwxrwx   0        0        0        0 2023-05-21 23:05:28.779037 okntool-3.0.0/okntool.egg-info/
+-rw-rw-rw-   0        0        0      555 2023-05-21 23:05:28.000000 okntool-3.0.0/okntool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-21 23:05:28.000000 okntool-3.0.0/okntool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 23:05:28.000000 okntool-3.0.0/okntool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-21 23:05:28.000000 okntool-3.0.0/okntool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-21 23:05:09.000000 okntool-3.0.0/okntool.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2023-05-21 23:05:28.000000 okntool-3.0.0/okntool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-21 23:05:28.000000 okntool-3.0.0/okntool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 23:05:28.780034 okntool-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1078 2023-05-21 22:34:58.000000 okntool-3.0.0/setup.py
```

### Comparing `okntool-2.0.9/LICENSE` & `okntool-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `okntool-2.0.9/PKG-INFO` & `okntool-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okntool
-Version: 2.0.9
+Version: 3.0.0
 Summary: OKN related graphs drawing program
 Home-page: https://github.com/jtur044/okntool
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: OKN related graphs drawing program
 Classifier: Programming Language :: Python :: 3
```

### Comparing `okntool-2.0.9/README.md` & `okntool-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `okntool-2.0.9/okntool/oknserver_graph_plot_config.json` & `okntool-3.0.0/okntool/oknserver_graph_plot_config.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9715909090909091%*

 * *Differences: {"'trial_plot'": "{'x_axis_limit': [0, 7], 'y_axis_limit': [0.4, 0.5], 'mean_offset': 0.15, "*

 * *                 "'axis_adjustment_types': OrderedDict([('1', 'manual'), ('2', 'min_max'), ('3', "*

 * *                 "'mean_offset')]), 'axis_adjustment_type_number': 3}"}*

```diff
@@ -184,26 +184,41 @@
         "y_label_font_size": 40,
         "y_label_rotation": 90,
         "y_label_weight": "bold",
         "y_label_x_position": 0.06,
         "y_label_y_position": 0.5
     },
     "trial_plot": {
+        "axis_adjustment_type_number": 3,
+        "axis_adjustment_types": {
+            "1": "manual",
+            "2": "min_max",
+            "3": "mean_offset"
+        },
         "graph_line_color": "black",
         "graph_line_thickness": 1,
         "image_scale": 5,
+        "mean_offset": 0.15,
         "output_image_name": "trial_sensor_ts_vs_x_nom.png",
         "qp_column_name": "is_qp",
         "qp_line_color": "red",
         "qp_line_thickness": 2,
         "signal_csv_folder_name": "result",
         "signal_csv_name": "signal.csv",
         "sp_column_name": "is_sp",
         "sp_line_color": "green",
         "sp_line_thickness": 2,
         "title": "Sensor timestamp Vs Pupil x position",
+        "x_axis_limit": [
+            0,
+            7
+        ],
         "x_data_column_name": "sensor_timestamp",
         "x_label": "sensor timestamp",
+        "y_axis_limit": [
+            0.4,
+            0.5
+        ],
         "y_data_column_name": "updated_x_nom",
         "y_label": "pupil position"
     }
 }
```

### Comparing `okntool-2.0.9/okntool/okntool.py` & `okntool-3.0.0/okntool/okntool.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 import csv
 import numpy as np
 import matplotlib.pyplot as plt
 import os
 import pkg_resources
 from matplotlib.lines import Line2D
 
+logmar_level_array = [1.0, 0.9, 0.8, 0.7, 0.6, 0.5, 0.4, 0.3, 0.2, 0.1, 0.0, -0.1, -0.2,
+                      "no logMAR", "right_down", "right_up", "left_down", "left_up"]
+
 
 # This function is to get header position from the given array
 def get_index(search_input, array_in):
     idx_found = False
     return_idx = None
     for idx, val in enumerate(array_in):
         if val == search_input:
@@ -41,14 +44,16 @@
                               "right_down": "right_down", "right_up": "right_up",
                               "left_down": "left_down", "left_up": "left_up"}
 
     try:
         out_string = disk_logmar_equivalent[disk_string_input]
     except KeyError:
         out_string = disk_string_input
+    if out_string not in logmar_level_array:
+        logmar_level_array.append(out_string)
 
     return out_string
 
 
 # This function is to get trial id, disk_string, logmar_level from the given dir string
 def get_trial_id_name(string_input):
     start_index = string_input.find("trial-")
@@ -113,14 +118,21 @@
             first_value = raw_value
             first_value_recorded = True
         value_input = raw_value - first_value
         x_array.append(value_input)
 
         y_array.append(float(row[y_header_position]))
 
+    x_limits, y_limits, x_array, y_array = get_draw_info_for_trial_plot(trial_plot_info_input, x_array, y_array)
+
+    x_lower_limit = x_limits["lower_limit"]
+    x_upper_limit = x_limits["upper_limit"]
+    y_lower_limit = y_limits["lower_limit"]
+    y_upper_limit = y_limits["upper_limit"]
+
     file_to_open = open(signal_dir_input)
     csv_reader2 = csv.reader(file_to_open)
     header_array2 = []
     rows2 = []
     count_one2 = 0
 
     for row in csv_reader2:
@@ -174,14 +186,16 @@
     plt.plot(x_array, qp_array, color=qp_line_color, linewidth=qp_line_thickness)
     gaze_csv_dir = os.path.join(os.path.split(os.path.split(os.path.split(input_dir)[0])[0])[0], "gaze.csv")
     folder_name = os.path.basename(os.path.split(input_dir)[0])
     trial_id, condition = str(folder_name).split("_", 1)
     plt.title(title)
     plt.xlabel(x_label)
     plt.ylabel(y_label)
+    plt.xlim(x_lower_limit, x_upper_limit)
+    plt.ylim(y_upper_limit, y_lower_limit)
     x_axis_array = np.arange(start=min(x_array), stop=max(x_array), step=1)
     plt.xticks(x_axis_array)
     event_marker_exist = string_exist("event_marker", gaze_csv_dir, "event_string")
     if event_marker_exist:
         event_marker_info = get_event_marker_info(gaze_csv_dir, trial_id)
         for marker_time in event_marker_info:
             plt.axvline(x=float(marker_time), color=graph_line_color,
@@ -227,15 +241,15 @@
                                                           axis_adjustment_types, axis_adjustment_type_number)
         adjust_limit_dict = {"x_adjust_limit": x_adjust_limit, "y_adjust_limit": y_adjust_limit}
         for folder_name in folder_array:
             trial_id, disk_condition = str(folder_name).split("_", 1)
             data_dir_to_be_used = os.path.join(data_dir, folder_name, f"updated_{folder_name}.csv")
             x_array = get_data_array(data_dir_to_be_used, x_data_column_name)
             y_array = get_data_array(data_dir_to_be_used, y_data_column_name)
-            y_mean = np.mean(y_array)
+            y_mean = np.nanmean(y_array)
             y_array = [value - y_mean for value in y_array]
             signal_csv_dir = os.path.join(data_dir, folder_name, signal_csv_folder_name, signal_csv_name)
             sp_array, qp_array = get_sp_and_qp_array(signal_csv_dir, sp_column_name, qp_column_name,
                                                      y_array)
             plot_info = {"trial_id": trial_id, "disk_condition": disk_condition,
                          "x_label": x_label, "y_label": y_label,
                          "x_array": x_array, "y_array": y_array,
@@ -401,16 +415,14 @@
     output_image_name = summary_plot_info_input["output_image_name"]
     display_output_dir = os.path.join(folder_dir_input, output_image_name)
     gaze_csv_dir = str(folder_dir_input).replace(os.path.basename(folder_dir_input), "gaze.csv")
     print(f"Gaze csv dir:{gaze_csv_dir}")
 
     if type(max_graph_in_a_row) == str and str(max_graph_in_a_row).lower() == "none":
         final_plot_array = []
-        logmar_level_array = [1.0, 0.9, 0.8, 0.7, 0.6, 0.5, 0.4, 0.3, 0.2, 0.1, 0.0, -0.1, -0.2,
-                              "no logMAR", "right_down", "right_up", "left_down", "left_up"]
         for logmar_level in logmar_level_array:
             temp_logmar_info_array = []
 
             for info in plot_data_array:
                 if info["logmar"] == logmar_level:
                     temp_logmar_info_array.append(info)
 
@@ -634,15 +646,14 @@
                                                            linestyle=":",
                                                            linewidth=graph_line_thickness)
 
                             for ax in axs.flat:
                                 ax.set(xlabel=x_label, ylabel=y_label)
 
                         if num_plot_to_be_deleted > 0:
-                            "here here"
                             for index in range(num_plot_to_be_deleted):
                                 # print(int(final_column_length) - index)
                                 column_index_to_be_deleted = int(final_column_length) - (index + 1)
                                 axs[row_index, column_index_to_be_deleted].set_axis_off()
 
                         # Hide x labels and tick labels for top plots and y ticks for right plots.
                         for ax in axs.flat:
@@ -713,16 +724,14 @@
         else:
             print("There is nothing to plot")
     else:
         if int(max_graph_in_a_row) <= 0:
             print(f"Max graph in a row must be greater than zero but the input is {int(max_graph_in_a_row)}")
         else:
             final_plot_array = []
-            logmar_level_array = [1.0, 0.9, 0.8, 0.7, 0.6, 0.5, 0.4, 0.3, 0.2, 0.1, 0.0, -0.1, -0.2,
-                                  "no logMAR", "right_down", "right_up", "left_down", "left_up"]
             for logmar_level in logmar_level_array:
                 temp_logmar_info_array = []
 
                 for info in plot_data_array:
                     if info["logmar"] == logmar_level:
                         if len(temp_logmar_info_array) >= max_graph_in_a_row:
                             temp_dict = {"logmar_level": logmar_level, "info_array": temp_logmar_info_array}
@@ -854,16 +863,14 @@
     y_lower_limit = y_adjust_limit["lower_limit"]
     y_upper_limit = y_adjust_limit["upper_limit"]
 
     output_image_name = tidy_plot_info_input["output_image_name"]
     display_output_dir = os.path.join(folder_dir_input, output_image_name)
 
     final_plot_array = []
-    logmar_level_array = [1.0, 0.9, 0.8, 0.7, 0.6, 0.5, 0.4, 0.3, 0.2, 0.1, 0.0, -0.1, -0.2,
-                          "no logMAR", "right_down", "right_up", "left_down", "left_up"]
     for logmar_level in logmar_level_array:
         temp_logmar_info_array = []
 
         for info in plot_info:
             if info["logmar"] == logmar_level:
                 temp_logmar_info_array.append(info)
 
@@ -940,15 +947,15 @@
                             axx.spines['bottom'].set_visible(axis_right_top_left_bottom_borders[3])
 
                     if num_plot_to_be_deleted > 0:
                         for index in range(num_plot_to_be_deleted):
                             column_index_to_be_deleted = int(final_column_length) - (index + 1)
                             axs[row_index, column_index_to_be_deleted].set_axis_off()
 
-                    # Hide all x-axis labels inside the combined graph and show left and outside.
+                    # Hide all x axis labels inside the combined graph and show left and outside.
                     for ax in axs.flat:
                         ax.label_outer()
 
                 plt.tick_params(
                     axis='x',  # changes apply to the x-axis
                     which='both',
                     left=False,
@@ -1206,28 +1213,28 @@
             x_upper_limit_array.append(max(x_array))
             y_array = get_data_array(data_dir_to_be_used, y_header_input)
             y_lower_limit_array.append(min(y_array))
             y_upper_limit_array.append(max(y_array))
 
         x_adjust_limit = {"lower_limit": int(min(x_lower_limit_array)),
                           "upper_limit": int(max(x_upper_limit_array))}
-        y_adjust_limit = {"lower_limit": round(np.mean(y_lower_limit_array), 2),
-                          "upper_limit": round(np.mean(y_upper_limit_array), 2)}
+        y_adjust_limit = {"lower_limit": round(np.nanmean(y_lower_limit_array), 2),
+                          "upper_limit": round(np.nanmean(y_upper_limit_array), 2)}
         print(f"x_adjust_limit:{x_adjust_limit}")
         print(f"y_adjust_limit:{y_adjust_limit}")
 
     elif adjustment_type == "mean_offset":
         x_lower_limit_array = []
         x_upper_limit_array = []
         for folder in folder_array_input:
             data_dir_to_be_used = os.path.join(data_dir_input, folder, f"updated_{folder}.csv")
             x_array = get_data_array(data_dir_to_be_used, x_header_input)
             x_lower_limit_array.append(min(x_array))
             x_upper_limit_array.append(max(x_array))
-            # y_array = get_data_array(data_dir_to_be_used, y_header_input)
+            y_array = get_data_array(data_dir_to_be_used, y_header_input)
 
         x_adjust_limit = {"lower_limit": int(min(x_lower_limit_array)),
                           "upper_limit": int(max(x_upper_limit_array))}
         y_adjust_limit = {"lower_limit": round(float(- mean_offset_input), 2),
                           "upper_limit": round(float(mean_offset_input), 2)}
         print(f"x_adjust_limit:{x_adjust_limit}")
         print(f"y_adjust_limit:{y_adjust_limit}")
@@ -1252,14 +1259,58 @@
                           "upper_limit": round(max(y_upper_limit_array), 2)}
         print(f"x_adjust_limit:{x_adjust_limit}")
         print(f"y_adjust_limit:{y_adjust_limit}")
 
     return x_adjust_limit, y_adjust_limit
 
 
+def get_draw_info_for_trial_plot(config_info_input, x_array_input, y_array_input):
+    x_axis_limit = config_info_input["x_axis_limit"]
+    y_axis_limit = config_info_input["y_axis_limit"]
+    mean_offset = config_info_input["mean_offset"]
+    axis_adjustment_types = config_info_input["axis_adjustment_types"]
+    axis_adjustment_type_number = config_info_input["axis_adjustment_type_number"]
+    adjustment_type = axis_adjustment_types[str(axis_adjustment_type_number)]
+    print(f"axis_adjustment_type:{adjustment_type}")
+    if adjustment_type == "manual":
+        x_adjust_limit = {"lower_limit": x_axis_limit[0], "upper_limit": x_axis_limit[1]}
+        y_adjust_limit = {"lower_limit": y_axis_limit[0], "upper_limit": y_axis_limit[1]}
+        print(f"x_adjust_limit:{x_adjust_limit}")
+        print(f"y_adjust_limit:{y_adjust_limit}")
+
+    elif adjustment_type == "mean_offset":
+        x_adjust_limit = {"lower_limit": int(min(x_array_input)),
+                          "upper_limit": int(max(x_array_input))}
+        y_adjust_limit = {"lower_limit": round(float(- mean_offset), 2),
+                          "upper_limit": round(float(mean_offset), 2)}
+
+        y_mean = np.nanmean(y_array_input)
+        temp_array = []
+        for num in y_array_input:
+            if not np.isnan(num):
+                temp_number = num - y_mean
+                temp_array.append(temp_number)
+            else:
+                temp_array.append(num)
+        y_array_input = temp_array
+
+        print(f"x_adjust_limit:{x_adjust_limit}")
+        print(f"y_adjust_limit:{y_adjust_limit}")
+
+    else:
+        x_adjust_limit = {"lower_limit": int(min(x_array_input)),
+                          "upper_limit": int(max(x_array_input))}
+        y_adjust_limit = {"lower_limit": round(min(y_array_input), 2),
+                          "upper_limit": round(max(y_array_input), 2)}
+        print(f"x_adjust_limit:{x_adjust_limit}")
+        print(f"y_adjust_limit:{y_adjust_limit}")
+
+    return x_adjust_limit, y_adjust_limit, x_array_input, y_array_input
+
+
 def get_va_by_phase_name(csv_dir_input, phase_header_input, final_logmar_header_input, phase_name_input):
     file_to_open = open(csv_dir_input)
     csv_reader = csv.reader(file_to_open)
     header_array = []
     rows = []
     count_one = 0
 
@@ -1278,20 +1329,14 @@
     for row in rows:
         if row[phase_header_position] == phase_name_input:
             va_output = float(row[final_logmar_header_position])
 
     return va_output
 
 
-def get_config_location():
-    config_dir = pkg_resources.resource_filename("okntool", "oknserver_graph_plot_config.json")
-
-    return config_dir
-
-
 def string_exist(string_to_check, csv_to_check, column_to_check):
     file_to_open = open(csv_to_check)
     csv_reader = csv.reader(file_to_open)
     header_array = []
     rows = []
     count = 0
 
@@ -1342,18 +1387,23 @@
                 # event_marker_time_f = float(event_marker_sts - start_marker)
                 # print(event_marker_time_f - event_marker_time_i)
                 event_marker_array.append(float(event_marker_sts - start_marker))
 
     return event_marker_array
 
 
+def get_config_location():
+    config_dir = pkg_resources.resource_filename("okntool", "oknserver_graph_plot_config.json")
+    return config_dir
+
+
 def main():
     parser = argparse.ArgumentParser(prog='okntool',
                                      description='okn related graphs plotting program.')
-    parser.add_argument('--version', action='version', version='2.0.9'),
+    parser.add_argument('--version', action='version', version='3.0.0'),
     parser.add_argument("-t", dest="plot_type", required=True, default=sys.stdin,
                         help="trial, summary, (staircase or progress) or tidy", metavar="plot type")
     parser.add_argument("-d", dest="directory_input", required=True, default=sys.stdin,
                         help="directory folder to be processed", metavar="directory")
     parser.add_argument("-c", dest="config_dir", required=False, default=sys.stdin,
                         help=f"config file to be used", metavar="config location")
```

### Comparing `okntool-2.0.9/okntool.egg-info/PKG-INFO` & `okntool-3.0.0/okntool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: okntool
-Version: 2.0.9
+Version: 3.0.0
 Summary: OKN related graphs drawing program
 Home-page: https://github.com/jtur044/okntool
 Author: Zaw Lin Tun
 Author-email: zawlintun1511@gmail.com
 License: Apache Software
 Keywords: OKN related graphs drawing program
 Classifier: Programming Language :: Python :: 3
```

### Comparing `okntool-2.0.9/setup.py` & `okntool-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('requirements.txt') as f:
     requirements = f.readlines()
 
 long_description = 'Command line program to draw okn related graphs.'
 
 setup(
     name='okntool',
-    version='2.0.9',
+    version='3.0.0',
     author='Zaw Lin Tun',
     author_email='zawlintun1511@gmail.com',
     url='https://github.com/jtur044/okntool',
     description='OKN related graphs drawing program',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache Software",
```

