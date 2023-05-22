# Comparing `tmp/traitsui-7.4.3.tar.gz` & `tmp/traitsui-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traitsui-7.4.3.tar", last modified: Thu Jan 12 15:35:18 2023, max compression
+gzip compressed data, was "traitsui-8.0.0.tar", last modified: Mon May 22 15:07:08 2023, max compression
```

## Comparing `traitsui-7.4.3.tar` & `traitsui-8.0.0.tar`

### file list

```diff
@@ -1,1060 +1,1060 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.893211 traitsui-7.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    42470 2023-01-12 15:35:01.000000 traitsui-7.4.3/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-01-12 15:35:01.000000 traitsui-7.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-01-12 15:35:01.000000 traitsui-7.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-01-12 15:35:18.893211 traitsui-7.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-01-12 15:35:01.000000 traitsui-7.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26449 2023-01-12 15:35:01.000000 traitsui-7.4.3/README_example.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.749209 traitsui-7.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/api.css
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.749209 traitsui-7.4.3/docs/releases/
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/releases/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.753209 traitsui-7.4.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.753209 traitsui-7.4.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/_static/default.css
--rw-r--r--   0 runner    (1001) docker     (123)    12938 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/_static/e-logo-rev.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/_static/et.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.753209 traitsui-7.4.3/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/_templates/search.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.753209 traitsui-7.4.3/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.753209 traitsui-7.4.3/docs/source/demos/
--rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/demos/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/e-logo-rev.png
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.753209 traitsui-7.4.3/docs/source/traitsui_dev_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_dev_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12940 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_dev_guide/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.753209 traitsui-7.4.3/docs/source/traitsui_user_manual/
--rw-r--r--   0 runner    (1001) docker     (123)    40262 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/adapters.rst
--rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/advanced_view.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15727 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/custom_view.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.757209 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/configure_traits_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/configure_traits_view_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/configure_traits_view_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/default_trait_editors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/default_traits_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/default_traits_view2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/enum_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/handler_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/instance_editor_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/mixed_styles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/multi_object_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/multiple_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/tree_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/examples/wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)    44546 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/factories_advanced_extra.rst
--rw-r--r--   0 runner    (1001) docker     (123)    48820 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/factories_basic.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/factory_intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (123)    26564 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/handler.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.765209 traitsui-7.4.3/docs/source/traitsui_user_manual/images/
--rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/ArrayEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    31800 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/Auto_update_TabularEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    18250 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/BooleanEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    25277 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/ButtonEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)   136429 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/CSVListEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    30686 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/CheckListEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    67783 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/CodeEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    24171 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/ColorEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    30732 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/CompoundEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    40284 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/DataFrameEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    29229 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/DatetimeEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    45058 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/DirectoryEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    51855 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/Dynamic_EnumEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    69313 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/EnumEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    26841 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/FileEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    34967 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/FontEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)   183346 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/HTMLEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/HTML_editor.png
--rw-r--r--   0 runner    (1001) docker     (123)    23464 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/ImageEnumEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    56162 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/InstanceEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    55913 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/ListEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    41149 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/ListStrEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    22734 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/RGBColorEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    46064 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/RangeEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    30984 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/SetEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    72355 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/TableEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    38070 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/TextEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    50097 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/TitleEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    50534 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/TreeEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)    46529 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/TupleEditor_demo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/alter_title_after.png
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/alter_title_before.png
--rw-r--r--   0 runner    (1001) docker     (123)    28539 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/array_view_editor.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    32421 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/color_picker_windows.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/custom_enum_editor.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/default_text_editor.png
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/delete_item_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    28592 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/font_dialog_windows.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    20452 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/html_code_editor.png
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/insert_item_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/key_binding_editor.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/led_editor.png
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/list_with_context_menu.png
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/move_down_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/move_up_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/no_sort_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/notebook_list_editor.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/read_only_editor.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/search_table_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    12101 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/shell_editor.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/simple_enum_editor_closed.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/simple_enum_editor_open.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/table_column_selection.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/table_prefs.png
--rw-r--r--   0 runner    (1001) docker     (123)    32469 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/tabular_editor.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/text_editor.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/text_editor_integers.png
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/text_editor_strings.png
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/text_editors_passwords.png
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex1.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex12.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex13.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex16.png
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex2.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex3.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex4.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex7.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/value_editor.png
--rw-r--r--   0 runner    (1001) docker     (123)    18085 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/wizard_dialog_1.png
--rw-r--r--   0 runner    (1001) docker     (123)    20059 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/images/wizard_dialog_2.png
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/predefined_traits.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.765209 traitsui-7.4.3/docs/source/traitsui_user_manual/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/scripts/regenerate_example_screenshots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.765209 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.765209 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/discussions/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/discussions/automated_vs_manual_test.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/discussions/compatibility_pyface_testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/discussions/debugging-gui-tests-at-runtime.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/discussions/event_loop_and_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/discussions/target_interaction_location.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/discussions/working_of_extensions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.765209 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/howtos/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/howtos/add_new_interaction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/howtos/add_new_location.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.765209 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/references/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/references/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/substitutions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.765209 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/tutorials/first_test.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.741209 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/tutorials/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.769209 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/tutorials/images/first_test/
--rw-r--r--   0 runner    (1001) docker     (123)    20612 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/tutorials/images/first_test/init-app.png
--rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/tutorials/images/first_test/modified-fields.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.769209 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/tutorials/images/test_with_nested_object/
--rw-r--r--   0 runner    (1001) docker     (123)    29097 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/tutorials/images/test_with_nested_object/init-app.png
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing/tutorials/test_with_nested_object.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/tips.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24053 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/traitsui_user_manual/view.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.769209 traitsui-7.4.3/docs/source/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.769209 traitsui-7.4.3/docs/source/tutorials/code_snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/code_snippets/code_block0.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/code_snippets/code_block1.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/code_snippets/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/code_snippets/echo_box.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/code_snippets/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/code_snippets/event_loop_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/code_snippets/event_loop_wx.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/code_snippets/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/code_snippets/mpl_figure_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/code_snippets/thread_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/code_snippets/traits_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.773209 traitsui-7.4.3/docs/source/tutorials/images/
--rw-r--r--   0 runner    (1001) docker     (123)   381388 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/images/application1.png
--rw-r--r--   0 runner    (1001) docker     (123)   386443 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/images/application2.png
--rw-r--r--   0 runner    (1001) docker     (123)   371915 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/images/application3.png
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/images/code_block1.png
--rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/images/container.png
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/images/interactive.png
--rw-r--r--   0 runner    (1001) docker     (123)    29983 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/images/mpl_figure_editor.png
--rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/images/traits_thread.png
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    39260 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/source/tutorials/traits_ui_scientific_app.rst
--rw-r--r--   0 runner    (1001) docker     (123)  1907712 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/traits_ui.ppt
--rw-r--r--   0 runner    (1001) docker     (123)   664962 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/traits_ui_slides.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-01-12 15:35:01.000000 traitsui-7.4.3/docs/traitsuidocreadme.txt
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-01-12 15:35:01.000000 traitsui-7.4.3/edm.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.773209 traitsui-7.4.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.773209 traitsui-7.4.3/examples/demo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.785209 traitsui-7.4.3/examples/demo/Advanced/
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Adapted_tree_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Apply_Revert_handler_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Auto_editable_readonly_table_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Auto_update_TabularEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Date_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Date_range_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Dynamic_EnumEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Dynamic_range_trait_and_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Dynamic_views_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Dynamically_changing_buttons_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/HDF5_tree_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/HDF5_tree_demo2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/History_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Invalid_state_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/ListStrAdapter_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/ListStrEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/List_editor_notebook_selection_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/List_editors_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/MVC_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Multi_select_string_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Multi_thread_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Multi_thread_demo_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/NumPy_array_tabular_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/NumPy_array_view_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Popup_Dialog_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Property_List_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Scrubber_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Settable_cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Statusbar_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/String_list_ui_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Table_editor_with_checkbox_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Table_editor_with_context_menu_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Table_editor_with_live_search_and_cell_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Table_editor_with_progress_column.py
--rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Tabular_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Tabular_editor_with_context_menu_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Time_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/Tree_editor_required_traits_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)  1087120 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/test_fixed.h5
--rw-r--r--   0 runner    (1001) docker     (123)  1101753 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/test_fixed_compressed.h5
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/test_h5pydata.h5
--rw-r--r--   0 runner    (1001) docker     (123)   356712 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/test_table_dc.h5
--rw-r--r--   0 runner    (1001) docker     (123)    85584 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/test_table_no_dc.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.785209 traitsui-7.4.3/examples/demo/Advanced/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Advanced/tests/test_List_editor_notebook_selection_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.785209 traitsui-7.4.3/examples/demo/Applications/
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Applications/Python_source_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Applications/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.789209 traitsui-7.4.3/examples/demo/Applications/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Applications/images/GG5.png
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Applications/images/TFB.png
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Applications/images/blue_ball.png
--rw-r--r--   0 runner    (1001) docker     (123)    65791 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Applications/images/header.png
--rw-r--r--   0 runner    (1001) docker     (123)    65461 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Applications/images/notebook_close.png
--rw-r--r--   0 runner    (1001) docker     (123)    87952 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Applications/images/notebook_open.png
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Applications/images/red_ball.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Applications/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.789209 traitsui-7.4.3/examples/demo/Applications/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Applications/tests/test_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.789209 traitsui-7.4.3/examples/demo/Dynamic_Forms/
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Dynamic_Forms/dynamic_form_using_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Dynamic_Forms/dynamic_range_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Dynamic_Forms/dynamic_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Dynamic_Forms/enabled_when.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Dynamic_Forms/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.789209 traitsui-7.4.3/examples/demo/Dynamic_Forms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Dynamic_Forms/tests/test_visible_when.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Dynamic_Forms/visible_when.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.789209 traitsui-7.4.3/examples/demo/Extras/
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Extras/Image_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Extras/LED_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Extras/Tree_editor_with_TreeNodeRenderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Extras/animated_GIF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.789209 traitsui-7.4.3/examples/demo/Extras/images/
--rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Extras/images/info.png
--rw-r--r--   0 runner    (1001) docker     (123)    23579 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Extras/images/logo_32x32.gif
--rw-r--r--   0 runner    (1001) docker     (123)    39542 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Extras/images/logo_48x48.gif
--rw-r--r--   0 runner    (1001) docker     (123)    57367 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Extras/images/logo_64x64.gif
--rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Extras/images/python-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Extras/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.789209 traitsui-7.4.3/examples/demo/Extras/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Extras/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Extras/tests/test_Image_editor_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.789209 traitsui-7.4.3/examples/demo/Extras/windows/
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Extras/windows/flash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Extras/windows/internet_explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.793209 traitsui-7.4.3/examples/demo/Misc/
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Misc/demo_group_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Misc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Misc/using_springs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.797210 traitsui-7.4.3/examples/demo/Standard_Editors/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/ArrayEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/BooleanEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/BooleanEditor_simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/ButtonEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/ButtonEditor_simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/CSVListEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/CheckListEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/CheckListEditor_simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/CodeEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/ColorEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/CompoundEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/DataFrameEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/DatetimeEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/DirectoryEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/EnumEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/FileEditor_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.797210 traitsui-7.4.3/examples/demo/Standard_Editors/File_Dialog/
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/File_Dialog/File_Open.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Custom_Extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/File_Dialog/File_Open_with_FileInfo_Extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/File_Dialog/File_Open_with_ImageInfo_Extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Multiple_Extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/File_Dialog/File_Open_with_TextInfo_Extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/FontEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/HTMLEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/ImageEnumEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/InstanceEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/ListEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/RGBColorEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/RangeEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/SetEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/TableEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/TextEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/TitleEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/TreeEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/TupleEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/VideoEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.797210 traitsui-7.4.3/examples/demo/Standard_Editors/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_BooleanEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_BooleanEditor_simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_ButtonEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_ButtonEditor_simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_CheckListEditor_simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_EnumEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_FileEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_InstanceEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_ListEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_RangeEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_TableEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_TextEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/examples.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    43203 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/demo/traits_ui_demo.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.797210 traitsui-7.4.3/examples/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/default.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.797210 traitsui-7.4.3/examples/tutorials/doc_examples/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/doc_examples/default.css
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/doc_examples/doc_examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.797210 traitsui-7.4.3/examples/tutorials/doc_examples/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/doc_examples/examples/include_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/doc_examples/examples/lesson.desc
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/doc_examples/examples/override_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/doc_examples/examples/view_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/doc_examples/examples/view_multi_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/doc_examples/examples/view_standalone.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/doc_examples/lesson.desc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.801210 traitsui-7.4.3/examples/tutorials/traitsui_4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/default.css
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/deferred.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.801210 traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/animated_gif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/flash.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/ie_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/led.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.801210 traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/tabular_editor/
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/tabular_editor/numpy_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/tabular_editor/python_source_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/tabular_editor/sm_person_example.py
--rw-r--r--   0 runner    (1001) docker     (123)    50543 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/tabular_editor/tabular_editor.htm
--rw-r--r--   0 runner    (1001) docker     (123)    42131 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/tabular_editor/tabular_editor.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/tabular_editor/tutorial.desc
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/tutorial.desc
--rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/model_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/traitsui_4.0/tutorial.desc
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-01-12 15:35:01.000000 traitsui-7.4.3/examples/tutorials/tutor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-01-12 15:35:01.000000 traitsui-7.4.3/image_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-01-12 15:35:01.000000 traitsui-7.4.3/image_LICENSE_Eclipse.txt
--rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-01-12 15:35:01.000000 traitsui-7.4.3/image_LICENSE_Nuvola.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-01-12 15:35:01.000000 traitsui-7.4.3/image_LICENSE_OOo.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.801210 traitsui-7.4.3/integrationtests/
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/styled_date_editor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11264 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/test_all_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.805209 traitsui-7.4.3/integrationtests/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/array_editor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/buttons_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/check_list_editor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/check_list_editor_test2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/code_editor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/enum_dynamic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/enum_editor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/html_editor_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.805209 traitsui-7.4.3/integrationtests/ui/images/
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/images/bottom_left_origin.gif
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/images/bottom_right_origin.gif
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/images/top_left_origin.gif
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/images/top_right_origin.gif
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/instance_drag_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/instance_editor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/instance_editor_test2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/instance_editor_test3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/instance_editor_test4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/instance_editor_test5.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/instance_editor_test6.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/large_range_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/list_traits_ui_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/set_dynamic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/shell_editor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/table_editor_focus_bug.py
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/table_editor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/table_editor_test2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/table_list_editor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/test_ui3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/test_ui4.py
--rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/test_ui5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/text_editor_invalid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-01-12 15:35:01.000000 traitsui-7.4.3/integrationtests/ui/tree_editor_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-12 15:35:01.000000 traitsui-7.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-12 15:35:18.893211 traitsui-7.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11754 2023-01-12 15:35:01.000000 traitsui-7.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.813210 traitsui-7.4.3/traitsui/
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-01-12 15:35:18.000000 traitsui-7.4.3/traitsui/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/basic_editor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/color_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/context_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/default_dock_window_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/delegating_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/dock_window_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/dockable_view_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    28072 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editor_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.817210 traitsui-7.4.3/traitsui/editors/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/array_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/boolean_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/button_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/check_list_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/code_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/color_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/compound_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/csv_list_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/custom_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/date_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/date_range_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/datetime_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/default_override.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/directory_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/dnd_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/drop_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/enum_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/file_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/font_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/history_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/html_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/image_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/image_enum_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/instance_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/key_binding_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/list_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/list_str_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/null_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/popup_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/progress_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/range_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/rgb_color_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/scrubber_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/search_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/set_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7489 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/shell_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/styled_date_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/table_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/tabular_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/text_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/time_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/title_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/tree_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/tuple_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/value_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/editors/video_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.741209 traitsui-7.4.3/traitsui/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.817210 traitsui-7.4.3/traitsui/examples/demo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.825210 traitsui-7.4.3/traitsui/examples/demo/Advanced/
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Adapted_tree_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Apply_Revert_handler_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Auto_editable_readonly_table_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Auto_update_TabularEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Date_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Date_range_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Dynamic_EnumEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Dynamic_range_trait_and_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Dynamic_views_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Dynamically_changing_buttons_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/HDF5_tree_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/HDF5_tree_demo2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/History_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Invalid_state_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/ListStrAdapter_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/ListStrEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/List_editor_notebook_selection_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/List_editors_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/MVC_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Multi_select_string_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Multi_thread_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Multi_thread_demo_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/NumPy_array_tabular_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/NumPy_array_view_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Popup_Dialog_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Property_List_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Scrubber_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Settable_cached_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Statusbar_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/String_list_ui_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Table_editor_with_checkbox_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Table_editor_with_context_menu_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Table_editor_with_live_search_and_cell_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Table_editor_with_progress_column.py
--rw-r--r--   0 runner    (1001) docker     (123)    12349 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Tabular_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Tabular_editor_with_context_menu_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Time_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/Tree_editor_required_traits_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)  1087120 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/test_fixed.h5
--rw-r--r--   0 runner    (1001) docker     (123)  1101753 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/test_fixed_compressed.h5
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/test_h5pydata.h5
--rw-r--r--   0 runner    (1001) docker     (123)   356712 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/test_table_dc.h5
--rw-r--r--   0 runner    (1001) docker     (123)    85584 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/test_table_no_dc.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.825210 traitsui-7.4.3/traitsui/examples/demo/Advanced/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Advanced/tests/test_List_editor_notebook_selection_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.829210 traitsui-7.4.3/traitsui/examples/demo/Applications/
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Applications/Python_source_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Applications/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.829210 traitsui-7.4.3/traitsui/examples/demo/Applications/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Applications/images/GG5.png
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Applications/images/TFB.png
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Applications/images/blue_ball.png
--rw-r--r--   0 runner    (1001) docker     (123)    65791 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Applications/images/header.png
--rw-r--r--   0 runner    (1001) docker     (123)    65461 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Applications/images/notebook_close.png
--rw-r--r--   0 runner    (1001) docker     (123)    87952 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Applications/images/notebook_open.png
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Applications/images/red_ball.png
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Applications/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.829210 traitsui-7.4.3/traitsui/examples/demo/Applications/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Applications/tests/test_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.829210 traitsui-7.4.3/traitsui/examples/demo/Dynamic_Forms/
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Dynamic_Forms/dynamic_form_using_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Dynamic_Forms/dynamic_range_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Dynamic_Forms/dynamic_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Dynamic_Forms/enabled_when.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Dynamic_Forms/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.829210 traitsui-7.4.3/traitsui/examples/demo/Dynamic_Forms/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Dynamic_Forms/tests/test_visible_when.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Dynamic_Forms/visible_when.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.829210 traitsui-7.4.3/traitsui/examples/demo/Extras/
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Extras/Image_editor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Extras/LED_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Extras/Tree_editor_with_TreeNodeRenderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Extras/animated_GIF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.829210 traitsui-7.4.3/traitsui/examples/demo/Extras/images/
--rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Extras/images/info.png
--rw-r--r--   0 runner    (1001) docker     (123)    23579 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Extras/images/logo_32x32.gif
--rw-r--r--   0 runner    (1001) docker     (123)    39542 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Extras/images/logo_48x48.gif
--rw-r--r--   0 runner    (1001) docker     (123)    57367 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Extras/images/logo_64x64.gif
--rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Extras/images/python-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Extras/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.829210 traitsui-7.4.3/traitsui/examples/demo/Extras/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Extras/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Extras/tests/test_Image_editor_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.829210 traitsui-7.4.3/traitsui/examples/demo/Extras/windows/
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Extras/windows/flash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Extras/windows/internet_explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.833210 traitsui-7.4.3/traitsui/examples/demo/Misc/
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Misc/demo_group_size.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Misc/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Misc/using_springs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.833210 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/ArrayEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/BooleanEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/BooleanEditor_simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/ButtonEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/ButtonEditor_simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/CSVListEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/CheckListEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/CheckListEditor_simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/CodeEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/ColorEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/CompoundEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/DataFrameEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/DatetimeEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/DirectoryEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/EnumEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/FileEditor_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.837210 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/File_Dialog/
--rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Custom_Extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_FileInfo_Extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_ImageInfo_Extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Multiple_Extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_TextInfo_Extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/FontEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/HTMLEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/ImageEnumEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/InstanceEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/ListEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/RGBColorEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/RangeEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/SetEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/TableEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/TextEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/TitleEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/TreeEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/TupleEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/VideoEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.837210 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_BooleanEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_BooleanEditor_simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_ButtonEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_ButtonEditor_simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_CheckListEditor_simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_EnumEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_FileEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_InstanceEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_ListEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_RangeEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_TableEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_TextEditor_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/examples.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    43203 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/examples/demo/traits_ui_demo.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.837210 traitsui-7.4.3/traitsui/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/extras/_demo_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    34730 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/extras/_demo_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/extras/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/extras/checkbox_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/extras/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/extras/edit_column.py
--rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/extras/has_dynamic_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.837210 traitsui-7.4.3/traitsui/extras/images/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/extras/images/next.png
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/extras/images/parent.png
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/extras/images/previous.png
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/extras/images/reload.png
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/extras/images/run.png
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/extras/progress_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/extras/saving.py
--rw-r--r--   0 runner    (1001) docker     (123)    20213 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/file_dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    20173 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/help_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.837210 traitsui-7.4.3/traitsui/images/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/images/frame.png
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/include.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/instance_choice.py
--rw-r--r--   0 runner    (1001) docker     (123)    19265 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/item.py
--rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/list_str_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/mimedata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.841210 traitsui-7.4.3/traitsui/null/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/null/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/null/color_trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/null/font_trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/null/rgb_color_trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/null/toolkit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.853210 traitsui-7.4.3/traitsui/qt4/
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/array_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/array_view_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/boolean_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/button_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/check_list_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/clipboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    10713 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/code_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/color_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/color_trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/compound_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/csv_list_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/custom_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/data_frame_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/date_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/date_range_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/datetime_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/directory_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/drop_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/editor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/enum_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.853210 traitsui-7.4.3/traitsui/qt4/extra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/extra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/extra/bounds_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/extra/checkbox_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/extra/led_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/extra/progress_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/extra/qt_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/extra/range_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/extra/table_image_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/file_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/font_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/font_trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/history_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/html_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/image_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/image_enum_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.853210 traitsui-7.4.3/traitsui/qt4/images/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/images/closetab.png
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/images/frame.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/images/list_editor.png
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/images/next.png
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/images/previous.png
--rw-r--r--   0 runner    (1001) docker     (123)    16305 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/instance_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/key_binding_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/key_event_to_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    27771 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/list_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/list_str_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/list_str_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/null_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/progress_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    26269 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/range_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/rgb_color_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/rgb_color_trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/search_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16188 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/set_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/shell_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/styled_date_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    50813 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/table_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    32678 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/tabular_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13340 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/tabular_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.857210 traitsui-7.4.3/traitsui/qt4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/tests/test_color_trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/tests/test_font_trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/tests/test_tabular_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/tests/test_ui_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/tests/test_ui_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/text_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/time_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/title_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)    67050 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/tree_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/tree_node_renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/tuple_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13831 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/ui_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/ui_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8174 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/ui_live.py
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/ui_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    48127 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/ui_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/value_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17880 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/video_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/qt4/view_application.py
--rw-r--r--   0 runner    (1001) docker     (123)    19877 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/table_column.py
--rw-r--r--   0 runner    (1001) docker     (123)    20132 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/table_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    28053 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tabular_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.857210 traitsui-7.4.3/traitsui/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/_exception_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.857210 traitsui-7.4.3/traitsui/testing/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/data/test.mp4
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.857210 traitsui-7.4.3/traitsui/testing/tester/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_abstract_target_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_dynamic_target_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.861210 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/_common_ui_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/_traitsui_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/default_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.861210 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_control_widget_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13753 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_interaction_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_registry_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.865210 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/boolean_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/button_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/check_list_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/directory_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/editor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/enum_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/file_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/font_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/instance_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/list_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/range_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/table_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/text_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/ui_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/default_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.865210 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/tests/test_control_widget_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/tests/test_interaction_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.865210 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/tests/test_default_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/tests/test_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.865210 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_control_widget_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_interaction_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_registry_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.865210 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/boolean_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/button_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/check_list_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/directory_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/editor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/enum_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/file_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/font_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/instance_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/list_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/range_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/text_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/ui_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/default_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.869210 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/tests/test_control_widget_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/tests/test_interaction_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/locator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/target_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.869210 traitsui-7.4.3/traitsui/testing/tester/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/tests/test_ui_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/tests/test_ui_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/ui_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tester/ui_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.869210 traitsui-7.4.3/traitsui/testing/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tests/test_exception_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/testing/tests/test_gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.873210 traitsui-7.4.3/traitsui/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8850 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.877210 traitsui-7.4.3/traitsui/tests/editors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_animatedGIF_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_boolean_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_button_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_check_list_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_code_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_csv_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_date_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_date_range_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_datetime_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_default_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_directory_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_drop_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15722 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_enum_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_file_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_font_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11636 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_html_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_image_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15567 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_image_enum_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_instance_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_list_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_liststr_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    26581 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_liststr_editor_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_range_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_range_editor_spinner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_range_editor_text.py
--rw-r--r--   0 runner    (1001) docker     (123)    19959 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_set_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_shell_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_styled_date_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    20245 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_table_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_tabular_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_text_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9767 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_tree_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_tuple_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/editors/test_video_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.877210 traitsui-7.4.3/traitsui/tests/null_backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/null_backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/null_backend/test_font_trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/null_backend/test_null_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_color_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_context_value.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    32502 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_shadow_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_splitter_prefs_restored.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_toolkit_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_tree_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    13981 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_ui_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_ui_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    37042 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_undo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_view_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/test_visible_when_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.877210 traitsui-7.4.3/traitsui/tests/ui_editors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/ui_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tests/ui_editors/test_data_frame_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/toolkit_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    56122 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tree_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/tree_node_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30438 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/ui_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.877210 traitsui-7.4.3/traitsui/ui_editors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/ui_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/ui_editors/array_view_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/ui_editors/data_frame_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/ui_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/ui_traits.py
--rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/undo.py
--rw-r--r--   0 runner    (1001) docker     (123)    15158 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/value_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/view_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/view_elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.889211 traitsui-7.4.3/traitsui/wx/
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/animated_gif_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/array_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/array_view_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/boolean_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/button_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/check_list_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14316 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/code_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/color_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/color_trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/compound_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/csv_list_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/custom_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/data_frame_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28963 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/date_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/directory_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/dnd_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/drop_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/editor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15251 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/enum_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.889211 traitsui-7.4.3/traitsui/wx/extra/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/extra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/extra/bounds_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/extra/led_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.889211 traitsui-7.4.3/traitsui/wx/extra/windows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/extra/windows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/extra/windows/flash_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/extra/windows/ie_html_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13746 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/file_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/font_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/font_trait.py
--rw-r--r--   0 runner    (1001) docker     (123)    20133 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/history_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/history_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/html_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/image_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/image_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/image_enum_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16383 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/image_slice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.893211 traitsui-7.4.3/traitsui/wx/images/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/cb_hover_off.png
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/cb_hover_on.png
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/cb_off.png
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/cb_on.png
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/file.png
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/frame.ico
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/group.png
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/hs_color_map.png
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/item.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/list_editor.png
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/nb_open.png
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/object.png
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/open.png
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/table_add.png
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/table_colors.png
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/table_delete.png
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/table_delete_synthetic.png
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/table_display.png
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/table_move_down.png
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/table_move_up.png
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/table_no_sort.png
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/table_prefs.png
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/table_search.png
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/table_synthetic.png
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/images/table_undelete.png
--rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/instance_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/key_binding_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/key_event_to_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    27202 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/list_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    34425 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/list_str_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/null_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/popup_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/progress_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30530 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/range_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/rgb_color_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/rgb_color_trait.py
--rw-r--r--   0 runner    (1001) docker     (123)    17475 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/scrubber_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/search_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/set_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/shell_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    54724 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/table_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    26267 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/table_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    41849 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/tabular_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.893211 traitsui-7.4.3/traitsui/wx/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/tests/test_color_trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/tests/test_font_trait.py
--rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/text_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/time_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/title_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)    60342 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/tree_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/tuple_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/ui_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/ui_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/ui_live.py
--rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/ui_modal.py
--rw-r--r--   0 runner    (1001) docker     (123)    42230 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/ui_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/ui_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/ui_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/value_editor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-01-12 15:35:01.000000 traitsui-7.4.3/traitsui/wx/view_application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 15:35:18.813210 traitsui-7.4.3/traitsui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-01-12 15:35:18.000000 traitsui-7.4.3/traitsui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    43683 2023-01-12 15:35:18.000000 traitsui-7.4.3/traitsui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 15:35:18.000000 traitsui-7.4.3/traitsui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-12 15:35:18.000000 traitsui-7.4.3/traitsui.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 15:35:18.000000 traitsui-7.4.3/traitsui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-12 15:35:18.000000 traitsui-7.4.3/traitsui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-12 15:35:18.000000 traitsui-7.4.3/traitsui.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.127806 traitsui-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    43996 2023-05-22 15:06:53.000000 traitsui-8.0.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-22 15:06:53.000000 traitsui-8.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-22 15:06:53.000000 traitsui-8.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-22 15:07:08.127806 traitsui-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-22 15:06:53.000000 traitsui-8.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26449 2023-05-22 15:06:53.000000 traitsui-8.0.0/README_example.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.011807 traitsui-8.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/api.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.011807 traitsui-8.0.0/docs/releases/
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/releases/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.011807 traitsui-8.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.011807 traitsui-8.0.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    13514 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/_static/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12938 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/_static/e-logo-rev.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/_static/et.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.011807 traitsui-8.0.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/_templates/search.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.011807 traitsui-8.0.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.011807 traitsui-8.0.0/docs/source/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/demos/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/e-logo-rev.png
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.011807 traitsui-8.0.0/docs/source/traitsui_dev_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_dev_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12940 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_dev_guide/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.011807 traitsui-8.0.0/docs/source/traitsui_user_manual/
+-rw-r--r--   0 runner    (1001) docker     (123)    40261 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/adapters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/advanced_view.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15727 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/custom_view.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.015807 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/configure_traits_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/configure_traits_view_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/configure_traits_view_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/default_trait_editors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/default_traits_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/default_traits_view2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/enum_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/handler_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/instance_editor_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/mixed_styles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/multi_object_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/multiple_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/tree_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/examples/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44546 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/factories_advanced_extra.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    48820 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/factories_basic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14349 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/factory_intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26564 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/handler.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.023807 traitsui-8.0.0/docs/source/traitsui_user_manual/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/ArrayEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31800 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/Auto_update_TabularEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18250 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/BooleanEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25277 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/ButtonEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   136429 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/CSVListEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30686 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/CheckListEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    67783 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/CodeEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24171 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/ColorEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30732 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/CompoundEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40284 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/DataFrameEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29229 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/DatetimeEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    45058 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/DirectoryEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    51855 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/Dynamic_EnumEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    69313 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/EnumEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26841 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/FileEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    34967 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/FontEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   183346 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/HTMLEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/HTML_editor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23464 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/ImageEnumEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56162 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/InstanceEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55913 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/ListEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41149 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/ListStrEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22734 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/RGBColorEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46064 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/RangeEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30984 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/SetEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    72355 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/TableEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    38070 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/TextEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50097 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/TitleEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50534 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/TreeEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    46529 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/TupleEditor_demo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/alter_title_after.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/alter_title_before.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28539 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/array_view_editor.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    32421 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/color_picker_windows.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/custom_enum_editor.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/default_text_editor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/delete_item_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    28592 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/font_dialog_windows.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    20452 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/html_code_editor.png
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/insert_item_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/key_binding_editor.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/led_editor.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/list_with_context_menu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/move_down_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/move_up_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/no_sort_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/notebook_list_editor.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/read_only_editor.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/search_table_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    12101 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/shell_editor.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/simple_enum_editor_closed.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/simple_enum_editor_open.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    18303 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/table_column_selection.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/table_prefs.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32469 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/tabular_editor.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/text_editor.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/text_editor_integers.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/text_editor_strings.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/text_editors_passwords.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex1.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex12.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex13.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex3.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex4.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex7.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/value_editor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18085 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/wizard_dialog_1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20059 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/images/wizard_dialog_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/predefined_traits.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.023807 traitsui-8.0.0/docs/source/traitsui_user_manual/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/scripts/regenerate_example_screenshots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.023807 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.027807 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/discussions/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/discussions/automated_vs_manual_test.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/discussions/compatibility_pyface_testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/discussions/debugging-gui-tests-at-runtime.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/discussions/event_loop_and_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/discussions/target_interaction_location.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/discussions/working_of_extensions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.027807 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/howtos/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/howtos/add_new_interaction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/howtos/add_new_location.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.027807 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/references/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/references/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/substitutions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.027807 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/tutorials/first_test.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:07.995807 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/tutorials/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.027807 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/tutorials/images/first_test/
+-rw-r--r--   0 runner    (1001) docker     (123)    20612 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/tutorials/images/first_test/init-app.png
+-rw-r--r--   0 runner    (1001) docker     (123)    24338 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/tutorials/images/first_test/modified-fields.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.027807 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/tutorials/images/test_with_nested_object/
+-rw-r--r--   0 runner    (1001) docker     (123)    29097 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/tutorials/images/test_with_nested_object/init-app.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing/tutorials/test_with_nested_object.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/tips.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24053 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/traitsui_user_manual/view.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.027807 traitsui-8.0.0/docs/source/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.027807 traitsui-8.0.0/docs/source/tutorials/code_snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/code_snippets/code_block0.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/code_snippets/code_block1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/code_snippets/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/code_snippets/echo_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/code_snippets/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/code_snippets/event_loop_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/code_snippets/event_loop_wx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/code_snippets/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/code_snippets/mpl_figure_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/code_snippets/thread_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/code_snippets/traits_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.031807 traitsui-8.0.0/docs/source/tutorials/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   381388 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/images/application1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   386443 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/images/application2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   371915 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/images/application3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/images/code_block1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/images/container.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/images/interactive.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29983 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/images/mpl_figure_editor.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/images/traits_thread.png
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    39260 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/source/tutorials/traits_ui_scientific_app.rst
+-rw-r--r--   0 runner    (1001) docker     (123)  1907712 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/traits_ui.ppt
+-rw-r--r--   0 runner    (1001) docker     (123)   664962 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/traits_ui_slides.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-22 15:06:53.000000 traitsui-8.0.0/docs/traitsuidocreadme.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-22 15:06:53.000000 traitsui-8.0.0/edm.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.031807 traitsui-8.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.031807 traitsui-8.0.0/examples/demo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.039807 traitsui-8.0.0/examples/demo/Advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Adapted_tree_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Apply_Revert_handler_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Auto_editable_readonly_table_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Auto_update_TabularEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Date_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Date_range_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Dynamic_EnumEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Dynamic_range_trait_and_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Dynamic_views_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Dynamically_changing_buttons_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/HDF5_tree_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/HDF5_tree_demo2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/History_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Invalid_state_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/ListStrAdapter_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/ListStrEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/List_editor_notebook_selection_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/List_editors_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/MVC_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Multi_select_string_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Multi_thread_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Multi_thread_demo_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/NumPy_array_tabular_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/NumPy_array_view_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Popup_Dialog_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Property_List_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Scrubber_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Settable_cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Statusbar_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/String_list_ui_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Table_editor_with_checkbox_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Table_editor_with_context_menu_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Table_editor_with_live_search_and_cell_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Table_editor_with_progress_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12359 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Tabular_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Tabular_editor_with_context_menu_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Time_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/Tree_editor_required_traits_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)  1087120 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/test_fixed.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  1101753 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/test_fixed_compressed.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/test_h5pydata.h5
+-rw-r--r--   0 runner    (1001) docker     (123)   356712 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/test_table_dc.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    85584 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/test_table_no_dc.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.039807 traitsui-8.0.0/examples/demo/Advanced/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Advanced/tests/test_List_editor_notebook_selection_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.039807 traitsui-8.0.0/examples/demo/Applications/
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Applications/Python_source_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Applications/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.039807 traitsui-8.0.0/examples/demo/Applications/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Applications/images/GG5.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Applications/images/TFB.png
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Applications/images/blue_ball.png
+-rw-r--r--   0 runner    (1001) docker     (123)    65791 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Applications/images/header.png
+-rw-r--r--   0 runner    (1001) docker     (123)    65461 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Applications/images/notebook_close.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87952 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Applications/images/notebook_open.png
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Applications/images/red_ball.png
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Applications/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.039807 traitsui-8.0.0/examples/demo/Applications/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Applications/tests/test_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.039807 traitsui-8.0.0/examples/demo/Dynamic_Forms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Dynamic_Forms/dynamic_form_using_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Dynamic_Forms/dynamic_range_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Dynamic_Forms/dynamic_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Dynamic_Forms/enabled_when.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Dynamic_Forms/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.039807 traitsui-8.0.0/examples/demo/Dynamic_Forms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Dynamic_Forms/tests/test_visible_when.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Dynamic_Forms/visible_when.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.043807 traitsui-8.0.0/examples/demo/Extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Extras/Image_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Extras/LED_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Extras/Tree_editor_with_TreeNodeRenderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Extras/animated_GIF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.043807 traitsui-8.0.0/examples/demo/Extras/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Extras/images/info.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23579 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Extras/images/logo_32x32.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    39542 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Extras/images/logo_48x48.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    57367 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Extras/images/logo_64x64.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Extras/images/python-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Extras/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.043807 traitsui-8.0.0/examples/demo/Extras/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Extras/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Extras/tests/test_Image_editor_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.043807 traitsui-8.0.0/examples/demo/Extras/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Extras/windows/flash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Extras/windows/internet_explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.043807 traitsui-8.0.0/examples/demo/Misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Misc/demo_group_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Misc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Misc/using_springs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.047807 traitsui-8.0.0/examples/demo/Standard_Editors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/ArrayEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/BooleanEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/BooleanEditor_simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/ButtonEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/ButtonEditor_simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/CSVListEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/CheckListEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/CheckListEditor_simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/CodeEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/ColorEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/CompoundEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/DataFrameEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/DatetimeEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/DirectoryEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/EnumEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/FileEditor_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.047807 traitsui-8.0.0/examples/demo/Standard_Editors/File_Dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/File_Dialog/File_Open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Custom_Extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/File_Dialog/File_Open_with_FileInfo_Extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/File_Dialog/File_Open_with_ImageInfo_Extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Multiple_Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/File_Dialog/File_Open_with_TextInfo_Extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/FontEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/HTMLEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/ImageEnumEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/InstanceEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/ListEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/RGBColorEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/RangeEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/SetEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/TableEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/TextEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/TitleEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/TreeEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/TupleEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/VideoEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.047807 traitsui-8.0.0/examples/demo/Standard_Editors/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_BooleanEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_BooleanEditor_simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_ButtonEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_ButtonEditor_simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_CheckListEditor_simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_EnumEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_FileEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_InstanceEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_ListEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_RangeEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_TableEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_TextEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/examples.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    43203 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/demo/traits_ui_demo.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.047807 traitsui-8.0.0/examples/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/default.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.051807 traitsui-8.0.0/examples/tutorials/doc_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/doc_examples/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/doc_examples/doc_examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.051807 traitsui-8.0.0/examples/tutorials/doc_examples/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/doc_examples/examples/include_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/doc_examples/examples/lesson.desc
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/doc_examples/examples/override_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/doc_examples/examples/view_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/doc_examples/examples/view_multi_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/doc_examples/examples/view_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/doc_examples/lesson.desc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.051807 traitsui-8.0.0/examples/tutorials/traitsui_4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/default.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/deferred.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.051807 traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/animated_gif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/flash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/ie_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/led.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.051807 traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/tabular_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/tabular_editor/numpy_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/tabular_editor/python_source_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/tabular_editor/sm_person_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50543 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/tabular_editor/tabular_editor.htm
+-rw-r--r--   0 runner    (1001) docker     (123)    42131 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/tabular_editor/tabular_editor.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/tabular_editor/tutorial.desc
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/tutorial.desc
+-rw-r--r--   0 runner    (1001) docker     (123)     8892 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/model_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/traitsui_4.0/tutorial.desc
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-22 15:06:53.000000 traitsui-8.0.0/examples/tutorials/tutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-22 15:06:53.000000 traitsui-8.0.0/image_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-05-22 15:06:53.000000 traitsui-8.0.0/image_LICENSE_Eclipse.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-05-22 15:06:53.000000 traitsui-8.0.0/image_LICENSE_Nuvola.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-22 15:06:53.000000 traitsui-8.0.0/image_LICENSE_OOo.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.051807 traitsui-8.0.0/integrationtests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/styled_date_editor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11264 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/test_all_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.055807 traitsui-8.0.0/integrationtests/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/array_editor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/buttons_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/check_list_editor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/check_list_editor_test2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/code_editor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/enum_dynamic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/enum_editor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/html_editor_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.055807 traitsui-8.0.0/integrationtests/ui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/images/bottom_left_origin.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/images/bottom_right_origin.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/images/top_left_origin.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/images/top_right_origin.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/instance_drag_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/instance_editor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/instance_editor_test2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/instance_editor_test3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/instance_editor_test4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/instance_editor_test5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/instance_editor_test6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/large_range_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/list_traits_ui_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/set_dynamic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/shell_editor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/table_editor_focus_bug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/table_editor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/table_editor_test2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/table_list_editor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/test_ui3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/test_ui4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9981 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/test_ui5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/text_editor_invalid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-05-22 15:06:53.000000 traitsui-8.0.0/integrationtests/ui/tree_editor_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-22 15:06:53.000000 traitsui-8.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 15:07:08.127806 traitsui-8.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.063807 traitsui-8.0.0/traitsui/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8468 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6063 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/basic_editor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/color_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/context_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/default_dock_window_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/delegating_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/dock_window_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/dockable_view_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28072 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10647 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editor_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.067807 traitsui-8.0.0/traitsui/editors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/array_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2364 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/boolean_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/button_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/check_list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/code_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/color_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/compound_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13593 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/csv_list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/custom_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/date_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/date_range_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/datetime_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/default_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/directory_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/dnd_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/drop_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/enum_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/file_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/font_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/history_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/html_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/image_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/image_enum_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/instance_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/key_binding_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/list_str_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/null_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/popup_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/progress_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9829 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/range_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/rgb_color_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/scrubber_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/search_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/set_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/shell_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/styled_date_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/table_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/tabular_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/text_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/time_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/title_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/tree_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/tuple_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/value_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/editors/video_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:07.999807 traitsui-8.0.0/traitsui/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.067807 traitsui-8.0.0/traitsui/examples/demo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.075807 traitsui-8.0.0/traitsui/examples/demo/Advanced/
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Adapted_tree_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Apply_Revert_handler_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Auto_editable_readonly_table_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Auto_update_TabularEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Date_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Date_range_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Dynamic_EnumEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Dynamic_range_trait_and_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Dynamic_views_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Dynamically_changing_buttons_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7697 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/HDF5_tree_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9810 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/HDF5_tree_demo2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/History_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Invalid_state_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/ListStrAdapter_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/ListStrEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/List_editor_notebook_selection_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/List_editors_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/MVC_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Multi_select_string_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Multi_thread_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Multi_thread_demo_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/NumPy_array_tabular_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/NumPy_array_view_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Popup_Dialog_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Property_List_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7177 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Scrubber_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Settable_cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Statusbar_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4565 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/String_list_ui_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Table_editor_with_checkbox_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Table_editor_with_context_menu_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14930 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Table_editor_with_live_search_and_cell_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Table_editor_with_progress_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12359 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Tabular_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Tabular_editor_with_context_menu_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Time_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/Tree_editor_required_traits_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)  1087120 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/test_fixed.h5
+-rw-r--r--   0 runner    (1001) docker     (123)  1101753 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/test_fixed_compressed.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/test_h5pydata.h5
+-rw-r--r--   0 runner    (1001) docker     (123)   356712 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/test_table_dc.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    85584 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/test_table_no_dc.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.075807 traitsui-8.0.0/traitsui/examples/demo/Advanced/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Advanced/tests/test_List_editor_notebook_selection_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.075807 traitsui-8.0.0/traitsui/examples/demo/Applications/
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Applications/Python_source_browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Applications/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.079807 traitsui-8.0.0/traitsui/examples/demo/Applications/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Applications/images/GG5.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Applications/images/TFB.png
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Applications/images/blue_ball.png
+-rw-r--r--   0 runner    (1001) docker     (123)    65791 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Applications/images/header.png
+-rw-r--r--   0 runner    (1001) docker     (123)    65461 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Applications/images/notebook_close.png
+-rw-r--r--   0 runner    (1001) docker     (123)    87952 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Applications/images/notebook_open.png
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Applications/images/red_ball.png
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Applications/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.079807 traitsui-8.0.0/traitsui/examples/demo/Applications/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Applications/tests/test_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.079807 traitsui-8.0.0/traitsui/examples/demo/Dynamic_Forms/
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Dynamic_Forms/dynamic_form_using_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Dynamic_Forms/dynamic_range_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Dynamic_Forms/dynamic_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Dynamic_Forms/enabled_when.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Dynamic_Forms/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.079807 traitsui-8.0.0/traitsui/examples/demo/Dynamic_Forms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Dynamic_Forms/tests/test_visible_when.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Dynamic_Forms/visible_when.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.079807 traitsui-8.0.0/traitsui/examples/demo/Extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Extras/Image_editor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Extras/LED_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Extras/Tree_editor_with_TreeNodeRenderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Extras/animated_GIF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.079807 traitsui-8.0.0/traitsui/examples/demo/Extras/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8743 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Extras/images/info.png
+-rw-r--r--   0 runner    (1001) docker     (123)    23579 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Extras/images/logo_32x32.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    39542 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Extras/images/logo_48x48.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    57367 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Extras/images/logo_64x64.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Extras/images/python-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Extras/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.079807 traitsui-8.0.0/traitsui/examples/demo/Extras/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Extras/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Extras/tests/test_Image_editor_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.079807 traitsui-8.0.0/traitsui/examples/demo/Extras/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Extras/windows/flash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Extras/windows/internet_explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.079807 traitsui-8.0.0/traitsui/examples/demo/Misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Misc/demo_group_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Misc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Misc/using_springs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.083807 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/ArrayEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/BooleanEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/BooleanEditor_simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/ButtonEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/ButtonEditor_simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/CSVListEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/CheckListEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/CheckListEditor_simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/CodeEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/ColorEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/CompoundEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/DataFrameEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/DatetimeEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/DirectoryEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/EnumEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/FileEditor_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.083807 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/File_Dialog/
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Custom_Extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_FileInfo_Extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_ImageInfo_Extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Multiple_Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_TextInfo_Extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/FontEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/HTMLEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/ImageEnumEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/InstanceEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/ListEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/RGBColorEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4636 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/RangeEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3444 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/SetEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/TableEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/TextEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/TitleEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/TreeEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/TupleEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/VideoEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.087807 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_BooleanEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_BooleanEditor_simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_ButtonEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_ButtonEditor_simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_CheckListEditor_simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_EnumEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_FileEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_InstanceEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_ListEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_RangeEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_TableEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_TextEditor_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/examples.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    43203 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/examples/demo/traits_ui_demo.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.087807 traitsui-8.0.0/traitsui/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/extras/_demo_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34730 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/extras/_demo_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/extras/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/extras/checkbox_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/extras/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/extras/edit_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14886 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/extras/has_dynamic_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.087807 traitsui-8.0.0/traitsui/extras/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/extras/images/next.png
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/extras/images/parent.png
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/extras/images/previous.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/extras/images/reload.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/extras/images/run.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/extras/progress_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/extras/saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20213 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/file_dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24493 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20189 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/help_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.087807 traitsui-8.0.0/traitsui/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/images/frame.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/instance_choice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19265 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12084 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/list_str_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/mimedata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.087807 traitsui-8.0.0/traitsui/null/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/null/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/null/color_trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/null/font_trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/null/rgb_color_trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/null/toolkit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.095806 traitsui-8.0.0/traitsui/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/array_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/array_view_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/boolean_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/button_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/check_list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/clipboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10702 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/code_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/color_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/color_trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/compound_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/csv_list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/custom_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/data_frame_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/date_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/date_range_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/datetime_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/directory_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/drop_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14709 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/editor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16640 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/enum_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.095806 traitsui-8.0.0/traitsui/qt/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/extra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/extra/bounds_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/extra/checkbox_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/extra/led_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/extra/progress_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/extra/qt_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/extra/range_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/extra/table_image_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10792 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/file_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/font_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/font_trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/history_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/html_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/image_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/image_enum_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.095806 traitsui-8.0.0/traitsui/qt/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/images/closetab.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/images/frame.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/images/list_editor.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/images/next.png
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/images/previous.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16391 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/instance_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/key_binding_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/key_event_to_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27771 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20640 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/list_str_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/list_str_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/null_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/progress_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26172 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/range_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/rgb_color_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/rgb_color_trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/search_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16188 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/set_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/shell_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/styled_date_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50812 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/table_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17099 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/tabular_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13339 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/tabular_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.099806 traitsui-8.0.0/traitsui/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/tests/test_color_trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6667 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/tests/test_font_trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/tests/test_tabular_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/tests/test_ui_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/tests/test_ui_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/text_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/time_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/title_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14358 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67050 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/tree_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/tree_node_renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/tuple_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13831 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/ui_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/ui_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8174 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/ui_live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/ui_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48126 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/ui_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/value_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17880 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/video_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt/view_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.099806 traitsui-8.0.0/traitsui/qt4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/qt4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19877 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/table_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20132 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/table_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28053 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tabular_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.099806 traitsui-8.0.0/traitsui/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/_exception_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.099806 traitsui-8.0.0/traitsui/testing/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/data/test.mp4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.099806 traitsui-8.0.0/traitsui/testing/tester/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_abstract_target_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_dynamic_target_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.099806 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/_common_ui_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/_traitsui_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/default_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.103807 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_control_widget_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13752 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_interaction_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_registry_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.103807 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/boolean_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/button_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/check_list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/directory_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/editor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/enum_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/file_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/font_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/instance_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/range_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4137 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/table_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/text_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/ui_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/default_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.103807 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/tests/test_control_widget_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8771 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/tests/test_interaction_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.103807 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/tests/test_default_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/tests/test_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.103807 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_control_widget_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_interaction_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_registry_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.107807 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/boolean_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/button_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/check_list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/directory_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/editor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/enum_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/file_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/font_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/instance_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/range_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/text_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/ui_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/default_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.107807 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/tests/test_control_widget_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/tests/test_interaction_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/locator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/target_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.107807 traitsui-8.0.0/traitsui/testing/tester/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7743 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/tests/test_ui_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/tests/test_ui_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/ui_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tester/ui_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.107807 traitsui-8.0.0/traitsui/testing/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tests/test_exception_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/testing/tests/test_gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.111806 traitsui-8.0.0/traitsui/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.115806 traitsui-8.0.0/traitsui/tests/editors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_animatedGIF_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4334 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_boolean_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_button_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17967 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_check_list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_code_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_csv_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_date_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8774 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_date_range_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_datetime_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_default_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3993 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_directory_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_drop_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15721 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_enum_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_file_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_font_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_html_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_image_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_image_enum_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14616 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_instance_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_liststr_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26580 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_liststr_editor_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19634 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_range_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_range_editor_spinner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_range_editor_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19959 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_set_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_shell_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_styled_date_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20245 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_table_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_tabular_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14180 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_text_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9767 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_tree_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_tuple_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/editors/test_video_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.115806 traitsui-8.0.0/traitsui/tests/null_backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/null_backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/null_backend/test_font_trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/null_backend/test_null_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_color_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_context_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32502 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_editors_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8023 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_shadow_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_splitter_prefs_restored.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_toolkit_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_tree_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13978 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_ui_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_ui_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36556 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_undo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_view_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/test_visible_when_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.115806 traitsui-8.0.0/traitsui/tests/ui_editors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/ui_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17052 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tests/ui_editors/test_data_frame_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/toolkit_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56102 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tree_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/tree_node_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30346 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/ui_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.115806 traitsui-8.0.0/traitsui/ui_editors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/ui_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5398 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/ui_editors/array_view_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/ui_editors/data_frame_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/ui_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6915 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/ui_traits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14243 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/undo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15158 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/value_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/view_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/view_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.123806 traitsui-8.0.0/traitsui/wx/
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/animated_gif_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/array_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/array_view_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/boolean_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/button_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/check_list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14340 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/code_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/color_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/color_trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/compound_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/csv_list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/custom_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/data_frame_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28963 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/date_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/directory_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/dnd_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/drop_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/editor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15251 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/enum_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.123806 traitsui-8.0.0/traitsui/wx/extra/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/extra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8024 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/extra/bounds_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/extra/led_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.123806 traitsui-8.0.0/traitsui/wx/extra/windows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/extra/windows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/extra/windows/flash_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/extra/windows/ie_html_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13755 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/file_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10614 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/font_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/font_trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20133 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/history_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/history_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/html_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/image_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/image_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/image_enum_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16383 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/image_slice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.127806 traitsui-8.0.0/traitsui/wx/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/cb_hover_off.png
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/cb_hover_on.png
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/cb_off.png
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/cb_on.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/frame.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/group.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/hs_color_map.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/item.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      404 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/list_editor.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/nb_open.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/object.png
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/open.png
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/table_add.png
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/table_colors.png
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/table_delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/table_delete_synthetic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/table_display.png
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/table_move_down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/table_move_up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/table_no_sort.png
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/table_prefs.png
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/table_search.png
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/table_synthetic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/images/table_undelete.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/instance_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/key_binding_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/key_event_to_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27202 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/list_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34469 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/list_str_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/null_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/popup_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/progress_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30433 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/range_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/rgb_color_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/rgb_color_trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17475 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/scrubber_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/search_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16957 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/set_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/shell_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54724 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/table_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26267 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/table_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41893 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/tabular_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.127806 traitsui-8.0.0/traitsui/wx/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/tests/test_color_trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6545 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/tests/test_font_trait.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/text_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/time_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/title_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60342 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/tree_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/tuple_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/ui_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/ui_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14601 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/ui_live.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/ui_modal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42230 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/ui_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/ui_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/ui_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/value_editor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-05-22 15:06:53.000000 traitsui-8.0.0/traitsui/wx/view_application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 15:07:08.063807 traitsui-8.0.0/traitsui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5609 2023-05-22 15:07:07.000000 traitsui-8.0.0/traitsui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    43565 2023-05-22 15:07:07.000000 traitsui-8.0.0/traitsui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 15:07:07.000000 traitsui-8.0.0/traitsui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-22 15:07:07.000000 traitsui-8.0.0/traitsui.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-22 15:07:07.000000 traitsui-8.0.0/traitsui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 15:07:07.000000 traitsui-8.0.0/traitsui.egg-info/top_level.txt
```

### Comparing `traitsui-7.4.3/CHANGES.txt` & `traitsui-8.0.0/CHANGES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,62 @@
 Traits UI Changelog
 ===================
 
+Release 8.0.0
+-------------
+
+This is a major release that provides support for PySide 6.4 and 6.5 as well
+as Python 3.11.  It includes a number of backwards-incompatible changes
+following the example of Pyface 8.0.0, most notable is moving the
+`traitsui.qt4.*` modules to `traitsui.qt.*`.  As with Pyface 8.0 we include
+a backwards-compatibility mode which allows importing from the 'qt4' namespace
+via:
+
+- setting the ETS toolkit to `"qt4"`
+- setting the ETS_QT4_IMPORTS environment variable
+- manually adding appropriate finders to sys.meta_path
+
+This release also removes a number of features deprecated since TraitsUI 7.0.
+
+Thanks To
+---------
+
+* David Baddeley
+* Mark Dickinson
+* Dominik Gresch
+* hopeful0
+* Chengyu Liu
+* Orion Poplawski
+* Corran Webster
+
+Features
+--------
+
+* Be strict about 'handler.init()' return values (#2008)
+* Move 'traitsui.qt4.*' to 'traitsui.qt.*' (#2004)
+* Remove deprecated 'format' trait (#2002)
+* Deprecate imports from traitsui.editors (use traitsui.editors.api) (#2000)
+* Remove backwards-compatibility mode in undo/redo code (#1999)
+* Support for Python 3.11 and PySide 6.4+ (#1994)
+
+Fixes
+-----
+
+* Fix uses of None in date range editor (#2019)
+* Add comments for Wx-only examples (#2011, #2020)
+* Replace uses of "fast_ui" dispatch with "ui" dispatch (#2009)
+* Fix FileDialog selection actions (#2003)
+* Fix regression in Wx version of FileEditor (#1993)
+* Fix missing attribute of InstanceFactoryChocie (#1989)
+
+Test suite
+----------
+
+* Replace some relative imports in tests (#1985)
+
 Release 7.4.3
 -------------
 
 This is a small bugfix release which resolves some bugs that have come to light
 as we get more experience with PySide 6, together with changes to run CI on
 more recent Python versions and current Github infrastructure.
```

### Comparing `traitsui-7.4.3/LICENSE.txt` & `traitsui-8.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/README.rst` & `traitsui-8.0.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 - PyQt5
 
 Backends have additional dependencies and there are optional dependencies on
 NumPy and Pandas for some editors.
 
 TraitsUI along with all dependencies can be installed in a straightforward way
 using the `Enthought Deployment Manager <http://docs.enthought.com/edm/>`__,
-``pip`` or other .
+``pip`` or other package managers.
 
 .. end_of_long_description
 
 Running the Test Suite
 ----------------------
 
 To run the test suite, you will need to install Git and
```

### Comparing `traitsui-7.4.3/README_example.png` & `traitsui-8.0.0/README_example.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/Makefile` & `traitsui-8.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/README.rst` & `traitsui-8.0.0/docs/README.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/api.css` & `traitsui-8.0.0/docs/api.css`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/make.bat` & `traitsui-8.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/releases/README.rst` & `traitsui-8.0.0/docs/releases/README.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/_static/default.css` & `traitsui-8.0.0/docs/source/_static/default.css`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/_static/e-logo-rev.jpg` & `traitsui-8.0.0/docs/source/_static/e-logo-rev.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/_static/et.png` & `traitsui-8.0.0/docs/source/_static/et.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/_templates/search.html` & `traitsui-8.0.0/docs/source/_templates/search.html`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/conf.py` & `traitsui-8.0.0/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,15 +224,14 @@
 # Documents to append as an appendix to all manuals.
 # latex_appendices = []
 
 # If false, no module index is generated.
 # latex_use_modindex = True
 
 # Autodoc options
-autodo_mock_imports = ["wx", "PySide", "PyQt", "PyQt5"]
 
 # Intersphinx configuration
 intersphinx_mapping = {
     'traits': ('http://docs.enthought.com/traits', None),
     'pyface': ('http://docs.enthought.com/pyface', None),
 }
```

### Comparing `traitsui-7.4.3/docs/source/demos/index.rst` & `traitsui-8.0.0/docs/source/demos/index.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/e-logo-rev.png` & `traitsui-8.0.0/docs/source/e-logo-rev.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_dev_guide/index.rst` & `traitsui-8.0.0/docs/source/traitsui_dev_guide/index.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_dev_guide/testing.rst` & `traitsui-8.0.0/docs/source/traitsui_dev_guide/testing.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/adapters.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/adapters.rst`

 * *Files 0% similar despite different names*

```diff
@@ -248,15 +248,15 @@
 Custom Renderers
 ----------------
 
 The Qt backend allows users to completely override the rendering of cells in
 a TreeEditor.  To do this, the TreeNode should override the
 :py:meth:`TreeNode.get_renderer` method to return an instance of a
 subclass of :py:class:`~traitsui.tree_node_renderer.AbstractTreeNodeRenderer`.
-A :py:class:`~traitsui.qt4.tree_node_renderers.WordWrapRenderer` is available
+A :py:class:`~traitsui.qt.tree_node_renderers.WordWrapRenderer` is available
 to provide basic word-wrapped layout in a cell, but user-defined subclasses
 can do any rendering that they want by implementing their own
 :py:class:`~traitsui.tree_node_renderer.AbstractTreeNodeRenderer` subclass.
 
 :py:class:`~traitsui.tree_node_renderer.AbstractTreeNodeRenderer` is an
 abstract base class, and subclasses must implement two methods:
```

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/advanced_view.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/advanced_view.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/custom_view.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/custom_view.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/examples/configure_traits_view.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/examples/configure_traits_view.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/examples/configure_traits_view_buttons.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/examples/configure_traits_view_buttons.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/examples/configure_traits_view_group.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/examples/configure_traits_view_group.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/examples/default_trait_editors.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/examples/default_trait_editors.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/examples/default_traits_view.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/examples/default_traits_view.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/examples/default_traits_view2.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/examples/default_traits_view2.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/examples/enum_editor.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/examples/enum_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/examples/handler_override.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/examples/handler_override.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/examples/instance_editor_selection.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/examples/instance_editor_selection.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/examples/key_bindings.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/examples/key_bindings.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/examples/mixed_styles.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/examples/mixed_styles.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/examples/multi_object_view.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/examples/multi_object_view.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/examples/multiple_views.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/examples/multiple_views.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/examples/tree_editor.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/examples/tree_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/examples/wizard.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/examples/wizard.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/factories_advanced_extra.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/factories_advanced_extra.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/factories_basic.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/factories_basic.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/factory_intro.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/factory_intro.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/glossary.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/glossary.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/handler.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/handler.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/ArrayEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/ArrayEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/Auto_update_TabularEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/Auto_update_TabularEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/BooleanEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/BooleanEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/ButtonEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/ButtonEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/CSVListEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/CSVListEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/CheckListEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/CheckListEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/CodeEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/CodeEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/ColorEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/ColorEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/CompoundEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/CompoundEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/DataFrameEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/DataFrameEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/DatetimeEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/DatetimeEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/DirectoryEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/DirectoryEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/Dynamic_EnumEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/Dynamic_EnumEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/EnumEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/EnumEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/FileEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/FileEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/FontEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/FontEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/HTMLEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/HTMLEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/HTML_editor.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/HTML_editor.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/ImageEnumEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/ImageEnumEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/InstanceEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/InstanceEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/ListEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/ListEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/ListStrEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/ListStrEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/RGBColorEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/RGBColorEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/RangeEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/RangeEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/SetEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/SetEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/TableEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/TableEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/TextEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/TextEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/TitleEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/TitleEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/TreeEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/TreeEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/TupleEditor_demo.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/TupleEditor_demo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/alter_title_after.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/alter_title_after.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/alter_title_before.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/alter_title_before.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/array_view_editor.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/array_view_editor.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/color_picker_windows.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/color_picker_windows.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/custom_enum_editor.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/custom_enum_editor.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/default_text_editor.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/default_text_editor.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/delete_item_icon.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/delete_item_icon.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/font_dialog_windows.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/font_dialog_windows.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/html_code_editor.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/html_code_editor.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/key_binding_editor.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/key_binding_editor.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/led_editor.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/led_editor.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/list_with_context_menu.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/list_with_context_menu.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/move_down_icon.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/move_down_icon.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/move_up_icon.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/move_up_icon.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/no_sort_icon.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/no_sort_icon.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/notebook_list_editor.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/notebook_list_editor.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/read_only_editor.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/read_only_editor.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/search_table_icon.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/search_table_icon.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/shell_editor.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/shell_editor.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/simple_enum_editor_closed.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/simple_enum_editor_closed.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/simple_enum_editor_open.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/simple_enum_editor_open.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/table_column_selection.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/table_column_selection.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/tabular_editor.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/tabular_editor.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/text_editor.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/text_editor.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/text_editor_integers.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/text_editor_integers.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/text_editor_strings.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/text_editor_strings.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/text_editors_passwords.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/text_editors_passwords.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex1.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex1.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex12.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex12.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex13.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex13.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex16.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex16.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex2.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex2.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex3.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex3.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex4.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex4.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/ui_for_ex7.jpg` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/ui_for_ex7.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/value_editor.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/value_editor.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/wizard_dialog_1.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/wizard_dialog_1.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/images/wizard_dialog_2.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/images/wizard_dialog_2.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/index.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/index.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/intro.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/intro.rst`

 * *Files 8% similar despite different names*

```diff
@@ -115,17 +115,17 @@
 .. index:: ETSConfig.toolkit
 
 The values of **ETSConfig.toolkit** that are supported by TraitsUI version |version|
 are:
 
 .. index:: wxPython toolkit, Qt toolkit, null toolkit
 
-* 'qt4' or 'qt': `PyQt <http://riverbankcomputing.co.uk/pyqt/>`_ or
-  `Qt for Python/PySide2 <https://doc.qt.io/qtforpython/>`_, which provides Python
-  bindings for the `Qt <https://www.qt.io/>`_ framework version 4 or 5.
+* 'qt' or 'qt4': `PyQt5 <http://riverbankcomputing.co.uk/pyqt/>`_,
+  `PySide2 or PySide6 <https://doc.qt.io/qtforpython/>`_, which provides Python
+  bindings for the `Qt <https://www.qt.io/>`_ framework version 5 or 6.
 * 'wx': `wxPython <http://www.wxpython.org>`_, which provides Python bindings
   for the `wxWidgets <http://wxwidgets.org>`_ toolkit.
 * 'null': A do-nothing toolkit, for situations where neither of the other
   toolkits is installed, but Traits is needed for non-UI purposes.
 
 The default behavior of TraitsUI is to search for available toolkit-specific
 packages in the order listed, and uses the first one it finds. The programmer or
@@ -140,14 +140,45 @@
    traits.  For example, at the beginning of a program::
 
        from traits.etsconfig.api import ETSConfig
        ETSConfig.toolkit = 'wx'
 
 #. The user can define a value for the ETS_TOOLKIT environment variable.
 
+Toolkit selection is largely carried out in Pyface rather than TraitsUI, where
+further details can be found.
+
+The "qt4" Toolkit
+`````````````````
+
+The "qt4" toolkit is the same as the "qt" toolkit in almost all respects:
+in older versions of TraitsUI it was the standard name for all the Qt-based
+toolkits whether or not they were actually using Qt4.
+
+However it does trigger some backwards-compatibility code that may be useful
+for legacy applications. In particular it installs import hooks that makes the
+``traitsui.qt4.*`` package namespace an alias for ``traitsui.qt.*`` modules.
+
+This backwards-compatibility code can also be invoked by setting the
+``ETS_QT4_IMPORTS`` environment variable to any non-empty value, or adding
+an instance of the :py:class:`pyface.ui.ShadowedModuleFinder` module finder
+to :py:attr:`sys.meta_path` list.
+
+..  warning::
+
+    Library code which imports from ``traitsui.qt4.*`` should not use this
+    compatibility code.  Instead it should be updated to import from
+    ``traitsui.qt.*`` as soon as practical.  Backwards-compatibility can be
+    achieved fairly easily by using :py:attr:`traitsui.toolkit.toolkit` to
+    access objects rather than direct imports.
+
+This backwards-compatibility code will be removed in TraitsUI 9, and
+applications which rely on the particulars of the implementation are encouraged
+to migrate to the newer import locations as soon as practical.
+
 .. _structure-of-this-guide:
 
 Structure of this Manual
 ------------------------
 
 The intent of this guide is to present the capabilities of the TraitsUI package
 in usable increments, so that you can create and display gradually more
```

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/predefined_traits.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/predefined_traits.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/scripts/regenerate_example_screenshots.py` & `traitsui-8.0.0/docs/source/traitsui_user_manual/scripts/regenerate_example_screenshots.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing/discussions/automated_vs_manual_test.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing/discussions/automated_vs_manual_test.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing/discussions/compatibility_pyface_testing.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing/discussions/compatibility_pyface_testing.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing/discussions/debugging-gui-tests-at-runtime.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing/discussions/debugging-gui-tests-at-runtime.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing/discussions/event_loop_and_exceptions.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing/discussions/event_loop_and_exceptions.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing/discussions/target_interaction_location.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing/discussions/target_interaction_location.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing/discussions/working_of_extensions.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing/discussions/working_of_extensions.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing/howtos/add_new_interaction.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing/howtos/add_new_interaction.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing/howtos/add_new_location.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing/howtos/add_new_location.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing/references/examples.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing/references/examples.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing/substitutions.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing/substitutions.rst`

 * *Files 2% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 .. |UIWrapper.find_by_name| replace:: :func:`~traitsui.testing.tester.ui_wrapper.UIWrapper.find_by_name`
 .. |UIWrapper.help| replace:: :func:`~traitsui.testing.tester.ui_wrapper.UIWrapper.help`
 .. |UIWrapper.inspect| replace:: :func:`~traitsui.testing.tester.ui_wrapper.UIWrapper.inspect`
 .. |UIWrapper.locate| replace:: :func:`~traitsui.testing.tester.ui_wrapper.UIWrapper.locate`
 .. |UIWrapper.perform| replace:: :func:`~traitsui.testing.tester.ui_wrapper.UIWrapper.perform`
 .. |UIWrapper._target| replace:: :attr:`~traitsui.testing.tester.ui_wrapper.UIWrapper._target`
 
-.. |ModalDialogTester| replace:: :class:`~pyface.ui.qt4.util.modal_dialog_tester.ModalDialogTester`
-.. |GuiTestAssistant| replace:: :class:`~pyface.ui.qt4.util.gui_test_assistant.GuiTestAssistant`
+.. |ModalDialogTester| replace:: :class:`~pyface.ui.qt.util.modal_dialog_tester.ModalDialogTester`
+.. |GuiTestAssistant| replace:: :class:`~pyface.ui.qt.util.gui_test_assistant.GuiTestAssistant`
```

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing/tutorials/first_test.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing/tutorials/first_test.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing/tutorials/images/first_test/init-app.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing/tutorials/images/first_test/init-app.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing/tutorials/images/first_test/modified-fields.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing/tutorials/images/first_test/modified-fields.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing/tutorials/images/test_with_nested_object/init-app.png` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing/tutorials/images/test_with_nested_object/init-app.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing/tutorials/test_with_nested_object.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing/tutorials/test_with_nested_object.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/testing.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/testing.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/tips.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/tips.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/traitsui_user_manual/view.rst` & `traitsui-8.0.0/docs/source/traitsui_user_manual/view.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/tutorials/code_snippets/code_block1.py` & `traitsui-8.0.0/docs/source/tutorials/code_snippets/code_block1.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/tutorials/code_snippets/container.py` & `traitsui-8.0.0/docs/source/tutorials/code_snippets/container.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/tutorials/code_snippets/mpl_figure_editor.py` & `traitsui-8.0.0/docs/source/tutorials/code_snippets/mpl_figure_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/tutorials/code_snippets/traits_thread.py` & `traitsui-8.0.0/docs/source/tutorials/code_snippets/traits_thread.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/tutorials/images/application1.png` & `traitsui-8.0.0/docs/source/tutorials/images/application1.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/tutorials/images/application2.png` & `traitsui-8.0.0/docs/source/tutorials/images/application2.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/tutorials/images/application3.png` & `traitsui-8.0.0/docs/source/tutorials/images/application3.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/tutorials/images/code_block1.png` & `traitsui-8.0.0/docs/source/tutorials/images/code_block1.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/tutorials/images/container.png` & `traitsui-8.0.0/docs/source/tutorials/images/container.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/tutorials/images/interactive.png` & `traitsui-8.0.0/docs/source/tutorials/images/interactive.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/tutorials/images/mpl_figure_editor.png` & `traitsui-8.0.0/docs/source/tutorials/images/mpl_figure_editor.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/tutorials/images/traits_thread.png` & `traitsui-8.0.0/docs/source/tutorials/images/traits_thread.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/source/tutorials/traits_ui_scientific_app.rst` & `traitsui-8.0.0/docs/source/tutorials/traits_ui_scientific_app.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/traits_ui.ppt` & `traitsui-8.0.0/docs/traits_ui.ppt`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/docs/traits_ui_slides.pdf` & `traitsui-8.0.0/docs/traits_ui_slides.pdf`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Adapted_tree_editor_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Adapted_tree_editor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Apply_Revert_handler_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Apply_Revert_handler_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Auto_editable_readonly_table_cells.py` & `traitsui-8.0.0/examples/demo/Advanced/Auto_editable_readonly_table_cells.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Auto_update_TabularEditor_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Auto_update_TabularEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Date_editor_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Date_editor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Date_range_editor_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Date_range_editor_demo.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,11 +43,11 @@
         print(self.date_range)
 
 
 # -- Set Up The Demo ------------------------------------------------------
 
 
 if __name__ == "__main__":
-    if ETSConfig.toolkit == "qt4":
+    if ETSConfig.toolkit in {"qt", "qt4"}:
         # DateRangeEditor is currently only available for qt backend.
         demo = DateRangeEditorDemo()
         demo.configure_traits()
```

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Dynamic_EnumEditor_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Dynamic_EnumEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Dynamic_range_trait_and_editor.py` & `traitsui-8.0.0/examples/demo/Advanced/Dynamic_range_trait_and_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Dynamic_views_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Dynamic_views_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Dynamically_changing_buttons_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Dynamically_changing_buttons_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/HDF5_tree_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/HDF5_tree_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/HDF5_tree_demo2.py` & `traitsui-8.0.0/examples/demo/Advanced/HDF5_tree_demo2.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/History_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/History_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Invalid_state_handling.py` & `traitsui-8.0.0/examples/demo/Advanced/Invalid_state_handling.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/ListStrAdapter_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/ListStrAdapter_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/ListStrEditor_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/ListStrEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/List_editor_notebook_selection_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/List_editor_notebook_selection_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/List_editors_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/List_editors_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/MVC_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/MVC_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Multi_select_string_list.py` & `traitsui-8.0.0/examples/demo/Advanced/Multi_select_string_list.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Multi_thread_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Multi_thread_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Multi_thread_demo_2.py` & `traitsui-8.0.0/examples/demo/Advanced/Multi_thread_demo_2.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/NumPy_array_tabular_editor_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/NumPy_array_tabular_editor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/NumPy_array_view_editor_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/NumPy_array_view_editor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Popup_Dialog_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Popup_Dialog_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Property_List_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Property_List_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Scrubber_editor_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Scrubber_editor_demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,18 @@
 
 - A dynamic range. This consists of three scrubbers: one
   to control the low end of the range, one to control the high end, and one
   that uses the high and low values to determine its range.
 
 For comparison purposes, the example also shows the same traits displayed using
 their default editors.
+
+Notes:
+
+- This demo only works on the wx backend.
 """
 
 # -- Imports --------------------------------------------------------------
 
 from traits.api import HasTraits, Range, Float
 
 from traitsui.api import View, VGroup, HGroup, Item, ScrubberEditor, spring
```

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Settable_cached_property.py` & `traitsui-8.0.0/examples/demo/Advanced/Settable_cached_property.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Statusbar_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Statusbar_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/String_list_ui_editor.py` & `traitsui-8.0.0/examples/demo/Advanced/String_list_ui_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     TabularEditor,
     View,
 )
 
 if ETSConfig.toolkit == 'wx':
     from traitsui.wx.ui_editor import UIEditor
 else:
-    from traitsui.qt4.ui_editor import UIEditor
+    from traitsui.qt.ui_editor import UIEditor
 
 
 # -- Define the reusable StringListEditor class and its helper classes --------
 
 # Define the tabular adapter used by the Traits UI string list editor:
 class MultiSelectAdapter(TabularAdapter):
```

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Table_editor_with_checkbox_column.py` & `traitsui-8.0.0/examples/demo/Advanced/Table_editor_with_checkbox_column.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Table_editor_with_context_menu_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Table_editor_with_context_menu_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Table_editor_with_live_search_and_cell_editor.py` & `traitsui-8.0.0/examples/demo/Advanced/Table_editor_with_live_search_and_cell_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Table_editor_with_progress_column.py` & `traitsui-8.0.0/examples/demo/Advanced/Table_editor_with_progress_column.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Tabular_editor_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Tabular_editor_demo.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 # -- Tabular Editor Definition --------------------------------------------
 # The tabular editor works in conjunction with an adapter class, derived from
 # TabularAdapter.
 tabular_editor = TabularEditor(
     adapter=ReportAdapter(),
     operations=['move', 'edit'],
     # Row titles are not supported in WX:
-    show_row_titles=ETSConfig.toolkit == 'qt4',
+    show_row_titles=(ETSConfig.toolkit in {"qt", "qt4"}),
 )
 
 
 # -- Report Class Definition ----------------------------------------------
 class Report(HasTraits):
 
     people = List(Person)
```

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Tabular_editor_with_context_menu_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Tabular_editor_with_context_menu_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Time_editor_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Time_editor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/Tree_editor_required_traits_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/Tree_editor_required_traits_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/test_fixed.h5` & `traitsui-8.0.0/examples/demo/Advanced/test_fixed.h5`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/test_fixed_compressed.h5` & `traitsui-8.0.0/examples/demo/Advanced/test_fixed_compressed.h5`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/test_h5pydata.h5` & `traitsui-8.0.0/examples/demo/Advanced/test_h5pydata.h5`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/test_table_dc.h5` & `traitsui-8.0.0/examples/demo/Advanced/test_table_dc.h5`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/test_table_no_dc.h5` & `traitsui-8.0.0/examples/demo/Advanced/test_table_no_dc.h5`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Advanced/tests/test_List_editor_notebook_selection_demo.py` & `traitsui-8.0.0/examples/demo/Advanced/tests/test_List_editor_notebook_selection_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Applications/Python_source_browser.py` & `traitsui-8.0.0/examples/demo/Applications/Python_source_browser.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Applications/converter.py` & `traitsui-8.0.0/examples/demo/Applications/converter.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Applications/images/GG5.png` & `traitsui-8.0.0/examples/demo/Applications/images/GG5.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Applications/images/TFB.png` & `traitsui-8.0.0/examples/demo/Applications/images/TFB.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Applications/images/blue_ball.png` & `traitsui-8.0.0/examples/demo/Applications/images/blue_ball.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Applications/images/header.png` & `traitsui-8.0.0/examples/demo/Applications/images/header.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Applications/images/notebook_close.png` & `traitsui-8.0.0/examples/demo/Applications/images/notebook_close.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Applications/images/notebook_open.png` & `traitsui-8.0.0/examples/demo/Applications/images/notebook_open.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Applications/images/red_ball.png` & `traitsui-8.0.0/examples/demo/Applications/images/red_ball.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Applications/tests/test_converter.py` & `traitsui-8.0.0/examples/demo/Applications/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Dynamic_Forms/dynamic_form_using_instances.py` & `traitsui-8.0.0/examples/demo/Dynamic_Forms/dynamic_form_using_instances.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Dynamic_Forms/dynamic_range_editor.py` & `traitsui-8.0.0/examples/demo/Dynamic_Forms/dynamic_range_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         # Dynamic simple slider demo:
         Group(
             Item(
                 'value',
                 editor=RangeEditor(
                     low_name='low',
                     high_name='high',
-                    format='%.1f',
+                    format_str='%.1f',
                     label_width=28,
                     mode='auto',
                 ),
             ),
             '_',
             Item('low'),
             Item('high'),
@@ -95,15 +95,15 @@
         # Dynamic large range slider demo:
         Group(
             Item(
                 'value',
                 editor=RangeEditor(
                     low_name='low',
                     high_name='high',
-                    format='%.1f',
+                    format_str='%.1f',
                     label_width=28,
                     mode='xslider',
                 ),
             ),
             '_',
             Item('low'),
             Item('high'),
@@ -119,15 +119,15 @@
             Item(
                 'int_value',
                 editor=RangeEditor(
                     low=0,
                     high=20,
                     low_name='int_low',
                     high_name='int_high',
-                    format='%d',
+                    format_str='%d',
                     is_float=False,
                     label_width=28,
                     mode='spinner',
                 ),
             ),
             '_',
             Item('int_low'),
```

### Comparing `traitsui-7.4.3/examples/demo/Dynamic_Forms/dynamic_selector.py` & `traitsui-8.0.0/examples/demo/Dynamic_Forms/dynamic_selector.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Dynamic_Forms/enabled_when.py` & `traitsui-8.0.0/examples/demo/Dynamic_Forms/enabled_when.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Dynamic_Forms/tests/test_visible_when.py` & `traitsui-8.0.0/examples/demo/Dynamic_Forms/tests/test_visible_when.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Dynamic_Forms/visible_when.py` & `traitsui-8.0.0/examples/demo/Dynamic_Forms/visible_when.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Extras/Image_editor_demo.py` & `traitsui-8.0.0/examples/demo/Extras/Image_editor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Extras/LED_display.py` & `traitsui-8.0.0/examples/demo/Extras/LED_display.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from traitsui.api import View, Item, HGroup, Handler, UIInfo, spring
 
 from traits.etsconfig.api import ETSConfig
 
 if ETSConfig.toolkit == 'wx':
     from traitsui.wx.extra.led_editor import LEDEditor
 else:
-    from traitsui.qt4.extra.led_editor import LEDEditor
+    from traitsui.qt.extra.led_editor import LEDEditor
 
 # Handler class for the LEDDemo class view:
 
 
 class LEDDemoHandler(Handler):
 
     # The UIInfo object associated with the UI:
```

### Comparing `traitsui-7.4.3/examples/demo/Extras/Tree_editor_with_TreeNodeRenderer.py` & `traitsui-8.0.0/examples/demo/Extras/Tree_editor_with_TreeNodeRenderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import numpy as np
 
 from pyface.qt import QtCore, QtGui, qt_api
 from traits.api import Array, Float, HasTraits, Instance, Int, List, Str
 
 from traitsui.api import TreeEditor, TreeNode, UItem, View, RGBColor
 from traitsui.tree_node_renderer import AbstractTreeNodeRenderer
-from traitsui.qt4.tree_editor import WordWrapRenderer
+from traitsui.qt.tree_editor import WordWrapRenderer
 
 
 class MyDataElement(HasTraits):
     """A node in a tree of data."""
 
     #: Some text to display.
     text = Str()
```

### Comparing `traitsui-7.4.3/examples/demo/Extras/animated_GIF.py` & `traitsui-8.0.0/examples/demo/Extras/animated_GIF.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Extras/images/info.png` & `traitsui-8.0.0/examples/demo/Extras/images/info.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Extras/images/logo_32x32.gif` & `traitsui-8.0.0/examples/demo/Extras/images/logo_32x32.gif`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Extras/images/logo_48x48.gif` & `traitsui-8.0.0/examples/demo/Extras/images/logo_48x48.gif`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Extras/images/logo_64x64.gif` & `traitsui-8.0.0/examples/demo/Extras/images/logo_64x64.gif`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Extras/images/python-logo.png` & `traitsui-8.0.0/examples/demo/Extras/images/python-logo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Extras/tests/test_Image_editor_demo.py` & `traitsui-8.0.0/examples/demo/Extras/tests/test_Image_editor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Extras/windows/flash.py` & `traitsui-8.0.0/examples/demo/Extras/windows/flash.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Extras/windows/internet_explorer.py` & `traitsui-8.0.0/examples/demo/Extras/windows/internet_explorer.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Misc/demo_group_size.py` & `traitsui-8.0.0/examples/demo/Misc/demo_group_size.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Misc/using_springs.py` & `traitsui-8.0.0/examples/demo/Misc/using_springs.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/ArrayEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/ArrayEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/BooleanEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/BooleanEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/BooleanEditor_simple_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/BooleanEditor_simple_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/ButtonEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/ButtonEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/ButtonEditor_simple_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/ButtonEditor_simple_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/CSVListEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/CSVListEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/CheckListEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/CheckListEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/CheckListEditor_simple_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/CheckListEditor_simple_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/CodeEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/CodeEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/ColorEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/ColorEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/CompoundEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/CompoundEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/DataFrameEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/DataFrameEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/DatetimeEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/DatetimeEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/DirectoryEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/DirectoryEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/EnumEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/EnumEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/FileEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/FileEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/File_Dialog/File_Open.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/File_Dialog/File_Open.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Custom_Extension.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Custom_Extension.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/File_Dialog/File_Open_with_FileInfo_Extension.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/File_Dialog/File_Open_with_FileInfo_Extension.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/File_Dialog/File_Open_with_ImageInfo_Extension.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/File_Dialog/File_Open_with_ImageInfo_Extension.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Multiple_Extensions.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Multiple_Extensions.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/File_Dialog/File_Open_with_TextInfo_Extension.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/File_Dialog/File_Open_with_TextInfo_Extension.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/FontEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/FontEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/HTMLEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/HTMLEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/ImageEnumEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/ImageEnumEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/InstanceEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/InstanceEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/ListEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/ListEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/RGBColorEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/RGBColorEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/RangeEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/RangeEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/SetEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/SetEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/TableEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/TableEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/TextEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/TextEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/TitleEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/TitleEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/TreeEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/TreeEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/TupleEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/TupleEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/VideoEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/VideoEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_BooleanEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_BooleanEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_BooleanEditor_simple_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_BooleanEditor_simple_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_ButtonEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_ButtonEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_ButtonEditor_simple_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_ButtonEditor_simple_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_CheckListEditor_simple_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_CheckListEditor_simple_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_EnumEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_EnumEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_FileEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_FileEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_InstanceEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_InstanceEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_ListEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_ListEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_RangeEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_RangeEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_TableEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_TableEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/Standard_Editors/tests/test_TextEditor_demo.py` & `traitsui-8.0.0/examples/demo/Standard_Editors/tests/test_TextEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/demo/traits_ui_demo.jpg` & `traitsui-8.0.0/examples/demo/traits_ui_demo.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/doc_examples/default.css` & `traitsui-8.0.0/examples/tutorials/doc_examples/default.css`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/doc_examples/doc_examples.rst` & `traitsui-8.0.0/examples/tutorials/doc_examples/doc_examples.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/doc_examples/examples/include_extra.py` & `traitsui-8.0.0/examples/tutorials/doc_examples/examples/include_extra.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/doc_examples/examples/lesson.desc` & `traitsui-8.0.0/examples/tutorials/doc_examples/examples/lesson.desc`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/doc_examples/examples/view_multi_object.py` & `traitsui-8.0.0/examples/tutorials/doc_examples/examples/view_multi_object.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/doc_examples/examples/view_standalone.py` & `traitsui-8.0.0/examples/tutorials/doc_examples/examples/view_standalone.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/traitsui_4.0/buttons.py` & `traitsui-8.0.0/examples/tutorials/traitsui_4.0/buttons.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/traitsui_4.0/default.css` & `traitsui-8.0.0/examples/tutorials/traitsui_4.0/default.css`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/traitsui_4.0/deferred.py` & `traitsui-8.0.0/examples/tutorials/traitsui_4.0/deferred.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/animated_gif.py` & `traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/animated_gif.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,18 @@
     A string that specifies the extended name of a trait that specifies whether
     the animated GIF file is playing or not. If not specified, the default is to
     play the animated GIF file endlessly.
 
 The value associated with **AnimatedGIFEditor** should be the name of the
 animated GIF image file to be displayed. No user editing of the value is
 provided by this editor, it is display only.
+
+Notes:
+
+- This demo only works on the wx backend.
 """
 
 # --[Imports]--------------------------------------------------------------
 
 from os.path import join, dirname
 
 from traits.api import HasTraits, File, Bool, Int
```

### Comparing `traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/flash.py` & `traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/flash.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/ie_html.py` & `traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/ie_html.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/led.py` & `traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/led.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/tabular_editor/numpy_array.py` & `traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/tabular_editor/numpy_array.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/tabular_editor/python_source_browser.py` & `traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/tabular_editor/python_source_browser.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/tabular_editor/sm_person_example.py` & `traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/tabular_editor/sm_person_example.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/tabular_editor/tabular_editor.htm` & `traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/tabular_editor/tabular_editor.htm`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/traitsui_4.0/editors/tabular_editor/tabular_editor.rst` & `traitsui-8.0.0/examples/tutorials/traitsui_4.0/editors/tabular_editor/tabular_editor.rst`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/traitsui_4.0/items.py` & `traitsui-8.0.0/examples/tutorials/traitsui_4.0/items.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/traitsui_4.0/model_view.py` & `traitsui-8.0.0/examples/tutorials/traitsui_4.0/model_view.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/examples/tutorials/tutor.py` & `traitsui-8.0.0/examples/tutorials/tutor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/image_LICENSE.txt` & `traitsui-8.0.0/image_LICENSE.txt`

 * *Files 7% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 traitsui/extras/images:
                            next.png | Nuvola
                          parent.png | Nuvola
                        previous.png | Nuvola
                          reload.png | Nuvola
                             run.png | Nuvola
 
-traitsui/qt4/images:
+traitsui/qt/images:
                        closetab.png | Qt
                            next.png | Qt
                        previous.png | Qt
 
 traitsui/wx/images:
                           group.png | Nuvola
                            item.png | Eclipse
```

### Comparing `traitsui-7.4.3/image_LICENSE_Eclipse.txt` & `traitsui-8.0.0/image_LICENSE_Eclipse.txt`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/image_LICENSE_Nuvola.txt` & `traitsui-8.0.0/image_LICENSE_Nuvola.txt`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/image_LICENSE_OOo.txt` & `traitsui-8.0.0/image_LICENSE_OOo.txt`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/styled_date_editor_test.py` & `traitsui-8.0.0/integrationtests/styled_date_editor_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/test_all_examples.py` & `traitsui-8.0.0/integrationtests/test_all_examples.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/array_editor_test.py` & `traitsui-8.0.0/integrationtests/ui/array_editor_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/buttons_test.py` & `traitsui-8.0.0/integrationtests/ui/buttons_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/check_list_editor_test.py` & `traitsui-8.0.0/integrationtests/ui/check_list_editor_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/check_list_editor_test2.py` & `traitsui-8.0.0/integrationtests/ui/check_list_editor_test2.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/code_editor_test.py` & `traitsui-8.0.0/integrationtests/ui/code_editor_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/enum_dynamic_test.py` & `traitsui-8.0.0/integrationtests/ui/enum_dynamic_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/enum_editor_test.py` & `traitsui-8.0.0/integrationtests/ui/enum_editor_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/html_editor_test.py` & `traitsui-8.0.0/integrationtests/ui/html_editor_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/images/bottom_left_origin.gif` & `traitsui-8.0.0/integrationtests/ui/images/bottom_left_origin.gif`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/images/bottom_right_origin.gif` & `traitsui-8.0.0/integrationtests/ui/images/bottom_right_origin.gif`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/images/top_left_origin.gif` & `traitsui-8.0.0/integrationtests/ui/images/top_left_origin.gif`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/images/top_right_origin.gif` & `traitsui-8.0.0/integrationtests/ui/images/top_right_origin.gif`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/instance_drag_test.py` & `traitsui-8.0.0/integrationtests/ui/instance_drag_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/instance_editor_test.py` & `traitsui-8.0.0/integrationtests/ui/instance_editor_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/instance_editor_test2.py` & `traitsui-8.0.0/integrationtests/ui/instance_editor_test2.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/instance_editor_test3.py` & `traitsui-8.0.0/integrationtests/ui/instance_editor_test3.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/instance_editor_test4.py` & `traitsui-8.0.0/integrationtests/ui/instance_editor_test4.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/instance_editor_test5.py` & `traitsui-8.0.0/integrationtests/ui/instance_editor_test5.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/instance_editor_test6.py` & `traitsui-8.0.0/integrationtests/ui/instance_editor_test6.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/large_range_editor.py` & `traitsui-8.0.0/integrationtests/ui/large_range_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/list_traits_ui_test.py` & `traitsui-8.0.0/integrationtests/ui/list_traits_ui_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/set_dynamic_test.py` & `traitsui-8.0.0/integrationtests/ui/set_dynamic_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/shell_editor_test.py` & `traitsui-8.0.0/integrationtests/ui/shell_editor_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/table_editor_focus_bug.py` & `traitsui-8.0.0/integrationtests/ui/table_editor_focus_bug.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/table_editor_test.py` & `traitsui-8.0.0/integrationtests/ui/table_editor_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/table_editor_test2.py` & `traitsui-8.0.0/integrationtests/ui/table_editor_test2.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/table_list_editor_test.py` & `traitsui-8.0.0/integrationtests/ui/table_list_editor_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/test_ui.py` & `traitsui-8.0.0/integrationtests/ui/test_ui.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/test_ui3.py` & `traitsui-8.0.0/integrationtests/ui/test_ui3.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/test_ui4.py` & `traitsui-8.0.0/integrationtests/ui/test_ui4.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/test_ui5.py` & `traitsui-8.0.0/integrationtests/ui/test_ui5.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/text_editor_invalid.py` & `traitsui-8.0.0/integrationtests/ui/text_editor_invalid.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/integrationtests/ui/tree_editor_test.py` & `traitsui-8.0.0/integrationtests/ui/tree_editor_test.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/_version.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/README.txt`

 * *Files 24% similar despite different names*

```diff
@@ -4,22 +4,13 @@
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-# THIS FILE IS GENERATED FROM SETUP.PY
+""" This package contains implementations for testing TraitsUI UI editors
+with Wx.
 
-#: The full version of the package, including a development suffix
-#: for unreleased versions of the package.
-version = '7.4.3'
-
-#: The full version of the package, same as 'version'
-#: Kept for backward compatibility
-full_version = version
-
-#: The Git revision from which this release was made.
-git_revision = 'Unknown'
-
-#: Flag whether this is a final release
-is_released = True
+The top-level module ``default_registry`` serves external packages and hides
+implementation details internal to this package.
+"""
```

### Comparing `traitsui-7.4.3/traitsui/api.py` & `traitsui-8.0.0/traitsui/api.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/base_panel.py` & `traitsui-8.0.0/traitsui/base_panel.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/basic_editor_factory.py` & `traitsui-8.0.0/traitsui/basic_editor_factory.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/color_column.py` & `traitsui-8.0.0/traitsui/color_column.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/context_value.py` & `traitsui-8.0.0/traitsui/context_value.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/default_dock_window_theme.py` & `traitsui-8.0.0/traitsui/default_dock_window_theme.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/delegating_handler.py` & `traitsui-8.0.0/traitsui/delegating_handler.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/dock_window_theme.py` & `traitsui-8.0.0/traitsui/dock_window_theme.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/dockable_view_element.py` & `traitsui-8.0.0/traitsui/dockable_view_element.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editor.py` & `traitsui-8.0.0/traitsui/editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editor_factory.py` & `traitsui-8.0.0/traitsui/editor_factory.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/api.py` & `traitsui-8.0.0/traitsui/editors/api.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/array_editor.py` & `traitsui-8.0.0/traitsui/editors/array_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/boolean_editor.py` & `traitsui-8.0.0/traitsui/editors/boolean_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/button_editor.py` & `traitsui-8.0.0/traitsui/editors/button_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/check_list_editor.py` & `traitsui-8.0.0/traitsui/editors/check_list_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/code_editor.py` & `traitsui-8.0.0/traitsui/editors/code_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/color_editor.py` & `traitsui-8.0.0/traitsui/editors/color_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/compound_editor.py` & `traitsui-8.0.0/traitsui/editors/compound_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/csv_list_editor.py` & `traitsui-8.0.0/traitsui/editors/csv_list_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/custom_editor.py` & `traitsui-8.0.0/traitsui/editors/custom_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/date_editor.py` & `traitsui-8.0.0/traitsui/editors/date_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/date_range_editor.py` & `traitsui-8.0.0/traitsui/editors/date_range_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/datetime_editor.py` & `traitsui-8.0.0/traitsui/editors/datetime_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/default_override.py` & `traitsui-8.0.0/traitsui/editors/default_override.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/directory_editor.py` & `traitsui-8.0.0/traitsui/editors/directory_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/dnd_editor.py` & `traitsui-8.0.0/traitsui/editors/dnd_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/drop_editor.py` & `traitsui-8.0.0/traitsui/editors/drop_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/enum_editor.py` & `traitsui-8.0.0/traitsui/editors/enum_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/file_editor.py` & `traitsui-8.0.0/traitsui/editors/file_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/font_editor.py` & `traitsui-8.0.0/traitsui/editors/font_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/history_editor.py` & `traitsui-8.0.0/traitsui/editors/history_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/html_editor.py` & `traitsui-8.0.0/traitsui/editors/html_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/image_editor.py` & `traitsui-8.0.0/traitsui/editors/image_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/image_enum_editor.py` & `traitsui-8.0.0/traitsui/editors/image_enum_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/instance_editor.py` & `traitsui-8.0.0/traitsui/editors/instance_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/key_binding_editor.py` & `traitsui-8.0.0/traitsui/editors/key_binding_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/list_editor.py` & `traitsui-8.0.0/traitsui/editors/list_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/list_str_editor.py` & `traitsui-8.0.0/traitsui/editors/list_str_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/null_editor.py` & `traitsui-8.0.0/traitsui/editors/null_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/popup_editor.py` & `traitsui-8.0.0/traitsui/editors/popup_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/progress_editor.py` & `traitsui-8.0.0/traitsui/editors/progress_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/range_editor.py` & `traitsui-8.0.0/traitsui/editors/range_editor.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,19 +63,14 @@
 
     #: The name of an [object.]trait that defines the high value for the range
     high_name = Str()
 
     #: Formatting string used to format value and labels
     format_str = Str("%s")
 
-    #: Deprecated: Please use ``format_str`` instead.
-    #: See enthought/traitsui#1704
-    #: Formatting string used to format value and labels.
-    format = Property(Str, observe='format_str')
-
     #: Is the range for floating pointer numbers (vs. integers)?
     is_float = Bool(Undefined)
 
     #: Function to evaluate floats/ints when they are assigned to an object
     #: trait
     evaluate = Any()
```

### Comparing `traitsui-7.4.3/traitsui/editors/rgb_color_editor.py` & `traitsui-8.0.0/traitsui/editors/rgb_color_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/scrubber_editor.py` & `traitsui-8.0.0/traitsui/editors/scrubber_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/search_editor.py` & `traitsui-8.0.0/traitsui/editors/search_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/set_editor.py` & `traitsui-8.0.0/traitsui/editors/set_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/shell_editor.py` & `traitsui-8.0.0/traitsui/editors/shell_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 
         locals = None
         self._base_locals = None
         value = self.value
         if self.factory.share and isinstance(value, dict):
             locals = value
         self._shell = shell = PythonShell(parent)
+        shell.create()
         self.control = shell.control
         if locals:
             for item in locals.items():
                 shell.bind(*item)
         if locals is None:
             object = self.object
             shell.bind("self", object)
```

### Comparing `traitsui-7.4.3/traitsui/editors/styled_date_editor.py` & `traitsui-8.0.0/traitsui/editors/styled_date_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/table_editor.py` & `traitsui-8.0.0/traitsui/editors/table_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/tabular_editor.py` & `traitsui-8.0.0/traitsui/editors/tabular_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/text_editor.py` & `traitsui-8.0.0/traitsui/editors/text_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/time_editor.py` & `traitsui-8.0.0/traitsui/editors/time_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/title_editor.py` & `traitsui-8.0.0/traitsui/editors/title_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/tree_editor.py` & `traitsui-8.0.0/traitsui/editors/tree_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/tuple_editor.py` & `traitsui-8.0.0/traitsui/editors/tuple_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/value_editor.py` & `traitsui-8.0.0/traitsui/editors/value_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/editors/video_editor.py` & `traitsui-8.0.0/traitsui/editors/video_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Adapted_tree_editor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Adapted_tree_editor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Apply_Revert_handler_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Apply_Revert_handler_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Auto_editable_readonly_table_cells.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Auto_editable_readonly_table_cells.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Auto_update_TabularEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Auto_update_TabularEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Date_editor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Date_editor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Date_range_editor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Date_range_editor_demo.py`

 * *Files 15% similar despite different names*

```diff
@@ -43,11 +43,11 @@
         print(self.date_range)
 
 
 # -- Set Up The Demo ------------------------------------------------------
 
 
 if __name__ == "__main__":
-    if ETSConfig.toolkit == "qt4":
+    if ETSConfig.toolkit in {"qt", "qt4"}:
         # DateRangeEditor is currently only available for qt backend.
         demo = DateRangeEditorDemo()
         demo.configure_traits()
```

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Dynamic_EnumEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Dynamic_EnumEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Dynamic_range_trait_and_editor.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Dynamic_range_trait_and_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Dynamic_views_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Dynamic_views_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Dynamically_changing_buttons_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Dynamically_changing_buttons_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/HDF5_tree_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/HDF5_tree_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/HDF5_tree_demo2.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/HDF5_tree_demo2.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/History_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/History_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Invalid_state_handling.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Invalid_state_handling.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/ListStrAdapter_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/ListStrAdapter_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/ListStrEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/ListStrEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/List_editor_notebook_selection_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/List_editor_notebook_selection_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/List_editors_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/List_editors_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/MVC_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/MVC_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Multi_select_string_list.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Multi_select_string_list.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Multi_thread_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Multi_thread_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Multi_thread_demo_2.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Multi_thread_demo_2.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/NumPy_array_tabular_editor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/NumPy_array_tabular_editor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/NumPy_array_view_editor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/NumPy_array_view_editor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Popup_Dialog_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Popup_Dialog_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Property_List_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Property_List_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Scrubber_editor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Scrubber_editor_demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,18 @@
 
 - A dynamic range. This consists of three scrubbers: one
   to control the low end of the range, one to control the high end, and one
   that uses the high and low values to determine its range.
 
 For comparison purposes, the example also shows the same traits displayed using
 their default editors.
+
+Notes:
+
+- This demo only works on the wx backend.
 """
 
 # -- Imports --------------------------------------------------------------
 
 from traits.api import HasTraits, Range, Float
 
 from traitsui.api import View, VGroup, HGroup, Item, ScrubberEditor, spring
```

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Settable_cached_property.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Settable_cached_property.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Statusbar_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Statusbar_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/String_list_ui_editor.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/String_list_ui_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     TabularEditor,
     View,
 )
 
 if ETSConfig.toolkit == 'wx':
     from traitsui.wx.ui_editor import UIEditor
 else:
-    from traitsui.qt4.ui_editor import UIEditor
+    from traitsui.qt.ui_editor import UIEditor
 
 
 # -- Define the reusable StringListEditor class and its helper classes --------
 
 # Define the tabular adapter used by the Traits UI string list editor:
 class MultiSelectAdapter(TabularAdapter):
```

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Table_editor_with_checkbox_column.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Table_editor_with_checkbox_column.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Table_editor_with_context_menu_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Table_editor_with_context_menu_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Table_editor_with_live_search_and_cell_editor.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Table_editor_with_live_search_and_cell_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Table_editor_with_progress_column.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Table_editor_with_progress_column.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Tabular_editor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Tabular_editor_demo.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 # -- Tabular Editor Definition --------------------------------------------
 # The tabular editor works in conjunction with an adapter class, derived from
 # TabularAdapter.
 tabular_editor = TabularEditor(
     adapter=ReportAdapter(),
     operations=['move', 'edit'],
     # Row titles are not supported in WX:
-    show_row_titles=ETSConfig.toolkit == 'qt4',
+    show_row_titles=(ETSConfig.toolkit in {"qt", "qt4"}),
 )
 
 
 # -- Report Class Definition ----------------------------------------------
 class Report(HasTraits):
 
     people = List(Person)
```

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Tabular_editor_with_context_menu_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Tabular_editor_with_context_menu_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Time_editor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Time_editor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/Tree_editor_required_traits_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/Tree_editor_required_traits_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/test_fixed.h5` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/test_fixed.h5`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/test_fixed_compressed.h5` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/test_fixed_compressed.h5`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/test_h5pydata.h5` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/test_h5pydata.h5`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/test_table_dc.h5` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/test_table_dc.h5`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/test_table_no_dc.h5` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/test_table_no_dc.h5`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Advanced/tests/test_List_editor_notebook_selection_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Advanced/tests/test_List_editor_notebook_selection_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Applications/Python_source_browser.py` & `traitsui-8.0.0/traitsui/examples/demo/Applications/Python_source_browser.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Applications/converter.py` & `traitsui-8.0.0/traitsui/examples/demo/Applications/converter.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Applications/images/GG5.png` & `traitsui-8.0.0/traitsui/examples/demo/Applications/images/GG5.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Applications/images/TFB.png` & `traitsui-8.0.0/traitsui/examples/demo/Applications/images/TFB.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Applications/images/blue_ball.png` & `traitsui-8.0.0/traitsui/examples/demo/Applications/images/blue_ball.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Applications/images/header.png` & `traitsui-8.0.0/traitsui/examples/demo/Applications/images/header.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Applications/images/notebook_close.png` & `traitsui-8.0.0/traitsui/examples/demo/Applications/images/notebook_close.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Applications/images/notebook_open.png` & `traitsui-8.0.0/traitsui/examples/demo/Applications/images/notebook_open.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Applications/images/red_ball.png` & `traitsui-8.0.0/traitsui/examples/demo/Applications/images/red_ball.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Applications/tests/test_converter.py` & `traitsui-8.0.0/traitsui/examples/demo/Applications/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Dynamic_Forms/dynamic_form_using_instances.py` & `traitsui-8.0.0/traitsui/examples/demo/Dynamic_Forms/dynamic_form_using_instances.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Dynamic_Forms/dynamic_range_editor.py` & `traitsui-8.0.0/traitsui/examples/demo/Dynamic_Forms/dynamic_range_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         # Dynamic simple slider demo:
         Group(
             Item(
                 'value',
                 editor=RangeEditor(
                     low_name='low',
                     high_name='high',
-                    format='%.1f',
+                    format_str='%.1f',
                     label_width=28,
                     mode='auto',
                 ),
             ),
             '_',
             Item('low'),
             Item('high'),
@@ -95,15 +95,15 @@
         # Dynamic large range slider demo:
         Group(
             Item(
                 'value',
                 editor=RangeEditor(
                     low_name='low',
                     high_name='high',
-                    format='%.1f',
+                    format_str='%.1f',
                     label_width=28,
                     mode='xslider',
                 ),
             ),
             '_',
             Item('low'),
             Item('high'),
@@ -119,15 +119,15 @@
             Item(
                 'int_value',
                 editor=RangeEditor(
                     low=0,
                     high=20,
                     low_name='int_low',
                     high_name='int_high',
-                    format='%d',
+                    format_str='%d',
                     is_float=False,
                     label_width=28,
                     mode='spinner',
                 ),
             ),
             '_',
             Item('int_low'),
```

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Dynamic_Forms/dynamic_selector.py` & `traitsui-8.0.0/traitsui/examples/demo/Dynamic_Forms/dynamic_selector.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Dynamic_Forms/enabled_when.py` & `traitsui-8.0.0/traitsui/examples/demo/Dynamic_Forms/enabled_when.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Dynamic_Forms/tests/test_visible_when.py` & `traitsui-8.0.0/traitsui/examples/demo/Dynamic_Forms/tests/test_visible_when.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Dynamic_Forms/visible_when.py` & `traitsui-8.0.0/traitsui/examples/demo/Dynamic_Forms/visible_when.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Extras/Image_editor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Extras/Image_editor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Extras/LED_display.py` & `traitsui-8.0.0/traitsui/examples/demo/Extras/LED_display.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from traitsui.api import View, Item, HGroup, Handler, UIInfo, spring
 
 from traits.etsconfig.api import ETSConfig
 
 if ETSConfig.toolkit == 'wx':
     from traitsui.wx.extra.led_editor import LEDEditor
 else:
-    from traitsui.qt4.extra.led_editor import LEDEditor
+    from traitsui.qt.extra.led_editor import LEDEditor
 
 # Handler class for the LEDDemo class view:
 
 
 class LEDDemoHandler(Handler):
 
     # The UIInfo object associated with the UI:
```

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Extras/Tree_editor_with_TreeNodeRenderer.py` & `traitsui-8.0.0/traitsui/examples/demo/Extras/Tree_editor_with_TreeNodeRenderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import numpy as np
 
 from pyface.qt import QtCore, QtGui, qt_api
 from traits.api import Array, Float, HasTraits, Instance, Int, List, Str
 
 from traitsui.api import TreeEditor, TreeNode, UItem, View, RGBColor
 from traitsui.tree_node_renderer import AbstractTreeNodeRenderer
-from traitsui.qt4.tree_editor import WordWrapRenderer
+from traitsui.qt.tree_editor import WordWrapRenderer
 
 
 class MyDataElement(HasTraits):
     """A node in a tree of data."""
 
     #: Some text to display.
     text = Str()
```

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Extras/animated_GIF.py` & `traitsui-8.0.0/traitsui/examples/demo/Extras/animated_GIF.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Extras/images/info.png` & `traitsui-8.0.0/traitsui/examples/demo/Extras/images/info.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Extras/images/logo_32x32.gif` & `traitsui-8.0.0/traitsui/examples/demo/Extras/images/logo_32x32.gif`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Extras/images/logo_48x48.gif` & `traitsui-8.0.0/traitsui/examples/demo/Extras/images/logo_48x48.gif`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Extras/images/logo_64x64.gif` & `traitsui-8.0.0/traitsui/examples/demo/Extras/images/logo_64x64.gif`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Extras/images/python-logo.png` & `traitsui-8.0.0/traitsui/examples/demo/Extras/images/python-logo.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Extras/tests/test_Image_editor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Extras/tests/test_Image_editor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Extras/windows/flash.py` & `traitsui-8.0.0/traitsui/examples/demo/Extras/windows/flash.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Extras/windows/internet_explorer.py` & `traitsui-8.0.0/traitsui/examples/demo/Extras/windows/internet_explorer.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Misc/demo_group_size.py` & `traitsui-8.0.0/traitsui/examples/demo/Misc/demo_group_size.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Misc/using_springs.py` & `traitsui-8.0.0/traitsui/examples/demo/Misc/using_springs.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/ArrayEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/ArrayEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/BooleanEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/BooleanEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/BooleanEditor_simple_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/BooleanEditor_simple_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/ButtonEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/ButtonEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/ButtonEditor_simple_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/ButtonEditor_simple_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/CSVListEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/CSVListEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/CheckListEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/CheckListEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/CheckListEditor_simple_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/CheckListEditor_simple_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/CodeEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/CodeEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/ColorEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/ColorEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/CompoundEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/CompoundEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/DataFrameEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/DataFrameEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/DatetimeEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/DatetimeEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/DirectoryEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/DirectoryEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/EnumEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/EnumEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/FileEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/FileEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Custom_Extension.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Custom_Extension.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_FileInfo_Extension.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_FileInfo_Extension.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_ImageInfo_Extension.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_ImageInfo_Extension.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Multiple_Extensions.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_Multiple_Extensions.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_TextInfo_Extension.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/File_Dialog/File_Open_with_TextInfo_Extension.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/FontEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/FontEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/HTMLEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/HTMLEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/ImageEnumEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/ImageEnumEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/InstanceEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/InstanceEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/ListEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/ListEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/RGBColorEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/RGBColorEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/RangeEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/RangeEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/SetEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/SetEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/TableEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/TableEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/TextEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/TextEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/TitleEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/TitleEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/TreeEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/TreeEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/TupleEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/TupleEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/VideoEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/VideoEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_BooleanEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_BooleanEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_BooleanEditor_simple_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_BooleanEditor_simple_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_ButtonEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_ButtonEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_ButtonEditor_simple_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_ButtonEditor_simple_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_CheckListEditor_simple_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_CheckListEditor_simple_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_EnumEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_EnumEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_FileEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_FileEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_InstanceEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_InstanceEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_ListEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_ListEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_RangeEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_RangeEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_TableEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_TableEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/Standard_Editors/tests/test_TextEditor_demo.py` & `traitsui-8.0.0/traitsui/examples/demo/Standard_Editors/tests/test_TextEditor_demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/examples/demo/traits_ui_demo.jpg` & `traitsui-8.0.0/traitsui/examples/demo/traits_ui_demo.jpg`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/extras/_demo_info.py` & `traitsui-8.0.0/traitsui/extras/_demo_info.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/extras/_demo_legacy.py` & `traitsui-8.0.0/traitsui/extras/_demo_legacy.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/extras/api.py` & `traitsui-8.0.0/traitsui/extras/api.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/extras/checkbox_column.py` & `traitsui-8.0.0/traitsui/extras/checkbox_column.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from traits.etsconfig.api import ETSConfig
 
 from ..table_column import ObjectColumn
 
 if ETSConfig.toolkit == "wx":
     from pyface.ui.wx.grid.checkbox_renderer import CheckboxRenderer
 elif ETSConfig.toolkit in {"qt", "qt4"}:
-    from ..qt4.extra.checkbox_renderer import CheckboxRenderer
+    from ..qt.extra.checkbox_renderer import CheckboxRenderer
 else:
     raise NotImplementedError("No checkbox renderer for backend")
 
 
 class CheckboxColumn(ObjectColumn):
     def __init__(self, **traits):
         """Initializes the object."""
```

### Comparing `traitsui-7.4.3/traitsui/extras/demo.py` & `traitsui-8.0.0/traitsui/extras/demo.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/extras/edit_column.py` & `traitsui-8.0.0/traitsui/extras/edit_column.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/extras/has_dynamic_views.py` & `traitsui-8.0.0/traitsui/extras/has_dynamic_views.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/extras/images/next.png` & `traitsui-8.0.0/traitsui/extras/images/next.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/extras/images/parent.png` & `traitsui-8.0.0/traitsui/extras/images/parent.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/extras/images/previous.png` & `traitsui-8.0.0/traitsui/extras/images/previous.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/extras/images/reload.png` & `traitsui-8.0.0/traitsui/extras/images/reload.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/extras/images/run.png` & `traitsui-8.0.0/traitsui/extras/images/run.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/extras/progress_column.py` & `traitsui-8.0.0/traitsui/extras/progress_column.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/extras/saving.py` & `traitsui-8.0.0/traitsui/extras/saving.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/file_dialog.py` & `traitsui-8.0.0/traitsui/file_dialog.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/group.py` & `traitsui-8.0.0/traitsui/group.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/handler.py` & `traitsui-8.0.0/traitsui/handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         constructed. It is provided so that the handler can save the
         reference to the UIInfo object in case it exposes viewable traits
         whose values are properties that depend upon items in the context
         being edited.
         """
         pass
 
-    def init(self, info):
+    def init(self, info: UIInfo) -> bool:
         """Initializes the controls of a user interface.
 
         This method is called after all user interface elements have been
         created, but before the user interface is displayed. Override this
         method to customize the user interface before it is displayed.
 
         Parameters
```

### Comparing `traitsui-7.4.3/traitsui/help.py` & `traitsui-8.0.0/traitsui/help.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/help_template.py` & `traitsui-8.0.0/traitsui/help_template.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/helper.py` & `traitsui-8.0.0/traitsui/helper.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/images/frame.png` & `traitsui-8.0.0/traitsui/images/frame.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/include.py` & `traitsui-8.0.0/traitsui/include.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/instance_choice.py` & `traitsui-8.0.0/traitsui/instance_choice.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/item.py` & `traitsui-8.0.0/traitsui/item.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/key_bindings.py` & `traitsui-8.0.0/traitsui/key_bindings.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/list_str_adapter.py` & `traitsui-8.0.0/traitsui/list_str_adapter.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/menu.py` & `traitsui-8.0.0/traitsui/menu.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/message.py` & `traitsui-8.0.0/traitsui/message.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/mimedata.py` & `traitsui-8.0.0/traitsui/mimedata.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
 # Import the toolkit specific version.
 from traitsui.toolkit import toolkit_object
 
-# WIP: Currently only supports qt4 backend. API might change without
+# WIP: Currently only supports qt backend. API might change without
 # prior notification
 PyMimeData = toolkit_object("clipboard:PyMimeData")
```

### Comparing `traitsui-7.4.3/traitsui/null/__init__.py` & `traitsui-8.0.0/traitsui/null/__init__.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/null/color_trait.py` & `traitsui-8.0.0/traitsui/null/color_trait.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/null/font_trait.py` & `traitsui-8.0.0/traitsui/null/font_trait.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/null/rgb_color_trait.py` & `traitsui-8.0.0/traitsui/null/rgb_color_trait.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/null/toolkit.py` & `traitsui-8.0.0/traitsui/null/toolkit.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/__init__.py` & `traitsui-8.0.0/traitsui/qt/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 # ----------------------------------------------------------------------------
 #  Define the reference to the exported GUIToolkit object:
 # ----------------------------------------------------------------------------
 
 from . import toolkit
 
 # Reference to the GUIToolkit object for Qt.
-toolkit = toolkit.GUIToolkit("traitsui", "qt4", "traitsui.qt4")
+toolkit = toolkit.GUIToolkit("traitsui", "qt", "traitsui.qt")
```

### Comparing `traitsui-7.4.3/traitsui/qt4/array_editor.py` & `traitsui-8.0.0/traitsui/qt/array_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/array_view_editor.py` & `traitsui-8.0.0/traitsui/qt/array_view_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/boolean_editor.py` & `traitsui-8.0.0/traitsui/qt/boolean_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/button_editor.py` & `traitsui-8.0.0/traitsui/qt/button_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/check_list_editor.py` & `traitsui-8.0.0/traitsui/qt/check_list_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/clipboard.py` & `traitsui-8.0.0/traitsui/qt/clipboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # ------------------------------------------------------------------------------
 
 """ Implements a wrapper around the PyQt clipboard that handles Python objects
 using pickle.
 """
 
 from pyface.qt import QtGui
-from pyface.ui.qt4.mimedata import PyMimeData, str2bytes
+from pyface.ui.qt.mimedata import PyMimeData, str2bytes
 from traits.api import HasTraits, Instance, Property
 
 
 # -------------------------------------------------------------------------
 #  '_Clipboard' class:
 # -------------------------------------------------------------------------
```

### Comparing `traitsui-7.4.3/traitsui/qt4/code_editor.py` & `traitsui-8.0.0/traitsui/qt/code_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,30 +21,28 @@
 # ------------------------------------------------------------------------------
 
 """ Defines a source code editor and code editor factory, for the PyQt user
 interface toolkit, useful for tools such as debuggers.
 """
 
 
-from pyface.qt import QtCore, QtGui
-
-from pyface.ui.qt4.code_editor.code_widget import AdvancedCodeWidget
+from pyface.qt import QtGui
+from pyface.key_pressed_event import KeyPressedEvent
+from pyface.ui.qt.code_editor.code_widget import AdvancedCodeWidget
 from traits.api import (
     Str,
     List,
     Int,
     Event,
     Bool,
     TraitError,
     observe,
 )
 from traits.trait_base import SequenceTypes
 
-from pyface.key_pressed_event import KeyPressedEvent
-
 from .constants import OKColor, ErrorColor
 from .editor import Editor
 from .helper import pixmap_cache
 
 
 # Marker line constants:
 MARK_MARKER = 0  # Marks a marked line
```

### Comparing `traitsui-7.4.3/traitsui/qt4/color_editor.py` & `traitsui-8.0.0/traitsui/qt/color_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,31 +42,31 @@
 # Standard color samples:
 color_samples = []
 
 # ---------------------------------------------------------------------------
 #  The PyQt ToolkitEditorFactory class.
 # ---------------------------------------------------------------------------
 
-## We need to add qt4-specific methods to the editor factory (since all editors
+## We need to add qt-specific methods to the editor factory (since all editors
 ## will be accessing these functions. Making these functions global functions
 ## in this file does not work quite well, since we want custom editors to
 ## override these methods easily.
 
 
 class ToolkitEditorFactory(BaseToolkitEditorFactory):
     """PyQt editor factory for color editors."""
 
-    def to_qt4_color(self, editor):
+    def to_qt_color(self, editor):
         """Gets the PyQt color equivalent of the object trait."""
         if self.mapped:
             return getattr(editor.object, editor.name + "_")
 
         return getattr(editor.object, editor.name)
 
-    def from_qt4_color(self, color):
+    def from_qt_color(self, color):
         """Gets the application equivalent of a PyQt value."""
         return color
 
     def str_color(self, color):
         """Returns the text representation of a specified color value."""
         if isinstance(color, QtGui.QColor):
             alpha = color.alpha()
@@ -91,24 +91,24 @@
     """Simple style of color editor, which displays a text field whose
     background color is the color value. Selecting the text field displays
     a dialog box for selecting a new color value.
     """
 
     def popup_editor(self):
         """Invokes the pop-up editor for an object trait."""
-        color = self.factory.to_qt4_color(self)
+        color = self.factory.to_qt_color(self)
         options = QtGui.QColorDialog.ColorDialogOption.ShowAlphaChannel
         if not self.factory.use_native_dialog:
             options |= QtGui.QColorDialog.ColorDialogOption.DontUseNativeDialog
         color = QtGui.QColorDialog.getColor(
             color, self.control, "Select Color", options
         )
 
         if color.isValid():
-            self.value = self.factory.from_qt4_color(color)
+            self.value = self.factory.from_qt_color(color)
             self.update_editor()
 
     def update_editor(self):
         """Updates the editor when the object trait changes externally to the
         editor.
         """
         super().update_editor()
@@ -140,15 +140,15 @@
         editor.
         """
         self._simple_field.update_editor()
 
     def update_object_from_swatch(self, color_text):
         """Updates the object trait when a color swatch is clicked."""
         color = QtGui.QColor(*[int(part) for part in color_text.split(",")])
-        self.value = self.factory.from_qt4_color(color)
+        self.value = self.factory.from_qt_color(color)
         self.update_editor()
 
     def string_value(self, color):
         """Returns the text representation of a specified color value."""
         return self.factory.str_color(color)
 
 
@@ -201,15 +201,15 @@
 # -------------------------------------------------------------------------
 #   Sets the color of the specified editor's color control:
 # -------------------------------------------------------------------------
 
 
 def set_color(editor):
     """Sets the color of the specified color control."""
-    color = editor.factory.to_qt4_color(editor)
+    color = editor.factory.to_qt_color(editor)
     pal = QtGui.QPalette(editor.control.palette())
 
     pal.setColor(QtGui.QPalette.ColorRole.Base, color)
 
     if color.red() > 192 or color.blue() > 192 or color.green() > 192:
         pal.setColor(QtGui.QPalette.ColorRole.Text, QtCore.Qt.GlobalColor.black)
     else:
```

### Comparing `traitsui-7.4.3/traitsui/qt4/color_trait.py` & `traitsui-8.0.0/traitsui/qt/color_trait.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,21 +90,21 @@
 
 # -------------------------------------------------------------------------
 #  Callable that returns an instance of the PyQtToolkitEditorFactory for color
 #  editors.
 # -------------------------------------------------------------------------
 
 ### FIXME: We have declared the 'editor' to be a function instead of  the
-# traitsui.qt4.color_editor.ToolkitEditorFactory class, since the
+# traitsui.qt.color_editor.ToolkitEditorFactory class, since the
 # latter is leading to too many circular imports. In the future, try to see if
 # there is a better way to do this.
 
 
 def get_color_editor(*args, **traits):
-    from traitsui.qt4.color_editor import ToolkitEditorFactory
+    from traitsui.qt.color_editor import ToolkitEditorFactory
 
     return ToolkitEditorFactory(*args, **traits)
 
 
 def PyQtColor(default="white", allow_none=False, **metadata):
     """Defines PyQt-specific color traits."""
     if default is None:
```

### Comparing `traitsui-7.4.3/traitsui/qt4/compound_editor.py` & `traitsui-8.0.0/traitsui/qt/compound_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/constants.py` & `traitsui-8.0.0/traitsui/qt/constants.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/csv_list_editor.py` & `traitsui-8.0.0/traitsui/qt/csv_list_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/custom_editor.py` & `traitsui-8.0.0/traitsui/qt/custom_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/data_frame_editor.py` & `traitsui-8.0.0/traitsui/qt/data_frame_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/date_editor.py` & `traitsui-8.0.0/traitsui/qt/date_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/date_range_editor.py` & `traitsui-8.0.0/traitsui/qt/date_range_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/datetime_editor.py` & `traitsui-8.0.0/traitsui/qt/datetime_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/directory_editor.py` & `traitsui-8.0.0/traitsui/qt/directory_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/drop_editor.py` & `traitsui-8.0.0/traitsui/qt/drop_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         pal.setColor(QtGui.QPalette.ColorRole.Base, self.ok_color)
         self.control.setPalette(pal)
 
         # Install EventFilter on control to handle DND events.
         drop_event_filter = _DropEventFilter(self.control)
         self.control.installEventFilter(drop_event_filter)
 
-        self.control._qt4_editor = self
+        self.control._qt_editor = self
 
     def dispose(self):
         """Disposes of the content of an editor."""
         if self.factory.readonly:
             # enthought/traitsui#884
             _BaseEditor.dispose(self)
         else:
@@ -88,15 +88,15 @@
             self.dropEvent(event)
         elif typ == QtCore.QEvent.Type.DragEnter:
             self.dragEnterEvent(event)
         return super().eventFilter(source, event)
 
     def dropEvent(self, e):
         """Handles a Python object being dropped on the tree."""
-        editor = self.parent()._qt4_editor
+        editor = self.parent()._qt_editor
 
         klass = editor.factory.klass
 
         if editor.factory.binding:
             value = getattr(clipboard, "node", None)
         else:
             value = e.mimeData().instance()
@@ -115,15 +115,15 @@
             finally:
                 editor._no_update = False
 
             e.acceptProposedAction()
 
     def dragEnterEvent(self, e):
         """Handles a Python object being dragged over the tree."""
-        editor = self.parent()._qt4_editor
+        editor = self.parent()._qt_editor
 
         if editor.factory.binding:
             data = getattr(clipboard, "node", None)
         else:
             md = e.mimeData()
 
             if not isinstance(md, PyMimeData):
```

### Comparing `traitsui-7.4.3/traitsui/qt4/editor.py` & `traitsui-8.0.0/traitsui/qt/editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/editor_factory.py` & `traitsui-8.0.0/traitsui/qt/editor_factory.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/enum_editor.py` & `traitsui-8.0.0/traitsui/qt/enum_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/extra/bounds_editor.py` & `traitsui-8.0.0/traitsui/qt/extra/bounds_editor.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # Thanks for using Enthought open source!
 
 from pyface.qt import QtGui, QtCore
 
 from traits.api import Float, Any, Str, Union
 
 from traitsui.editors.api import RangeEditor
-from traitsui.qt4.editor import Editor
-from traitsui.qt4.extra.range_slider import RangeSlider
+from traitsui.qt.editor import Editor
+from traitsui.qt.extra.range_slider import RangeSlider
 
 
 class _BoundsEditor(Editor):
 
     evaluate = Any()
 
     min = Any()
@@ -37,27 +37,25 @@
 
         if not factory.high_name:
             self.high = factory.high
 
         self.max = factory.max
         self.min = factory.min
 
-        self.format = factory.format
-
         self.evaluate = factory.evaluate
         self.sync_value(factory.evaluate_name, "evaluate", "from")
 
         self.sync_value(factory.low_name, "low", "both")
         self.sync_value(factory.high_name, "high", "both")
 
         self.control = QtGui.QWidget()
         panel = QtGui.QHBoxLayout(self.control)
         panel.setContentsMargins(0, 0, 0, 0)
 
-        self._label_lo = QtGui.QLineEdit(self.format % self.low)
+        self._label_lo = QtGui.QLineEdit(self.format_str % self.low)
         self._label_lo.editingFinished.connect(self.update_low_on_enter)
         panel.addWidget(self._label_lo)
 
         # The default size is a bit too big and probably doesn't need to grow.
         sh = self._label_lo.sizeHint()
         sh.setWidth(sh.width() // 2)
         self._label_lo.setMaximumSize(sh)
@@ -70,15 +68,15 @@
         slider.setSingleStep(100)
         slider.setLow(self._convert_to_slider(self.low))
         slider.setHigh(self._convert_to_slider(self.high))
 
         slider.sliderMoved.connect(self.update_object_on_scroll)
         panel.addWidget(slider)
 
-        self._label_hi = QtGui.QLineEdit(self.format % self.high)
+        self._label_hi = QtGui.QLineEdit(self.format_str % self.high)
         self._label_hi.editingFinished.connect(self.update_high_on_enter)
         panel.addWidget(self._label_hi)
 
         # The default size is a bit too big and probably doesn't need to grow.
         sh = self._label_hi.sizeHint()
         sh.setWidth(sh.width() // 2)
         self._label_hi.setMaximumSize(sh)
@@ -91,44 +89,44 @@
         try:
             try:
                 low = eval(str(self._label_lo.text()).strip())
                 if self.evaluate is not None:
                     low = self.evaluate(low)
             except Exception as ex:
                 low = self.low
-                self._label_lo.setText(self.format % self.low)
+                self._label_lo.setText(self.format_str % self.low)
 
             if not self.factory.is_float:
                 low = int(low)
 
             if low > self.high:
                 low = self.high - self._step_size()
-                self._label_lo.setText(self.format % low)
+                self._label_lo.setText(self.format_str % low)
 
             self.control.slider.setLow(self._convert_to_slider(low))
             self.low = low
         except:
             pass
 
     def update_high_on_enter(self):
         try:
             try:
                 high = eval(str(self._label_hi.text()).strip())
                 if self.evaluate is not None:
                     high = self.evaluate(high)
             except:
                 high = self.high
-                self._label_hi.setText(self.format % self.high)
+                self._label_hi.setText(self.format_str % self.high)
 
             if not self.factory.is_float:
                 high = int(high)
 
             if high < self.low:
                 high = self.low + self._step_size()
-                self._label_hi.setText(self.format % high)
+                self._label_hi.setText(self.format_str % high)
 
             self.control.slider.setHigh(self._convert_to_slider(high))
             self.high = high
         except:
             pass
 
     def update_object_on_scroll(self, pos):
@@ -176,23 +174,23 @@
             + (value - self.min) / self._step_size()
         )
 
     def _low_changed(self, low):
         if self.control is None:
             return
         if self._label_lo is not None:
-            self._label_lo.setText(self.format % low)
+            self._label_lo.setText(self.format_str % low)
 
         self.control.slider.setLow(self._convert_to_slider(low))
 
     def _high_changed(self, high):
         if self.control is None:
             return
         if self._label_hi is not None:
-            self._label_hi.setText(self.format % high)
+            self._label_hi.setText(self.format_str % high)
 
         self.control.slider.setHigh(self._convert_to_slider(self.high))
 
 
 class BoundsEditor(RangeEditor):
 
     min = Union(None, Float)
```

### Comparing `traitsui-7.4.3/traitsui/qt4/extra/checkbox_renderer.py` & `traitsui-8.0.0/traitsui/qt/extra/checkbox_renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     box for a false value.
 """
 
 # System library imports
 from pyface.qt import QtCore, QtGui
 
 # ETS imports
-from traitsui.qt4.table_editor import TableDelegate
+from traitsui.qt.table_editor import TableDelegate
 
 
 class CheckboxRenderer(TableDelegate):
     """A renderer which displays a checked-box for a True value and an
     unchecked box for a false value.
     """
```

### Comparing `traitsui-7.4.3/traitsui/qt4/extra/led_editor.py` & `traitsui-8.0.0/traitsui/qt/extra/led_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
 from pyface.qt import QtGui
-from traitsui.qt4.editor import Editor
+from traitsui.qt.editor import Editor
 from traitsui.basic_editor_factory import BasicEditorFactory
 from traits.api import Any, Undefined
 
 
 class _LEDEditor(Editor):
     def init(self, parent):
         self.control = QtGui.QLCDNumber()
```

### Comparing `traitsui-7.4.3/traitsui/qt4/extra/progress_renderer.py` & `traitsui-8.0.0/traitsui/qt/extra/progress_renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """ A renderer which displays a progress bar. """
 
 # System library imports
 import sys
 from pyface.qt import QtCore, QtGui
 
 # ETS imports
-from traitsui.qt4.table_editor import TableDelegate
+from traitsui.qt.table_editor import TableDelegate
 
 
 class ProgressRenderer(TableDelegate):
     """A renderer which displays a progress bar."""
 
     # -------------------------------------------------------------------------
     #  QAbstractItemDelegate interface
```

### Comparing `traitsui-7.4.3/traitsui/qt4/extra/qt_view.py` & `traitsui-8.0.0/traitsui/qt/extra/qt_view.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/extra/range_slider.py` & `traitsui-8.0.0/traitsui/qt/extra/range_slider.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/extra/table_image_renderer.py` & `traitsui-8.0.0/traitsui/qt/extra/table_image_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """
 
 # System library imports
 from pyface.qt import QtCore, QtGui
 
 # ETS imports
 from traits.api import Bool
-from traitsui.qt4.table_editor import TableDelegate
+from traitsui.qt.table_editor import TableDelegate
 
 
 class TableImageRenderer(TableDelegate):
     """A renderer which will display a cell-specific image in addition to some
     text displayed in the same way the default renderer would.
     """
```

### Comparing `traitsui-7.4.3/traitsui/qt4/file_editor.py` & `traitsui-8.0.0/traitsui/qt/file_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
     def _create_file_dialog(self):
         """Creates the correct type of file dialog."""
         wildcard = " ".join(self.factory.filter)
         dlg = FileDialog(
             parent=self.get_control_widget(),
             default_path=self._file_name.text(),
-            action="save" if self.factory.dialog_style == "save as" else "open",
+            action="save as" if self.factory.dialog_style == "save" else "open",
             wildcard=wildcard,
         )
         return dlg
 
 
 class CustomEditor(SimpleTextEditor):
     """Custom style of file editor, consisting of a file system tree view."""
```

### Comparing `traitsui-7.4.3/traitsui/qt4/font_editor.py` & `traitsui-8.0.0/traitsui/qt/font_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,28 +59,28 @@
     "48",
     "72",
 ]
 
 # ---------------------------------------------------------------------------
 #  The PyQtToolkitEditorFactory class.
 # ---------------------------------------------------------------------------
-## We need to add qt4-specific methods to the editor factory, and so we create
+## We need to add qt-specific methods to the editor factory, and so we create
 ## a subclass of the BaseToolkitEditorFactory.
 
 
 class ToolkitEditorFactory(BaseToolkitEditorFactory):
     """PyQt editor factory for font editors."""
 
-    def to_qt4_font(self, editor):
+    def to_qt_font(self, editor):
         """Returns a QFont object corresponding to a specified object's font
         trait.
         """
         return QtGui.QFont(editor.value)
 
-    def from_qt4_font(self, font):
+    def from_qt_font(self, font):
         """Gets the application equivalent of a QFont value."""
         return font
 
     def str_font(self, font):
         """Returns the text representation of the specified object trait value."""
         weight = {QtGui.QFont.Weight.Light: " Light", QtGui.QFont.Weight.Bold: " Bold"}.get(
             font.weight(), ""
@@ -102,19 +102,19 @@
     a text representation of the font value (using that font if possible).
     Clicking the field displays a font selection dialog box.
     """
 
     def popup_editor(self):
         """Invokes the pop-up editor for an object trait."""
         fnt, ok = QtGui.QFontDialog.getFont(
-            self.factory.to_qt4_font(self), self.control
+            self.factory.to_qt_font(self), self.control
         )
 
         if ok:
-            self.value = self.factory.from_qt4_font(fnt)
+            self.value = self.factory.from_qt_font(fnt)
             self.update_editor()
 
     def update_editor(self):
         """Updates the editor when the object trait changes externally to the
         editor.
         """
         super().update_editor()
@@ -164,37 +164,37 @@
         self._bold = self._italic = False
 
         layout.addLayout(layout2)
 
     def update_object(self):
         """Handles the user changing the contents of the font text control."""
         self.value = str(self._font.text())
-        self._set_font(self.factory.to_qt4_font(self))
+        self._set_font(self.factory.to_qt_font(self))
         self.update_editor()
 
     def update_object_parts(self):
         """Handles the user modifying one of the font components."""
         fnt = self._facename.currentFont()
 
         fnt.setBold(self._bold)
         fnt.setItalic(self._italic)
 
         psz = int(self._point_size.currentText())
         fnt.setPointSize(psz)
 
-        self.value = self.factory.from_qt4_font(fnt)
+        self.value = self.factory.from_qt_font(fnt)
 
         self._font.setText(self.str_value)
         self._set_font(fnt)
 
     def update_editor(self):
         """Updates the editor when the object trait changes externally to the
         editor.
         """
-        font = self.factory.to_qt4_font(self)
+        font = self.factory.to_qt_font(self)
 
         self._bold = font.bold()
         self._italic = font.italic()
 
         self._facename.setCurrentFont(font)
 
         try:
@@ -263,15 +263,15 @@
 # -------------------------------------------------------------------------
 #  Set the editor control's font to match a specified font:
 # -------------------------------------------------------------------------
 
 
 def set_font(editor):
     """Sets the editor control's font to match a specified font."""
-    editor.control.setFont(editor.factory.to_qt4_font(editor))
+    editor.control.setFont(editor.factory.to_qt_font(editor))
 
 
 # Define the names SimpleEditor, CustomEditor, TextEditor and ReadonlyEditor
 # which are looked up by the editor factory for the font editor.
 SimpleEditor = SimpleFontEditor
 CustomEditor = CustomFontEditor
 TextEditor = TextFontEditor
```

### Comparing `traitsui-7.4.3/traitsui/qt4/font_trait.py` & `traitsui-8.0.0/traitsui/qt/font_trait.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,21 +190,21 @@
 
 # -------------------------------------------------------------------------
 #  Callable that returns an instance of the PyQtToolkitEditorFactory for font
 #  editors.
 # -------------------------------------------------------------------------
 
 ### FIXME: We have declared the 'editor' to be a function instead of  the
-# traitsui.qt4.font_editor.ToolkitEditorFactory class, since the
+# traitsui.qt.font_editor.ToolkitEditorFactory class, since the
 # latter is leading to too many circular imports. In the future, try to see if
 # there is a better way to do this.
 
 
 def get_font_editor(*args, **traits):
-    from traitsui.qt4.font_editor import ToolkitEditorFactory
+    from traitsui.qt.font_editor import ToolkitEditorFactory
 
     return ToolkitEditorFactory(*args, **traits)
 
 
 # -------------------------------------------------------------------------
 #  Define a PyQt specific font trait:
 # -------------------------------------------------------------------------
```

### Comparing `traitsui-7.4.3/traitsui/qt4/helper.py` & `traitsui-8.0.0/traitsui/qt/helper.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/history_editor.py` & `traitsui-8.0.0/traitsui/qt/history_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/html_editor.py` & `traitsui-8.0.0/traitsui/qt/html_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/image_editor.py` & `traitsui-8.0.0/traitsui/qt/image_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/image_enum_editor.py` & `traitsui-8.0.0/traitsui/qt/image_enum_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/images/frame.png` & `traitsui-8.0.0/traitsui/qt/images/frame.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/images/next.png` & `traitsui-8.0.0/traitsui/qt/images/next.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/images/previous.png` & `traitsui-8.0.0/traitsui/qt/images/previous.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/instance_editor.py` & `traitsui-8.0.0/traitsui/qt/instance_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 from traits.api import HasTraits, Instance, Property
 from traits.observation.api import trait
 
 from traitsui.ui_traits import AView
 from traitsui.helper import user_name_for
 from traitsui.handler import Handler
-from traitsui.instance_choice import InstanceChoiceItem
+from traitsui.instance_choice import InstanceChoice, InstanceChoiceItem
 from .editor import Editor
 from .drop_editor import _DropEventFilter
 from .constants import DropColor
 from .helper import position_window
 
 
 OrientationMap = {
@@ -178,19 +178,20 @@
         items = []
         adapter = factory.adapter
         for value in values:
             if not isinstance(value, InstanceChoiceItem):
                 value = adapter(object=value)
             # rebuild_items when an item's name changes so it is reflected by
             # combobox. This change was added to fix enthought/traitsui#1641
-            value.object.observe(
-                self.rebuild_items,
-                trait(value.name_trait, optional=True),
-                dispatch="ui",
-            )
+            if isinstance(value, InstanceChoice):
+                value.object.observe(
+                    self.rebuild_items,
+                    trait(value.name_trait, optional=True),
+                    dispatch="ui",
+                )
             items.append(value)
 
         self._items = items
 
         return items
 
     def rebuild_items(self, event=None):
```

### Comparing `traitsui-7.4.3/traitsui/qt4/key_binding_editor.py` & `traitsui-8.0.0/traitsui/qt/key_binding_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/key_event_to_name.py` & `traitsui-8.0.0/traitsui/qt/key_event_to_name.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/list_editor.py` & `traitsui-8.0.0/traitsui/qt/list_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/list_str_editor.py` & `traitsui-8.0.0/traitsui/qt/list_str_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/list_str_model.py` & `traitsui-8.0.0/traitsui/qt/list_str_model.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/menu.py` & `traitsui-8.0.0/traitsui/qt/menu.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/null_editor.py` & `traitsui-8.0.0/traitsui/qt/null_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/progress_editor.py` & `traitsui-8.0.0/traitsui/qt/progress_editor.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # Thanks for using Enthought open source!
 
 import time
 
 from pyface.qt import QtGui, QtCore
 
 from traits.api import Instance, Int, Str
-from traitsui.qt4.editor import Editor
-from pyface.ui.qt4.progress_dialog import ProgressDialog
+from pyface.ui.qt.progress_dialog import ProgressDialog
+from traitsui.qt.editor import Editor
 
 
 class _ProgressDialog(ProgressDialog):
     def close(self):
         """Overwritten to disable closing."""
         pass
```

### Comparing `traitsui-7.4.3/traitsui/qt4/range_editor.py` & `traitsui-8.0.0/traitsui/qt/range_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,17 +76,14 @@
 
     #: Low value for the slider range
     low = Any()
 
     #: High value for the slider range
     high = Any()
 
-    #: Deprecated: This trait is no longer used. See enthought/traitsui#1704
-    format = Str()
-
     def init(self, parent):
         """Finishes initializing the editor by creating the underlying toolkit
         widget.
         """
         factory = self.factory
         if not factory.low_name:
             self.low = factory.low
```

### Comparing `traitsui-7.4.3/traitsui/qt4/rgb_color_editor.py` & `traitsui-8.0.0/traitsui/qt/rgb_color_editor.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,39 +28,39 @@
 
 from pyface.qt import QtGui
 
 from traits.trait_base import SequenceTypes
 
 # Note: The ToolkitEditorFactory class imported from color_editor is a
 # subclass of the abstract ToolkitEditorFactory class
-# (in traitsui.api) with qt4-specific methods defined.
-# We need to override the implementations of the qt4-specific methods here.
+# (in traitsui.api) with qt-specific methods defined.
+# We need to override the implementations of the qt-specific methods here.
 from .color_editor import ToolkitEditorFactory as BaseColorToolkitEditorFactory
 
 # -------------------------------------------------------------------------
 #  The PyQt4 ToolkitEditorFactory class.
 # -------------------------------------------------------------------------
 
 
 class ToolkitEditorFactory(BaseColorToolkitEditorFactory):
     """PyQt editor factory for color editors."""
 
-    def to_qt4_color(self, editor):
+    def to_qt_color(self, editor):
         """Gets the PyQt color equivalent of the object trait."""
         try:
             color = getattr(editor.object, editor.name + "_")
         except AttributeError:
             color = getattr(editor.object, editor.name)
 
         c = QtGui.QColor()
         c.setRgbF(color[0], color[1], color[2])
 
         return c
 
-    def from_qt4_color(self, color):
+    def from_qt_color(self, color):
         """Gets the application equivalent of a PyQt value."""
         return (color.redF(), color.greenF(), color.blueF())
 
     def str_color(self, color):
         """Returns the text representation of a specified color value."""
         if type(color) in SequenceTypes:
             return "(%d,%d,%d)" % (
```

### Comparing `traitsui-7.4.3/traitsui/qt4/rgb_color_trait.py` & `traitsui-8.0.0/traitsui/qt/rgb_color_trait.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     range from 0.0 to 1.0.
 """
 
 
 from traits.api import Trait, TraitError
 from traits.trait_base import SequenceTypes
 
-from traitsui.qt4.color_trait import standard_colors
+from traitsui.qt.color_trait import standard_colors
 
 # -------------------------------------------------------------------------
 #  Convert a number into an RGB tuple:
 # -------------------------------------------------------------------------
 
 
 def range_check(value):
```

### Comparing `traitsui-7.4.3/traitsui/qt4/search_editor.py` & `traitsui-8.0.0/traitsui/qt/search_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/set_editor.py` & `traitsui-8.0.0/traitsui/qt/set_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/shell_editor.py` & `traitsui-8.0.0/traitsui/qt/shell_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/styled_date_editor.py` & `traitsui-8.0.0/traitsui/qt/styled_date_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/table_editor.py` & `traitsui-8.0.0/traitsui/qt/table_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1324,15 +1324,15 @@
                 editor=InstanceEditor(view_name="selected_filter_view"),
             ),
             id="TableFilterEditorSplit",
             show_labels=False,
             layout="split",
             orientation="horizontal",
         ),
-        id="traitsui.qt4.table_editor.TableFilterEditor",
+        id="traitsui.qt.table_editor.TableFilterEditor",
         buttons=["OK", "Cancel"],
         kind="livemodal",
         resizable=True,
         width=800,
         height=400,
         title="Customize filters",
     )
```

### Comparing `traitsui-7.4.3/traitsui/qt4/table_model.py` & `traitsui-8.0.0/traitsui/qt/table_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,22 +32,22 @@
 from .clipboard import PyMimeData
 
 
 # set up logging for the module
 logger = logging.getLogger(__name__)
 
 
-# Mapping for trait alignment values to qt4 horizontal alignment constants
+# Mapping for trait alignment values to qt horizontal alignment constants
 h_alignment_map = {
     "left": QtCore.Qt.AlignmentFlag.AlignLeft,
     "center": QtCore.Qt.AlignmentFlag.AlignHCenter,
     "right": QtCore.Qt.AlignmentFlag.AlignRight,
 }
 
-# Mapping for trait alignment values to qt4 vertical alignment constants
+# Mapping for trait alignment values to qt vertical alignment constants
 v_alignment_map = {
     "top": QtCore.Qt.AlignmentFlag.AlignTop,
     "center": QtCore.Qt.AlignmentFlag.AlignVCenter,
     "bottom": QtCore.Qt.AlignmentFlag.AlignBottom,
 }
 
 # MIME type for internal table drag/drop operations
```

### Comparing `traitsui-7.4.3/traitsui/qt4/tabular_editor.py` & `traitsui-8.0.0/traitsui/qt/tabular_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,18 +36,18 @@
 
 from traitsui.tabular_adapter import TabularAdapter
 from traitsui.helper import compute_column_widths
 from .editor import Editor
 from .tabular_model import TabularModel
 
 SCROLL_TO_POSITION_HINT_MAP = {
-    "center": QtGui.QTableView.PositionAtCenter,
-    "top": QtGui.QTableView.PositionAtTop,
-    "bottom": QtGui.QTableView.PositionAtBottom,
-    "visible": QtGui.QTableView.EnsureVisible,
+    "center": QtGui.QTableView.ScrollHint.PositionAtCenter,
+    "top": QtGui.QTableView.ScrollHint.PositionAtTop,
+    "bottom": QtGui.QTableView.ScrollHint.PositionAtBottom,
+    "visible": QtGui.QTableView.ScrollHint.EnsureVisible,
 }
 
 
 class HeaderEventFilter(QtCore.QObject):
     def __init__(self, editor):
         super().__init__()
         self.editor = editor
@@ -502,24 +502,26 @@
                 )
                 # Once selected, scroll to the column
                 self.scroll_to_column = selected_column
 
     def _scroll_to_row_changed(self, row):
         """Scroll to the given row."""
         scroll_hint = SCROLL_TO_POSITION_HINT_MAP.get(
-            self.factory.scroll_to_position_hint, self.control.EnsureVisible
+            self.factory.scroll_to_position_hint,
+            self.control.ScrollHint.EnsureVisible
         )
         self.control.scrollTo(
             self.model.index(row, max(self.selected_column, 0)), scroll_hint
         )
 
     def _scroll_to_column_changed(self, column):
         """Scroll to the given column."""
         scroll_hint = SCROLL_TO_POSITION_HINT_MAP.get(
-            self.factory.scroll_to_position_hint, self.control.EnsureVisible
+            self.factory.scroll_to_position_hint,
+            self.control.ScrollHint.EnsureVisible
         )
         self.control.scrollTo(
             self.model.index(max(self.selected_row, 0), column), scroll_hint
         )
 
     # -- Table Control Event Handlers -----------------------------------------
```

### Comparing `traitsui-7.4.3/traitsui/qt4/tabular_model.py` & `traitsui-8.0.0/traitsui/qt/tabular_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from pyface.qt import QtCore, QtGui
 
 from traitsui.ui_traits import SequenceTypes
 from .clipboard import PyMimeData
 
 
-# Mapping for trait alignment values to qt4 alignment values:
+# Mapping for trait alignment values to qt alignment values:
 alignment_map = {
     "left": QtCore.Qt.AlignmentFlag.AlignLeft,
     "right": QtCore.Qt.AlignmentFlag.AlignRight,
     "center": QtCore.Qt.AlignmentFlag.AlignHCenter,
     "justify": QtCore.Qt.AlignmentFlag.AlignJustify,
 }
```

### Comparing `traitsui-7.4.3/traitsui/qt4/tests/test_color_trait.py` & `traitsui-8.0.0/traitsui/qt/tests/test_color_trait.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import unittest
 
 from pyface.qt import QtGui
 from pyface.color import Color as PyfaceColor
 from traits.api import HasStrictTraits, TraitError
 
-from traitsui.qt4.color_trait import PyQtColor
+from traitsui.qt.color_trait import PyQtColor
 
 
 class ObjectWithColor(HasStrictTraits):
 
     color = PyQtColor()
```

### Comparing `traitsui-7.4.3/traitsui/qt4/tests/test_font_trait.py` & `traitsui-8.0.0/traitsui/qt/tests/test_font_trait.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/tests/test_helper.py` & `traitsui-8.0.0/traitsui/qt/tests/test_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 # Thanks for using Enthought open source!
 
 import textwrap
 import unittest
 
 from pyface.qt import is_pyqt, qt_api, QtCore, QtGui
 from traitsui.tests._tools import is_mac_os, requires_toolkit, ToolkitName
-from traitsui.qt4.helper import qobject_is_valid, wrap_text_with_elision
-from traitsui.qt4.font_trait import create_traitsfont
+from traitsui.qt.helper import qobject_is_valid, wrap_text_with_elision
+from traitsui.qt.font_trait import create_traitsfont
 
 
 lorem_ipsum = (
     "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod "
     "tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim "
     "veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea "
     "commodo consequat.\n"
```

### Comparing `traitsui-7.4.3/traitsui/qt4/tests/test_tabular_model.py` & `traitsui-8.0.0/traitsui/qt/tests/test_tabular_model.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/tests/test_ui_base.py` & `traitsui-8.0.0/traitsui/qt/tests/test_ui_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,9 +33,10 @@
         parent_view = View(Item("number"), title="Parent")
         nested = View(Item("number"), resizable=True, title="Nested")
         with create_ui(obj, dict(view=parent_view)) as ui:
             with create_ui(obj2, dict(parent=ui.control, view=nested)) as ui2:
                 from pyface.qt import QtCore
 
                 self.assertFalse(
-                    ui2.control.windowFlags() & QtCore.Qt.WindowState.WindowMaximized
+                    ui2.control.windowState()
+                    & QtCore.Qt.WindowState.WindowMaximized
                 )
```

### Comparing `traitsui-7.4.3/traitsui/qt4/tests/test_ui_panel.py` & `traitsui-8.0.0/traitsui/qt/tests/test_ui_panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,47 +133,47 @@
             ),
         )
         return view
 
 
 @requires_toolkit([ToolkitName.qt])
 class TestUIPanel(unittest.TestCase):
-    def setup_qt4_dock_window(self):
+    def setup_qt_dock_window(self):
         from pyface.qt import QtGui
 
         # set up the dock window for qt
         main_window = QtGui.QMainWindow()
         self.addCleanup(process_cascade_events)
         self.addCleanup(main_window.close)
         dock = QtGui.QDockWidget("testing", main_window)
         dock.setWidget(QtGui.QMainWindow())
         return main_window, dock
 
-    def test_panel_has_toolbar_buttons_qt4(self):
+    def test_panel_has_toolbar_buttons_qt(self):
         from pyface.qt import QtGui
 
-        _, dock = self.setup_qt4_dock_window()
+        _, dock = self.setup_qt_dock_window()
 
         # add panel
         panel = FooPanel()
         with create_ui(panel, dict(parent=dock.widget(), kind="panel")) as ui:
             dock.widget().setCentralWidget(ui.control)
 
             # There should be a toolbar for the panel
             self.assertIsNotNone(dock.findChild(QtGui.QToolBar))
 
             # There should be buttons too
             # Not searching from dock because the dock panel has buttons for
             # popping up and closing the panel
             self.assertIsNotNone(ui.control.findChild(QtGui.QPushButton))
 
-    def test_subpanel_has_toolbar_no_buttons_qt4(self):
+    def test_subpanel_has_toolbar_no_buttons_qt(self):
         from pyface.qt import QtGui
 
-        _, dock = self.setup_qt4_dock_window()
+        _, dock = self.setup_qt_dock_window()
 
         # add panel
         panel = FooPanel()
         parent = dock.widget()
         with create_ui(panel, dict(parent=parent, kind="subpanel")) as ui:
             dock.widget().setCentralWidget(ui.control)
```

### Comparing `traitsui-7.4.3/traitsui/qt4/text_editor.py` & `traitsui-8.0.0/traitsui/qt/text_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/time_editor.py` & `traitsui-8.0.0/traitsui/qt/time_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/title_editor.py` & `traitsui-8.0.0/traitsui/qt/title_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/toolkit.py` & `traitsui-8.0.0/traitsui/qt/toolkit.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/tree_editor.py` & `traitsui-8.0.0/traitsui/qt/tree_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/tree_node_renderers.py` & `traitsui-8.0.0/traitsui/qt/tree_node_renderers.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/tuple_editor.py` & `traitsui-8.0.0/traitsui/qt/tuple_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/ui_base.py` & `traitsui-8.0.0/traitsui/qt/ui_base.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/ui_editor.py` & `traitsui-8.0.0/traitsui/qt/ui_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/ui_live.py` & `traitsui-8.0.0/traitsui/qt/ui_live.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/ui_modal.py` & `traitsui-8.0.0/traitsui/qt/ui_modal.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/ui_panel.py` & `traitsui-8.0.0/traitsui/qt/ui_panel.py`

 * *Files 0% similar despite different names*

```diff
@@ -599,15 +599,15 @@
                 scroll_area.setWidgetResizable(True)
                 outer = scroll_area
 
             # See if we need to control the visual appearance of the group.
             if group.visible_when != "" or group.enabled_when != "":
                 # Make sure that outer is a widget and inner is a layout.
                 # Hiding a layout is not properly supported by Qt (the
-                # workaround in ``traitsui.qt4.editor._visible_changed_helper``
+                # workaround in ``traitsui.qt.editor._visible_changed_helper``
                 # often leaves undesirable blank space).
                 if outer is None:
                     outer = inner = QtGui.QBoxLayout(self.direction)
                 if isinstance(outer, QtGui.QLayout):
                     widget = QtGui.QWidget()
                     widget.setLayout(outer)
                     outer = widget
```

### Comparing `traitsui-7.4.3/traitsui/qt4/value_editor.py` & `traitsui-8.0.0/traitsui/qt/value_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/video_editor.py` & `traitsui-8.0.0/traitsui/qt/video_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/qt4/view_application.py` & `traitsui-8.0.0/traitsui/qt/view_application.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/table_column.py` & `traitsui-8.0.0/traitsui/table_column.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/table_filter.py` & `traitsui-8.0.0/traitsui/table_filter.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tabular_adapter.py` & `traitsui-8.0.0/traitsui/tabular_adapter.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/README.txt` & `traitsui-8.0.0/traitsui/testing/README.txt`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/__init__.py` & `traitsui-8.0.0/traitsui/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/_exception_handling.py` & `traitsui-8.0.0/traitsui/testing/_exception_handling.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/_gui.py` & `traitsui-8.0.0/traitsui/testing/_gui.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/api.py` & `traitsui-8.0.0/traitsui/testing/api.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/data/test.mp4` & `traitsui-8.0.0/traitsui/testing/data/test.mp4`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/README.txt` & `traitsui-8.0.0/traitsui/testing/tester/README.txt`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/__init__.py` & `traitsui-8.0.0/traitsui/testing/tester/__init__.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_abstract_target_registry.py` & `traitsui-8.0.0/traitsui/testing/tester/_abstract_target_registry.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_dynamic_target_registry.py` & `traitsui-8.0.0/traitsui/testing/tester/_dynamic_target_registry.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/README.txt` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/README.txt`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/__init__.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/_common_ui_targets.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/_common_ui_targets.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/_compat.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/_compat.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/_layout.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/_layout.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/_traitsui_ui.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/_traitsui_ui.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/default_registry.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/default_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     """
     # side-effect to determine current toolkit
     from pyface.toolkit import toolkit_object  # noqa
 
     if ETSConfig.toolkit == "null":
         registries = []
     else:
-        toolkit = {'wx': 'wx', 'qt4': 'qt4', 'qt': 'qt4'}[ETSConfig.toolkit]
+        toolkit = {'wx': 'wx', 'qt4': 'qt', 'qt': 'qt'}[ETSConfig.toolkit]
         this_package, _ = __name__.rsplit(".", 1)
         module = importlib.import_module(
             ".default_registry", this_package + '.' + toolkit
         )
         registries = module.get_default_registries()
 
     ui_registry = TargetRegistry()
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/README.txt` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/README.txt`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/__init__.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_control_widget_registry.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_control_widget_registry.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_interaction_helpers.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_interaction_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from pyface.qt import QtCore, QtGui
 from pyface.qt.QtTest import QTest
 
 from traitsui.testing.tester._ui_tester_registry._compat import (
     check_key_compat,
 )
 from traitsui.testing.tester.exceptions import Disabled
-from traitsui.qt4.key_event_to_name import key_map as _KEY_MAP
+from traitsui.qt.key_event_to_name import key_map as _KEY_MAP
 
 
 def key_click(widget, key, delay):
     """Performs a key click of the given key on the given widget after
     a delay.
 
     Parameters
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_registry_helper.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_registry_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from traitsui.testing.tester.command import (
     KeyClick,
     KeySequence,
     MouseClick,
 )
 from traitsui.testing.tester.query import DisplayedText
-from traitsui.testing.tester._ui_tester_registry.qt4 import (
+from traitsui.testing.tester._ui_tester_registry.qt import (
     _interaction_helpers,
 )
 
 
 def register_editable_textbox_handlers(registry, target_class, widget_getter):
     """Register common interactions for an editable textbox (in Qt)
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/README.txt` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/README.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
 """ The organization in this package should more or less mirror that of
-the ``traitsui.qt4`` package and contains the corresponding logic for testing.
+the ``traitsui.qt`` package and contains the corresponding logic for testing.
 
 Note that once new implementations are added, they may need to be exposed
 via the ``default_registry`` module (one level up from this package).
 """
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/__init__.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,12 +5,12 @@
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
 """ The organization in this package should more or less mirror that of
-the ``traitsui.qt4`` package and contains the corresponding logic for testing.
+the ``traitsui.qt`` package and contains the corresponding logic for testing.
 
 Note that once new implementations are added, they may need to be exposed
 via the ``default_registry`` module (one level up from this package).
 """
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/boolean_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/boolean_editor.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
 from traitsui.testing.tester.command import MouseClick
 from traitsui.testing.tester.query import DisplayedText, IsChecked
-from traitsui.testing.tester._ui_tester_registry.qt4 import (
+from traitsui.testing.tester._ui_tester_registry.qt import (
     _interaction_helpers,
 )
-from traitsui.qt4.boolean_editor import ReadonlyEditor, SimpleEditor
+from traitsui.qt.boolean_editor import ReadonlyEditor, SimpleEditor
 
 
 def register(registry):
     """Register solvers/handlers specific to qt Boolean Editors
     for the given registry.
 
     If there are any conflicts, an error will occur.
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/button_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/button_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
 from traitsui.testing.tester.command import MouseClick
 from traitsui.testing.tester.query import DisplayedText
-from traitsui.testing.tester._ui_tester_registry.qt4 import (
+from traitsui.testing.tester._ui_tester_registry.qt import (
     _interaction_helpers,
 )
-from traitsui.qt4.button_editor import CustomEditor, SimpleEditor
+from traitsui.qt.button_editor import CustomEditor, SimpleEditor
 
 
 def register(registry):
     """Register solvers/handlers specific to qt Button Editors
     for the given registry.
 
     If there are any conflicts, an error will occur.
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/check_list_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/check_list_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-from traitsui.qt4.check_list_editor import CustomEditor
+from traitsui.qt.check_list_editor import CustomEditor
 from traitsui.testing.tester.command import MouseClick
 from traitsui.testing.tester.locator import Index
 from traitsui.testing.tester._ui_tester_registry._common_ui_targets import (
     BaseSourceWithLocation,
 )
 from traitsui.testing.tester._ui_tester_registry._layout import (
     column_major_to_row_major,
 )
-from traitsui.testing.tester._ui_tester_registry.qt4 import (
+from traitsui.testing.tester._ui_tester_registry.qt import (
     _interaction_helpers,
 )
 
 
 class _IndexedCustomCheckListEditor(BaseSourceWithLocation):
     """Wrapper for CheckListEditor + locator.Index"""
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/directory_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/directory_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-from traitsui.testing.tester._ui_tester_registry.qt4._registry_helper import (
+from traitsui.testing.tester._ui_tester_registry.qt._registry_helper import (
     register_editable_textbox_handlers,
 )
-from traitsui.qt4.directory_editor import SimpleEditor
+from traitsui.qt.directory_editor import SimpleEditor
 
 
 def register(registry):
     """Register interactions for the given registry.
 
     If there are any conflicts, an error will occur.
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/editor_factory.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/editor_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
 from traitsui.testing.tester.query import DisplayedText
-from traitsui.testing.tester._ui_tester_registry.qt4._registry_helper import (
+from traitsui.testing.tester._ui_tester_registry.qt._registry_helper import (
     register_editable_textbox_handlers,
 )
-from traitsui.qt4.editor_factory import ReadonlyEditor, TextEditor
+from traitsui.qt.editor_factory import ReadonlyEditor, TextEditor
 
 
 def register(registry):
     """Register interactions for the given registry.
 
     If there are any conflicts, an error will occur.
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/enum_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/enum_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-from traitsui.qt4.enum_editor import (
+from traitsui.qt.enum_editor import (
     ListEditor,
     RadioEditor,
     SimpleEditor,
 )
 from traitsui.testing.tester.command import (
     KeyClick,
     KeySequence,
     MouseClick,
 )
 from traitsui.testing.tester.locator import Index
 from traitsui.testing.tester.query import DisplayedText, SelectedText
 from traitsui.testing.tester._ui_tester_registry._common_ui_targets import (
     BaseSourceWithLocation,
 )
-from traitsui.testing.tester._ui_tester_registry.qt4 import (
+from traitsui.testing.tester._ui_tester_registry.qt import (
     _interaction_helpers,
 )
 from traitsui.testing.tester._ui_tester_registry._layout import (
     column_major_to_row_major,
 )
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/file_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/file_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-from traitsui.testing.tester._ui_tester_registry.qt4._registry_helper import (
+from traitsui.testing.tester._ui_tester_registry.qt._registry_helper import (
     register_editable_textbox_handlers,
 )
-from traitsui.qt4.file_editor import SimpleEditor
+from traitsui.qt.file_editor import SimpleEditor
 
 
 def register(registry):
     """Register interactions for the given registry.
 
     If there are any conflicts, an error will occur.
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/font_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/font_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-from traitsui.testing.tester._ui_tester_registry.qt4._registry_helper import (
+from traitsui.testing.tester._ui_tester_registry.qt._registry_helper import (
     register_editable_textbox_handlers,
 )
-from traitsui.qt4.font_editor import TextFontEditor
+from traitsui.qt.font_editor import TextFontEditor
 
 
 def register(registry):
     """Register interactions pertaining to (Qt) FontEditor for the given
     registry.
 
     Parameters
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/instance_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/instance_editor.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 
 from traitsui.testing.tester.command import MouseClick
 from traitsui.testing.tester.locator import Index
 from traitsui.testing.tester.query import SelectedText
 from traitsui.testing.tester._ui_tester_registry._common_ui_targets import (
     BaseSourceWithLocation,
 )
-from traitsui.testing.tester._ui_tester_registry.qt4._interaction_helpers import (  # noqa
+from traitsui.testing.tester._ui_tester_registry.qt._interaction_helpers import (  # noqa
     mouse_click_combobox,
     mouse_click_qwidget,
 )
 from traitsui.testing.tester._ui_tester_registry._traitsui_ui import (
     register_traitsui_ui_solvers,
 )
-from traitsui.qt4.instance_editor import CustomEditor, SimpleEditor
+from traitsui.qt.instance_editor import CustomEditor, SimpleEditor
 
 
 def _get_nested_ui_simple(target):
     """Obtains a nested UI within a Simple Instance Editor.
 
     Parameters
     ----------
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/list_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/list_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 from traitsui.testing.tester.locator import Index
 from traitsui.testing.tester._ui_tester_registry._common_ui_targets import (
     BaseSourceWithLocation,
 )
 from traitsui.testing.tester._ui_tester_registry._traitsui_ui import (
     register_traitsui_ui_solvers,
 )
-from traitsui.testing.tester._ui_tester_registry.qt4 import (
+from traitsui.testing.tester._ui_tester_registry.qt import (
     _interaction_helpers,
 )
-from traitsui.qt4.list_editor import CustomEditor, NotebookEditor, SimpleEditor
+from traitsui.qt.list_editor import CustomEditor, NotebookEditor, SimpleEditor
 
 
 class _IndexedNotebookEditor(BaseSourceWithLocation):
     """Wrapper for a ListEditor (Notebook) with an index."""
 
     source_class = NotebookEditor
     locator_class = Index
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/range_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/range_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-from traitsui.qt4.range_editor import (
+from traitsui.qt.range_editor import (
     LargeRangeSliderEditor,
     LogRangeSliderEditor,
     RangeTextEditor,
     SimpleSliderEditor,
 )
 
 from traitsui.testing.tester.command import KeyClick
 from traitsui.testing.tester.locator import Slider, Textbox
-from traitsui.testing.tester._ui_tester_registry.qt4 import (
+from traitsui.testing.tester._ui_tester_registry.qt import (
     _interaction_helpers,
     _registry_helper,
 )
 
 
 class LocatedTextbox:
     """Wrapper class for a located Textbox in Qt.
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/table_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/table_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-from traitsui.qt4.table_editor import SimpleEditor
+from traitsui.qt.table_editor import SimpleEditor
 
 from traitsui.testing.tester.command import (
     MouseClick,
     MouseDClick,
     KeyClick,
     KeySequence,
 )
@@ -21,15 +21,15 @@
     DisplayedText,
     Selected,
     SelectedIndices,
 )
 from traitsui.testing.tester._ui_tester_registry._common_ui_targets import (
     BaseSourceWithLocation
 )
-from traitsui.testing.tester._ui_tester_registry.qt4 import (
+from traitsui.testing.tester._ui_tester_registry.qt import (
     _interaction_helpers
 )
 
 
 def _query_table_editor_selected(wrapper, interaction):
     selected = wrapper._target.selected
     if not isinstance(selected, list):
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/text_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/text_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
 from traitsui.testing.tester.query import DisplayedText
-from traitsui.testing.tester._ui_tester_registry.qt4 import (
+from traitsui.testing.tester._ui_tester_registry.qt import (
     _interaction_helpers,
 )
-from traitsui.testing.tester._ui_tester_registry.qt4._registry_helper import (
+from traitsui.testing.tester._ui_tester_registry.qt._registry_helper import (
     register_editable_textbox_handlers,
 )
-from traitsui.qt4.text_editor import CustomEditor, ReadonlyEditor, SimpleEditor
+from traitsui.qt.text_editor import CustomEditor, ReadonlyEditor, SimpleEditor
 
 
 def register(registry):
     """Register interactions for the given registry.
 
     If there are any conflicts, an error will occur.
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/ui_base.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/ui_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-from traitsui.qt4.ui_base import ButtonEditor
+from traitsui.qt.ui_base import ButtonEditor
 from traitsui.testing.tester.command import MouseClick
 from traitsui.testing.tester.query import DisplayedText
-from traitsui.testing.tester._ui_tester_registry.qt4 import (
+from traitsui.testing.tester._ui_tester_registry.qt import (
     _interaction_helpers,
 )
 
 
 def register(registry):
     """Register solvers/handlers specific to qt ui_base Editors
     for the given registry.
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/default_registry.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/default_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
 from traitsui.testing.tester.target_registry import TargetRegistry
-from traitsui.testing.tester._ui_tester_registry.qt4._traitsui import (
+from traitsui.testing.tester._ui_tester_registry.qt._traitsui import (
     boolean_editor,
     button_editor,
     check_list_editor,
     directory_editor,
     editor_factory,
     enum_editor,
     file_editor,
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/tests/test_control_widget_registry.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/tests/test_control_widget_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 try:
     from pyface.qt import QtGui
 except ImportError:
     if is_qt():
         raise
 else:
-    from traitsui.testing.tester._ui_tester_registry.qt4._control_widget_registry import (  # noqa: E501
+    from traitsui.testing.tester._ui_tester_registry.qt._control_widget_registry import (  # noqa: E501
         get_widget_registry,
     )
 
 
 class TargetWithControl:
     """An object holding a control attribute."""
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/qt4/tests/test_interaction_helpers.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/qt/tests/test_interaction_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from traitsui.tests._tools import (
     is_qt,
     requires_toolkit,
     ToolkitName,
 )
 from traitsui.testing.tester import command
 from traitsui.testing.tester.exceptions import Disabled
-from traitsui.testing.tester._ui_tester_registry.qt4 import (
+from traitsui.testing.tester._ui_tester_registry.qt import (
     _interaction_helpers,
 )
 
 try:
     from pyface.qt import QtGui
 except ImportError:
     if is_qt():
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/tests/test_default_registry.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/tests/test_default_registry.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/tests/test_layout.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/README.txt` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/__init__.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/__init__.py` & `traitsui-8.0.0/traitsui/tests/test_editors_imports.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,13 +4,16 @@
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
 
-""" This package contains implementations for testing TraitsUI UI editors
-with Wx.
+import unittest
 
-The top-level module ``default_registry`` serves external packages and hides
-implementation details internal to this package.
-"""
+
+class TestEditorsImports(unittest.TestCase):
+
+    def test_editors_import_warns(self):
+        # Importing from traitsui.editors is deprecated
+        with self.assertWarns(DeprecationWarning):
+            from traitsui.editors import BooleanEditor
```

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_control_widget_registry.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_control_widget_registry.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_interaction_helpers.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_interaction_helpers.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_registry_helper.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_registry_helper.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/README.txt` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/README.txt`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/__init__.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/__init__.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/boolean_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/boolean_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/button_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/button_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/check_list_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/check_list_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/directory_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/directory_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/editor_factory.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/editor_factory.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/enum_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/enum_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/file_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/file_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/font_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/font_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/instance_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/instance_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/list_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/list_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/range_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/range_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/text_editor.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/text_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/ui_base.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/_traitsui/ui_base.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/default_registry.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/default_registry.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/tests/test_control_widget_registry.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/tests/test_control_widget_registry.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/_ui_tester_registry/wx/tests/test_interaction_helpers.py` & `traitsui-8.0.0/traitsui/testing/tester/_ui_tester_registry/wx/tests/test_interaction_helpers.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/command.py` & `traitsui-8.0.0/traitsui/testing/tester/command.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/exceptions.py` & `traitsui-8.0.0/traitsui/testing/tester/exceptions.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/locator.py` & `traitsui-8.0.0/traitsui/testing/tester/locator.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/query.py` & `traitsui-8.0.0/traitsui/testing/tester/query.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/target_registry.py` & `traitsui-8.0.0/traitsui/testing/tester/target_registry.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/tests/test_registry.py` & `traitsui-8.0.0/traitsui/testing/tester/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/tests/test_ui_tester.py` & `traitsui-8.0.0/traitsui/testing/tester/tests/test_ui_tester.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/tests/test_ui_wrapper.py` & `traitsui-8.0.0/traitsui/testing/tester/tests/test_ui_wrapper.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/ui_tester.py` & `traitsui-8.0.0/traitsui/testing/tester/ui_tester.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tester/ui_wrapper.py` & `traitsui-8.0.0/traitsui/testing/tester/ui_wrapper.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tests/test_api.py` & `traitsui-8.0.0/traitsui/testing/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/testing/tests/test_exception_handling.py` & `traitsui-8.0.0/traitsui/testing/tests/test_exception_handling.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,16 @@
         gui = GUI()
         with self.assertRaises(
             RuntimeError
         ) as exception_context, self.assertLogs("traitsui") as watcher:
             with reraise_exceptions():
                 gui.invoke_later(raise_error_1)
                 gui.invoke_later(raise_error_2)
-                gui.process_events()
+                gui.invoke_after(100, gui.stop_event_loop)
+                gui.start_event_loop()
 
         error_msg = str(exception_context.exception)
         self.assertIn("ZeroDivisionError", error_msg)
         self.assertIn("IndexError", error_msg)
         log_content1, log_content2 = watcher.output
         self.assertIn("ZeroDivisionError", log_content1)
         self.assertIn("IndexError", log_content2)
```

### Comparing `traitsui-7.4.3/traitsui/testing/tests/test_gui.py` & `traitsui-8.0.0/traitsui/testing/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/_tools.py` & `traitsui-8.0.0/traitsui/tests/_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
     Yields
     ------
     ui: UI
     """
     return UITester().create_ui(object=object, ui_kwargs=ui_kwargs)
 
 
-# ######### Utility tools to test on both qt4 and wx
+# ######### Utility tools to test on both qt and wx
 
 
 def get_children(node):
     if is_wx():
         return node.GetChildren()
     else:
         return node.children()
```

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_animatedGIF_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_animatedGIF_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_boolean_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_boolean_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_button_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_button_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_check_list_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_check_list_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_code_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_code_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
                 style=self.style,
             )
         )
         return traits_view
 
 
 class TestCodeEditor(BaseTestMixin, unittest.TestCase):
+
     def setUp(self):
         BaseTestMixin.setUp(self)
 
     def tearDown(self):
         BaseTestMixin.tearDown(self)
 
     @requires_toolkit([ToolkitName.qt])
```

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_csv_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_csv_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_date_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_date_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 class TestDateEditorCustomQt(BaseTestMixin, unittest.TestCase):
     def setUp(self):
         BaseTestMixin.setUp(self)
 
     def tearDown(self):
         BaseTestMixin.tearDown(self)
 
-    def test_single_select_qt4(self):
+    def test_single_select_qt(self):
         with self.launch_editor(single_select_custom_view) as (foo, editor):
             date = datetime.date(2018, 2, 3)
             self.click_date_on_editor(editor, date)
             self.assertEqual(foo.single_date, date)
 
     def test_multi_select_dates_on_editor(self):
         with self.launch_editor(multi_select_custom_view) as (foo, editor):
@@ -89,24 +89,24 @@
             for date in dates:
                 self.check_select_status(
                     editor=editor, date=date, selected=True
                 )
 
             self.assertEqual(foo.dates, sorted(dates))
 
-    def test_multi_select_qt4_styles_reset(self):
+    def test_multi_select_qt_styles_reset(self):
         with self.launch_editor(multi_select_custom_view) as (foo, editor):
             date = datetime.date(2018, 2, 1)
             self.click_date_on_editor(editor, date)
             self.check_select_status(editor=editor, date=date, selected=True)
 
             self.click_date_on_editor(editor, date)
             self.check_select_status(editor=editor, date=date, selected=False)
 
-    def test_multi_select_qt4_set_model_dates(self):
+    def test_multi_select_qt_set_model_dates(self):
         # Test setting the dates from the model object.
         with self.launch_editor(multi_select_custom_view) as (foo, editor):
             foo.dates = [datetime.date(2010, 1, 2), datetime.date(2010, 2, 1)]
 
             for date in foo.dates:
                 self.check_select_status(
                     editor=editor, date=date, selected=True
@@ -147,15 +147,15 @@
             self.assertEqual(
                 textformat.fontWeight(),
                 QtGui.QFont.Weight.Normal,
                 "{!r} is not unselected.".format(date),
             )
             self.assertEqual(
                 textformat.background().style(),
-                0,  # Qt.BrushStyle.NoBrush,
+                QtCore.Qt.BrushStyle.NoBrush,
                 "Expected brush to have been reset.",
             )
             self.check_date_bgcolor(editor, date, (0, 0, 0))
 
     def click_date_on_editor(self, editor, date):
         from pyface.qt import QtCore
```

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_date_range_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_date_range_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     requires_toolkit,
     ToolkitName,
 )
 
 
 class Foo(HasTraits):
 
-    date_range = Tuple(Date, Date)
+    date_range = Tuple(Date(allow_none=True), Date(allow_none=True))
 
 
 def default_custom_view():
     """Default view of DateRangeEditor"""
     view = View(
         Item(name="date_range", style="custom", editor=DateRangeEditor())
     )
@@ -251,15 +251,15 @@
             self.assertEqual(
                 textformat.fontWeight(),
                 QtGui.QFont.Weight.Normal,
                 "{!r} is not unselected.".format(date),
             )
             self.assertEqual(
                 textformat.background().style(),
-                0,  # Qt.BrushStyle.NoBrush,
+                QtCore.Qt.BrushStyle.NoBrush,
                 "Expected brush to have been reset.",
             )
             self.assertEqual(
                 textformat.background().color().green(),
                 0,
                 "Expected color to have been reset.",
             )
```

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_datetime_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_datetime_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_default_override.py` & `traitsui-8.0.0/traitsui/tests/editors/test_default_override.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_directory_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_directory_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_drop_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_drop_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_enum_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_enum_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
             combobox.perform(KeySequence("two"))
 
             self.assertEqual(enum_edit.value, "one")
             combobox.perform(KeyClick("Enter"))
             self.assertEqual(enum_edit.value, "two")
 
     def test_simple_editor_resizable(self):
-        # Smoke test for `qt4.enum_editor.SimpleEditor.set_size_policy`
+        # Smoke test for `qt.enum_editor.SimpleEditor.set_size_policy`
         enum_edit = EnumModel()
         resizable_view = View(UItem("value", style="simple", resizable=True))
 
         tester = UITester()
         with tester.create_ui(enum_edit, dict(view=resizable_view)):
             pass
```

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_file_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_file_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_font_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_font_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_html_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_html_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
 def qt_target_registry():
     """Return an instance of TargetRegistry for testing Qt + HTMLEditor
 
     Returns
     -------
     target_registry : TargetRegistry
     """
-    from traitsui.qt4.html_editor import SimpleEditor
+    from traitsui.qt.html_editor import SimpleEditor
 
     registry = TargetRegistry()
     registry.register_interaction(
         target_class=SimpleEditor,
         interaction_class=MouseClick,
         handler=lambda wrapper, _: qt_mouse_click_web_view(
             wrapper._target.control, wrapper.delay
```

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_image_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_image_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_image_enum_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_image_enum_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,17 +28,17 @@
 
 # Import needed bitmap/pixmap cache and prepare for patching
 if is_wx():
     from traitsui.wx.helper import bitmap_cache as image_cache
 
     cache_to_patch = "traitsui.wx.image_enum_editor.bitmap_cache"
 elif is_qt():
-    from traitsui.qt4.helper import pixmap_cache as image_cache
+    from traitsui.qt.helper import pixmap_cache as image_cache
 
-    cache_to_patch = "traitsui.qt4.image_enum_editor.pixmap_cache"
+    cache_to_patch = "traitsui.qt.image_enum_editor.pixmap_cache"
 
 is_linux = sys.platform == 'linux'
 
 
 class EnumModel(HasTraits):
 
     value = Enum('top left', 'top right', 'bottom left', 'bottom right')
```

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_instance_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_instance_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_list_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_list_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_liststr_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_liststr_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_liststr_editor_selection.py` & `traitsui-8.0.0/traitsui/tests/editors/test_liststr_editor_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -740,15 +740,15 @@
         self.assertEqual(selected_1, [1])
         self.assertEqual(selected_2, [0])
 
     @requires_toolkit([ToolkitName.qt])
     def test_selection_listener_disconnected(self):
         """Check that selection listeners get correctly disconnected"""
         from pyface.qt.QtGui import QApplication, QItemSelectionModel
-        from pyface.ui.qt4.util.testing import event_loop
+        from pyface.ui.qt.util.testing import event_loop
 
         obj = ListStrEditorWithSelectedIndex(values=["value1", "value2"])
 
         with reraise_exceptions():
             qt_app = QApplication.instance()
             if qt_app is None:
                 qt_app = QApplication([])
```

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_range_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_range_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Thanks for using Enthought open source!
 
 import platform
 import unittest
 
 from pyface.constant import OK
 from pyface.toolkit import toolkit_object
-from traits.api import HasTraits, Float, Int, Range
+from traits.api import HasTraits, Float, Int, Range, TraitError
 from traits.testing.api import UnittestTools
 from traitsui.api import Item, RangeEditor, UItem, View
 from traitsui.testing.api import (
     DisplayedText,
     KeyClick,
     KeySequence,
     Slider,
@@ -49,18 +49,18 @@
     with a local reigstry for tests.
 
     Parameters
     ----------
     registry : TargetRegistry
         The registry being registered to.
     """
-    from traitsui.testing.tester._ui_tester_registry.qt4 import (
+    from traitsui.testing.tester._ui_tester_registry.qt import (
         _registry_helper,
     )
-    from traitsui.qt4.range_editor import SimpleSpinEditor
+    from traitsui.qt.range_editor import SimpleSpinEditor
 
     _registry_helper.register_editable_textbox_handlers(
         registry=registry,
         target_class=SimpleSpinEditor,
         widget_getter=lambda wrapper: wrapper._target.control.lineEdit(),
     )
 
@@ -386,49 +386,53 @@
             float_value_text = float_value_field.locate(Textbox())
             self.assertEqual(
                 float_value_text.inspect(DisplayedText()), "00:00.1"
             )
 
     def test_editor_factory_format(self):
         """
-        format trait on RangeEditor editor factory has been deprecated in
-        favor of format_str. However, behavior should be unchanged.
+        format trait on RangeEditor editor factory has been removed in
+        favor of format_str.
         """
         model = RangeModel()
-        with self.assertWarns(DeprecationWarning):
+        with self.assertRaises(TraitError):
             view = View(
                 Item("float_value", editor=RangeEditor(format="%s ..."))
             )
+
+    def test_editor_factory_format_str(self):
+        """
+        format trait on RangeEditor editor factory has been deprecated in
+        favor of format_str. However, behavior should be unchanged.
+        """
+        model = RangeModel()
+        view = View(
+            Item("float_value", editor=RangeEditor(format_str="%s ..."))
+        )
         tester = UITester()
         with tester.create_ui(model, dict(view=view)) as ui:
             float_value_field = tester.find_by_name(ui, "float_value")
             float_value_text = float_value_field.locate(Textbox())
             self.assertEqual(
                 float_value_text.inspect(DisplayedText()), "0.1 ..."
             )
 
-    def test_editor_format(self):
+    def test_editor_format_str(self):
         """
-        The format trait on an Editor instance previously potentially
-        could override the factory. Now that is not the case.
+        The format trait on an Editor instance has been removed.
         """
         model = RangeModel()
-        with self.assertWarns(DeprecationWarning):
-            view = View(
-                Item("float_value", editor=RangeEditor(format="%s ..."))
-            )
+        view = View(
+            Item("float_value", editor=RangeEditor(format_str="%s ..."))
+        )
         tester = UITester()
         with tester.create_ui(model, dict(view=view)) as ui:
             float_value_field = tester.find_by_name(ui, "float_value")
-            float_value_field._target.format = "%s +++"
-            model.float_value = 0.2
-            float_value_text = float_value_field.locate(Textbox())
-            self.assertEqual(
-                float_value_text.inspect(DisplayedText()), "0.2 ..."
-            )
+            with self.assertRaises(TraitError):
+                float_value_field._target.format = "%s +++"
 
     # regression test for enthought/traitsui#737. Hangs with a popup
     # dialog on wx. (xref: enthought/traitsui#1901)
     @requires_toolkit([ToolkitName.qt])
     def test_set_text_out_of_range(self):
         model = RangeModel()
         view = View(
```

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_range_editor_spinner.py` & `traitsui-8.0.0/traitsui/tests/editors/test_range_editor_spinner.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_range_editor_text.py` & `traitsui-8.0.0/traitsui/tests/editors/test_range_editor_text.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_set_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_set_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_shell_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_shell_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
             editor=ShellEditor(share=share),
         )
     )
 
 
 @requires_toolkit([ToolkitName.qt, ToolkitName.wx])
 class TestShellEditor(BaseTestMixin, unittest.TestCase):
+
     def setUp(self):
         BaseTestMixin.setUp(self)
 
     def tearDown(self):
         BaseTestMixin.tearDown(self)
 
     def smoke_test(self, locals_type, share):
```

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_styled_date_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_styled_date_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_table_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_table_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_tabular_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_tabular_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_text_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_text_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_tree_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_tree_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_tuple_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_tuple_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/editors/test_video_editor.py` & `traitsui-8.0.0/traitsui/tests/editors/test_video_editor.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 #
 # This software is provided without warranty under the terms of the BSD
 # license included in LICENSE.txt and may be redistributed only under
 # the conditions described in the aforementioned license. The license
 # is also available online at http://www.enthought.com/licenses/BSD.txt
 #
 # Thanks for using Enthought open source!
+
+import os
 import unittest
+import subprocess
+import sys
 
 try:
     import numpy as np  # noqa: F401
 except ImportError:
     raise unittest.SkipTest("Can't import NumPy: skipping")
 import pkg_resources
 
@@ -19,14 +23,26 @@
 from traitsui.api import ContextValue, Item, View
 from traitsui.editors.video_editor import MediaStatus, PlayerState, VideoEditor
 from traitsui.tests._tools import BaseTestMixin, create_ui, is_qt5, is_qt6
 
 filename = pkg_resources.resource_filename('traitsui.testing', 'data/test.mp4')
 
 
+# Is a MacOS machine lacking the standard Metal APIs?
+metal_api_missing = False
+if sys.platform == 'darwin' and is_qt6:
+    # TODO: would be nice to detect if Qt build _uses_ Metal
+    result = subprocess.run(
+        ["system_profiler", "SPDisplaysDataType"],
+        capture_output=True,
+        check=True,
+    )
+    metal_api_missing = (b'Metal Family: Supported' not in result.stdout)
+
+
 class MovieTheater(HasTraits):
     url = File(filename)
 
     state = PlayerState()
     duration = Float()
     position = Range(low=0.0, high='duration')
     error = Str()
@@ -35,14 +51,15 @@
     muted = Bool(True)
     volume = Range(0.0, 100.0)
     playback_rate = Float(1.0)
     image_func = Callable()
 
 
 @unittest.skipIf(not is_qt5() and not is_qt6(), 'Requires Qt5 or 6')
+@unittest.skipIf(metal_api_missing, "Mac Qt6 video editor requires Metal API")
 class TestVideoEditor(BaseTestMixin, unittest.TestCase):
     def setUp(self):
         BaseTestMixin.setUp(self)
 
     def tearDown(self):
         BaseTestMixin.tearDown(self)
```

### Comparing `traitsui-7.4.3/traitsui/tests/null_backend/test_font_trait.py` & `traitsui-8.0.0/traitsui/tests/null_backend/test_font_trait.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/null_backend/test_null_toolkit.py` & `traitsui-8.0.0/traitsui/tests/null_backend/test_null_toolkit.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_actions.py` & `traitsui-8.0.0/traitsui/tests/test_actions.py`

 * *Files 7% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         Item("action_successful", style="readonly"),
         menubar=menubar,
         toolbar=toolbar,
         buttons=[TestAction, "OK"],
     )
 
 
-# ----- qt4 helper functions
+# ----- qt helper functions
 
 
 def _qt_trigger_action(container_class, ui):
     toolbar = ui.control.findChild(container_class)
     action = toolbar.actions()[0]
     action.trigger()
 
@@ -121,15 +121,15 @@
     button = bbox.buttons()[1]
     button.click()
 
 
 class TestActions(BaseTestMixin, unittest.TestCase):
 
     def _test_actions(self, trigger_action_func):
-        """Template test for wx, qt4, menu, and toolbar testing."""
+        """Template test for wx, qt, menu, and toolbar testing."""
         # Behavior: when clicking on a menu or toolbar action,
         # the corresponding function should be executed
 
         # create dialog with toolbar adn menu
         dialog = DialogWithToolbar()
         with reraise_exceptions(), create_ui(dialog) as ui:
 
@@ -145,32 +145,32 @@
     def test_qt_toolbar_action(self):
         # Behavior: when clicking on a toolbar action, the corresponding
         # function should be executed
 
         # Bug: in the Qt4 backend, a
         # TypeError: perform() takes exactly 2 arguments (1 given) was raised
         # instead
+        from pyface.ui.qt.action.tool_bar_manager import _ToolBar
 
-        qt_trigger_toolbar_action = partial(
-            _qt_trigger_action, pyface.ui.qt4.action.tool_bar_manager._ToolBar
-        )
+        qt_trigger_toolbar_action = partial(_qt_trigger_action, _ToolBar)
 
         self._test_actions(qt_trigger_toolbar_action)
 
     @requires_toolkit([ToolkitName.qt])
     def test_qt_menu_action(self):
         # Behavior: when clicking on a menu action, the corresponding function
         # should be executed
 
         # Bug: in the Qt4 backend, a
         # TypeError: perform() takes exactly 2 arguments (1 given) was raised
         # instead
+        from pyface.ui.qt.action.menu_manager import _Menu
 
         qt_trigger_menu_action = partial(
-            _qt_trigger_action, pyface.ui.qt4.action.menu_manager._Menu
+            _qt_trigger_action, _Menu
         )
 
         self._test_actions(qt_trigger_menu_action)
 
     @requires_toolkit([ToolkitName.qt])
     def test_qt_button_action(self):
         # Behavior: when clicking on a button action, the corresponding
@@ -266,33 +266,31 @@
     def test_qt_toolbar_action(self):
         # Behavior: when clicking on a toolbar action, the corresponding
         # function should be executed
 
         # Bug: in the Qt4 backend, a
         # TypeError: perform() takes exactly 2 arguments (1 given) was raised
         # instead
+        from pyface.ui.qt.action.tool_bar_manager import _ToolBar
 
-        qt_trigger_toolbar_action = partial(
-            _qt_trigger_action, pyface.ui.qt4.action.tool_bar_manager._ToolBar
-        )
+        qt_trigger_toolbar_action = partial(_qt_trigger_action, _ToolBar)
 
         self._test_actions(qt_trigger_toolbar_action)
 
     @requires_toolkit([ToolkitName.qt])
     def test_qt_menu_action(self):
         # Behavior: when clicking on a menu action, the corresponding function
         # should be executed
 
         # Bug: in the Qt4 backend, a
         # TypeError: perform() takes exactly 2 arguments (1 given) was raised
         # instead
+        from pyface.ui.qt.action.menu_manager import _Menu
 
-        qt_trigger_menu_action = partial(
-            _qt_trigger_action, pyface.ui.qt4.action.menu_manager._Menu
-        )
+        qt_trigger_menu_action = partial(_qt_trigger_action, _Menu)
 
         self._test_actions(qt_trigger_menu_action)
 
     # ----- wx tests
 
     @unittest.skipIf(
         not is_mac_os,
```

### Comparing `traitsui-7.4.3/traitsui/tests/test_color_column.py` & `traitsui-8.0.0/traitsui/tests/test_color_column.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_context_value.py` & `traitsui-8.0.0/traitsui/tests/test_context_value.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_controller.py` & `traitsui-8.0.0/traitsui/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_datetime.py` & `traitsui-8.0.0/traitsui/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_editor.py` & `traitsui-8.0.0/traitsui/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_handler.py` & `traitsui-8.0.0/traitsui/tests/test_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,11 +301,9 @@
             object.edit_traits(handler=handler)
 
     @skipIf(is_null(), "Null toolkit can't create UI")
     def test_handler_init_none(self):
         object = SampleObject()
         handler = SampleHandler(init_return_value=None)
 
-        with self.assertWarns(DeprecationWarning):
-            ui = object.edit_traits(handler=handler)
-
-        ui.dispose()
+        with self.assertRaises(ValueError):
+            object.edit_traits(handler=handler)
```

### Comparing `traitsui-7.4.3/traitsui/tests/test_helper.py` & `traitsui-8.0.0/traitsui/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_key_bindings.py` & `traitsui-8.0.0/traitsui/tests/test_key_bindings.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import unittest
 from unittest.mock import Mock
 
 from traits.testing.api import UnittestTools
 
 
-from ..key_bindings import KeyBinding, KeyBindings, KeyBindingsHandler
+from traitsui.key_bindings import KeyBinding, KeyBindings, KeyBindingsHandler
 
 
 class Controller1:
 
     def __init__(self):
         self.called = None
```

### Comparing `traitsui-7.4.3/traitsui/tests/test_labels.py` & `traitsui-8.0.0/traitsui/tests/test_labels.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_layout.py` & `traitsui-8.0.0/traitsui/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_regression.py` & `traitsui-8.0.0/traitsui/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_shadow_group.py` & `traitsui-8.0.0/traitsui/tests/test_shadow_group.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_splitter_prefs_restored.py` & `traitsui-8.0.0/traitsui/tests/test_splitter_prefs_restored.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_theme.py` & `traitsui-8.0.0/traitsui/tests/test_theme.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_toolkit.py` & `traitsui-8.0.0/traitsui/tests/test_toolkit.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_toolkit_traits.py` & `traitsui-8.0.0/traitsui/tests/test_toolkit_traits.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_tree_node.py` & `traitsui-8.0.0/traitsui/tests/test_tree_node.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_ui.py` & `traitsui-8.0.0/traitsui/tests/test_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
         foo = FooDialog()
         with create_ui(foo) as ui:
 
             # decorate children's `deleteLater` function to check that it is
             # called on `reset`. check only with the editor parts (only widgets
             # are scheduled.
-            # See traitsui.qt4.toolkit.GUIToolkit.destroy_children)
+            # See traitsui.qt.toolkit.GUIToolkit.destroy_children)
             for c in ui.control.children():
                 c.deleteLater = count_calls(c.deleteLater)
 
             ui.reset(destroy=True)
 
             # the top control is still there
             self.assertIsNotNone(ui.control)
@@ -155,23 +155,23 @@
         from pyface import qt
 
         foo = FooDialog()
         with create_ui(foo) as ui:
 
             self.assertEqual(len(ui._editors), 2)
             self.assertIsInstance(
-                ui._editors[0], traitsui.qt4.text_editor.SimpleEditor
+                ui._editors[0], traitsui.qt.text_editor.SimpleEditor
             )
             self.assertIsInstance(ui._editors[0].control, qt.QtGui.QLineEdit)
 
             ui.reset(destroy=False)
 
             self.assertEqual(len(ui._editors), 2)
             self.assertIsInstance(
-                ui._editors[0], traitsui.qt4.text_editor.SimpleEditor
+                ui._editors[0], traitsui.qt.text_editor.SimpleEditor
             )
             self.assertIsNone(ui._editors[0].control)
 
             # children are still there: check first text control
             text_ctrl = ui.control.findChild(qt.QtGui.QLineEdit)
             self.assertIsNotNone(text_ctrl)
```

### Comparing `traitsui-7.4.3/traitsui/tests/test_ui_panel.py` & `traitsui-8.0.0/traitsui/tests/test_ui_panel.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_ui_traits.py` & `traitsui-8.0.0/traitsui/tests/test_ui_traits.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/test_undo.py` & `traitsui-8.0.0/traitsui/tests/test_undo.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,28 +57,14 @@
     def undo(self):
         pass
 
     def redo(self):
         pass
 
 
-class TestAbstractUndoItem(UnittestTools, unittest.TestCase):
-    def test_merge_undo_deprecated(self):
-        undo_item = LegacyUndoItem()
-        other_item = LegacyUndoItem()
-
-        with catch_warnings(record=True) as w:
-            result = undo_item.merge(other_item)
-            self.assertEqual(len(w), 1)
-            self.assertTrue(issubclass(w[0].category, DeprecationWarning))
-            self.assertIn("merge_undo", str(w[0].message))
-
-        self.assertFalse(result)
-
-
 class TestUndoItem(UnittestTools, unittest.TestCase):
     def test_undo(self):
         example = SimpleExample(value=11)
 
         undo_item = UndoItem(
             object=example,
             name='value',
```

### Comparing `traitsui-7.4.3/traitsui/tests/test_view_application.py` & `traitsui-8.0.0/traitsui/tests/test_view_application.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import unittest
 
 from pyface.timer.api import CallbackTimer
 from traits.api import HasTraits, Instance, Int
 from traitsui.api import Handler, Item, UIInfo, View, toolkit
 
-from ._tools import (
+from traitsui.tests._tools import (
     BaseTestMixin,
     GuiTestAssistant,
     is_qt,
     no_gui_test_assistant,
 )
 
 
@@ -98,15 +98,15 @@
             self.closed = True
         else:
             raise NotImplementedError("Can't close current backend")
 
     def click_button(self, text):
         if is_qt():
             from pyface.qt.QtGui import QPushButton
-            from pyface.ui.qt4.util.testing import find_qt_widget
+            from pyface.ui.qt.util.testing import find_qt_widget
 
             button = find_qt_widget(
                 self.handler.info.ui.control,
                 QPushButton,
                 lambda widget: widget.text() == text,
             )
             if button is None:
```

### Comparing `traitsui-7.4.3/traitsui/tests/test_visible_when_layout.py` & `traitsui-8.0.0/traitsui/tests/test_visible_when_layout.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tests/ui_editors/test_data_frame_editor.py` & `traitsui-8.0.0/traitsui/tests/ui_editors/test_data_frame_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/theme.py` & `traitsui-8.0.0/traitsui/theme.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/toolkit.py` & `traitsui-8.0.0/traitsui/toolkit.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/toolkit_traits.py` & `traitsui-8.0.0/traitsui/toolkit_traits.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/tree_node.py` & `traitsui-8.0.0/traitsui/tree_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,26 +246,26 @@
         del self.get_children(object)[index]
 
     def when_children_replaced(self, object, listener, remove):
         """Sets up or removes a listener for children being replaced on a
         specified object.
         """
         object.on_trait_change(
-            listener, self.children, remove=remove, dispatch="fast_ui"
+            listener, self.children, remove=remove, dispatch="ui"
         )
 
     def when_children_changed(self, object, listener, remove):
         """Sets up or removes a listener for children being changed on a
         specified object.
         """
         object.on_trait_change(
             listener,
             self.children + "_items",
             remove=remove,
-            dispatch="fast_ui",
+            dispatch="ui",
         )
 
     def get_label(self, object):
         """Gets the label to display for a specified object."""
         label = self.label
         if label[:1] == "=":
             return label[1:]
@@ -1352,26 +1352,26 @@
         del self.tno_get_children(node)[index]
 
     def tno_when_children_replaced(self, node, listener, remove):
         """Sets up or removes a listener for children being replaced on a
         specified object.
         """
         self.on_trait_change(
-            listener, node.children, remove=remove, dispatch="fast_ui"
+            listener, node.children, remove=remove, dispatch="ui"
         )
 
     def tno_when_children_changed(self, node, listener, remove):
         """Sets up or removes a listener for children being changed on a
         specified object.
         """
         self.on_trait_change(
             listener,
             node.children + "_items",
             remove=remove,
-            dispatch="fast_ui",
+            dispatch="ui",
         )
 
     def tno_get_label(self, node):
         """Gets the label to display for a specified object."""
         label = node.label
         if label[:1] == "=":
             return label[1:]
```

### Comparing `traitsui-7.4.3/traitsui/tree_node_renderer.py` & `traitsui-8.0.0/traitsui/tree_node_renderer.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/ui.py` & `traitsui-8.0.0/traitsui/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,19 +397,17 @@
 
         # Invoke the handler's 'init' method, and abort if it indicates
         # failure:
         started = handler.init(info)
         if started is False:
             raise TraitError("User interface creation aborted")
         elif not isinstance(started, bool):
-            warn(
+            raise ValueError(
                 "Handler.init() must return True or False, but instead "
-                f"returned {started}.  "
-                "This will become an error in a future release.",
-                DeprecationWarning,
+                f"returned {started}."
             )
 
         # For each Handler method whose name is of the form
         # 'object_name_changed', where 'object' is the name of an object in the
         # UI's 'context', create a trait notification handler that will call
         # the method whenever 'object's 'name' trait changes. Also invoke the
         # method immediately so initial user interface state can be correctly
```

### Comparing `traitsui-7.4.3/traitsui/ui_editor.py` & `traitsui-8.0.0/traitsui/ui_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/ui_editors/array_view_editor.py` & `traitsui-8.0.0/traitsui/ui_editors/array_view_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/ui_editors/data_frame_editor.py` & `traitsui-8.0.0/traitsui/ui_editors/data_frame_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/ui_info.py` & `traitsui-8.0.0/traitsui/ui_info.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/ui_traits.py` & `traitsui-8.0.0/traitsui/ui_traits.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/undo.py` & `traitsui-8.0.0/traitsui/undo.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,28 +68,14 @@
 
     def redo(self):
         """Re-does the change."""
         raise NotImplementedError
 
     def merge(self, other):
         """Merges two undo items if possible."""
-        import warnings
-
-        warnings.warn(
-            "'merge_undo' is deprecated and will be removed in TraitsUI 8, "
-            "use 'merge' instead",
-            DeprecationWarning,
-        )
-        return self.merge_undo(other)
-
-    def merge_undo(self, undo_item):
-        """Merges two undo items if possible.
-
-        This method is deprecated.
-        """
         return False
 
 
 class UndoItem(AbstractUndoItem):
     """A change to an object trait, which can be undone."""
 
     # -------------------------------------------------------------------------
@@ -205,21 +191,14 @@
 
                 elif t1 in NumericTypes:
                     # Always merge simple numeric trait changes:
                     self.new_value = v2
                     return True
         return False
 
-    def merge_undo(self, undo_item):
-        """Merges two undo items if possible.
-
-        This is deprecated.
-        """
-        return self.merge(undo_item)
-
     def __repr__(self):
         """Returns a "pretty print" form of the object."""
         n = self.name
         cn = self.object.__class__.__name__
         return "undo( %s.%s = %s )\nredo( %s.%s = %s )" % (
             cn,
             n,
@@ -295,21 +274,14 @@
                     for i, item in enumerate(self.removed):
                         if item is not removed[i]:
                             break
                     else:
                         return True
         return False
 
-    def merge_undo(self, undo_item):
-        """Merges two undo items if possible.
-
-        This is deprecated.
-        """
-        return self.merge(undo_item)
-
     def __repr__(self):
         """Returns a 'pretty print' form of the object."""
         return "undo( %s.%s[%d:%d] = %s )" % (
             self.object.__class__.__name__,
             self.name,
             self.index,
             self.index + len(self.removed),
@@ -360,20 +332,14 @@
 
     #: The undo manager for the history.
     manager = Instance(IUndoManager, allow_none=False)
 
     #: The command stack for the history.
     stack = Instance(ICommandStack, allow_none=False)
 
-    #: List of accumulated undo changes.  Each item is a list of
-    #: AbstractUndoItems that should be done or undone as a group.
-    #: This trait should be considered private.
-    #: This trait is no longer used.
-    history = List()
-
     #: The current position in the list
     now = Property(Int, observe='stack._index')
 
     #: Fired when state changes to undoable
     undoable = Event(False)
 
     #: Fired when state changes to redoable
```

### Comparing `traitsui-7.4.3/traitsui/value_tree.py` & `traitsui-8.0.0/traitsui/value_tree.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/view.py` & `traitsui-8.0.0/traitsui/view.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/view_element.py` & `traitsui-8.0.0/traitsui/view_element.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/view_elements.py` & `traitsui-8.0.0/traitsui/view_elements.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/__init__.py` & `traitsui-8.0.0/traitsui/wx/__init__.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/animated_gif_editor.py` & `traitsui-8.0.0/traitsui/wx/animated_gif_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/array_editor.py` & `traitsui-8.0.0/traitsui/wx/array_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/array_view_editor.py` & `traitsui-8.0.0/traitsui/wx/array_view_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/boolean_editor.py` & `traitsui-8.0.0/traitsui/wx/boolean_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/button_editor.py` & `traitsui-8.0.0/traitsui/wx/button_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/check_list_editor.py` & `traitsui-8.0.0/traitsui/wx/check_list_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/code_editor.py` & `traitsui-8.0.0/traitsui/wx/code_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,14 +92,15 @@
         """Finishes initializing the editor by creating the underlying toolkit
         widget.
         """
         factory = self.factory
         self._editor = editor = PythonEditor(
             parent, show_line_numbers=factory.show_line_numbers
         )
+        editor.create()
         self.control = control = editor.control
 
         # There are a number of events which aren't well documented that look
         # to be useful in future implmentations, below are a subset of the
         # events that look interesting:
         #    EVT_STC_AUTOCOMP_SELECTION
         #    EVT_STC_HOTSPOT_CLICK
```

### Comparing `traitsui-7.4.3/traitsui/wx/color_editor.py` & `traitsui-8.0.0/traitsui/wx/color_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/color_trait.py` & `traitsui-8.0.0/traitsui/wx/color_trait.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/compound_editor.py` & `traitsui-8.0.0/traitsui/wx/compound_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/constants.py` & `traitsui-8.0.0/traitsui/wx/constants.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/csv_list_editor.py` & `traitsui-8.0.0/traitsui/wx/csv_list_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/custom_editor.py` & `traitsui-8.0.0/traitsui/wx/custom_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/data_frame_editor.py` & `traitsui-8.0.0/traitsui/wx/data_frame_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/date_editor.py` & `traitsui-8.0.0/traitsui/wx/date_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/directory_editor.py` & `traitsui-8.0.0/traitsui/wx/directory_editor.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     and a **Browse** button that opens a directory-selection dialog box.
     """
 
     def _create_file_dialog(self):
         """Creates the correct type of file dialog."""
         dlg = DirectoryDialog(
             parent=self.get_control_widget(),
-            default_path=self._file_name.text(),
+            default_path=self._file_name.GetValue(),
         )
         return dlg
 
     def _create_file_popup(self):
         """Creates the correct type of file popup."""
         return PopupDirectory(
             control=self.control,
```

### Comparing `traitsui-7.4.3/traitsui/wx/dnd_editor.py` & `traitsui-8.0.0/traitsui/wx/dnd_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/drop_editor.py` & `traitsui-8.0.0/traitsui/wx/drop_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/editor.py` & `traitsui-8.0.0/traitsui/wx/editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/editor_factory.py` & `traitsui-8.0.0/traitsui/wx/editor_factory.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/enum_editor.py` & `traitsui-8.0.0/traitsui/wx/enum_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/extra/bounds_editor.py` & `traitsui-8.0.0/traitsui/wx/extra/bounds_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,30 +38,30 @@
         if not factory.high_name:
             self.high = factory.high
             self.max = self.high
 
         self.max = factory.max
         self.min = factory.min
 
-        self.format = factory.format
+        self.format_str = factory.format
 
         self.evaluate = factory.evaluate
         self.sync_value(factory.evaluate_name, "evaluate", "from")
 
         self.sync_value(factory.low_name, "low", "both")
         self.sync_value(factory.high_name, "high", "both")
 
         self.control = panel = TraitsUIPanel(parent, -1)
         sizer = wx.FlexGridSizer(2, 3, 0, 0)
 
         # low text box
         self._label_lo = wx.TextCtrl(
             panel,
             -1,
-            self.format % self.low,
+            self.format_str % self.low,
             size=wx.Size(56, 20),
             style=wx.TE_PROCESS_ENTER,
         )
         sizer.Add(self._label_lo, 0, wx.ALIGN_CENTER)
         self._label_lo.Bind(wx.EVT_TEXT_ENTER, self.update_low_on_enter)
         self._label_lo.Bind(wx.EVT_KILL_FOCUS, self.update_low_on_enter)
 
@@ -100,15 +100,15 @@
         self.control.rslider.Bind(wx.EVT_SCROLL, self.update_object_on_scroll)
         sizer.Add(self.control.rslider, 1, wx.EXPAND)
 
         # high text box
         self._label_hi = wx.TextCtrl(
             panel,
             -1,
-            self.format % self.high,
+            self.format_str % self.high,
             size=wx.Size(56, 20),
             style=wx.TE_PROCESS_ENTER,
         )
         sizer.Add(self._label_hi, 0, wx.ALIGN_CENTER)
         self._label_hi.Bind(wx.EVT_TEXT_ENTER, self.update_high_on_enter)
         self._label_hi.Bind(wx.EVT_KILL_FOCUS, self.update_high_on_enter)
 
@@ -132,22 +132,22 @@
         try:
             try:
                 low = eval(str(self._label_lo.GetValue()).strip())
                 if self.evaluate is not None:
                     low = self.evaluate(low)
             except Exception as ex:
                 low = self.low
-                self._label_lo.SetValue(self.format % self.low)
+                self._label_lo.SetValue(self.format_str % self.low)
 
             if not self.factory.is_float:
                 low = int(low)
 
             if low > self.high:
                 low = self.high - self._step_size()
-                self._label_lo.SetValue(self.format % low)
+                self._label_lo.SetValue(self.format_str % low)
 
             self.control.lslider.SetValue(self._convert_to_slider(low))
             self.low = low
         except:
             pass
 
     def update_high_on_enter(self, event):
@@ -156,22 +156,22 @@
         try:
             try:
                 high = eval(str(self._label_hi.GetValue()).strip())
                 if self.evaluate is not None:
                     high = self.evaluate(high)
             except:
                 high = self.high
-                self._label_hi.SetValue(self.format % self.high)
+                self._label_hi.SetValue(self.format_str % self.high)
 
             if not self.factory.is_float:
                 high = int(high)
 
             if high < self.low:
                 high = self.low + self._step_size()
-                self._label_hi.SetValue(self.format % high)
+                self._label_hi.SetValue(self.format_str % high)
 
             self.control.rslider.SetValue(self._convert_to_slider(high))
             self.high = high
         except:
             pass
 
     def update_object_on_scroll(self, evt):
@@ -225,23 +225,23 @@
             + (value - self.min) / self._step_size()
         )
 
     def _low_changed(self, low):
         if self.control is None:
             return
         if self._label_lo is not None:
-            self._label_lo.SetValue(self.format % low)
+            self._label_lo.SetValue(self.format_str % low)
 
         self.control.lslider.SetValue(self._convert_to_slider(low))
 
     def _high_changed(self, high):
         if self.control is None:
             return
         if self._label_hi is not None:
-            self._label_hi.SetValue(self.format % high)
+            self._label_hi.SetValue(self.format_str % high)
 
         self.control.rslider.SetValue(self._convert_to_slider(self.high))
 
 
 class BoundsEditor(RangeEditor):
 
     min = Union(None, Float)
```

### Comparing `traitsui-7.4.3/traitsui/wx/extra/led_editor.py` & `traitsui-8.0.0/traitsui/wx/extra/led_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/extra/windows/flash_editor.py` & `traitsui-8.0.0/traitsui/wx/extra/windows/flash_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/extra/windows/ie_html_editor.py` & `traitsui-8.0.0/traitsui/wx/extra/windows/ie_html_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/file_editor.py` & `traitsui-8.0.0/traitsui/wx/file_editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
         if self.history is not None:
             self._no_update = True
             self.history.value = self.str_value
             self._no_update = False
         else:
             self._file_name.SetValue(self.str_value)
 
-    def show_file_dialog(self, event):
+    def show_file_dialog(self, event=None):
         """Displays the pop-up file dialog."""
         if self.history is not None:
             self.popup = self._create_file_popup()
         else:
             dlg = self._create_file_dialog()
             dlg.open()
 
@@ -202,16 +202,16 @@
         if len(self.factory.filter) > 0:
             wildcard = "|".join(self.factory.filter)
         else:
             wildcard = "All Files (*.*)|*.*"
 
         dlg = FileDialog(
             parent=self.get_control_widget(),
-            default_path=self._file_name.text(),
-            action="save" if self.factory.dialog_style == "save as" else "open",
+            default_path=self._file_name.GetValue(),
+            action="save as" if self.factory.dialog_style == "save" else "open",
             wildcard=wildcard,
         )
         return dlg
 
     def _create_file_popup(self):
         """Creates the correct type of file popup."""
         return PopupFile(
```

### Comparing `traitsui-7.4.3/traitsui/wx/font_editor.py` & `traitsui-8.0.0/traitsui/wx/font_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/font_trait.py` & `traitsui-8.0.0/traitsui/wx/font_trait.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,20 +45,20 @@
 # Strings to ignore in text representations of fonts
 font_noise = ["pt", "point", "family"]
 
 
 def font_to_str(font):
     """Converts a wx.Font into a string description of itself."""
     family = {
-        wx.FONTFAMILY_DECORATIVE: "decorative family",
-        wx.FONTFAMILY_ROMAN: "roman family",
-        wx.FONTFAMILY_SCRIPT: "script family",
-        wx.FONTFAMILY_SWISS: "swiss family",
-        wx.FONTFAMILY_MODERN: "modern family",
-        wx.FONTFAMILY_TELETYPE: "typewriter family",
+        wx.FONTFAMILY_DECORATIVE: "decorative ",
+        wx.FONTFAMILY_ROMAN: "roman ",
+        wx.FONTFAMILY_SCRIPT: "script ",
+        wx.FONTFAMILY_SWISS: "swiss ",
+        wx.FONTFAMILY_MODERN: "modern ",
+        wx.FONTFAMILY_TELETYPE: "typewriter ",
     }.get(font.GetFamily(), "")
     weight = {wx.FONTWEIGHT_LIGHT: " Light", wx.FONTWEIGHT_BOLD: " Bold"}.get(
         font.GetWeight(), ""
     )
     style = {wx.FONTSTYLE_SLANT: " Oblique", wx.FONTSTYLE_ITALIC: " Italic"}.get(
         font.GetStyle(), ""
     )
```

### Comparing `traitsui-7.4.3/traitsui/wx/helper.py` & `traitsui-8.0.0/traitsui/wx/helper.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/history_control.py` & `traitsui-8.0.0/traitsui/wx/history_control.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/history_editor.py` & `traitsui-8.0.0/traitsui/wx/history_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/html_editor.py` & `traitsui-8.0.0/traitsui/wx/html_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/image_control.py` & `traitsui-8.0.0/traitsui/wx/image_control.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/image_editor.py` & `traitsui-8.0.0/traitsui/wx/image_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/image_enum_editor.py` & `traitsui-8.0.0/traitsui/wx/image_enum_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/image_slice.py` & `traitsui-8.0.0/traitsui/wx/image_slice.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/images/file.png` & `traitsui-8.0.0/traitsui/wx/images/file.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/images/frame.ico` & `traitsui-8.0.0/traitsui/wx/images/frame.ico`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/images/group.png` & `traitsui-8.0.0/traitsui/wx/images/group.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/images/hs_color_map.png` & `traitsui-8.0.0/traitsui/wx/images/hs_color_map.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/images/item.png` & `traitsui-8.0.0/traitsui/wx/images/item.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/images/nb_open.png` & `traitsui-8.0.0/traitsui/wx/images/nb_open.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/images/object.png` & `traitsui-8.0.0/traitsui/wx/images/object.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/images/open.png` & `traitsui-8.0.0/traitsui/wx/images/open.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/images/table_colors.png` & `traitsui-8.0.0/traitsui/wx/images/table_colors.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/images/table_move_down.png` & `traitsui-8.0.0/traitsui/wx/images/table_move_down.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/images/table_move_up.png` & `traitsui-8.0.0/traitsui/wx/images/table_move_up.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/images/table_no_sort.png` & `traitsui-8.0.0/traitsui/wx/images/table_no_sort.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/images/table_search.png` & `traitsui-8.0.0/traitsui/wx/images/table_search.png`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/instance_editor.py` & `traitsui-8.0.0/traitsui/wx/instance_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/key_binding_editor.py` & `traitsui-8.0.0/traitsui/wx/key_binding_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/key_event_to_name.py` & `traitsui-8.0.0/traitsui/wx/key_event_to_name.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/list_editor.py` & `traitsui-8.0.0/traitsui/wx/list_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/list_str_editor.py` & `traitsui-8.0.0/traitsui/wx/list_str_editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,15 +313,15 @@
                 index -= 1
                 if index < 0:
                     index = None
 
         if index is None:
             visible = top + pn - 2
             if visible >= 0 and visible < control.GetItemCount():
-                control.EnsureVisible(visible)
+                control.ScrollHint.EnsureVisible(visible)
             if self.factory.multi_select:
                 for index in self.multi_selected_indices:
                     if 0 <= index < n:
                         control.SetItemState(
                             index,
                             wx.LIST_STATE_SELECTED,
                             wx.LIST_STATE_SELECTED,
@@ -332,23 +332,23 @@
                         self.selected_index,
                         wx.LIST_STATE_SELECTED,
                         wx.LIST_STATE_SELECTED,
                     )
             return
 
         if 0 <= (index - top) < pn:
-            control.EnsureVisible(
+            control.ScrollHint.EnsureVisible(
                 min(top + pn - 2, control.GetItemCount() - 1)
             )
         elif index < top:
-            control.EnsureVisible(
+            control.ScrollHint.EnsureVisible(
                 min(index + pn - 1, control.GetItemCount() - 1)
             )
         else:
-            control.EnsureVisible(index)
+            control.ScrollHint.EnsureVisible(index)
 
         control.SetItemState(
             index,
             wx.LIST_STATE_SELECTED | wx.LIST_STATE_FOCUSED,
             wx.LIST_STATE_SELECTED | wx.LIST_STATE_FOCUSED,
         )
```

### Comparing `traitsui-7.4.3/traitsui/wx/menu.py` & `traitsui-8.0.0/traitsui/wx/menu.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/null_editor.py` & `traitsui-8.0.0/traitsui/wx/null_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/popup_editor.py` & `traitsui-8.0.0/traitsui/wx/popup_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/progress_editor.py` & `traitsui-8.0.0/traitsui/wx/progress_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/range_editor.py` & `traitsui-8.0.0/traitsui/wx/range_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,17 +70,14 @@
 
     #: Low value for the slider range
     low = Any()
 
     #: High value for the slider range
     high = Any()
 
-    #: Deprecated: This trait is no longer used. See enthought/traitsui#1704
-    format = Str()
-
     #: Flag indicating that the UI is in the process of being updated
     ui_changing = Bool(False)
 
     def init(self, parent):
         """Finishes initializing the editor by creating the underlying toolkit
         widget.
         """
```

### Comparing `traitsui-7.4.3/traitsui/wx/rgb_color_editor.py` & `traitsui-8.0.0/traitsui/wx/rgb_color_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/rgb_color_trait.py` & `traitsui-8.0.0/traitsui/wx/rgb_color_trait.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/scrubber_editor.py` & `traitsui-8.0.0/traitsui/wx/scrubber_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/search_editor.py` & `traitsui-8.0.0/traitsui/wx/search_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/set_editor.py` & `traitsui-8.0.0/traitsui/wx/set_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/shell_editor.py` & `traitsui-8.0.0/traitsui/wx/shell_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/table_editor.py` & `traitsui-8.0.0/traitsui/wx/table_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/table_model.py` & `traitsui-8.0.0/traitsui/wx/table_model.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/tabular_editor.py` & `traitsui-8.0.0/traitsui/wx/tabular_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -490,27 +490,27 @@
                 row -= 1
                 if row < 0:
                     row = None
 
         if row is None:
             visible = bottom
             if visible >= 0 and visible < control.GetItemCount():
-                control.EnsureVisible(visible)
+                control.ScrollHint.EnsureVisible(visible)
             return
 
         if 0 <= (row - top) < pn:
-            control.EnsureVisible(
+            control.ScrollHint.EnsureVisible(
                 min(top + pn - 2, control.GetItemCount() - 1)
             )
         elif row < top:
-            control.EnsureVisible(
+            control.ScrollHint.EnsureVisible(
                 min(row + pn - 1, control.GetItemCount() - 1)
             )
         else:
-            control.EnsureVisible(row)
+            control.ScrollHint.EnsureVisible(row)
 
         control.SetItemState(
             row,
             wx.LIST_STATE_SELECTED | wx.LIST_STATE_FOCUSED,
             wx.LIST_STATE_SELECTED | wx.LIST_STATE_FOCUSED,
         )
```

### Comparing `traitsui-7.4.3/traitsui/wx/tests/test_color_trait.py` & `traitsui-8.0.0/traitsui/wx/tests/test_color_trait.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/tests/test_font_trait.py` & `traitsui-8.0.0/traitsui/wx/tests/test_font_trait.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 class FontExample(HasTraits):
 
     font = WxFont()
 
 
-class TestPyQtFont(unittest.TestCase):
+class TestWxFont(unittest.TestCase):
 
     def test_create_traitsfont(self):
         expected_outcomes = {}
         expected_outcomes[""] = TraitsFont(
             10, wx.FONTFAMILY_DEFAULT, wx.FONTSTYLE_NORMAL, wx.FONTWEIGHT_NORMAL
         )
 
@@ -71,75 +71,75 @@
 
         for name, expected in expected_outcomes.items():
             with self.subTest(name=name):
                 result = create_traitsfont(name)
 
                 # test we get expected font
                 self.assertIsInstance(result, TraitsFont)
-                self.assert_qfont_equal(result, expected)
+                self.assert_wxfont_equal(result, expected)
 
                 # round-trip trhough font_to_str
                 result_2 = create_traitsfont(font_to_str(result))
-                self.assert_qfont_equal(result, result_2)
+                self.assert_wxfont_equal(result, result_2)
 
     def test_create_traitsfont_wx_font(self):
         font = wx.Font(
             18, wx.FONTFAMILY_SCRIPT, wx.FONTSTYLE_SLANT, wx.FONTWEIGHT_BOLD, True, "Comic Sans",
         )
         traits_font = create_traitsfont(font)
 
         self.assertIsInstance(traits_font, TraitsFont)
-        self.assert_qfont_equal(traits_font, font)
+        self.assert_wxfont_equal(traits_font, font)
 
     def test_create_traitsfont_system_default(self):
         font = wx.SystemSettings.GetFont(wx.SYS_DEFAULT_GUI_FONT)
         traits_font = create_traitsfont(font)
 
         self.assertIsInstance(traits_font, TraitsFont)
-        self.assert_qfont_equal(traits_font, font)
+        self.assert_wxfont_equal(traits_font, font)
 
     def test_create_traitsfont_pyface_font(self):
         args = simple_parser("18 pt Bold Oblique Underline Courier")
         font = PyfaceFont(**args)
         traits_font = create_traitsfont(font)
 
         self.assertIsInstance(traits_font, TraitsFont)
-        self.assert_qfont_equal(traits_font, font.to_toolkit())
+        self.assert_wxfont_equal(traits_font, font.to_toolkit())
 
     def test_font_trait_default(self):
         obj = FontExample()
 
         self.assertIsInstance(obj.font, TraitsFont)
-        self.assert_qfont_equal(obj.font, wx.SystemSettings.GetFont(wx.SYS_DEFAULT_GUI_FONT))
+        self.assert_wxfont_equal(obj.font, wx.SystemSettings.GetFont(wx.SYS_DEFAULT_GUI_FONT))
 
     def test_font_trait_str(self):
         obj = FontExample(font="18 pt Bold Oblique Underline Comic Sans script")
         wx_font = TraitsFont(
             18, wx.FONTFAMILY_DEFAULT, wx.FONTSTYLE_SLANT, wx.FONTWEIGHT_BOLD, True, "Comic Sans",
         )
 
         self.assertIsInstance(obj.font, TraitsFont)
-        self.assert_qfont_equal(obj.font, wx_font)
+        self.assert_wxfont_equal(obj.font, wx_font)
 
     def test_font_trait_wx_font(self):
         wx_font = TraitsFont(
             18, wx.FONTFAMILY_DEFAULT, wx.FONTSTYLE_SLANT, wx.FONTWEIGHT_BOLD, True, "Comic Sans",
         )
         obj = FontExample(font=wx_font)
 
         self.assertIsInstance(obj.font, TraitsFont)
-        self.assert_qfont_equal(obj.font, wx_font)
+        self.assert_wxfont_equal(obj.font, wx_font)
 
     def test_font_trait_pyface_font(self):
         args = simple_parser("18 pt Bold Oblique Underline Courier typewriter")
         font = PyfaceFont(**args)
         obj = FontExample(font=font)
 
         self.assertIsInstance(obj.font, TraitsFont)
-        self.assert_qfont_equal(obj.font, font.to_toolkit())
+        self.assert_wxfont_equal(obj.font, font.to_toolkit())
 
     def test_font_trait_none(self):
         obj = FontExample(font=None)
 
         self.assertIsNone(obj.font)
 
     def test_font_trait_bad(self):
```

### Comparing `traitsui-7.4.3/traitsui/wx/text_editor.py` & `traitsui-8.0.0/traitsui/wx/text_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/time_editor.py` & `traitsui-8.0.0/traitsui/wx/time_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/title_editor.py` & `traitsui-8.0.0/traitsui/wx/title_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/toolkit.py` & `traitsui-8.0.0/traitsui/wx/toolkit.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/tree_editor.py` & `traitsui-8.0.0/traitsui/wx/tree_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/tuple_editor.py` & `traitsui-8.0.0/traitsui/wx/tuple_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/ui_base.py` & `traitsui-8.0.0/traitsui/wx/ui_base.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/ui_editor.py` & `traitsui-8.0.0/traitsui/wx/ui_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/ui_live.py` & `traitsui-8.0.0/traitsui/wx/ui_live.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/ui_modal.py` & `traitsui-8.0.0/traitsui/wx/ui_modal.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/ui_panel.py` & `traitsui-8.0.0/traitsui/wx/ui_panel.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/ui_window.py` & `traitsui-8.0.0/traitsui/wx/ui_window.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/ui_wizard.py` & `traitsui-8.0.0/traitsui/wx/ui_wizard.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/value_editor.py` & `traitsui-8.0.0/traitsui/wx/value_editor.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui/wx/view_application.py` & `traitsui-8.0.0/traitsui/wx/view_application.py`

 * *Files identical despite different names*

### Comparing `traitsui-7.4.3/traitsui.egg-info/SOURCES.txt` & `traitsui-8.0.0/traitsui.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 README_example.png
 edm.yaml
 image_LICENSE.txt
 image_LICENSE_Eclipse.txt
 image_LICENSE_Nuvola.txt
 image_LICENSE_OOo.txt
 pyproject.toml
-setup.cfg
-setup.py
 docs/Makefile
 docs/README.rst
 docs/api.css
 docs/make.bat
 docs/traits_ui.ppt
 docs/traits_ui_slides.pdf
 docs/traitsuidocreadme.txt
@@ -361,15 +359,14 @@
 integrationtests/ui/text_editor_invalid.py
 integrationtests/ui/tree_editor_test.py
 integrationtests/ui/images/bottom_left_origin.gif
 integrationtests/ui/images/bottom_right_origin.gif
 integrationtests/ui/images/top_left_origin.gif
 integrationtests/ui/images/top_right_origin.gif
 traitsui/__init__.py
-traitsui/_version.py
 traitsui/api.py
 traitsui/base_panel.py
 traitsui/basic_editor_factory.py
 traitsui/color_column.py
 traitsui/context_value.py
 traitsui/default_dock_window_theme.py
 traitsui/delegating_handler.py
@@ -408,15 +405,14 @@
 traitsui/view.py
 traitsui/view_element.py
 traitsui/view_elements.py
 traitsui.egg-info/PKG-INFO
 traitsui.egg-info/SOURCES.txt
 traitsui.egg-info/dependency_links.txt
 traitsui.egg-info/entry_points.txt
-traitsui.egg-info/not-zip-safe
 traitsui.egg-info/requires.txt
 traitsui.egg-info/top_level.txt
 traitsui/editors/__init__.py
 traitsui/editors/api.py
 traitsui/editors/array_editor.py
 traitsui/editors/boolean_editor.py
 traitsui/editors/button_editor.py
@@ -612,100 +608,101 @@
 traitsui/extras/images/run.png
 traitsui/images/frame.png
 traitsui/null/__init__.py
 traitsui/null/color_trait.py
 traitsui/null/font_trait.py
 traitsui/null/rgb_color_trait.py
 traitsui/null/toolkit.py
+traitsui/qt/__init__.py
+traitsui/qt/array_editor.py
+traitsui/qt/array_view_editor.py
+traitsui/qt/boolean_editor.py
+traitsui/qt/button_editor.py
+traitsui/qt/check_list_editor.py
+traitsui/qt/clipboard.py
+traitsui/qt/code_editor.py
+traitsui/qt/color_editor.py
+traitsui/qt/color_trait.py
+traitsui/qt/compound_editor.py
+traitsui/qt/constants.py
+traitsui/qt/csv_list_editor.py
+traitsui/qt/custom_editor.py
+traitsui/qt/data_frame_editor.py
+traitsui/qt/date_editor.py
+traitsui/qt/date_range_editor.py
+traitsui/qt/datetime_editor.py
+traitsui/qt/directory_editor.py
+traitsui/qt/drop_editor.py
+traitsui/qt/editor.py
+traitsui/qt/editor_factory.py
+traitsui/qt/enum_editor.py
+traitsui/qt/file_editor.py
+traitsui/qt/font_editor.py
+traitsui/qt/font_trait.py
+traitsui/qt/helper.py
+traitsui/qt/history_editor.py
+traitsui/qt/html_editor.py
+traitsui/qt/image_editor.py
+traitsui/qt/image_enum_editor.py
+traitsui/qt/instance_editor.py
+traitsui/qt/key_binding_editor.py
+traitsui/qt/key_event_to_name.py
+traitsui/qt/list_editor.py
+traitsui/qt/list_str_editor.py
+traitsui/qt/list_str_model.py
+traitsui/qt/menu.py
+traitsui/qt/null_editor.py
+traitsui/qt/progress_editor.py
+traitsui/qt/range_editor.py
+traitsui/qt/rgb_color_editor.py
+traitsui/qt/rgb_color_trait.py
+traitsui/qt/search_editor.py
+traitsui/qt/set_editor.py
+traitsui/qt/shell_editor.py
+traitsui/qt/styled_date_editor.py
+traitsui/qt/table_editor.py
+traitsui/qt/table_model.py
+traitsui/qt/tabular_editor.py
+traitsui/qt/tabular_model.py
+traitsui/qt/text_editor.py
+traitsui/qt/time_editor.py
+traitsui/qt/title_editor.py
+traitsui/qt/toolkit.py
+traitsui/qt/tree_editor.py
+traitsui/qt/tree_node_renderers.py
+traitsui/qt/tuple_editor.py
+traitsui/qt/ui_base.py
+traitsui/qt/ui_editor.py
+traitsui/qt/ui_live.py
+traitsui/qt/ui_modal.py
+traitsui/qt/ui_panel.py
+traitsui/qt/value_editor.py
+traitsui/qt/video_editor.py
+traitsui/qt/view_application.py
+traitsui/qt/extra/__init__.py
+traitsui/qt/extra/bounds_editor.py
+traitsui/qt/extra/checkbox_renderer.py
+traitsui/qt/extra/led_editor.py
+traitsui/qt/extra/progress_renderer.py
+traitsui/qt/extra/qt_view.py
+traitsui/qt/extra/range_slider.py
+traitsui/qt/extra/table_image_renderer.py
+traitsui/qt/images/closetab.png
+traitsui/qt/images/frame.png
+traitsui/qt/images/list_editor.png
+traitsui/qt/images/next.png
+traitsui/qt/images/previous.png
+traitsui/qt/tests/__init__.py
+traitsui/qt/tests/test_color_trait.py
+traitsui/qt/tests/test_font_trait.py
+traitsui/qt/tests/test_helper.py
+traitsui/qt/tests/test_tabular_model.py
+traitsui/qt/tests/test_ui_base.py
+traitsui/qt/tests/test_ui_panel.py
 traitsui/qt4/__init__.py
-traitsui/qt4/array_editor.py
-traitsui/qt4/array_view_editor.py
-traitsui/qt4/boolean_editor.py
-traitsui/qt4/button_editor.py
-traitsui/qt4/check_list_editor.py
-traitsui/qt4/clipboard.py
-traitsui/qt4/code_editor.py
-traitsui/qt4/color_editor.py
-traitsui/qt4/color_trait.py
-traitsui/qt4/compound_editor.py
-traitsui/qt4/constants.py
-traitsui/qt4/csv_list_editor.py
-traitsui/qt4/custom_editor.py
-traitsui/qt4/data_frame_editor.py
-traitsui/qt4/date_editor.py
-traitsui/qt4/date_range_editor.py
-traitsui/qt4/datetime_editor.py
-traitsui/qt4/directory_editor.py
-traitsui/qt4/drop_editor.py
-traitsui/qt4/editor.py
-traitsui/qt4/editor_factory.py
-traitsui/qt4/enum_editor.py
-traitsui/qt4/file_editor.py
-traitsui/qt4/font_editor.py
-traitsui/qt4/font_trait.py
-traitsui/qt4/helper.py
-traitsui/qt4/history_editor.py
-traitsui/qt4/html_editor.py
-traitsui/qt4/image_editor.py
-traitsui/qt4/image_enum_editor.py
-traitsui/qt4/instance_editor.py
-traitsui/qt4/key_binding_editor.py
-traitsui/qt4/key_event_to_name.py
-traitsui/qt4/list_editor.py
-traitsui/qt4/list_str_editor.py
-traitsui/qt4/list_str_model.py
-traitsui/qt4/menu.py
-traitsui/qt4/null_editor.py
-traitsui/qt4/progress_editor.py
-traitsui/qt4/range_editor.py
-traitsui/qt4/rgb_color_editor.py
-traitsui/qt4/rgb_color_trait.py
-traitsui/qt4/search_editor.py
-traitsui/qt4/set_editor.py
-traitsui/qt4/shell_editor.py
-traitsui/qt4/styled_date_editor.py
-traitsui/qt4/table_editor.py
-traitsui/qt4/table_model.py
-traitsui/qt4/tabular_editor.py
-traitsui/qt4/tabular_model.py
-traitsui/qt4/text_editor.py
-traitsui/qt4/time_editor.py
-traitsui/qt4/title_editor.py
-traitsui/qt4/toolkit.py
-traitsui/qt4/tree_editor.py
-traitsui/qt4/tree_node_renderers.py
-traitsui/qt4/tuple_editor.py
-traitsui/qt4/ui_base.py
-traitsui/qt4/ui_editor.py
-traitsui/qt4/ui_live.py
-traitsui/qt4/ui_modal.py
-traitsui/qt4/ui_panel.py
-traitsui/qt4/value_editor.py
-traitsui/qt4/video_editor.py
-traitsui/qt4/view_application.py
-traitsui/qt4/extra/__init__.py
-traitsui/qt4/extra/bounds_editor.py
-traitsui/qt4/extra/checkbox_renderer.py
-traitsui/qt4/extra/led_editor.py
-traitsui/qt4/extra/progress_renderer.py
-traitsui/qt4/extra/qt_view.py
-traitsui/qt4/extra/range_slider.py
-traitsui/qt4/extra/table_image_renderer.py
-traitsui/qt4/images/closetab.png
-traitsui/qt4/images/frame.png
-traitsui/qt4/images/list_editor.png
-traitsui/qt4/images/next.png
-traitsui/qt4/images/previous.png
-traitsui/qt4/tests/__init__.py
-traitsui/qt4/tests/test_color_trait.py
-traitsui/qt4/tests/test_font_trait.py
-traitsui/qt4/tests/test_helper.py
-traitsui/qt4/tests/test_tabular_model.py
-traitsui/qt4/tests/test_ui_base.py
-traitsui/qt4/tests/test_ui_panel.py
 traitsui/testing/README.txt
 traitsui/testing/__init__.py
 traitsui/testing/_exception_handling.py
 traitsui/testing/_gui.py
 traitsui/testing/api.py
 traitsui/testing/data/test.mp4
 traitsui/testing/tester/README.txt
@@ -722,39 +719,39 @@
 traitsui/testing/tester/_ui_tester_registry/README.txt
 traitsui/testing/tester/_ui_tester_registry/__init__.py
 traitsui/testing/tester/_ui_tester_registry/_common_ui_targets.py
 traitsui/testing/tester/_ui_tester_registry/_compat.py
 traitsui/testing/tester/_ui_tester_registry/_layout.py
 traitsui/testing/tester/_ui_tester_registry/_traitsui_ui.py
 traitsui/testing/tester/_ui_tester_registry/default_registry.py
-traitsui/testing/tester/_ui_tester_registry/qt4/README.txt
-traitsui/testing/tester/_ui_tester_registry/qt4/__init__.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_control_widget_registry.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_interaction_helpers.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_registry_helper.py
-traitsui/testing/tester/_ui_tester_registry/qt4/default_registry.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/README.txt
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/__init__.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/boolean_editor.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/button_editor.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/check_list_editor.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/directory_editor.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/editor_factory.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/enum_editor.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/file_editor.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/font_editor.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/instance_editor.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/list_editor.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/range_editor.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/table_editor.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/text_editor.py
-traitsui/testing/tester/_ui_tester_registry/qt4/_traitsui/ui_base.py
-traitsui/testing/tester/_ui_tester_registry/qt4/tests/__init__.py
-traitsui/testing/tester/_ui_tester_registry/qt4/tests/test_control_widget_registry.py
-traitsui/testing/tester/_ui_tester_registry/qt4/tests/test_interaction_helpers.py
+traitsui/testing/tester/_ui_tester_registry/qt/README.txt
+traitsui/testing/tester/_ui_tester_registry/qt/__init__.py
+traitsui/testing/tester/_ui_tester_registry/qt/_control_widget_registry.py
+traitsui/testing/tester/_ui_tester_registry/qt/_interaction_helpers.py
+traitsui/testing/tester/_ui_tester_registry/qt/_registry_helper.py
+traitsui/testing/tester/_ui_tester_registry/qt/default_registry.py
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/README.txt
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/__init__.py
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/boolean_editor.py
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/button_editor.py
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/check_list_editor.py
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/directory_editor.py
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/editor_factory.py
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/enum_editor.py
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/file_editor.py
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/font_editor.py
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/instance_editor.py
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/list_editor.py
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/range_editor.py
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/table_editor.py
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/text_editor.py
+traitsui/testing/tester/_ui_tester_registry/qt/_traitsui/ui_base.py
+traitsui/testing/tester/_ui_tester_registry/qt/tests/__init__.py
+traitsui/testing/tester/_ui_tester_registry/qt/tests/test_control_widget_registry.py
+traitsui/testing/tester/_ui_tester_registry/qt/tests/test_interaction_helpers.py
 traitsui/testing/tester/_ui_tester_registry/tests/__init__.py
 traitsui/testing/tester/_ui_tester_registry/tests/test_default_registry.py
 traitsui/testing/tester/_ui_tester_registry/tests/test_layout.py
 traitsui/testing/tester/_ui_tester_registry/wx/README.txt
 traitsui/testing/tester/_ui_tester_registry/wx/__init__.py
 traitsui/testing/tester/_ui_tester_registry/wx/_control_widget_registry.py
 traitsui/testing/tester/_ui_tester_registry/wx/_interaction_helpers.py
@@ -790,14 +787,15 @@
 traitsui/tests/_tools.py
 traitsui/tests/test_actions.py
 traitsui/tests/test_color_column.py
 traitsui/tests/test_context_value.py
 traitsui/tests/test_controller.py
 traitsui/tests/test_datetime.py
 traitsui/tests/test_editor.py
+traitsui/tests/test_editors_imports.py
 traitsui/tests/test_handler.py
 traitsui/tests/test_helper.py
 traitsui/tests/test_key_bindings.py
 traitsui/tests/test_labels.py
 traitsui/tests/test_layout.py
 traitsui/tests/test_regression.py
 traitsui/tests/test_shadow_group.py
```

