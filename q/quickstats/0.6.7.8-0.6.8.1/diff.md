# Comparing `tmp/quickstats-0.6.7.8.tar.gz` & `tmp/quickstats-0.6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstats-0.6.7.8.tar", last modified: Mon Apr 10 20:19:27 2023, max compression
+gzip compressed data, was "quickstats-0.6.8.1.tar", last modified: Mon May 22 12:55:36 2023, max compression
```

## Comparing `quickstats-0.6.7.8.tar` & `quickstats-0.6.8.1.tar`

### file list

```diff
@@ -1,237 +1,239 @@
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/README.md
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/bin/
--rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1603 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/bin/quickstats
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      626 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-04-10 18:07:42.000000 quickstats-0.6.7.8/quickstats/_version.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/analysis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.7.8/quickstats/analysis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.7.8/quickstats/analysis/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.7.8/quickstats/analysis/analysis_path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2023-03-14 14:12:10.000000 quickstats-0.6.7.8/quickstats/analysis/config_format_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    41488 2023-02-18 18:09:50.000000 quickstats-0.6.7.8/quickstats/analysis/data_loading.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/analysis/data_preprocessing.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    86085 2023-03-23 15:12:41.000000 quickstats-0.6.7.8/quickstats/analysis/event_categorization.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/analysis/multi_class_boundary_tree.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9328 2023-03-05 13:58:00.000000 quickstats-0.6.7.8/quickstats/analysis/ntuple_conversion_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31710 2023-04-03 17:20:21.000000 quickstats-0.6.7.8/quickstats/analysis/ntuple_process_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8790 2023-04-06 13:30:03.000000 quickstats-0.6.7.8/quickstats/analysis/sample_poly_param_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/analysis/systematics/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2023-03-07 22:17:53.000000 quickstats-0.6.7.8/quickstats/analysis/systematics/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29659 2023-04-10 19:52:47.000000 quickstats-0.6.7.8/quickstats/analysis/systematics/base_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9774 2023-04-03 12:27:59.000000 quickstats-0.6.7.8/quickstats/analysis/systematics/gaussian_shape_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6796 2023-03-14 18:47:57.000000 quickstats-0.6.7.8/quickstats/analysis/systematics/normalization_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11786 2023-03-07 22:18:13.000000 quickstats-0.6.7.8/quickstats/analysis/systematics/systematics_evaluation_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/clis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.7.8/quickstats/clis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    33609 2023-03-20 15:35:32.000000 quickstats-0.6.7.8/quickstats/clis/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.7.8/quickstats/clis/inspect_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.7.8/quickstats/clis/inspect_ws.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16773 2023-02-14 22:32:02.000000 quickstats-0.6.7.8/quickstats/clis/likelihood_fit.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7818 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/clis/likelihood_scan.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/clis/limit_setting.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1327 2023-02-14 22:29:19.000000 quickstats-0.6.7.8/quickstats/clis/processor_cli.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13393 2023-04-06 15:18:32.000000 quickstats-0.6.7.8/quickstats/clis/workspace_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/components/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/components/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3084 2022-04-07 12:50:48.000000 quickstats-0.6.7.8/quickstats/components/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13927 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/components/analysis_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8656 2023-04-05 18:11:38.000000 quickstats-0.6.7.8/quickstats/components/asimov_generator.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    30254 2023-04-07 15:54:53.000000 quickstats-0.6.7.8/quickstats/components/asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2464 2023-01-04 09:02:54.000000 quickstats-0.6.7.8/quickstats/components/basics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31828 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/components/extended_minimizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    95853 2023-04-07 15:44:09.000000 quickstats-0.6.7.8/quickstats/components/extended_model.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5575 2022-08-09 03:12:09.000000 quickstats-0.6.7.8/quickstats/components/extended_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15808 2023-04-05 14:33:57.000000 quickstats-0.6.7.8/quickstats/components/likelihood.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/components/modelling/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.7.8/quickstats/components/modelling/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.7.8/quickstats/components/modelling/component_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20163 2023-03-30 14:17:36.000000 quickstats-0.6.7.8/quickstats/components/modelling/data_modelling.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.7.8/quickstats/components/modelling/model_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.7.8/quickstats/components/modelling/parameter_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5552 2023-03-27 16:00:16.000000 quickstats-0.6.7.8/quickstats/components/modelling/pdf_fit_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3541 2022-09-18 12:41:58.000000 quickstats-0.6.7.8/quickstats/components/modelling/tree_data_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10839 2022-04-07 03:18:15.000000 quickstats-0.6.7.8/quickstats/components/nuisance_parameter_harmonizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16921 2023-03-08 10:24:33.000000 quickstats-0.6.7.8/quickstats/components/nuisance_parameter_pull.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/components/processors/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.7.8/quickstats/components/processors/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1985 2022-07-21 18:30:19.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/auxiliary.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1072 2023-03-05 12:07:49.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_as_numpy.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2580 2022-08-29 07:36:48.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_base_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      710 2022-07-20 13:58:23.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_declare.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      821 2022-07-19 21:53:12.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      937 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_export.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_filter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1076 2022-08-29 06:56:49.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_global_variables.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_helper_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_hybrid_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_if_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_if_not_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_load_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_max.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_mean.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_min.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_nested_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_rdf_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_redefine.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1657 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_report.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-03-05 12:11:04.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_safe_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_safe_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2204 2022-11-10 10:03:00.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_save.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      654 2022-07-19 21:53:28.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_save_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_stat.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_sum.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_treename.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7708 2022-08-29 03:05:08.000000 quickstats-0.6.7.8/quickstats/components/processors/builtin_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6361 2022-07-21 19:15:41.000000 quickstats-0.6.7.8/quickstats/components/processors/roo_config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6267 2023-01-17 14:15:49.000000 quickstats-0.6.7.8/quickstats/components/processors/roo_processor.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5397 2021-09-16 21:06:55.000000 quickstats-0.6.7.8/quickstats/components/pvalue_toys.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3517 2022-07-20 11:52:20.000000 quickstats-0.6.7.8/quickstats/components/roo_inspector.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3107 2022-09-17 18:29:41.000000 quickstats-0.6.7.8/quickstats/components/root_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21144 2022-07-28 22:30:24.000000 quickstats-0.6.7.8/quickstats/components/toy_limit_calculator.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/components/workspaces/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      551 2023-01-13 12:37:11.000000 quickstats-0.6.7.8/quickstats/components/workspaces/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9929 2023-04-06 15:37:48.000000 quickstats-0.6.7.8/quickstats/components/workspaces/asimov_handler.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1734 2023-01-08 18:44:57.000000 quickstats-0.6.7.8/quickstats/components/workspaces/core_argument_sets.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.7.8/quickstats/components/workspaces/sample.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2023-03-11 17:09:50.000000 quickstats-0.6.7.8/quickstats/components/workspaces/settings.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8304 2023-04-06 16:51:30.000000 quickstats-0.6.7.8/quickstats/components/workspaces/systematic.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.7.8/quickstats/components/workspaces/systematics_domain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    53246 2023-01-09 16:47:15.000000 quickstats-0.6.7.8/quickstats/components/workspaces/ws_comparer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.7.8/quickstats/components/workspaces/ws_modifier_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10895 2023-03-20 15:33:53.000000 quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    87128 2023-03-20 15:19:21.000000 quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_builder_v1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    77944 2023-03-14 19:54:53.000000 quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_builder_v2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    45969 2023-01-04 17:04:30.000000 quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_combiner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    49107 2023-02-08 09:09:43.000000 quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_modifier.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/concurrent/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      228 2022-03-27 20:47:33.000000 quickstats-0.6.7.8/quickstats/concurrent/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2666 2022-09-21 07:46:09.000000 quickstats-0.6.7.8/quickstats/concurrent/abstract_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.7.8/quickstats/concurrent/logging.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5890 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/concurrent/parameterised_asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10317 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/concurrent/parameterised_likelihood.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3983 2022-09-20 17:52:34.000000 quickstats-0.6.7.8/quickstats/concurrent/parameterised_runner.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/core/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/core/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      811 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/core/abstract_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20616 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/core/configs.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/core/configurable_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/core/dataclass_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      977 2022-05-11 20:30:59.000000 quickstats-0.6.7.8/quickstats/core/decorators.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2201 2023-03-30 08:35:19.000000 quickstats-0.6.7.8/quickstats/core/enums.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2023-02-14 22:36:19.000000 quickstats-0.6.7.8/quickstats/core/methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.7.8/quickstats/core/path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.7.8/quickstats/core/virtual_trees.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/interface/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2022-01-31 04:51:23.000000 quickstats-0.6.7.8/quickstats/interface/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/interface/cppyy/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-31 03:26:35.000000 quickstats-0.6.7.8/quickstats/interface/cppyy/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.7.8/quickstats/interface/cppyy/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1032 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/interface/cppyy/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/interface/cppyy/vectorize.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/interface/root/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.7.8/quickstats/interface/root/RooAbsData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3951 2023-04-05 16:18:32.000000 quickstats-0.6.7.8/quickstats/interface/root/RooAbsPdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.7.8/quickstats/interface/root/RooArgSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2023-03-12 16:17:52.000000 quickstats-0.6.7.8/quickstats/interface/root/RooCategory.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    32809 2023-04-03 12:29:10.000000 quickstats-0.6.7.8/quickstats/interface/root/RooDataSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.7.8/quickstats/interface/root/RooMsgService.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5440 2023-03-13 14:55:24.000000 quickstats-0.6.7.8/quickstats/interface/root/RooRealVar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.7.8/quickstats/interface/root/TArrayData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.7.8/quickstats/interface/root/TF1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1995 2023-02-28 09:57:47.000000 quickstats-0.6.7.8/quickstats/interface/root/TFile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2023-03-28 23:56:03.000000 quickstats-0.6.7.8/quickstats/interface/root/TH1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5489 2022-08-23 03:10:20.000000 quickstats-0.6.7.8/quickstats/interface/root/TH2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.7.8/quickstats/interface/root/TObject.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      856 2023-03-12 13:27:02.000000 quickstats-0.6.7.8/quickstats/interface/root/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.7.8/quickstats/interface/root/helper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.7.8/quickstats/interface/root/inspection.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.7.8/quickstats/interface/root/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13697 2023-03-13 15:22:18.000000 quickstats-0.6.7.8/quickstats/interface/root/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-02-24 22:56:11.000000 quickstats-0.6.7.8/quickstats/interface/root/roofit_extension.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/macros/
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/macros/AsymptoticCLsTool/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.7.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.7.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/macros/FlexibleInterpVarMkII/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.7.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.7.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/macros/QuickStatsCore/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1231 2022-05-07 02:55:05.000000 quickstats-0.6.7.8/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.7.8/quickstats/macros/QuickStatsCore/RooFitExt.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.7.8/quickstats/macros/QuickStatsCore/RooFitExt.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/macros/ResponseFunction/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13946 2022-04-21 19:55:45.000000 quickstats-0.6.7.8/quickstats/macros/ResponseFunction/ResponseFunction.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2022-05-16 03:18:22.000000 quickstats-0.6.7.8/quickstats/macros/ResponseFunction/ResponseFunction.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/macros/RooTwoSidedCBShape/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.7.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.7.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/maths/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.7.8/quickstats/maths/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1130 2023-03-10 17:21:22.000000 quickstats-0.6.7.8/quickstats/maths/interpolation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5548 2023-03-30 08:30:53.000000 quickstats-0.6.7.8/quickstats/maths/numerics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22465 2023-04-02 17:22:53.000000 quickstats-0.6.7.8/quickstats/maths/statistics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3480 2023-03-14 15:34:34.000000 quickstats-0.6.7.8/quickstats/maths/statistics_jitted.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.7.8/quickstats/maths/symbolics.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/parsers/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.7.8/quickstats/parsers/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.7.8/quickstats/parsers/config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15568 2023-02-14 22:40:29.000000 quickstats-0.6.7.8/quickstats/parsers/param_parser.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/plots/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1441 2023-03-29 12:38:13.000000 quickstats-0.6.7.8/quickstats/plots/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12881 2023-04-03 01:58:46.000000 quickstats-0.6.7.8/quickstats/plots/abstract_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14145 2023-03-29 14:21:34.000000 quickstats-0.6.7.8/quickstats/plots/bidirectional_bar_chart.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.7.8/quickstats/plots/collective_data_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2750 2023-04-01 10:15:48.000000 quickstats-0.6.7.8/quickstats/plots/color_schemes.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5121 2023-04-02 16:46:10.000000 quickstats-0.6.7.8/quickstats/plots/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2687 2023-04-01 08:20:12.000000 quickstats-0.6.7.8/quickstats/plots/correlation_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5968 2023-03-22 14:09:34.000000 quickstats-0.6.7.8/quickstats/plots/general_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.7.8/quickstats/plots/general_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3731 2022-09-09 08:30:51.000000 quickstats-0.6.7.8/quickstats/plots/histo_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2023-03-21 16:34:42.000000 quickstats-0.6.7.8/quickstats/plots/hypotest_inverter_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5749 2023-04-06 23:36:13.000000 quickstats-0.6.7.8/quickstats/plots/likelihood_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9916 2023-04-10 17:13:17.000000 quickstats-0.6.7.8/quickstats/plots/likelihood_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.7.8/quickstats/plots/likelihood_scan_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    26322 2022-04-19 14:42:15.000000 quickstats-0.6.7.8/quickstats/plots/np_ranking_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    25242 2023-03-30 08:39:20.000000 quickstats-0.6.7.8/quickstats/plots/pdf_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.7.8/quickstats/plots/sample_purity_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10293 2023-03-27 13:06:51.000000 quickstats-0.6.7.8/quickstats/plots/score_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.7.8/quickstats/plots/stat_plot_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18642 2023-04-02 13:33:12.000000 quickstats-0.6.7.8/quickstats/plots/template.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.7.8/quickstats/plots/test_statistic_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-01-04 09:02:56.000000 quickstats-0.6.7.8/quickstats/plots/upper_limit_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11855 2023-04-07 17:48:01.000000 quickstats-0.6.7.8/quickstats/plots/upper_limit_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.7.8/quickstats/plots/upper_limit_3D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5069 2022-08-24 13:05:29.000000 quickstats-0.6.7.8/quickstats/plots/upper_limit_benchmark_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    23733 2023-04-03 02:04:48.000000 quickstats-0.6.7.8/quickstats/plots/variable_distribution_plot.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/resources/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2023-03-20 15:25:27.000000 quickstats-0.6.7.8/quickstats/resources/default_workspace_extensions.json
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.7.8/quickstats/root_checker.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/stylesheets/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.7.8/quickstats/stylesheets/quick_default.mplstyle
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats/utils/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.7.8/quickstats/utils/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10897 2023-03-07 15:00:08.000000 quickstats-0.6.7.8/quickstats/utils/common_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.7.8/quickstats/utils/condor_tasks.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16140 2023-03-25 23:04:40.000000 quickstats-0.6.7.8/quickstats/utils/data_conversion.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.7.8/quickstats/utils/hep_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3862 2023-01-06 12:43:25.000000 quickstats-0.6.7.8/quickstats/utils/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      335 2021-05-17 13:11:29.000000 quickstats-0.6.7.8/quickstats/utils/process_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    25617 2023-04-06 16:59:06.000000 quickstats-0.6.7.8/quickstats/utils/roofit_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.7.8/quickstats/utils/roostats_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12361 2023-01-04 09:02:56.000000 quickstats-0.6.7.8/quickstats/utils/root_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1225 2023-04-02 03:14:44.000000 quickstats-0.6.7.8/quickstats/utils/string_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15011 2023-03-14 18:38:57.000000 quickstats-0.6.7.8/quickstats/utils/xml_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/quickstats.egg-info/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-04-10 20:19:26.000000 quickstats-0.6.7.8/quickstats.egg-info/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8855 2023-04-10 20:19:26.000000 quickstats-0.6.7.8/quickstats.egg-info/SOURCES.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-04-10 20:19:26.000000 quickstats-0.6.7.8/quickstats.egg-info/dependency_links.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-04-10 20:19:26.000000 quickstats-0.6.7.8/quickstats.egg-info/requires.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-04-10 20:19:26.000000 quickstats-0.6.7.8/quickstats.egg-info/top_level.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-04-10 20:19:27.000000 quickstats-0.6.7.8/setup.cfg
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.7.8/setup.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:36.000000 quickstats-0.6.8.1/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-05-22 12:55:36.000000 quickstats-0.6.8.1/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/README.md
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:01.000000 quickstats-0.6.8.1/bin/
+-rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1651 2023-05-11 20:22:22.000000 quickstats-0.6.8.1/bin/quickstats
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:01.000000 quickstats-0.6.8.1/quickstats/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      626 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/quickstats/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-05-20 03:49:33.000000 quickstats-0.6.8.1/quickstats/_version.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:03.000000 quickstats-0.6.8.1/quickstats/analysis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.8.1/quickstats/analysis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.8.1/quickstats/analysis/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.8.1/quickstats/analysis/analysis_path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2023-03-14 14:12:10.000000 quickstats-0.6.8.1/quickstats/analysis/config_format_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    41649 2023-05-20 03:33:19.000000 quickstats-0.6.8.1/quickstats/analysis/data_loading.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/quickstats/analysis/data_preprocessing.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    85935 2023-05-20 03:34:59.000000 quickstats-0.6.8.1/quickstats/analysis/event_categorization.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/quickstats/analysis/multi_class_boundary_tree.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9286 2023-05-20 03:35:21.000000 quickstats-0.6.8.1/quickstats/analysis/ntuple_conversion_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31665 2023-05-20 03:35:44.000000 quickstats-0.6.8.1/quickstats/analysis/ntuple_process_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8856 2023-05-20 03:36:01.000000 quickstats-0.6.8.1/quickstats/analysis/sample_poly_param_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:04.000000 quickstats-0.6.8.1/quickstats/analysis/systematics/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2023-03-07 22:17:53.000000 quickstats-0.6.8.1/quickstats/analysis/systematics/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29550 2023-05-20 03:37:08.000000 quickstats-0.6.8.1/quickstats/analysis/systematics/base_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9774 2023-04-03 12:27:59.000000 quickstats-0.6.8.1/quickstats/analysis/systematics/gaussian_shape_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6796 2023-03-14 18:47:57.000000 quickstats-0.6.8.1/quickstats/analysis/systematics/normalization_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11815 2023-05-20 03:31:54.000000 quickstats-0.6.8.1/quickstats/analysis/systematics/systematics_evaluation_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:06.000000 quickstats-0.6.8.1/quickstats/clis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.8.1/quickstats/clis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    33847 2023-04-21 13:37:08.000000 quickstats-0.6.8.1/quickstats/clis/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.8.1/quickstats/clis/inspect_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.8.1/quickstats/clis/inspect_ws.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16785 2023-05-03 13:28:30.000000 quickstats-0.6.8.1/quickstats/clis/likelihood_fit.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7818 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/quickstats/clis/likelihood_scan.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/quickstats/clis/limit_setting.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1327 2023-02-14 22:29:19.000000 quickstats-0.6.8.1/quickstats/clis/processor_cli.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15178 2023-05-11 20:21:35.000000 quickstats-0.6.8.1/quickstats/clis/workspace_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:09.000000 quickstats-0.6.8.1/quickstats/components/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/quickstats/components/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3152 2023-05-21 14:45:07.000000 quickstats-0.6.8.1/quickstats/components/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13082 2023-05-21 14:42:47.000000 quickstats-0.6.8.1/quickstats/components/analysis_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8656 2023-04-05 18:11:38.000000 quickstats-0.6.8.1/quickstats/components/asimov_generator.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    30804 2023-05-20 02:55:29.000000 quickstats-0.6.8.1/quickstats/components/asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2464 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/quickstats/components/basics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31924 2023-05-20 02:58:35.000000 quickstats-0.6.8.1/quickstats/components/extended_minimizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    97245 2023-05-20 03:03:07.000000 quickstats-0.6.8.1/quickstats/components/extended_model.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5539 2023-05-20 03:03:29.000000 quickstats-0.6.8.1/quickstats/components/extended_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15647 2023-05-20 13:23:46.000000 quickstats-0.6.8.1/quickstats/components/likelihood.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:10.000000 quickstats-0.6.8.1/quickstats/components/modelling/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.8.1/quickstats/components/modelling/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.8.1/quickstats/components/modelling/component_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20157 2023-05-20 03:06:27.000000 quickstats-0.6.8.1/quickstats/components/modelling/data_modelling.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.8.1/quickstats/components/modelling/model_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.8.1/quickstats/components/modelling/parameter_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-05-20 03:07:18.000000 quickstats-0.6.8.1/quickstats/components/modelling/pdf_fit_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3532 2023-05-20 03:07:28.000000 quickstats-0.6.8.1/quickstats/components/modelling/tree_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10839 2022-04-07 03:18:15.000000 quickstats-0.6.8.1/quickstats/components/nuisance_parameter_harmonizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16921 2023-03-08 10:24:33.000000 quickstats-0.6.8.1/quickstats/components/nuisance_parameter_pull.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:11.000000 quickstats-0.6.8.1/quickstats/components/processors/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.8.1/quickstats/components/processors/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:15.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2066 2023-05-19 15:52:58.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/auxiliary.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1072 2023-03-05 12:07:49.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_as_numpy.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2660 2023-05-21 22:51:18.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_base_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-05-21 22:53:11.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_declare.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      821 2023-05-21 21:47:11.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      937 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_export.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_filter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1076 2022-08-29 06:56:49.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_global_variables.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_helper_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_hybrid_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_if_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_if_not_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_load_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1121 2023-05-21 22:55:55.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_load_macro.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_max.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_mean.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_min.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_nested_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_rdf_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_redefine.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1657 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_report.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-03-05 12:11:04.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_safe_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_safe_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2204 2022-11-10 10:03:00.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_save.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      654 2022-07-19 21:53:28.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_save_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_stat.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_sum.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_treename.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8316 2023-05-21 20:31:48.000000 quickstats-0.6.8.1/quickstats/components/processors/builtin_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6504 2023-05-21 22:51:45.000000 quickstats-0.6.8.1/quickstats/components/processors/roo_config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6646 2023-05-20 03:08:06.000000 quickstats-0.6.8.1/quickstats/components/processors/roo_processor.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5397 2021-09-16 21:06:55.000000 quickstats-0.6.8.1/quickstats/components/pvalue_toys.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3519 2023-05-20 03:04:57.000000 quickstats-0.6.8.1/quickstats/components/roo_inspector.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3083 2023-05-20 03:04:47.000000 quickstats-0.6.8.1/quickstats/components/root_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21336 2023-05-20 03:06:10.000000 quickstats-0.6.8.1/quickstats/components/toy_limit_calculator.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:19.000000 quickstats-0.6.8.1/quickstats/components/workspaces/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2023-05-11 12:58:08.000000 quickstats-0.6.8.1/quickstats/components/workspaces/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2023-05-20 03:10:01.000000 quickstats-0.6.8.1/quickstats/components/workspaces/asimov_handler.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2023-05-20 03:10:09.000000 quickstats-0.6.8.1/quickstats/components/workspaces/core_argument_sets.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.8.1/quickstats/components/workspaces/sample.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2023-03-11 17:09:50.000000 quickstats-0.6.8.1/quickstats/components/workspaces/settings.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8295 2023-05-20 03:10:27.000000 quickstats-0.6.8.1/quickstats/components/workspaces/systematic.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.8.1/quickstats/components/workspaces/systematics_domain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    53138 2023-05-20 03:11:16.000000 quickstats-0.6.8.1/quickstats/components/workspaces/ws_comparer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8837 2023-05-20 03:11:35.000000 quickstats-0.6.8.1/quickstats/components/workspaces/ws_decomposer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.8.1/quickstats/components/workspaces/ws_modifier_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10859 2023-05-20 03:12:06.000000 quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    87030 2023-05-20 03:16:06.000000 quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_builder_v1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    76213 2023-05-20 03:19:36.000000 quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_builder_v2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    45866 2023-05-20 03:21:08.000000 quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_combiner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    48960 2023-05-20 03:23:15.000000 quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_modifier.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:20.000000 quickstats-0.6.8.1/quickstats/concurrent/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      228 2022-03-27 20:47:33.000000 quickstats-0.6.8.1/quickstats/concurrent/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2654 2023-05-20 03:24:10.000000 quickstats-0.6.8.1/quickstats/concurrent/abstract_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.8.1/quickstats/concurrent/logging.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5884 2023-05-20 03:24:25.000000 quickstats-0.6.8.1/quickstats/concurrent/parameterised_asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10316 2023-05-20 03:24:47.000000 quickstats-0.6.8.1/quickstats/concurrent/parameterised_likelihood.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3983 2022-09-20 17:52:34.000000 quickstats-0.6.8.1/quickstats/concurrent/parameterised_runner.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:22.000000 quickstats-0.6.8.1/quickstats/core/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/core/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      811 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/core/abstract_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20587 2023-05-20 03:28:17.000000 quickstats-0.6.8.1/quickstats/core/configs.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/core/configurable_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/core/dataclass_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      971 2023-05-20 03:27:42.000000 quickstats-0.6.8.1/quickstats/core/decorators.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2201 2023-03-30 08:35:19.000000 quickstats-0.6.8.1/quickstats/core/enums.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2023-02-14 22:36:19.000000 quickstats-0.6.8.1/quickstats/core/methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.8.1/quickstats/core/path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.8.1/quickstats/core/virtual_trees.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:22.000000 quickstats-0.6.8.1/quickstats/interface/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2022-01-31 04:51:23.000000 quickstats-0.6.8.1/quickstats/interface/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:22.000000 quickstats-0.6.8.1/quickstats/interface/cppyy/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-31 03:26:35.000000 quickstats-0.6.8.1/quickstats/interface/cppyy/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.8.1/quickstats/interface/cppyy/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12040 2023-05-21 22:08:49.000000 quickstats-0.6.8.1/quickstats/interface/cppyy/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/interface/cppyy/vectorize.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:25.000000 quickstats-0.6.8.1/quickstats/interface/root/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.8.1/quickstats/interface/root/RooAbsData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9855 2023-05-20 12:12:25.000000 quickstats-0.6.8.1/quickstats/interface/root/RooAbsPdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.8.1/quickstats/interface/root/RooArgSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2023-03-12 16:17:52.000000 quickstats-0.6.8.1/quickstats/interface/root/RooCategory.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    44679 2023-05-20 12:08:58.000000 quickstats-0.6.8.1/quickstats/interface/root/RooDataSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.8.1/quickstats/interface/root/RooMsgService.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5451 2023-05-11 15:17:32.000000 quickstats-0.6.8.1/quickstats/interface/root/RooRealVar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.8.1/quickstats/interface/root/TArrayData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/interface/root/TF1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1995 2023-02-28 09:57:47.000000 quickstats-0.6.8.1/quickstats/interface/root/TFile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2023-05-20 12:06:46.000000 quickstats-0.6.8.1/quickstats/interface/root/TH1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5707 2023-05-03 13:36:36.000000 quickstats-0.6.8.1/quickstats/interface/root/TH2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.8.1/quickstats/interface/root/TObject.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      856 2023-03-12 13:27:02.000000 quickstats-0.6.8.1/quickstats/interface/root/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.8.1/quickstats/interface/root/helper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.8.1/quickstats/interface/root/inspection.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.8.1/quickstats/interface/root/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19576 2023-05-11 13:39:17.000000 quickstats-0.6.8.1/quickstats/interface/root/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-02-24 22:56:11.000000 quickstats-0.6.8.1/quickstats/interface/root/roofit_extension.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:01.000000 quickstats-0.6.8.1/quickstats/macros/
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:25.000000 quickstats-0.6.8.1/quickstats/macros/AsymptoticCLsTool/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.8.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.8.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:25.000000 quickstats-0.6.8.1/quickstats/macros/FlexibleInterpVarMkII/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.8.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.8.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:26.000000 quickstats-0.6.8.1/quickstats/macros/QuickStatsCore/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1231 2022-05-07 02:55:05.000000 quickstats-0.6.8.1/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.8.1/quickstats/macros/QuickStatsCore/RooFitExt.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.8.1/quickstats/macros/QuickStatsCore/RooFitExt.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:26.000000 quickstats-0.6.8.1/quickstats/macros/ResponseFunction/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13755 2023-04-25 19:09:18.000000 quickstats-0.6.8.1/quickstats/macros/ResponseFunction/ResponseFunction.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.6.8.1/quickstats/macros/ResponseFunction/ResponseFunction.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:26.000000 quickstats-0.6.8.1/quickstats/macros/RooTwoSidedCBShape/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.8.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.8.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:27.000000 quickstats-0.6.8.1/quickstats/maths/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.8.1/quickstats/maths/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1130 2023-03-10 17:21:22.000000 quickstats-0.6.8.1/quickstats/maths/interpolation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5548 2023-03-30 08:30:53.000000 quickstats-0.6.8.1/quickstats/maths/numerics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    24166 2023-05-20 11:38:14.000000 quickstats-0.6.8.1/quickstats/maths/statistics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2023-05-15 01:04:06.000000 quickstats-0.6.8.1/quickstats/maths/statistics_jitted.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.8.1/quickstats/maths/symbolics.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:27.000000 quickstats-0.6.8.1/quickstats/parsers/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.8.1/quickstats/parsers/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.8.1/quickstats/parsers/config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15875 2023-04-11 14:45:10.000000 quickstats-0.6.8.1/quickstats/parsers/param_parser.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:33.000000 quickstats-0.6.8.1/quickstats/plots/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1441 2023-03-29 12:38:13.000000 quickstats-0.6.8.1/quickstats/plots/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12818 2023-04-27 22:46:00.000000 quickstats-0.6.8.1/quickstats/plots/abstract_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14145 2023-03-29 14:21:34.000000 quickstats-0.6.8.1/quickstats/plots/bidirectional_bar_chart.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.8.1/quickstats/plots/collective_data_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2750 2023-04-01 10:15:48.000000 quickstats-0.6.8.1/quickstats/plots/color_schemes.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5180 2023-05-17 15:59:58.000000 quickstats-0.6.8.1/quickstats/plots/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4007 2023-05-17 16:00:48.000000 quickstats-0.6.8.1/quickstats/plots/correlation_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5968 2023-03-22 14:09:34.000000 quickstats-0.6.8.1/quickstats/plots/general_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.8.1/quickstats/plots/general_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3731 2022-09-09 08:30:51.000000 quickstats-0.6.8.1/quickstats/plots/histo_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2023-03-21 16:34:42.000000 quickstats-0.6.8.1/quickstats/plots/hypotest_inverter_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5749 2023-04-06 23:36:13.000000 quickstats-0.6.8.1/quickstats/plots/likelihood_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9916 2023-04-10 17:13:17.000000 quickstats-0.6.8.1/quickstats/plots/likelihood_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.8.1/quickstats/plots/likelihood_scan_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    26316 2023-04-17 19:54:51.000000 quickstats-0.6.8.1/quickstats/plots/np_ranking_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25696 2023-04-18 01:26:39.000000 quickstats-0.6.8.1/quickstats/plots/pdf_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.8.1/quickstats/plots/sample_purity_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10293 2023-03-27 13:06:51.000000 quickstats-0.6.8.1/quickstats/plots/score_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.8.1/quickstats/plots/stat_plot_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18642 2023-04-02 13:33:12.000000 quickstats-0.6.8.1/quickstats/plots/template.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.8.1/quickstats/plots/test_statistic_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-01-04 09:02:56.000000 quickstats-0.6.8.1/quickstats/plots/upper_limit_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2023-04-14 12:19:16.000000 quickstats-0.6.8.1/quickstats/plots/upper_limit_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.8.1/quickstats/plots/upper_limit_3D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5069 2022-08-24 13:05:29.000000 quickstats-0.6.8.1/quickstats/plots/upper_limit_benchmark_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    28679 2023-05-20 03:29:27.000000 quickstats-0.6.8.1/quickstats/plots/variable_distribution_plot.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:34.000000 quickstats-0.6.8.1/quickstats/resources/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2023-03-20 15:25:27.000000 quickstats-0.6.8.1/quickstats/resources/default_workspace_extensions.json
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.8.1/quickstats/root_checker.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:34.000000 quickstats-0.6.8.1/quickstats/stylesheets/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.8.1/quickstats/stylesheets/quick_default.mplstyle
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:36.000000 quickstats-0.6.8.1/quickstats/utils/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.8.1/quickstats/utils/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10897 2023-03-07 15:00:08.000000 quickstats-0.6.8.1/quickstats/utils/common_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.8.1/quickstats/utils/condor_tasks.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16140 2023-03-25 23:04:40.000000 quickstats-0.6.8.1/quickstats/utils/data_conversion.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.8.1/quickstats/utils/hep_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6634 2023-05-20 02:56:51.000000 quickstats-0.6.8.1/quickstats/utils/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      335 2021-05-17 13:11:29.000000 quickstats-0.6.8.1/quickstats/utils/process_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    26227 2023-05-20 21:07:10.000000 quickstats-0.6.8.1/quickstats/utils/roofit_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.8.1/quickstats/utils/roostats_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12379 2023-05-20 03:26:53.000000 quickstats-0.6.8.1/quickstats/utils/root_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1347 2023-05-21 21:45:53.000000 quickstats-0.6.8.1/quickstats/utils/string_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15011 2023-03-14 18:38:57.000000 quickstats-0.6.8.1/quickstats/utils/xml_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:02.000000 quickstats-0.6.8.1/quickstats.egg-info/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-05-22 12:54:53.000000 quickstats-0.6.8.1/quickstats.egg-info/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8968 2023-05-22 12:54:54.000000 quickstats-0.6.8.1/quickstats.egg-info/SOURCES.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-05-22 12:54:53.000000 quickstats-0.6.8.1/quickstats.egg-info/dependency_links.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-05-22 12:54:53.000000 quickstats-0.6.8.1/quickstats.egg-info/requires.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-05-22 12:54:53.000000 quickstats-0.6.8.1/quickstats.egg-info/top_level.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-05-22 12:55:36.000000 quickstats-0.6.8.1/setup.cfg
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.8.1/setup.py
```

### Comparing `quickstats-0.6.7.8/PKG-INFO` & `quickstats-0.6.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.7.8
+Version: 0.6.8.1
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.7.8/README.md` & `quickstats-0.6.8.1/README.md`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/bin/quickstats` & `quickstats-0.6.8.1/bin/quickstats`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
                                   toy_limit, add_macro, remove_macro)
 from quickstats.clis.inspect_ws import inspect_ws
 from quickstats.clis.inspect_rfile import inspect_rfile
 from quickstats.clis.limit_setting import limit_scan
 from quickstats.clis.processor_cli import process_rfile
 from quickstats.clis.likelihood_scan import likelihood_scan
 from quickstats.clis.likelihood_fit import likelihood_fit, np_correlation
-from quickstats.clis.workspace_tools import build_xml_ws, modify_ws, compare_ws, combine_ws
+from quickstats.clis.workspace_tools import build_xml_ws, modify_ws, compare_ws, combine_ws, decompose_ws
 
 @click.group()
 def cli():
     pass
 
 if __name__ == "__main__":
     cli.add_command(compile_macros)
@@ -36,8 +36,9 @@
     cli.add_command(generate_standard_asimov)
     cli.add_command(inspect_rfile)
     cli.add_command(process_rfile)
     cli.add_command(build_xml_ws)
     cli.add_command(modify_ws)
     cli.add_command(compare_ws)
     cli.add_command(combine_ws)
+    cli.add_command(decompose_ws)
     cli()
```

### Comparing `quickstats-0.6.7.8/quickstats/__init__.py` & `quickstats-0.6.8.1/quickstats/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/analysis/analysis_base.py` & `quickstats-0.6.8.1/quickstats/analysis/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/analysis/analysis_path_manager.py` & `quickstats-0.6.8.1/quickstats/analysis/analysis_path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/analysis/config_format_templates.py` & `quickstats-0.6.8.1/quickstats/analysis/config_format_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/analysis/data_loading.py` & `quickstats-0.6.8.1/quickstats/analysis/data_loading.py`

 * *Files 5% similar despite different names*

```diff
@@ -187,18 +187,18 @@
     def train_val_test_split(self, analysis_datasets:Dict,
                              data_transformer:DataTransformer,
                              **kwargs):
         
         n_splits     = self.config["n_splits"]
         random_state = self.config["random_state"]
         
-        self.stdout.info("INFO: Data will be split using the KFold method.")
-        self.stdout.info(f"   Analysis datasets used: {self.get_analysis_dataset_names()}")
-        self.stdout.info(f"         Number of splits: {n_splits}")
-        self.stdout.info(f"       KFold random state: {random_state}")
+        self.stdout.info("Data will be split using the KFold method.")
+        self.stdout.info(f"   Analysis datasets used: {self.get_analysis_dataset_names()}", bare=True)
+        self.stdout.info(f"         Number of splits: {n_splits}", bare=True)
+        self.stdout.info(f"       KFold random state: {random_state}", bare=True)
         
         from sklearn.model_selection import KFold
         
         index_variable = self.config.get("index_variable", None)
         kfolds = {}
         kfold_splits = {}
         combined_dataset = self.combine_analysis_datasets(list(analysis_datasets.values()))
@@ -265,18 +265,18 @@
     def get_analysis_dataset_names(self) -> List[str]:
         dataset_map = self.get_train_val_test_map()
         dataset_names = list(chain.from_iterable(dataset_map.values()))
         return dataset_names
     
     def train_val_test_split(self, analysis_datasets:Dict, data_transformer:DataTransformer):
         dataset_map = self.get_train_val_test_map()
-        self.stdout.info("INFO: Data will be split using custom analysis datasets.")
-        self.stdout.info(f'        Train dataset: {dataset_map["train"]}')
-        self.stdout.info(f'   Validation dataset: {dataset_map.get("val", None)}')
-        self.stdout.info(f'         Test dataset: {dataset_map.get("test", None)}')
+        self.stdout.info("Data will be split using custom analysis datasets.")
+        self.stdout.info(f'        Train dataset: {dataset_map["train"]}', bare=True)
+        self.stdout.info(f'   Validation dataset: {dataset_map.get("val", None)}', bare=True)
+        self.stdout.info(f'         Test dataset: {dataset_map.get("test", None)}', bare=True)
         result = {}
         for dataset_type, dataset_names in dataset_map.items():
             selected_datasets = [analysis_datasets[dataset_name] for dataset_name in dataset_names]
             combined_dataset = self.combine_analysis_datasets(selected_datasets)
             result.update(self.get_dataset_split(data_transformer, dataset_type, combined_dataset))
         return result
     
@@ -315,16 +315,16 @@
         if "test" in self.config["indices"]:
             split_indices["test"] = self.config["indices"]["test"]
         return split_indices
     
     def train_val_test_split(self, analysis_datasets:Dict, data_transformer:DataTransformer):
         
         index_variable = self.config["index_variable"]
-        self.stdout.info("INFO: Data will be split using custom event indices.")
-        self.stdout.info(f"       Index variable: {index_variable}")
+        self.stdout.info("Data will be split using custom event indices.")
+        self.stdout.info(f"       Index variable: {index_variable}", bare=True)
         
         analysis_dataset = analysis_datasets[None]
         concat_kwargs = {
             "axis": 1,
             "sort": False,
             "copy": False
         }
@@ -389,15 +389,15 @@
         return None
     
     def get_extra_variables(self):
         return self.config.get("extra_variables", [])
     
     def train_val_test_split(self, analysis_datasets:Dict, data_transformer:DataTransformer):
         
-        self.stdout.info("INFO: Data will be split using a user-defined function.")
+        self.stdout.info("Data will be split using a user-defined function.")
         
         split_func = self.config["split_func"]
         extra_variables = self.config.get("extra_variables", [])
         analysis_dataset = self.combine_analysis_datasets(list(analysis_datasets.values()))
         splitted_dataset = {}
         for sample, sample_dataset in analysis_dataset.items():
             x, y, weight = sample_dataset["x"], sample_dataset["y"], sample_dataset["weight"]
@@ -461,18 +461,18 @@
                           lumi_scale:Optional[float]=None):
         if (sample_scales is not None):
             self.sample_weight_scales = combine_dict(sample_scales)
         else:
             self.sample_weight_scales = None
         self.lumi_weight_scale = lumi_scale
         if self.lumi_weight_scale is not None:
-            self.stdout.info(f'INFO: Set luminosity weight scale to {self.lumi_weight_scale}')
+            self.stdout.info(f'Set luminosity weight scale to {self.lumi_weight_scale}')
         if self.sample_weight_scales is not None:
             for sample, scale_factor in self.sample_weight_scales.items():
-                self.stdout.info(f'INFO: Set event weight scale for the sample "{sample}" to {scale_factor}')
+                self.stdout.info(f'Set event weight scale for the sample "{sample}" to {scale_factor}')
 
     def set_data_transformer(self, data_transformer:Optional[DataTransformer]=None):
         if data_transformer is None:
             train_config = self.config["training"]
             sample_transformation  = train_config.get("sample_transformation", {})
             dataset_transformation = train_config.get("dataset_transformation", {})
             data_transformer = DataTransformer(sample_transformation=sample_transformation,
@@ -559,15 +559,15 @@
                                         subdirectory=kinematic_region,
                                         sample=sample,
                                         fmt=self.data_format)
         else:
             sample_path = self.get_file("train_sample",
                                         sample=sample,
                                         fmt=self.data_format)
-        self.stdout.info(f'INFO: Loading inputs for the sample "{sample}" from "{sample_path}"')
+        self.stdout.info(f'Loading inputs for the sample "{sample}" from "{sample_path}"')
         df = self._read_data_from_file(sample_path, key=key, columns=columns, selection=selection)
         if self.lumi_weight_scale is not None:
             if self.weight_variable is None:
                 raise RuntimeError("cannot apply luminosity weight scale: weight variable not set")
             df[self.weight_variable] = df[self.weight_variable] * self.lumi_weight_scale
         if self.sample_weight_scales is not None:
             if self.weight_variable is None:
@@ -734,15 +734,15 @@
             "class_label_map"        : class_label_map,
             "weight_variable"        : self.weight_variable,
             "selection"              : channel_config.get('selection', None),
             "selection_variables"    : channel_config.get('selection_variables', None),
             "kinematic_region"       : channel_config.get('kinematic_region', None),
             "split_algo"             : split_algo
         }
-        self.stdout.info(f"INFO: Loading data for the channel: {channel}")
+        self.stdout.info(f"Loading data for the channel: {channel}")
         return self.load_train_data(**kwargs)
         
     def print_channel_summary(self, channels:Optional[Union[List[str],str]]=None):
         if channels is None:
             channels = self.all_channels
         elif isinstance(channels, str):
             channels = [channels]
@@ -754,30 +754,30 @@
             test_samples = self.config['channels'][channel]['test_samples']
             train_variables = self.config['channels'][channel]['train_variables']
             class_labels = self.config['channels'][channel]['class_labels']
             train_samples = self.resolve_samples(train_samples)
             test_samples = self.resolve_samples(test_samples)
             train_variables = self.resolve_variables(train_variables)
             scale_factors = self.config['channels'][channel]['SF']
-            self.stdout.info("=============================== CHANNEL SUMMARY ===============================")
-            self.stdout.info("Channel Name: ".rjust(20) + f"{channel}")
-            self.stdout.info("Channel Selection: ".rjust(20) + f"{selection}")
-            self.stdout.info("*******************************************************************************")
-            self.stdout.info("Train Samples: ".rjust(20) + ", ".join(train_samples))
-            self.stdout.info("Test Samples: ".rjust(20) + ", ".join(test_samples))
-            self.stdout.info("*******************************************************************************")
-            self.stdout.info("Class Labels: ".rjust(20))
+            self.stdout.info("=============================== CHANNEL SUMMARY ===============================", bare=True)
+            self.stdout.info("Channel Name: ".rjust(20) + f"{channel}", bare=True)
+            self.stdout.info("Channel Selection: ".rjust(20) + f"{selection}", bare=True)
+            self.stdout.info("*******************************************************************************", bare=True)
+            self.stdout.info("Train Samples: ".rjust(20) + ", ".join(train_samples), bare=True)
+            self.stdout.info("Test Samples: ".rjust(20) + ", ".join(test_samples), bare=True)
+            self.stdout.info("*******************************************************************************", bare=True)
+            self.stdout.info("Class Labels: ".rjust(20), bare=True)
             for label in class_labels:
                 samples = self.resolve_samples(class_labels[label])
-                self.stdout.info(f"\t{label}: " + ", ".join(samples))
-            self.stdout.info("*******************************************************************************")
+                self.stdout.info(f"\t{label}: " + ", ".join(samples), bare=True)
+            self.stdout.info("*******************************************************************************", bare=True)
             self.stdout.info("Train Variables: ".rjust(20) + ", ".join(train_variables))
-            self.stdout.info("*******************************************************************************")
+            self.stdout.info("*******************************************************************************", bare=True)
             self.stdout.info("Scale Factors: ".rjust(20) + str(scale_factors))
-            self.stdout.info("*******************************************************************************")
+            self.stdout.info("*******************************************************************************", bare=True)
             self.stdout.info("")
             
             
 def index_modularity_split(index_variable:str, modulo:int,
                            train_remainders:List[int],
                            val_remainders:Optional[List[int]]=None,
                            test_remainders:Optional[List[int]]=None):
```

### Comparing `quickstats-0.6.7.8/quickstats/analysis/data_preprocessing.py` & `quickstats-0.6.8.1/quickstats/analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/analysis/event_categorization.py` & `quickstats-0.6.8.1/quickstats/analysis/event_categorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,29 +184,29 @@
         target_channels: list of string
             Channels to perform the initialization.
         """
         
         bc_ds = self.config["categorization"]["boundary_scan"].get("datasets", None)
         eval_ds = self.config["categorization"]["evaluation"].get("datasets", None)
         if bc_ds is not None:
-            self.stdout.info("INFO: Boundary scan will be performed on the following analysis "
+            self.stdout.info("Boundary scan will be performed on the following analysis "
                             f"dataset(s): {', '.join(bc_ds)}")
         else:
-            self.stdout.info("INFO: Boundary scan will be performed on the full analysis dataset.")
+            self.stdout.info("Boundary scan will be performed on the full analysis dataset.")
         if eval_ds is not None:
-            self.stdout.info("INFO: Statistical evaluation will be performed on the following analysis "
+            self.stdout.info("Statistical evaluation will be performed on the following analysis "
                             f"dataset(s): {', '.join(eval_ds)}")
         else:
-            self.stdout.info("INFO: Statistical evaluation will be performed on the full analysis dataset.")
+            self.stdout.info("Statistical evaluation will be performed on the full analysis dataset.")
             
         self.target_channels = self.resolve_channels(target_channels)
         channel_configs  = {}
         channel_metadata = {}
         for channel in self.target_channels:
-            self.stdout.info(f'INFO: Initializing configuration for the channel "{channel}"')
+            self.stdout.info(f'Initializing configuration for the channel "{channel}"')
             channel_config  = self.config['channels'][channel]
             train_variables = self.resolve_variables(channel_config['train_variables'])
             train_samples   = self.resolve_train_samples(channel)
             test_samples    = self.resolve_samples(channel_config['test_samples'])
             num_class = len(channel_config["class_labels"])
             # check that class labels are valid
             if num_class == 2:
@@ -714,15 +714,15 @@
         if apply_score:
             self.validate(check_model=True)
         else:
             self.validate(check_model=False)
         channel = self.active_channel
         channel_selection = self.channel_config['selection']
         kinematic_region  = self.channel_config['kinematic_region']
-        self.stdout.info(f"INFO: Loading inputs for the channel: {channel}")
+        self.stdout.info(f"Loading inputs for the channel: {channel}")
         if samples is None:
             samples = self.get_samples_to_load()
             
         channel_df = {}
         for sample in samples:
             sample_df = self.get_sample_df(sample, columns=None,
                                            selection=channel_selection,
@@ -862,47 +862,47 @@
         background_hists = class_score_hist['background']
         if (n_bins != len(signal_hists)) or (n_bins != len(background_hists)):
             raise RuntimeError("number of bins requested must match the number of bins in the class score "
                                "histograms")
         with Timer() as t:
             boundary_indices  = self.get_boundary_indices(n_bins, n_boundaries)
             n_combinations = len(boundary_indices)
-            self.stdout.info(f"INFO: Total number of boundary combinations: {n_combinations}")
+            self.stdout.info(f"Total number of boundary combinations: {n_combinations}")
             signal_yields     = self.get_region_yields(signal_hists, boundary_indices, filter_regions=filter_regions)
             background_yields = self.get_region_yields(background_hists, boundary_indices, filter_regions=filter_regions)
             # filter boundaries which the regions contain no signal or background yields
             valid_boundaries = np.all(background_yields != 0., axis=1) & np.all(signal_yields != 0., axis=1)
             # filter boundaries which the regions contain less than the minimum required yields for specific
             # samples such as the yy background
             if minimum_yields is not None:
                 for sample in minimum_yields:
                     if sample not in all_hists:
                         raise RuntimeError(f"the sample {sample} is not used in testing")
                     min_yield = minimum_yields[sample]
                     sample_yields = self.get_region_yields(all_hists[sample], boundary_indices, filter_regions=filter_regions)
                     valid_boundaries &= np.all(sample_yields > min_yield, axis=1)
-            self.stdout.info(f"INFO: Number of valid boundary combinations: {valid_boundaries.sum()}")
+            self.stdout.info(f"Number of valid boundary combinations: {valid_boundaries.sum()}")
             if valid_boundaries.sum() == 0:
-                self.stdout.info("INFO: Not enough combinations to scan due to minimum yield requirements. "
+                self.stdout.info("Not enough combinations to scan due to minimum yield requirements. "
                                  "No boundaries are set.")
                 return None
             combined_significances = get_combined_counting_significance(signal_yields[valid_boundaries],
                                                                         background_yields[valid_boundaries])
             bins = np.arange(0, 1, 1 / n_bins)
             max_boundary_idx = np.argmax(combined_significances)
             max_significance = combined_significances[max_boundary_idx]
             min_boundary_idx = np.argmin(combined_significances)
             min_significance = combined_significances[min_boundary_idx]
             if ((max_significance - min_significance) / min_significance) < 0.1:
-                self.stdout.info("INFO: Improvement in Z is less than 10%. "
+                self.stdout.info("Improvement in Z is less than 10%. "
                                  "No boundaries are set.")
                 return None
             max_bins         = boundary_indices[valid_boundaries][max_boundary_idx]
             max_boundary     = [bins[i] for i in max_bins]
-        self.stdout.info(f"INFO: Boundary scan finished. Total time taken: {t.interval:.3f}s")
+        self.stdout.info(f"Boundary scan finished. Total time taken: {t.interval:.3f}s")
         result = {
             'boundaries'  : [round(v, 8) for v in max_boundary],
             'significance': max_significance 
         }
         return result
     
     def load_boundaries(self, filename:Optional[str]=None,
@@ -919,15 +919,15 @@
             If None, the current channel is used.
         """
         channel = self._parse_channel(channel)
         if filename is None:
             filename = self.get_file("boundary_data", channel=channel)
         if not os.path.exists(filename):
             raise FileNotFoundError(f'boundary output "{filename}" does not exist')
-        self.stdout.info(f'INFO: Cached boundary output for the channel {channel} from "{filename}"')
+        self.stdout.info(f'Cached boundary output for the channel {channel} from "{filename}"')
         boundary_tree = MultiClassBoundaryTree(score_base_name=self.names["score"])
         boundary_tree.load_tree(filename)
         self.boundary_trees[channel] = boundary_tree
         self.update_valid_categories(channel)
         self.update_summary(channel)
         return boundary_tree
                 
@@ -954,15 +954,15 @@
             elif self._has_file("boundary_data", channel=channel):
                 filename = self.get_file("boundary_data", channel=channel)
                 self.load_boundaries(filename)
                 return None
             
         exclude_categories = channel_config["exclude_categories"]
         
-        self.stdout.info("INFO: Scanning score boundaries...")
+        self.stdout.info("Scanning score boundaries...")
         # run over class
         class_labels = self.get_class_labels()
         class_metadata = self.channel_metadata[channel]["classes"]
         for depth, class_label in enumerate(class_labels):
             class_config = class_metadata[class_label]['counting_significance']
             cut_maps = boundary_tree.get_cut_maps()
             # run over preceding class regions
@@ -975,28 +975,28 @@
                                           if category[:depth] == list(branch_index)]
                 else:
                     filter_regions = None
                 # multi-class case
                 if class_label:
                     if branch_index is not None:
                         preceding_category_label = self.get_category_label(branch_index)
-                        self.stdout.info(f"Class Name: {class_label} (region = {preceding_category_label})")
+                        self.stdout.info(f"Class Name: {class_label} (region = {preceding_category_label})", bare=True)
                     else:
-                        self.stdout.info(f"Class Name: {class_label}")
+                        self.stdout.info(f"Class Name: {class_label}", bare=True)
                 class_score_hist = self.get_class_score_hist(class_label, cut_expr)
                 result = self.scan_class_bounds(class_score_hist,
                                                 class_config['n_bins'],
                                                 class_config['n_boundaries'],
                                                 class_config['min_yield'],
                                                 filter_regions=filter_regions)
                 if result is not None:
                     # append the new boundaries to the preceding branch
                     boundary_tree.set_boundaries(class_label, **result, branch_index=branch_index)
-                    self.stdout.info("\t boundaries: {}".format(result['boundaries']))
-                    self.stdout.info("\t counting significance: {}".format(result['significance']))
+                    self.stdout.info("\t boundaries: {}".format(result['boundaries']), bare=True)
+                    self.stdout.info("\t counting significance: {}".format(result['significance']), bare=True)
         self.boundary_trees[channel] = boundary_tree
         self.update_valid_categories()
         self.update_summary()
     
     def update_valid_categories(self, channel:Optional[str]=None,
                                 ignore_boundary_result:bool=False):
         """
@@ -1108,15 +1108,15 @@
                     yields_err[category_name][key] = {"errlo": err_val, "errhi": err_val}
         return yields, yields_err
     
     def update_category_yields(self):
         """
         Update category yields for the test samples in the current channel after category labels are applied.
         """        
-        self.stdout.info(f"INFO: Evaluating sample yields")
+        self.stdout.info(f"Evaluating sample yields")
         yields, yields_err = self.get_category_yields()
         channel = self.active_channel
         self.category_yields[channel]     = yields
         self.category_yields_err[channel] = yields_err
         
     def apply_category(self, df:pd.DataFrame):
         """
@@ -1239,15 +1239,15 @@
         if resampling:
             df = self.get_resampled_df(df, random_state=resampling_random_state)
         if columns is not None:
             available_columns = list(df.columns)
             valid_columns = [c for c in columns if c in available_columns]
             missing_columns = [c for c in columns if c not in available_columns]
             if len(missing_columns) > 0:
-                self.stdout.debug(f'DEBUG: Found missing columns in the datafarme: {", ".join(missing_columns)}')
+                self.stdout.debug(f'Found missing columns in the datafarme: {", ".join(missing_columns)}')
             df = df[valid_columns]
         return df
     
     def get_resampled_df(self, df:pd.DataFrame,
                          random_state:Optional[int]=None):
         """
         Return dataframe with resampled events (for bootstrapping).
@@ -1285,15 +1285,15 @@
             category_df = self.get_category_df(sample, category_or_index)
             yields += category_df[weight_name].sum()
         return yields
     
     def evaluate_benchmark_significance(self):
         self.validate(check_df=True, check_boundaries=True, check_categories=True)
         if ('benchmark' not in self.config) or ('counting_significance' not in self.config['benchmark']):
-            self.stdout.info("INFO: No significance benchmark defined. Skipped evaluation.")
+            self.stdout.info("No significance benchmark defined. Skipped evaluation.")
         benchmark_config = self.config['benchmark']['counting_significance']
         benchmarks = list(benchmark_config)
         benchmark_significance = {}
         channel = self.active_channel
         category_labels = self.get_category_labels(valid_only=True)
         for benchmark in benchmarks:
             benchmark_significance[benchmark] = {}
@@ -1345,15 +1345,15 @@
         cache scores: bool, default = True
            Cache application of score columns (skipping apply score step).
         cat_event_number: (optional) dict
            If specified, event categorization will be performed on a specific set of events for each sample
            given in the dictionary. The format is { sample: array of event numbers }.
         """
         if event_indices is not None:
-            self.stdout.info("INFO: Categorization will be done on a given set of event numbers for each sample")
+            self.stdout.info("Categorization will be done on a given set of event numbers for each sample")
         self.set_active_channel(channel)
         self.load_channel_df(event_indices=event_indices, apply_score=not cache_scores)
         self.scan_bounds(cache=cache_boundaries)
         if not cache_categories:
             self.apply_categories()
         self.evaluate_benchmark_significance()
     
@@ -1400,15 +1400,15 @@
         hist = rf.get_Histo1D(**kwargs)
         # remove bins with negative weights
         from quickstats.interface.root import TH1
         neg_bin_indices, neg_bin_values = TH1.remove_negative_bins(hist)
         if len(neg_bin_indices) > 0:
             index_str = [f"{i}" for i in (neg_bin_indices + 1)]
             value_str = [f"{v}" for v in neg_bin_values]
-            self.stdout.warning(f'WARNING: Detected bins with negative weights '
+            self.stdout.warning(f'Detected bins with negative weights '
                                 f'(bins = {", ".join(index_str)}, '
                                 f'weights = {", ".join(value_str)}). '
                                 f'Bin weight will be set to 0.')
         rf.save_components(savepath, components=[hist])
         
     def save_dataframe_as_minitree(self, df:pd.DataFrame, savepath:str):
         """
@@ -1437,21 +1437,21 @@
         channel = self._parse_channel(channel)
         # save category summary
         savepath = self.get_file("category_summary", channel=channel)
         if channel not in self.summary:
             raise RuntimeError(f'category summary for the chanenl "{channel}" not initialized')
         with open(savepath, "w") as outfile:
             json.dump(self.summary[channel], outfile, indent=2)
-        self.stdout.info(f'INFO: Saved category summary to {savepath}')
+        self.stdout.info(f'Saved category summary to {savepath}')
         # save boundary data
         savepath = self.get_file("boundary_data", channel=channel)
         boundary_tree = self.get_boundary_tree(channel=channel)
         with open(savepath, "w") as outfile:
             json.dump(boundary_tree.tree, outfile, indent=2)
-        self.stdout.info(f'INFO: Saved boundary data to {savepath}')
+        self.stdout.info(f'Saved boundary data to {savepath}')
         
     def save_channel_yields(self, channel:Optional[str]=None,
                             resampling:bool=False,
                             resampling_random_state:Optional[int]=None) -> None:
         """
         Save yield information for a given channel.
         
@@ -1476,20 +1476,20 @@
         else:
             yields     = self.category_yields[channel]
             yields_err = self.category_yields_err[channel]
         for category, category_yields in yields.items():
             savepath = self.get_file("yield_data", category=category)
             with open(savepath, "w") as outfile:
                 json.dump(category_yields, outfile, indent=2)
-            self.stdout.info(f'INFO: Saved yield information to {savepath}')
+            self.stdout.info(f'Saved yield information to {savepath}')
         for category, category_yields_err in yields_err.items():
             savepath = self.get_file("yield_err_data", category=category)
             with open(savepath, "w") as outfile:
                 json.dump(category_yields_err, outfile, indent=2)
-            self.stdout.info(f'INFO: Saved yield uncertainty information to {savepath}')
+            self.stdout.info(f'Saved yield uncertainty information to {savepath}')
             
     def _get_minimal_sample_outputs(self):
         """Get minimal set of output samples to be saved; analysis specific
         """
         ARRAY     = CategorizationOutputFormat.ARRAY
         MINITREE  = CategorizationOutputFormat.MINITREE
         HISTOGRAM = CategorizationOutputFormat.HISTOGRAM        
@@ -1585,15 +1585,15 @@
         samples = self.channel_config['test_samples']
         sample_outputs = self._get_required_sample_outputs(mode=mode)
         self.check_missing_columns(columns)
         
         if resampling:
             self.stdout.info("NOTE: Resampling mode is enabled. The following outputs will "
                              "be saved with resampled events: csv, minitree, histogram, "
-                             "yield, data point.")
+                             "yield, data point.", bare=True)
         save_methods = {
             CategorizationOutputFormat.ARRAY     : self.save_dataframe_as_array,
             CategorizationOutputFormat.MINITREE  : self.save_dataframe_as_minitree,
             CategorizationOutputFormat.HISTOGRAM : self.save_dataframe_as_histogram,
         }
 
         for output_format in sample_outputs:
@@ -1617,18 +1617,18 @@
                                           resampling_random_state=resampling_random_state)
                 for output_format in CategorizationOutputFormat:
                     if sample not in sample_outputs[output_format]:
                         continue
                     savepath = self.get_file(output_format.filename, sample=sample,
                                              category=category_name, fmt=fmt)
                     if cache and os.path.exists(savepath):
-                        self.stdout.info(f'INFO: Cached {output_format.short_name} output from {savepath}')
+                        self.stdout.info(f'Cached {output_format.short_name} output from {savepath}')
                         continue
                     save_methods[output_format](df, savepath)
-                    self.stdout.info(f'INFO: Saved {output_format.short_name} output to {savepath}')
+                    self.stdout.info(f'Saved {output_format.short_name} output to {savepath}')
                     
         if save_yield:
             self.update_category_yields()
             self.path_manager.makedirs(["yield"])
             self.save_channel_yields(channel,
                                      resampling=resampling,
                                      resampling_random_state=resampling_random_state)
@@ -1648,23 +1648,23 @@
                 missing_column_by_sample[sample] = missing_columns
         if len(missing_column_by_sample) > 0:
             missing_same_columns = len(set(tuple(cols) for cols in missing_column_by_sample.values())) == 1
             all_samples_missing = set(missing_column_by_sample.keys()) == set(self.channel_df.keys())
             if missing_same_columns:
                 columns = list(missing_column_by_sample.values())[0]
                 if all_samples_missing:
-                    self.stdout.warning(f"WARNING: The following save columns are missing for all samples: "
+                    self.stdout.warning(f"The following save columns are missing for all samples: "
                                         f"{', '.join(columns)}")
                 else:
                     samples = list(missing_column_by_sample.keys())
-                    self.stdout.warning(f"WARNING: The following save columns are missing for the samples "
+                    self.stdout.warning(f"The following save columns are missing for the samples "
                                         f"{', '.join(samples)}: {', '.join(columns)}")
             else:
                 for sample, columns in missing_column_by_sample.items():
-                    self.stdout.warning(f"WARNING: The following save columns are missing for the sample {sample}: "
+                    self.stdout.warning(f"The following save columns are missing for the sample {sample}: "
                                         f"{', '.join(columns)}")
     
     def get_yield_files_and_description(self):
         result = {
             "yield_data"     : "yield information",
             "yield_err_data" : "yield uncertainty information"
         }
@@ -1674,45 +1674,45 @@
         self.validate(check_channels=True)
         category_names = self.get_all_category_names(valid_only=False)
         yield_info = self.get_yield_files_and_description()
         for yield_file, description in yield_info.items():
             merged_yield_file = f"merged_{yield_file}"
             savepath = self.get_file(merged_yield_file)
             if cache and os.path.exists(savepath):
-                self.stdout.info(f"INFO: Cached combined {description} from {savepath}")
+                self.stdout.info(f"Cached combined {description} from {savepath}")
             yield_data = {}
             for category_name in category_names:
                 filepath = self.get_file(yield_file, validate=True, category=category_name)
                 with open(filepath, "r") as file:
                     yield_data[category_name] = json.load(file)
             with open(savepath, "w") as outfile:
                 json.dump(yield_data, outfile, indent=2)
-                self.stdout.info(f"INFO: Saved combined {description} to {savepath}")
+                self.stdout.info(f"Saved combined {description} to {savepath}")
                 
     def save_combined_benchmark_significance(self, cache:bool=True):
         self.validate(check_channels=True)
         benchmark_savepath = self.get_file("benchmark_significance")
         if (is_valid_file(benchmark_savepath)) and cache:
-            self.stdout.info(f"INFO: Cached benchmark significance data from {benchmark_savepath}")
+            self.stdout.info(f"Cached benchmark significance data from {benchmark_savepath}")
             if not self.benchmark_significance:
                 with open(benchmark_savepath, "r") as file:
                     self.benchmark_significance = json.load(file)
         elif self.benchmark_significance:
             with open(benchmark_savepath, "w") as file:
                 json.dump(self.benchmark_significance, file)
-                self.stdout.info(f"INFO: Saved benchmark significance data to {benchmark_savepath}")
+                self.stdout.info(f"Saved benchmark significance data to {benchmark_savepath}")
                       
     def merge_category_outputs(self, save_yield:bool=True,
                                save_benchmark:bool=True,
                                cache:bool=True):
         for channel in self.target_channels:
             if channel not in self.boundary_trees:
                 self.load_boundaries(channel=channel)
         
-        self.stdout.info("INFO: Merging outputs from all channels...")
+        self.stdout.info("Merging outputs from all channels...")
        
         if save_yield:
             self.save_combined_yields(cache=cache)
 
         # merge benchmark significance
         if self.benchmark_significance:
             self.update_combined_benchmark_significance()
```

### Comparing `quickstats-0.6.7.8/quickstats/analysis/multi_class_boundary_tree.py` & `quickstats-0.6.8.1/quickstats/analysis/multi_class_boundary_tree.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/analysis/ntuple_conversion_tool.py` & `quickstats-0.6.8.1/quickstats/analysis/ntuple_conversion_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
                  **kwargs):
         super().__init__(analysis_config=analysis_config,
                          ntuple_dir=ntuple_dir,
                          array_dir=array_dir,
                          disable_config_message=True,
                          verbosity=verbosity,
                          **kwargs)
-        self.stdout.info(f'INFO: Initialized ntuple directory as "{self.get_directory("ntuple")}".')
-        self.stdout.info(f'INFO: Initialized array directory as "{self.get_directory("array")}".')
-        self.stdout.info(f'INFO: Initialized ntuple treename as "{self.treename}".')
+        self.stdout.info(f'Initialized ntuple directory as "{self.get_directory("ntuple")}".')
+        self.stdout.info(f'Initialized array directory as "{self.get_directory("array")}".')
+        self.stdout.info(f'Initialized ntuple treename as "{self.treename}".')
         
     @semistaticmethod
     def _save(self, df, outpath:str, fmt:str="csv",
               mode:str="a", complevel:int=None):
         
         assert (fmt in ["csv", "h5"])
         assert (mode in ["w", "a", "r"])
@@ -77,15 +77,15 @@
                  chunksize:int=100000,
                  library:str="quickstats",
                  kwargs:Optional[Dict]=None):
         
         if columns is None:
             columns = copy.deepcopy(self.DEFAULT_COLUMNS)
 
-        self.stdout.info(f'INFO: Processing file "{filename}"')
+        self.stdout.info(f'Processing file "{filename}"')
 
         #NTupleProcessTool.remove_csv(sample, outdir)
         
         if library == "quickstats":
             # does not support chunksize
             from quickstats.utils.data_conversion import root2dataframe
             df = root2dataframe(filename, treename, columns=columns,
@@ -126,15 +126,15 @@
             df = self._postprocess(df, **kwargs, sample_name=sample_name)
             
             if drop_columns is not None:
                 df = df.drop(drop_columns, axis=1)
                 
             outpath = self.get_array_sample_path(sample_name=sample_name, dirname=outdir, fmt=fmt)
             if i == 0:
-                self.stdout.info(f'INFO: Saving data array as "{outpath}"')
+                self.stdout.info(f'Saving data array as "{outpath}"')
                 self._save(df, outpath=outpath, fmt=fmt, 
                            mode='w', complevel=complevel)
             else:
                 self._save(df, outpath=outpath, fmt=fmt, 
                            mode='a', complevel=complevel)
                 
             self._finalize(df, **kwargs, sample_name=sample_name, outdir=outdir,
@@ -189,22 +189,22 @@
             
         if library == "quickstats":
             import ROOT
             if ROOT.IsImplicitMTEnabled():
                 ROOT.DisableImplicitMT()
             if parallel != 0:
                 parallel = 0
-                sys.stdout.write("INFO: Disabling multi-processing when using ROOT backend\n")            
+                sys.stdout.write("Disabling multi-processing when using ROOT backend\n")            
         
         ntuple_dir = self.get_directory("ntuple")
         array_dir = self.get_directory("array")
         
         for kinematic_region in kinematic_regions:
             if kinematic_region:
-                self.stdout.info(f'INFO: Converting ntuples in the kinematic region "{kinematic_region}"')
+                self.stdout.info(f'Converting ntuples in the kinematic region "{kinematic_region}"')
                 ntuple_subdir = os.path.join(ntuple_dir, kinematic_region)
                 array_subdir = os.path.join(array_dir, kinematic_region)
             else:
                 ntuple_subdir = ntuple_dir
                 array_subdir  = array_dir
                 
             if not os.path.exists(array_subdir):
```

### Comparing `quickstats-0.6.7.8/quickstats/analysis/ntuple_process_tool.py` & `quickstats-0.6.8.1/quickstats/analysis/ntuple_process_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,15 +378,15 @@
                         sample_types:Optional[List[str]]=None):
         if self.processor is None:
             raise RuntimeError("processor not initialized (probably missing a processor config)")
         paths = self.get_selected_paths(syst_themes=['Nominal'],
                                         samples=samples,
                                         sample_types=sample_types)
         if not paths:
-            self.stdout.warning('WARNING: No inputs matching the given conditions. Skipped processing.')
+            self.stdout.warning('No inputs matching the given conditions. Skipped processing.')
         paths = paths['Nominal']
         outdir = self.path_manager.base_path
         for sample in paths:
             self.processor.set_flags(self.processor_flags)
             for sample_type in paths[sample]:
                 sample_paths = paths[sample][sample_type]
                 sample_config = {
@@ -432,19 +432,19 @@
                     for subattributes in sample_subattributes:
                         file = source_path_func(subattributes, sample_subdir)
                         source_files.append(file)
                     main_attributes = dict(zip(group_level, indices))
                     main_attributes['sample'] = sample
                     target_file = target_path_func(main_attributes, sample_subdir)
                     if main_attributes['syst_theme'] == 'Nominal':
-                        self.stdout.info(f'INFO: Merging outputs for the sample "{sample}"')
+                        self.stdout.info(f'Merging outputs for the sample "{sample}"')
                     else:
                         syst_name = main_attributes['syst_name']
                         syst_var = main_attributes['syst_var']
-                        self.stdout.info(f'INFO: Merging outputs for the sample "{sample}" '
+                        self.stdout.info(f'Merging outputs for the sample "{sample}" '
                                          f'(systematic = "{syst_name}", variation = "{syst_var}")')
                     merge_func(source_files, target_file)
     
     def merge_samples(self, samples:Optional[List[str]]=None, subdirs:Optional[List[str]]=None):
         outdir = self.path_manager.get_directory("ntuple")
         self.merge_outputs(self.get_sample_outpath,
                            self.get_merged_sample_outpath,
@@ -566,15 +566,15 @@
         merged_df['efficiency'] = efficiency
         merged_df['cumulative_efficiency'] = cumul_efficiency
         if 'yield' in merged_df:
             yield_efficiency, yield_cumul_efficiency = self._get_efficiency_values(merged_df, 'yield')
             merged_df['yield_efficiency'] = yield_efficiency
             merged_df['yield_cumulative_efficiency'] = yield_cumul_efficiency
         merged_df.to_csv(outname, index=False)
-        self.stdout.info(f'INFO: Saved cutflow data as "{outname}"')
+        self.stdout.info(f'Saved cutflow data as "{outname}"')
         
     def load_cutflow_report(self, samples:Optional[List[str]]=None):
         import pandas as pd
         samples = self.get_validated_samples(samples, merged=True)
         
         sample_spec   = self.sample_config['samples']
         cutflow_dir   = self.path_manager.get_directory("cutflow")
@@ -584,15 +584,15 @@
             if sample not in samples:
                 continue
             sample_config = {
                 "name": sample
             }
             cutflow_file = self.get_merged_cutflow_outpath(sample_config, cutflow_dir)
             if not os.path.exists(cutflow_file):
-                self.stdout.warning(f'WARNING: Missing cutflow file for the sample "{sample}".')
+                self.stdout.warning(f'Missing cutflow file for the sample "{sample}".')
                 continue
             df = pd.read_csv(cutflow_file)
             cutflow_report[sample] = df
             
         self.cutflow_report = cutflow_report
 
     def plot_cutflow_report(self, samples:Optional[List[str]]=None,
@@ -617,15 +617,15 @@
         if label_map is None:
             label_map = {}
             
         # Loop over each sample and make a plot of the cutflow
         for sample in samples: 
             
             if sample not in self.cutflow_report:
-                self.stdout.warning(f'WARNING: Missing cutflow report for the sample "{sample}". Skipped.')
+                self.stdout.warning(f'Missing cutflow report for the sample "{sample}". Skipped.')
                 continue
 
             df = self.cutflow_report[sample].fillna(0)
 
             cut_labels = [label_map.get(name, name) for name in df["name"]]
 
             fig, axs = plt.subplots(3, 1, figsize=figsize)
```

### Comparing `quickstats-0.6.7.8/quickstats/analysis/sample_poly_param_tool.py` & `quickstats-0.6.8.1/quickstats/analysis/sample_poly_param_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                 components.append(component)
             symbol_name = f"Yield({','.join(components)})"
             symbol_names.append(symbol_name)
         return symbol_names
     
     def display_expression(self, expr):
         if not in_notebook():
-            self.stdout.info(str(expr))
+            self.stdout.info(str(expr), bare=True)
         else:
             from IPython import display
             display.display(expr)
             
     def display_sets(self, *objects):
         from sympy import FiniteSet
         self.display_expression(FiniteSet(*objects))
@@ -125,38 +125,38 @@
                                                                                         coefficients,
                                                                                         bases,
                                                                                         latex_map=latex_map)
         basis_value_map = dict(zip(bases, basis_values))
         basis_sample_map = dict(zip(bases, samples))
         formula_expr = self.initialize_formula(formula, parameter_symbols,
                                                coefficient_symbols, latex_map=latex_map)
-        self.stdout.info("Formula:")
+        self.stdout.info("Formula:", bare=True)
         self.display_expression(formula_expr)
-        self.stdout.info("Parameters:")
+        self.stdout.info("Parameters:", bare=True)
         self.display_sets(*parameter_symbols.values())
-        self.stdout.info("Coefficients:")
+        self.stdout.info("Coefficients:", bare=True)
         self.display_sets(*coefficient_symbols.values())
         solutions = self.solve_coefficients(formula_expr, parameter_symbols, coefficient_symbols,
                                            basis_symbols, basis_value_map)
         if len(solutions) == 0:
             raise RuntimeError("unable to solve the system of linear equations")
         elif len(solutions) > 1:
             raise RuntimeError("system of linear equations gives non-unique solutions")
         solution = solutions[0]
-        self.stdout.info("Solutions:")
+        self.stdout.info("Solutions:", bare=True)
         for coefficient in coefficient_symbols.values():
             self.display_equation(coefficient, solution[coefficient])
         subs = [(k, v) for k, v in solution.items()]
         resolved_formula = formula_expr.subs(subs).expand()
         coefficient_map = {basis:resolved_formula.coeff(basis_symbols[basis]) for basis in bases}
         inverse_latex_map = self._get_inverse_latex_map(latex_map)
         coefficient_map_delatexed = {}
         for basis, coefficient_formula in coefficient_map.items():
             coefficient_map_delatexed[basis] = self.get_delatexed_formula(coefficient_formula, inverse_latex_map)
-        self.stdout.info("Contribution from basis sample:")
+        self.stdout.info("Contribution from basis sample:", bare=True)
         for basis, expr in coefficient_map.items():
             self.display_equation(basis_symbols[basis], expr)
         for basis in bases:
             param_data['sample'].append(basis_sample_map[basis])
             for parameter, value in basis_value_map[basis].items():
                 param_data[parameter].append(to_rounded_float(value))
             basis_symbol = basis_symbols[basis]
```

### Comparing `quickstats-0.6.7.8/quickstats/analysis/systematics/base_systematics.py` & `quickstats-0.6.8.1/quickstats/analysis/systematics/base_systematics.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self.dataframe = None
         self.processed = False
         
     def append(self, dataframe):
         if self.dataframe is None:
             self.dataframe = dataframe
         else:
-            self.dataframe = self.dataframe.combine_first(dataframe)
+            self.dataframe = dataframe.combine_first(self.dataframe)
     
     def _resolve_choices(self, full_list:List,
                          choices:Optional[List]=None,
                          name:str="choices"):
         if choices is None:
             return list(full_list)
         invalid_choices = list(set(choices) - set(full_list))
@@ -159,16 +159,14 @@
         from quickstats.maths.statistics_jitted import random_poisson_elementwise_seed
         com_idx = df_nom.index.intersection(df_sys.index)
         # all events common, use same weights
         if (len(com_idx) == len(df_sys)) and (len(df_nom) == len(df_sys)):
             return nom_weights
         com_nom_loc = df_nom.index.get_indexer_for(com_idx)
         com_sys_loc = df_sys.index.get_indexer_for(com_idx)
-        from pdb import set_trace
-        set_trace()
         poisson_weights = np.zeros((n_toys, len(df_sys)))
         poisson_weights[:, com_sys_loc] = nom_weights[:, com_nom_loc]
         uncom_sys_idx = df_sys.index.difference(df_nom.index)
         if len(uncom_sys_idx):
             uncom_sys_loc = df_sys.index.get_indexer_for(uncom_sys_idx)
             uncom_sys_seeds = self.get_seeds(uncom_sys_idx)
             poisson_weights[:, uncom_sys_loc] = random_poisson_elementwise_seed(uncom_sys_seeds, n_toys)
@@ -201,23 +199,23 @@
                                        sample=sample,
                                        syst_name='Nominal',
                                        variation=None)
             for category in categories:
                 selection = category_selection[category]
                 cat_df_nom[category] = df_nom.query(selection).set_index(self.config['index']).sort_index()
             if n_toys is not None:
-                self.stdout.info(f'INFO: Evaluating bootstrap weights for the nominal sample')
+                self.stdout.info(f'Evaluating bootstrap weights for the nominal sample')
                 for category in categories:
                     toy_weights_nom[category] = self.get_nom_toy_weights(cat_df_nom[category], n_toys)
             for syst_theme in syst_themes:
                 syst_names_by_theme = self.get_syst_names_from_theme(syst_theme)
                 syst_names_by_theme = np.intersect1d(syst_names_by_theme, syst_names)
-                self.stdout.info(f"Sample: {sample}\tSystematic Theme: {syst_theme}")
+                self.stdout.info(f"Sample: {sample}\tSystematic Theme: {syst_theme}", bare=True)
                 for syst_name in syst_names_by_theme:
-                    self.stdout.info(f'INFO: Reading systematic data for the systematic "{syst_name}"')
+                    self.stdout.info(f'Reading systematic data for the systematic "{syst_name}"')
                     syst_data = {}
                     for variation in variations:
                         df_sys = self.get_input_df(syst_theme=syst_theme,
                                                    sample=sample,
                                                    syst_name=syst_name,
                                                    variation=variation)
                         for category in categories:
@@ -264,23 +262,23 @@
                      check_rel_effect:bool=False,
                      strict:bool=True):
         if check_dataframe or check_rel_effect:
             if self.dataframe is None:
                 if strict:
                     raise RuntimeError("systematics dataframe not initialized")
                 else:
-                    self.stdout.warning("WARNING: Systematics dataframe not initialized. Skipping.")
+                    self.stdout.warning("Systematics dataframe not initialized. Skipping.")
                     return False
         if check_rel_effect:
             primary_keys = self.resolve_primary_keys(self.SYST_TYPES)
             if any(primary_key not in self.dataframe.columns for primary_key in primary_keys):
                 if strict:
                     raise RuntimeError("systematic relative effects not evaluated")
                 else:
-                    self.stdout.warning("WARNING: Systematic relative effects not evaluated. Skipping.")
+                    self.stdout.warning("Systematic relative effects not evaluated. Skipping.")
                     return False
         return True
     
     def process_systematics_data(self, df_nom, df_sys, variation:str):
         raise NotImplementedError
         
     def get_dataframe(self, samples:List[str]=None,
@@ -506,31 +504,31 @@
     def post_process(self, merge_config:Optional[Dict]=None):
         pass_check = self.sanity_check(check_dataframe=True,
                                        check_rel_effect=True,
                                        strict=False)
         if not pass_check:
             return None
         # remove systematics with failed status
-        self.stdout.info("INFO: Filtering systematics with failed status")
+        self.stdout.info("Filtering systematics with failed status")
         self.remove_failed_results()
-        self.stdout.info("INFO: Merging JER systematics")
+        self.stdout.info("Merging JER systematics")
         self.merge_smear_systematics()
-        self.stdout.info("INFO: Applying systematics pruning")
+        self.stdout.info("Applying systematics pruning")
         self.prune_systematics()
         if merge_config is not None:
-            self.stdout.info("INFO: Merging systematics by max effect")
+            self.stdout.info("Merging systematics by max effect")
             merged_dataframe = self.get_merged_systematics_by_max_effect(self.dataframe,
                                                                          **merge_config)
             self.dataframe = self.dataframe.combine_first(merged_dataframe)
             self.prune_systematics()
-        self.stdout.info("INFO: Fixing systematics with same signs")
+        self.stdout.info("Fixing systematics with same signs")
         self.fix_same_sign()
         """
         if merge_condition is not None:
-            self.stdout.info("INFO: Merging systematics by maximum effect")
+            self.stdout.info("Merging systematics by maximum effect")
             self.dataframe = self.merge_df_by_max_effect(self.dataframe, merge_condition)
         """
         self.processed = True
 
     def save(self, filename:str):
         pass_check = self.sanity_check(check_dataframe=True, strict=False)
         if pass_check:
```

### Comparing `quickstats-0.6.7.8/quickstats/analysis/systematics/gaussian_shape_systematics.py` & `quickstats-0.6.8.1/quickstats/analysis/systematics/gaussian_shape_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/analysis/systematics/normalization_systematics.py` & `quickstats-0.6.8.1/quickstats/analysis/systematics/normalization_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/analysis/systematics/systematics_evaluation_tool.py` & `quickstats-0.6.8.1/quickstats/analysis/systematics/systematics_evaluation_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -178,17 +178,17 @@
         modules = {"yield": self.yield_syst_module, "shape": self.shape_syst_module}
         if syst_types is None:
             syst_types = self.syst_types
         for syst_type in syst_types:
             # discard certain unwanted systematics by pattern
             if self.discard_data is not None:
                 for item in self.discard_data:
-                    print("INFO: Discarding `{}` from {} systematics".format(item, syst_type))
+                    self.stdout.info("Discarding `{}` from {} systematics".format(item, syst_type))
                     modules[syst_type].discard(**self.discard_data[item])
-            print("INFO: Post-processing {} systematics results".format(syst_type))
+            self.stdout.info("Post-processing {} systematics results".format(syst_type))
             modules[syst_type].post_process(merge_condition=self.merge_condition)
             
     def load_result(self, syst_types=None, mode="processed"):
         modules = {"yield": self.yield_syst_module, "shape": self.shape_syst_module}
         if syst_types is None:
             syst_types = self.syst_types
         for syst_type in syst_types:
@@ -198,18 +198,18 @@
             elif mode == "processed":
                 basename = self.FILE_NAMES['individual_processed'].format(syst_type=syst_type)
             else:
                 raise ValueError("unknown mode: {}".format(mode))
             fname = os.path.join(dirname, basename)
             if os.path.exists(fname):
                 modules[syst_type].load(fname)
-                print("INFO: Loaded results for {} systematics from `{}`".format(syst_type, fname))
+                self.stdout.info("Loaded results for {} systematics from `{}`".format(syst_type, fname))
                 modules[syst_type].processed = (mode == "processed")
             else:
-                print("ERROR: No savaed results found for {} systematics (in `{}`)".format(syst_type, fname))
+                self.stdout.error("No saved results found for {} systematics (in `{}`)".format(syst_type, fname))
                 
     def save_result(self, syst_types=None):
         modules = {"yield": self.yield_syst_module, "shape": self.shape_syst_module}
         if syst_types is None:
             syst_types = self.syst_types
         for syst_type in syst_types:
             dirname = os.path.join(self.base_path, "results")
@@ -217,15 +217,15 @@
                 basename = self.FILE_NAMES['individual_processed'].format(syst_type=syst_type)
             else:
                 basename = self.FILE_NAMES['individual_detailed'].format(syst_type=syst_type)
             fname = os.path.join(dirname, basename)
             if not os.path.exists(dirname):
                 os.makedirs(dirname)
             modules[syst_type].save(fname)
-            print("INFO: Saved results for {} systematics in `{}`".format(syst_type, fname))
+            self.stdout.info("Saved results for {} systematics in `{}`".format(syst_type, fname))
             
     def get_combined_summary(self):
         modules = {"yield": self.yield_syst_module, "shape": self.shape_syst_module}
         combined_result = {}
         for syst_type in self.syst_types:
             if modules[syst_type].dataframe is None:
                 continue
@@ -238,15 +238,15 @@
         dirname = os.path.join(self.base_path, "results")
         basename = self.FILE_NAMES['combined_summary']
         if not os.path.exists(dirname):
             os.makedirs(dirname)
         fname = os.path.join(dirname, basename)
         with open(fname, 'w') as f:
             json.dump(combined_result, f, indent=2)
-        print("INFO: Saved combined summary in `{}`".format(fname))
+        self.stdout.info("Saved combined summary in `{}`".format(fname))
             
     def get_dataframe(self, syst_type, simplified=True):
         if syst_type == "yield":
             df = self.yield_syst_module.get_valid_dataframe("yield")
         elif syst_type == "shape":
             df = self.shape_syst_module.dataframe
         elif syst_type == "position_shape":
```

### Comparing `quickstats-0.6.7.8/quickstats/clis/core.py` & `quickstats-0.6.8.1/quickstats/clis/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -572,14 +572,18 @@
 @click.option('--offset/--no-offset', default=True, show_default=True,
               help='Use NLL offset.')
 @click.option('--print_level', type=int, default=-1, show_default=True,
               help='Minimizer print level')
 @click.option('-v', '--verbosity', default='INFO', show_default=True,
               type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR"], case_sensitive=False),
               help='Verbosity level.')
+@click.option('-f', '--fix', 'fix_param', default="", show_default=True,
+              help='Parameters to fix')
+@click.option('-r', '--profile', 'profile_param', default="", show_default=True,
+              help='Parameters to profile')
 @click.option('--snapshot', 'snapshot_name', default=None, help='Name of initial snapshot')
 @click.option('--parallel', type=int, default=-1, show_default=True,
               help='\b\n Parallelize job across the N workers.'
                    '\b\n Case  0: Jobs are run sequentially (for debugging).'
                    '\b\n Case -1: Jobs are run across N_CPU workers.')
 def toy_limit(**kwargs):
     """
```

### Comparing `quickstats-0.6.7.8/quickstats/clis/inspect_rfile.py` & `quickstats-0.6.8.1/quickstats/clis/inspect_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/clis/inspect_ws.py` & `quickstats-0.6.8.1/quickstats/clis/inspect_ws.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/clis/likelihood_fit.py` & `quickstats-0.6.8.1/quickstats/clis/likelihood_fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,15 +275,15 @@
     from quickstats.utils.common_utils import filter_by_wildcards
     if _kwargs['save_json'] or _kwargs['save_plot']:
         df = get_correlation_matrix(fit_result, lib='pandas')
         labels = list(df.columns)
         selected = filter_by_wildcards(labels, _kwargs['select'])
         selected = filter_by_wildcards(selected, _kwargs['remove'], exclusion=True)
         to_drop = list(set(labels) - set(selected))
-        df = df.drop(to_drop, axis=0).drop(to_drop, axis=1)
+        df = df.drop(to_drop, axis=0).drop(to_drop, axis=1).transpose()
         if _kwargs['save_json']:
             data = df.to_dict()
             outname = basename + ".json"
             with open(outname, "w") as out:
                 json.dump(data, out, indent=2)
             print(f"INFO: Saved correlation data to `{outname}`")
         if _kwargs['save_plot']:
```

### Comparing `quickstats-0.6.7.8/quickstats/clis/likelihood_scan.py` & `quickstats-0.6.8.1/quickstats/clis/likelihood_scan.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/clis/limit_setting.py` & `quickstats-0.6.8.1/quickstats/clis/limit_setting.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/clis/processor_cli.py` & `quickstats-0.6.8.1/quickstats/clis/processor_cli.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/clis/workspace_tools.py` & `quickstats-0.6.8.1/quickstats/clis/workspace_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -243,9 +243,42 @@
     _kwargs['minimizer_config'] = kwargs
     from quickstats.components.workspaces import XMLWSCombiner
     combiner = XMLWSCombiner(**_kwargs)
     combiner.create_combined_workspace(infiles=infiles, outfile=outfile,
                                        save_rename_ws=save_rename_ws,
                                        save_combine_ws=save_combine_ws,
                                        save_final_ws=True,
-                                       import_class_code=import_class_code)    
-    
+                                       import_class_code=import_class_code)
+    
+    
+@click.command(name='decompose_ws')
+@click.option('-i', '--infile', required=True, 
+              help='Path to the input workspace file')
+@click.option('-o', '--outfile', required=True, 
+              help='Path to the output workspace file')
+@click.option('--import-class-code/--no-import-class-code', 'import_class_code',
+              default=True, show_default=True,
+              help='Import class code')
+@click.option('-c', '--category_expr', default='*', show_default=True,
+              help='Categories to keep in the decomposed workspace (separated by commas). '
+              'Both category index and category label can be used. Category index can be '
+              'a single number or a range "<min_index>-<max_index>. Wildcard is supported '
+              'for category labels.')
+@click.option('-v', '--verbosity',  default="INFO", show_default=True,
+              help='verbosity level ("DEBUG", "INFO", "WARNING", "ERROR")')
+@click.option('--snapshots', 'snapshots_to_save', default=None, show_default=True,
+              help='Snapshots to save (separated by commas)'
+              'By default, all existing snapshots will be saved')
+@click.option('--rebuild-nuis/--no-rebuild-nuis', default=False, show_default=True,
+              help='Whether to rebuild the nuisance parameter set')
+@click.option('--rebuild-pdf/--no-rebuild-pdf', default=False, show_default=True,
+              help='Whether to rebuild category pdfs')
+def decompose_ws(**kwargs):
+    """
+    Decompose workspace into subcategories.
+    """
+    init_kwargs = {}
+    for key in ['verbosity']:
+        init_kwargs[key] = kwargs.pop(key)
+    from quickstats.components.workspaces import WSDecomposer
+    decomposer = WSDecomposer(**init_kwargs)
+    decomposer.create_decomposed_workspace(**kwargs)
```

### Comparing `quickstats-0.6.7.8/quickstats/components/__init__.py` & `quickstats-0.6.8.1/quickstats/components/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/analysis_base.py` & `quickstats-0.6.8.1/quickstats/components/analysis_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Optional, Union, List, Dict
 
 from quickstats.components import AnalysisObject, Likelihood, AsimovGenerator
+from quickstats.utils.common_utils import combine_dict
 
 class AnalysisBase(Likelihood, AsimovGenerator):
     def __init__(self, filename:str, poi_name:Optional[Union[str, List[str]]]=None,
                  data_name:str='combData', 
                  config:Optional[Union[Dict, str]]=None,
                  verbosity:Optional[Union[int, str]]="INFO", **kwargs):
+        config = combine_dict(config, kwargs)
         super().__init__(filename=filename,
                          poi_name=poi_name,
                          data_name=data_name,
                          config=config,
                          verbosity=verbosity)
         
     def plot_fit_summary(self, uncond_fit:bool=True, cond_fit:bool=True,
@@ -20,20 +22,20 @@
                          comparison_plot:bool=True,
                          comparison_options:Optional[Dict]=None,
                          **kwargs):
         data_name = self.model._data.GetName()
         snapshots = []
         if cond_fit:
             if not self.model.workspace.getSnapshot("condFit"):
-                self.stdout.warning("WARNING: No conditional fit is made. The corresponding plot will not be shown")
+                self.stdout.warning("No conditional fit is made. The corresponding plot will not be shown")
             else:
                 snapshots.append("condFit")
         if uncond_fit:
             if not self.model.workspace.getSnapshot("uncondFit"):
-                self.stdout.warning("WARNING: No unconditional fit is made. The corresponding plot will not be shown")
+                self.stdout.warning("No unconditional fit is made. The corresponding plot will not be shown")
             else:
                 snapshots.append("uncondFit")
         kwargs = {
             **kwargs,
             "categories": categories,
             "current_distributions": False,
             "datasets": [data_name],
@@ -49,16 +51,16 @@
             self.stdout.info("INFO: Using blinded fit result.")
         if comparison_plot:
             if comparison_options is None:
                 comparison_options = {}
             comparison_options['reference'] = data_name
             if "target" not in comparison_options:
                 if "uncondFit" in kwargs['snapshots']:
-                    self.stdout.info("INFO: Using data vs unconditional fit for comparison plot")
+                    self.stdout.info("Using data vs unconditional fit for comparison plot")
                     comparison_options["target"] = "uncondFit"
                 elif "condFit" in kwargs['snapshots']:
                     comparison_options["target"] = "condFit"
                 else:
-                    self.stdout.warning("WARNING: No fit results available. Comparison plot will not be made.")
+                    self.stdout.warning("No fit results available. Comparison plot will not be made.")
                     comparison_options = None
             kwargs['comparison_options'] = comparison_options
         self.model.plot_distributions(**kwargs)
```

### Comparing `quickstats-0.6.7.8/quickstats/components/analysis_object.py` & `quickstats-0.6.8.1/quickstats/components/analysis_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                  minimizer_type:str='Minuit2', minimizer_algo:str='Migrad', precision:float=0.001, 
                  eps:float=1.0, retry:int=1, strategy:int=1, print_level:int=-1, timer:bool=False,
                  num_cpu:int=1, offset:bool=True, optimize:int=2, eigen:bool=False, hesse:bool=False,
                  improve:int=0, fix_cache:bool=True, fix_multi:bool=True, max_calls:int=-1, 
                  max_iters:int=-1, constrain_nuis:bool=True, batch_mode:bool=False,
                  int_bin_precision:float=-1., preset_param:bool=False, minimizer_offset:int=1,
                  minimizer_cls=None, verbosity:Optional[Union[int, str]]="INFO"):
-        super().__init__(verbosity=verbosity)    
+        super().__init__(verbosity=verbosity)
         self.model = None
         self.minimizer = None
         self._use_blind_range = False
         if minimizer_cls is None:
             self.minimizer_cls = ExtendedMinimizer
         else:
             self.minimizer_cls = minimizer_cls
@@ -76,26 +76,26 @@
             self.setup_minimizer(**minimizer_options)
             self.sanity_check()
         
     def sanity_check(self):
         aux_vars = self.model.get_variables("auxiliary")
         floating_aux_vars = [v.GetName() for v in aux_vars if not v.isConstant()]
         if len(floating_aux_vars) > 0:
-            self.stdout.warning("WARNING: The following auxiliary variables (variables that are not "
+            self.stdout.warning("The following auxiliary variables (variables that are not "
                                 "part of the POIs, observables, nuisance parameters and global "
                                 f"observables) are floating: {','.join(floating_aux_vars)}. If this is "
                                 "not intended, please make sure to fix them before fitting.", "red")            
     
     def preset_parameters(self):
         ROOT.RooStats.SetAllConstant(self.model.global_observables, True)
         #ROOT.RooStats.SetAllConstant(self.model.nuisance_parameters, False)
         ROOT.RooStats.SetAllConstant(self.model.pois, True)
-        self.stdout.info("INFO: Preset POIs as constant parameters.")
+        self.stdout.info("Preset POIs as constant parameters.")
         #self.stdout.info("INFO: Preset nuisance parameters as floating parameters.")
-        self.stdout.info("INFO: Preset global observables as constant parameters.")
+        self.stdout.info("Preset global observables as constant parameters.")
     
     @property
     def use_blind_range(self):
         return self._use_blind_range
     
     @property
     def minimizer_options(self):
@@ -128,19 +128,19 @@
             # remove duplicates
             poi_name = list(set(poi_name))
             for pname in poi_name:
                 poi = self.model.get_poi(pname)
                 self.poi.add(poi)
                 true_poi_names.append(poi.GetName())
             if true_poi_names:
-                self.stdout.info('INFO: POIs set to {}'.format(", ".join([f"\"{name}\"" for name in true_poi_names])))
+                self.stdout.info('POIs set to {}'.format(", ".join([f"\"{name}\"" for name in true_poi_names])))
         else:
             self.poi = self.model.get_poi(poi_name)
             if poi_name is not None:
-                self.stdout.info(f'INFO: POI set to "{poi_name}"')
+                self.stdout.info(f'POI set to "{poi_name}"')
         
     def setup_model(self, **kwargs):
         model = ExtendedModel(**kwargs, verbosity=self.stdout.verbosity)
         self.model = model
     
     def setup_parameters(self, fix_param:str='', profile_param:str='', update_snapshot:bool=True):
         if not self.model:
@@ -175,22 +175,22 @@
         if ana_pois.size() == 0:
             return None
         aux_pois = ROOT.RooArgSet(ws_pois)
         aux_pois.remove(ana_pois)
         for profiled_param in profiled_parameters:
             if aux_pois.contains(profiled_param):
                 param_name = profiled_param.GetName()
-                self.stdout.warning(f"WARNING: Attemping to profile the parameter \"{param_name}\" which is a "
+                self.stdout.warning(f"Attemping to profile the parameter \"{param_name}\" which is a "
                                     f"POI defined in the workspace but not a POI used in this study. This "
                                     f"parameter will still be fixed during likelihood fit / limit setting. "
                                     f"Please designate the parameter as a POI in this study if intended.", "red")
         for fixed_param in fixed_parameters:
             if ana_pois.contains(fixed_param):
                 param_name = fixed_param.GetName()
-                self.stdout.warning(f"WARNING: Attemping to fix the parameter \"{param_name}\" which is a "
+                self.stdout.warning(f"Attemping to fix the parameter \"{param_name}\" which is a "
                                     f"POI used in this study. This parameter will still be floated during "
                                     f"unconditional likelihood fit / limit setting.", "red")
             
     def setup_minimizer(self, constrain_nuis:bool=True, **kwargs):
         
         minimizer = self.minimizer_cls("Minimizer", self.model.pdf, self.model.data,
                                        workspace=self.model.workspace,
@@ -203,15 +203,14 @@
             nll_options['global_observables'] = self.model.global_observables
             conditional_obs = self.model.model_config.GetConditionalObservables()
             if conditional_obs:
                 nll_options['conditional_observables'] = conditional_obs
             #nll_commands.append(ROOT.RooFit.ExternalConstraints(ROOT.RooArgSet()))
         
         minimizer_options = {k:v for k,v in kwargs.items() if k in ExtendedMinimizer._DEFAULT_MINIMIZER_OPTION_}
-
         minimizer.configure_nll(**nll_options)
         minimizer.configure(**minimizer_options)
         self.minimizer = minimizer
         self.default_nll_options = nll_options
         self.default_minimizer_options = minimizer_options
     
     def set_data(self, data_name:str='combData'):
@@ -227,48 +226,34 @@
         self.minimizer.configure_nll(range=sideband_range_name, split_range=True, update=True)
         self._use_blind_range = True
         
     def unset_blind_range(self):
         self.minimizer.nll = None
         self.minimizer.nll_commands.pop("RangeWithName", None)
         self.minimizer.nll_commands.pop("SplitRange", None)
-        self.stdout.info("INFO: Blind range removed from list of  NLL commands. NLL is reset.")
+        self.stdout.info("Blind range removed from list of  NLL commands. NLL is reset.")
         self._use_blind_range = False
-        
-    def load_snapshot(self, snapshot_name:Optional[str]=None):
-        if snapshot_name is not None:
-            snapshot = self.model.workspace.getSnapshot(snapshot_name)
-            if (not snapshot) and ('0x(nil)' in snapshot.__repr__()):
-                self.stdout.warning(f'WARNING: Snapshot "{snapshot_name}" does not exist.')
-            else:
-                self.model.workspace.loadSnapshot(snapshot_name)
-                self.stdout.debug(f'DEBUG: Loaded snapshot "{snapshot_name}"')
                 
     def restore_snapshot(self):
         self.load_snapshot(self.kCurrentSnapshotName)
     
     def get_variables(self, variable_type:Union[str, WSArgument], sort:bool=True):
         return self.model.get_variables(variable_type, sort=sort)
     
     def save_snapshot(self, snapshot_name:Optional[str]=None, 
                       variables:Optional[Union[ROOT.RooArgSet, str, WSArgument]]=None):
-        if snapshot_name is not None:
-            if variables is None:
-                self.model.workspace.saveSnapshot(snapshot_name, self.model.workspace.allVars())
-            else:
-                if isinstance(variables, (str, WSArgument)):
-                    variables = self.get_variables(variables)
-                self.model.workspace.saveSnapshot(snapshot_name, variables)
-            self.stdout.debug(f'DEBUG: Saved snapshot "{snapshot_name}"')
+        self.model.save_snapshot(snapshot_name, variables=variables)
+        
+    def load_snapshot(self, snapshot_name:Optional[str]=None):
+        self.model.load_snapshot(snapshot_name)
         
     def save(self, filename:str, recreate:bool=True, rebuild:bool=True):
         self.model.save(filename, recreate=recreate, rebuild=rebuild)
-        self.stdout.info(f'INFO: Saved workspace file as "{filename}"')
-        
-        
+        self.stdout.info(f'Saved workspace file as "{filename}"')
+                
     def decompose_nll(self, fmt:str="pandas"):
         from quickstats.utils.roofit_utils import decompose_nll
         if not self.minimizer.nll:
             self.minimizer.create_nll()
             result = decompose_nll(self.minimizer.nll, self.model.global_observables, fmt=fmt)
             self.minimizer.nll = None
             return result
```

### Comparing `quickstats-0.6.7.8/quickstats/components/asimov_generator.py` & `quickstats-0.6.8.1/quickstats/components/asimov_generator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/asymptotic_cls.py` & `quickstats-0.6.8.1/quickstats/components/asymptotic_cls.py`

 * *Files 7% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         self.better_negative_bands = better_negative_bands
         self.adjust_fit_range = adjust_fit_range
         self.direction = 1
         self.global_status = 0
         self.mu_exp = mu_exp
         if mu_guess == mu_exp:            
             mu_guess = mu_guess + 0.1
-            self.stdout.info(f"INFO: Changed mu_guess to {mu_guess} so that it is different from mu_exp")
+            self.stdout.info(f"Changed mu_guess to {mu_guess} so that it is different from mu_exp")
         self.mu_guess = mu_guess
         
         # define asimov data
         if asimov_data_name is not None:
             asimov_data_0 = self.model.workspace.data(asimov_data_name)
             if not asimov_data_0:
                 raise RuntimeError(f'failed to load dataset \"{asimov_data_name}\"')
@@ -132,25 +132,25 @@
 
     @semistaticmethod
     def load_extension(self):
         try:
             if not hasattr(ROOT, 'AsymptoticCLsTool'):
                 result = load_macro('AsymptoticCLsTool')
                 if hasattr(ROOT, 'AsymptoticCLsTool'):
-                    self.stdout.info('INFO: Loaded extension module "AsymptoticCLsTool"')
+                    self.stdout.info('Loaded extension module "AsymptoticCLsTool"')
         except Exception as e:
             print(e)
             
     def set_poi(self, poi_name:Optional[str]=None):
         if poi_name is None:
             self.poi = self.model.pois.first()
-            self.stdout.info('INFO: POI name not given. Set to first poi "{}" by default.'.format(self.poi.GetName()))
+            self.stdout.info('POI name not given. Set to first poi "{}" by default.'.format(self.poi.GetName()))
         else:
             self.poi = self.model.get_poi(poi_name)
-            self.stdout.info('INFO: POI set to "{}"'.format(poi_name))
+            self.stdout.info('POI set to "{}"'.format(poi_name))
         
     def set_poi_value(self, val:float):
         if math.isnan(val):
             raise ValueError("cannot set poi to nan")
         if ( val > 0 ) and (self.poi.getMax() < val):
             self.poi.setMax(2*val)
         if ( val < 0 ) and (self.poi.getMin() > val):
@@ -184,22 +184,22 @@
     def get_nll_val(self, nll:"ROOT.RooNLLVar"):
         snapshot_name = self.nll_maps[nll].get('snapshot', None)
         if snapshot_name:
             self.load_snapshot(snapshot_name)
         else:
             raise RuntimeError(f'Failed to load snapshot for nll "{nll.GetName()}"')
         if Verbosity.DEBUG >= self.stdout.verbosity:
-            self.stdout.debug("DEBUG: Before Fit ----------------------------------------------")
+            self.stdout.debug("Before Fit ----------------------------------------------")
             self.model.print_summary(items=['poi', 'nuisance_parameter', 'global_observable'])
         self.last_fit_status = self.minimizer.minimize(nll) 
         self.global_status += self.last_fit_status
         self.minimizer_calls += 1
         nll_val = nll.getVal()
         if Verbosity.DEBUG >= self.stdout.verbosity:
-            self.stdout.debug("DEBUG: After Fit ----------------------------------------------")
+            self.stdout.debug("After Fit ----------------------------------------------")
             self.model.print_summary(items=['poi', 'nuisance_parameter', 'global_observable'])          
         self.load_snapshot(self.nom_glob_name)
         return nll_val
     
     def create_nll(self, dataset:"ROOT.RooDataSet"):
         return self.minimizer._create_nll(dataset=dataset)
         
@@ -245,16 +245,16 @@
         theta_extrap = m*mu + theta_mu2 - m*mu2
         for i, param in enumerate(self.nuis):
             param.setVal(theta_extrap[i])
             
     def get_limit(self, nll:"ROOT.RooNLLVar", initial_guess:float, summary_label:Optional[int]=None):
         self.global_status = 0
         nll_name = nll.GetName()
-        self.stdout.info("----------------------------------")
-        self.stdout.info(f"Getting limit for nll: {nll_name}")
+        self.stdout.info("----------------------------------", bare=True)
+        self.stdout.info(f"Getting limit for nll: {nll_name}", bare=True)
         self.poi.setConstant(0)
         asimov_0_nll = self.summary[0]['nll']
         if nll == asimov_0_nll:
             self.set_poi_value(self.mu_exp)
             self.poi.setConstant(1)
         # case for observed limit
         if (nll not in self.nll_maps) or ('nll_mu_hat' not in self.nll_maps[nll]):
@@ -280,34 +280,34 @@
         sigma_b = sigma_guess
         mu_guess = self.LimitTool.findCrossing(sigma_guess, sigma_b, mu_hat)
         pmu = self.LimitTool.calcPmu(qmu, sigma_b, mu_guess)
         pb = self.LimitTool.calcPb(qmu, sigma_b, mu_guess)
         CLs = self.LimitTool.calcCLs(qmu, sigma_b, mu_guess)
         qmu95 = self.LimitTool.getQmu95(sigma_b, mu_guess)
         self.set_poi_value(mu_guess)
-        self.stdout.info(f"Initial guess:  {mu_guess}")
-        self.stdout.info(f"Sigma(obs):     {sigma_guess}")
-        self.stdout.info(f"Sigma(mu,0):    {sigma_b}")
-        self.stdout.info(f"muhat:          {mu_hat}")
-        self.stdout.info(f"qmu95:          {qmu95}")
-        self.stdout.info(f"qmu:            {qmu}")
-        self.stdout.info(f"pmu:            {pmu}")
-        self.stdout.info(f"1-pb:           {pb}")
-        self.stdout.info(f"CLs:            {CLs}")
+        self.stdout.info(f"Initial guess:  {mu_guess}", bare=True)
+        self.stdout.info(f"Sigma(obs):     {sigma_guess}", bare=True)
+        self.stdout.info(f"Sigma(mu,0):    {sigma_b}", bare=True)
+        self.stdout.info(f"muhat:          {mu_hat}", bare=True)
+        self.stdout.info(f"qmu95:          {qmu95}", bare=True)
+        self.stdout.info(f"qmu:            {qmu}", bare=True)
+        self.stdout.info(f"pmu:            {pmu}", bare=True)
+        self.stdout.info(f"1-pb:           {pb}", bare=True)
+        self.stdout.info(f"CLs:            {CLs}", bare=True)
 
         n_damping = 1
         guess_to_corr = {}
         damping_factor = 1.0
         n_iter = 0
         mu_pre = mu_hat
         mu_pre2 = mu_hat
         
         while (abs(mu_pre-mu_guess) > self.precision*mu_guess):
-            self.stdout.info('----------------------------------')
-            self.stdout.info('Starting iteration {} of {}'.format(n_iter, nll_name))
+            self.stdout.info('----------------------------------', bare=True)
+            self.stdout.info(f'Starting iteration {n_iter} of {nll_name}', bare=True)
             # do this to avoid comparing multiple minima in the conditional and unconditional fits           
             if (n_iter == 0):
                 self.load_nll_snapshot(nll, mu_hat)
             elif self.use_predictive_fit:
                 self.do_predictive_fit(nll, mu_pre2, mu_pre, mu_guess)
             else:
                 self.load_nll_snapshot(asimov_0_nll, mu_pre)
@@ -334,15 +334,15 @@
                 sigma_b = sigma_guess
                 qmuA = qmu
             corr = damping_factor*(mu_guess - self.LimitTool.findCrossing(sigma_guess, sigma_b, mu_hat))
             for first, second in guess_to_corr.items():
                 if (abs(first - (mu_guess - corr)) < self.direction*mu_guess*0.02) and \
                 (abs(corr) > self.direction*mu_guess*self.precision):
                     damping_factor *= 0.8
-                    self.stdout.info('Changing damping factor to {}, n_damping = {}'.format(damping_factor, n_damping))
+                    self.stdout.info(f'Changing damping factor to {damping_factor}, n_damping = {n_damping}', bare=True)
                     n_damping += 1
                     if n_damping > 10:
                         n_damping = 1
                         damping_factor = 1.0
                     corr *= damping_factor
                     break
             # subtract off the difference in the new and damped correction
@@ -352,28 +352,28 @@
             mu_guess -= corr
 
             pmu = self.LimitTool.calcPmu(qmu, sigma_b, mu_pre)
             pb = self.LimitTool.calcPb(qmu, sigma_b, mu_pre)
             CLs = self.LimitTool.calcCLs(qmu, sigma_b, mu_pre)
             qmu95 = self.LimitTool.getQmu95(sigma_b, mu_pre)
             
-            self.stdout.info(f"NLL:            {nll_name}")
-            self.stdout.info(f"Previous guess: {mu_pre}")
-            self.stdout.info(f"Sigma(obs):     {sigma_guess}")
-            self.stdout.info(f"Sigma(mu,0):    {sigma_b}")
-            self.stdout.info(f"muhat:          {mu_hat}")
-            self.stdout.info(f"pmu:            {pmu}")
-            self.stdout.info(f"1-pb:           {pb}")
-            self.stdout.info(f"CLs:            {CLs}")
-            self.stdout.info(f"qmu95:          {qmu95}")
-            self.stdout.info(f"qmu:            {qmu}")
-            self.stdout.info(f"qmuA0:          {qmuA}")
-            self.stdout.info(f"Precision:      {self.direction*mu_guess*self.precision}")
-            self.stdout.info(f"Correction:     {-corr}")
-            self.stdout.info(f"New guess:      {mu_guess}")
+            self.stdout.info(f"NLL:            {nll_name}", bare=True)
+            self.stdout.info(f"Previous guess: {mu_pre}", bare=True)
+            self.stdout.info(f"Sigma(obs):     {sigma_guess}", bare=True)
+            self.stdout.info(f"Sigma(mu,0):    {sigma_b}", bare=True)
+            self.stdout.info(f"muhat:          {mu_hat}", bare=True)
+            self.stdout.info(f"pmu:            {pmu}", bare=True)
+            self.stdout.info(f"1-pb:           {pb}", bare=True)
+            self.stdout.info(f"CLs:            {CLs}", bare=True)
+            self.stdout.info(f"qmu95:          {qmu95}", bare=True)
+            self.stdout.info(f"qmu:            {qmu}", bare=True)
+            self.stdout.info(f"qmuA0:          {qmuA}", bare=True)
+            self.stdout.info(f"Precision:      {self.direction*mu_guess*self.precision}", bare=True)
+            self.stdout.info(f"Correction:     {-corr}", bare=True)
+            self.stdout.info(f"New guess:      {mu_guess}", bare=True)
             
             n_iter += 1
             if (n_iter > 25):
                 raise RuntimeError('infinite loop detected in get_limit()')
         
         if summary_label is not None:
             summary = {
@@ -392,16 +392,16 @@
                 'correction': -corr,
                 'status': self.global_status
             }
             if summary_label not in self.summary:
                 self.summary[summary_label] = summary
             else:
                 self.summary[summary_label].update(summary)
-        self.stdout.info('Found limit for nll {}: {}'.format(nll_name, mu_guess))
-        self.stdout.info('Finished in {} itreations'.format(n_iter))
+        self.stdout.info(f'Found limit for nll {nll_name}: {mu_guess}', bare=True)
+        self.stdout.info(f'Finished in {n_iter} itreations', bare=True)
         return mu_guess
     
     @staticmethod
     def get_approx_limits(median_limit:float, target_cls:float=0.05):
         limits = {}
         sigma = median_limit/math.sqrt(3.84)
         limits[0]  = median_limit
@@ -432,43 +432,43 @@
         self.nll_maps[nll]['mu_hat'] = mu_hat
         self.nll_maps[nll]['nll_mu_hat'] = nll_mu_hat
         self.dataset_maps[dataset] = nll
         
     def print_failures(self):
         has_failtures = any(self.summary[sigma].get('status', 0) > 0 for sigma in self.summary)
         if has_failtures:
-            self.stdout.info('-----------------------------------------------')
-            self.stdout.info('Unresolved fit failures detected')
+            self.stdout.info('-----------------------------------------------', bare=True)
+            self.stdout.info('Unresolved fit failures detected', bare=True)
             for sigma in self.summary:
                 label = self._SIGMA_LABEL_.get(sigma, sigma)
-                self.stdout.info("{}:".format(label).ljust(10) + str(self.summary[sigma].get('status', None)))
-            self.stdout.info('-----------------------------------------------')
+                self.stdout.info("{}:".format(label).ljust(10) + str(self.summary[sigma].get('status', None)), bare=True)
+            self.stdout.info('-----------------------------------------------', bare=True)
 
     def print_summary(self):
         if (not self.limits) or (not self.approx_limits):
             print("No limits evaluated")
             return None
         print('')
         self.print_failures()
         if self.do_better_bands:
-            self.stdout.info('Guess for bands')
-        self.stdout.info(f'+2sigma:  {self.approx_limits[2]}')
-        self.stdout.info(f'+1sigma:  {self.approx_limits[1]}')
-        self.stdout.info(f'-1sigma:  {self.approx_limits[-1]}')
-        self.stdout.info(f'-2sigma:  {self.approx_limits[-2]}')
+            self.stdout.info('Guess for bands', bare=True)
+        self.stdout.info(f'+2sigma:  {self.approx_limits[2]}', bare=True)
+        self.stdout.info(f'+1sigma:  {self.approx_limits[1]}', bare=True)
+        self.stdout.info(f'-1sigma:  {self.approx_limits[-1]}', bare=True)
+        self.stdout.info(f'-2sigma:  {self.approx_limits[-2]}', bare=True)
         if self.do_better_bands:
-            self.stdout.info('\nCorrect bands')
-            self.stdout.info(f'+2sigma:  {self.limits[2]}')
-            self.stdout.info(f'+1sigma:  {self.limits[1]}')
-            self.stdout.info(f'-1sigma:  {self.limits[-1]}')
-            self.stdout.info(f'-2sigma:  {self.limits[-2]}')
-        self.stdout.info('Injected: {}'.format(self.limits['inj']))
-        self.stdout.info(f'Median:   {self.limits[0]}')
-        self.stdout.info('Observed: {}'.format(self.limits['obs']))
-        self.stdout.info('')
+            self.stdout.info('\nCorrect bands', bare=True)
+            self.stdout.info(f'+2sigma:  {self.limits[2]}', bare=True)
+            self.stdout.info(f'+1sigma:  {self.limits[1]}', bare=True)
+            self.stdout.info(f'-1sigma:  {self.limits[-1]}', bare=True)
+            self.stdout.info(f'-2sigma:  {self.limits[-2]}', bare=True)
+        self.stdout.info('Injected: {}'.format(self.limits['inj']), bare=True)
+        self.stdout.info(f'Median:   {self.limits[0]}', bare=True)
+        self.stdout.info('Observed: {}'.format(self.limits['obs']), bare=True)
+        self.stdout.info('', bare=True)
         
     def save(self, filename:str='limits.json', parameters:Optional[Dict]=None, summary:bool=False):
         with open(filename, "w") as file:
             if parameters is None:
                 json.dump(self.limits, file, indent=2)
             else:
                 json.dump({**parameters, **self.limits}, file, indent=2)
@@ -488,15 +488,15 @@
             self.direction = -1
             self.LimitTool.setDirection(-1)
         asimov_0_nll = self.summary[0]['nll']
         mu_guess = n*med_limit/math.sqrt(3.84)
         n_times_sigma = self.get_limit(asimov_0_nll, mu_guess)
         status = self.global_status
         sigma = n_times_sigma/n
-        self.stdout.info('Found N * sigma = {} * {}'.format(n, sigma))
+        self.stdout.info(f'Found N * sigma = {n} * {sigma}', bare=True)
         snapshot_0_name = self.nll_maps[asimov_0_nll]['snapshot']
         self.load_snapshot(snapshot_0_name)
         asimov_data_n = self.model.generate_asimov(self.poi.GetName(), poi_val=n_times_sigma,
                                                    do_fit=False, modify_globs=True,
                                                    restore_states=1,
                                                    minimizer_options=self.default_minimizer_options,
                                                    nll_options=self.default_nll_options)
@@ -527,15 +527,15 @@
         self.dataset_maps[self.data] = obs_nll
         self.save_snapshot(self.nom_glob_name, variables=WSArgument.GLOBAL_OBSERVABLE)
         self.save_snapshot(self.nom_nuis_name, variables=WSArgument.NUISANCE_PARAMETER)
         
         if self.asimov_data_0 is None:
             # generate asimov dataset on the fly
             fit_text = "postfit" if not self.do_blind else "nominal"
-            self.stdout.info(f"INFO: Generating asimov dataset with mu = {pretty_value(self.mu_exp)} using {fit_text} NP values")
+            self.stdout.info(f"Generating asimov dataset with mu = {pretty_value(self.mu_exp)} using {fit_text} NP values")
             asimov_data_0 = self.model.generate_asimov(self.poi.GetName(),
                                                        poi_val=self.mu_exp,
                                                        poi_profile=self.mu_exp, 
                                                        do_fit=not self.do_blind,
                                                        modify_globs=not self.do_blind,
                                                        dataset=self.data,
                                                        restore_states=1,
@@ -578,27 +578,26 @@
             limits[n] = self.evaluate_limit_band(n, med_limit)
         
         # compute observed limit
         self.load_conditional_snapshot(self.mu_exp, target=WSArgument.NUISANCE_PARAMETER)
         # relax the range for observed limit
         if not self.adjust_fit_range:
             self.poi.setRange(poi_range_tmp[0], poi_range_tmp[1])
-
         obs_limit = 0 if self.do_blind else self.get_limit(obs_nll, med_limit, 'obs')
         limits['obs'] = obs_limit
         
         # injection test not supported yet
         limits['inj'] = 0
         
         self.limits = limits
         self.approx_limits = approx_limits
         
         self.print_summary()
         
-        self.stdout.info(f'INFO: Finished with {self.minimizer_calls} calls to minimize(nll)')
+        self.stdout.info(f'Finished with {self.minimizer_calls} calls to minimize(nll)')
         return limits
 
     def evaluate_cls(self, poi:float):
         # TODO: maybe load nominal snapshot first
         self.reset()
         self.save_snapshot(self.nom_glob_name, variables="globs")
         self.save_snapshot(self.nom_nuis_name, variables="nuis")
@@ -614,24 +613,24 @@
         self.save_nll_snapshot(asimov_0_nll, 0)
         self.load_conditional_snapshot(0, target="globs")
         self.load_conditional_snapshot(0, target="nuis")
         nll_value = asimov_0_nll.getVal()
         self.fill_mappings(asimov_0_nll, asimov_data_0, 0, nll_value)
         
         nll_name = asimov_0_nll.GetName()
-        self.stdout.info("----------------------------------")
-        self.stdout.info(f"Getting CLs for nll: {nll_name}")
+        self.stdout.info("----------------------------------", bare=True)
+        self.stdout.info(f"Getting CLs for nll: {nll_name}", bare=True)
         
         qmu = self.get_qmu(asimov_0_nll, poi)
         sigma= self.LimitTool.getSigma(poi, 0, qmu)
         pmu = self.LimitTool.calcPmu(qmu, sigma, poi)
         pb = self.LimitTool.calcPb(qmu, sigma, poi)
         CLs = self.LimitTool.calcCLs(qmu, sigma, poi)
         qmu95 = self.LimitTool.getQmu95(sigma, poi)
-        self.stdout.info(f"POI:            {poi}")
-        self.stdout.info(f"Sigma:          {sigma}")
-        self.stdout.info(f"NLL(muhat):     {nll_value}")
-        self.stdout.info(f"qmu95:          {qmu95}")
-        self.stdout.info(f"qmu:            {qmu}")
-        self.stdout.info(f"pmu:            {pmu}")
-        self.stdout.info(f"1-pb:           {pb}")
-        self.stdout.info(f"CLs:            {CLs}")
+        self.stdout.info(f"POI:            {poi}", bare=True)
+        self.stdout.info(f"Sigma:          {sigma}", bare=True)
+        self.stdout.info(f"NLL(muhat):     {nll_value}", bare=True)
+        self.stdout.info(f"qmu95:          {qmu95}", bare=True)
+        self.stdout.info(f"qmu:            {qmu}", bare=True)
+        self.stdout.info(f"pmu:            {pmu}", bare=True)
+        self.stdout.info(f"1-pb:           {pb}", bare=True)
+        self.stdout.info(f"CLs:            {CLs}", bare=True)
```

### Comparing `quickstats-0.6.7.8/quickstats/components/basics.py` & `quickstats-0.6.8.1/quickstats/components/basics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/extended_minimizer.py` & `quickstats-0.6.8.1/quickstats/components/extended_minimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         self.fit_options = {}
         self.scan_options = {}
         #self.nll_command_list = ROOT.RooLinkedList()
         self.nll_commands = {}
         
         self.configure_default_minimizer_options()
         
-        self.stdout.info(f'INFO: Created ExtendedMinimizer("{self.name}") instance')
+        self.stdout.info(f'Created ExtendedMinimizer("{self.name}") instance')
         
     @property
     def data(self):
         return self._data
     
     @data.setter
     def data(self, val):
@@ -156,46 +156,46 @@
                     observable = pdf_cat.getObservables(dataset).first()
                     range_name = f"{named_range}_{cat_label}"
                     if observable.hasRange(range_name):
                         value_range = observable.getRange(range_name)
                         observable.setRange(named_range, value_range[0], value_range[1])
             index = [i for i, cmd in enumerate(nll_commands) if cmd.GetName() == "SplitRange"][0]
             nll_commands.pop(index)
-            self.stdout.warning("WARNING: Renamed observable ranges to fix a bug in ROOT")
+            self.stdout.warning("Renamed observable ranges to fix a bug in ROOT")
     
     def _create_nll(self, nll_commands:List["ROOT.RooCmdArg"]=None, 
                     dataset:Optional["ROOT.RooDataSet"]=None):
         if nll_commands is None:
             nll_commands = list(self.nll_commands.values())
         #self.nll = self.pdf.createNLL(self.data, nll_command_list)
         for command in nll_commands:
             if command.GetName() == "RangeWithName":
                 range_name = command.getString(0)
-                self.stdout.info(f"INFO: Using the range \"{range_name}\" for NLL calculation")
+                self.stdout.info(f"Using the range \"{range_name}\" for NLL calculation")
         if dataset is None:
             dataset = self.data
         
         if quickstats.root_version >= (6, 26, 0):
             self._bug_fix_create_nll(dataset, nll_commands)
             nll = self.pdf.createNLL(dataset, *nll_commands)
         else:
             if len(nll_commands) <= 6:
                 nll = self.pdf.createNLL(dataset, *nll_commands)
             # bug: can't have more than 6 arguments
             elif len(nll_commands) == 7:
                 reduced_command_list = [i for i in nll_commands if i.GetName() != 'NumCPU']
-                self.stdout.warning("WARNING: Maximum number (6) of NLL commands reached. "
+                self.stdout.warning("Maximum number (6) of NLL commands reached. "
                                     "Will remove `NumCPU` from the command list")
                 if len(reduced_command_list) <= 6:
                     nll = self.pdf.createNLL(dataset, *reduced_command_list)
                 else:
                     raise RuntimeError("due to a bug in ROOT, nll can not have more than 6 arguments")
             elif len(nll_commands) == 8:
                 reduced_command_list = [i for i in nll_commands if i.GetName() not in ['NumCPU', 'IntegrateBins']]
-                self.stdout.warning("WARNING: Maximum number (6) of NLL commands reached. "
+                self.stdout.warning("Maximum number (6) of NLL commands reached. "
                                     "Will remove `NumCPU` and `IntegrateBins` from the command list")
                 if len(reduced_command_list) <= 6:
                     nll = self.pdf.createNLL(dataset, *reduced_command_list)
                 else:
                     raise RuntimeError("due to a bug in ROOT, nll can not have more than 6 arguments")
             else:
                 raise RuntimeError("due to a bug in ROOT, nll can not have more than 6 arguments")
@@ -330,15 +330,15 @@
                     
         self.create_minimizer()
         status = 0
         attached_set = self.nll.getVariables()
         perform_minimization = any(not attached.isConstant() for attached in attached_set)
 
         if not perform_minimization:
-            self.stdout.info('INFO: ExtendedMinimizer::minimize("{}") no floating parameters found'
+            self.stdout.info('ExtendedMinimizer::minimize("{}") no floating parameters found'
                          '-- skipping minimization'.format(self.name))
         else:
             status = self.robust_minimize()
 
         # Evaluate errors with improve
         if self.config['improve']:
             self.minimizer.improve()
@@ -371,15 +371,15 @@
         if self.config['scan']:
             self.find_sigma()
 
         if self.config['save']:
             data_name = self.data.GetName()
             save_name = "fitresult_{}_{}".format(self.name, data_name)
             save_title = "Result of fit of p.d.f. {} to dataset {}".format(self.name, data_name)
-            self.stdout.info('INFO: ExtendedMinimizer::minimize("{}") saving results as {}'.format(self.name, save_name))
+            self.stdout.info('ExtendedMinimizer::minimize("{}") saving results as {}'.format(self.name, save_name))
             self.fit_result = self.minimizer.save(save_name, save_title)
         # if the 'scan' option is used, minimizer will get deleted before this line
         elif self.minimizer is not None:
             self.fit_result = self.minimizer.save()
 
         if self.cond_set.size() > 0:
             attached_set = self.nll.getVariables()
@@ -518,15 +518,15 @@
             eps = 0.001 * tol
             precision = 5.0*eps / (n_sigma**2)
         
         temp_options = {**scan_options}
         snapshot = self.cond_set.snapshot()
         for i in range(max_iter):
             self.stdout.info(f'{front_str} Parameter {par.GetName()} {n_sigma}sigma '
-                             f'iteration {i + 1}: start {val_guess} (MLE{val_guess - val_mle})')
+                             f'iteration {i + 1}: start {val_guess} (MLE{val_guess - val_mle})', bare=True)
             val_pre = val_guess
             
             poi_set = ROOT.RooArgSet(par).snapshot()
             poi_set.first().setVal(val_guess)
             
             scan_options['reuse_nll'] = 1
             scan_options['scan']      = 0
@@ -549,15 +549,15 @@
                 sigma_guess *= 10.0 # protect against t_mu <=0 and also don't move too far
             
             corr = damping_factor*(val_pre - val_mle - n_sigma*sigma_guess)
             
             for guess in guess_to_corr:
                 if (abs(guess - val_pre) < direction*val_pre*0.02):
                     damping_factor *= 0.8
-                    self.stdout.info(f'{front_str} Changing damping factor to {damping_factor}')
+                    self.stdout.info(f'{front_str} Changing damping factor to {damping_factor}', bare=True)
                     n_damping += 1
                     if n_damping > 10:
                         n_damping = 1
                         damping_factor = 1.0
                     corr *= damping_factor
                     break
             
@@ -568,35 +568,35 @@
             rel_precision = precision*abs(val_guess-val_mle)
             delta = val_guess - val_pre
             
             
             self.stdout.info('{} {} {:.3f} (MLE {:.3f}) -> {:.3f} (MLE {:.3f}), '
                              'change {:.3f}, precision {:.3f}, -2lnL {:.4f}, sigma(guess) {:.3f})'.format(
                              front_str, param_name, val_pre, val_pre - val_mle, val_guess, val_guess - val_mle,
-                             delta, rel_precision, t_mu, sigma_guess))
-            self.stdout.info('{} NLL:                 {}'.format(front_str, nll))
-            self.stdout.info('{} delta(NLL):          {}'.format(front_str, nll - nll_min))
-            self.stdout.info('{} nsigma*sigma(pre):   {}'.format(front_str, abs(val_pre - val_mle)))
-            self.stdout.info('{} sigma(guess):        {}'.format(front_str, sigma_guess))
-            self.stdout.info('{} par(guess):          {}'.format(front_str, val_guess + corr))
-            self.stdout.info('{} best-fit val:        {}'.format(front_str, val_mle))
-            self.stdout.info('{} tmu:                 {}'.format(front_str, t_mu))
-            self.stdout.info('{} Precision:           {}'.format(front_str, direction*val_guess*precision))
-            self.stdout.info('{} Correction:          {}'.format(front_str, -corr))
-            self.stdout.info('{} nsigma*sigma(guess): {}'.format(front_str, abs(val_guess-val_mle)))
+                             delta, rel_precision, t_mu, sigma_guess), bare=True)
+            self.stdout.info('{} NLL:                 {}'.format(front_str, nll), bare=True)
+            self.stdout.info('{} delta(NLL):          {}'.format(front_str, nll - nll_min), bare=True)
+            self.stdout.info('{} nsigma*sigma(pre):   {}'.format(front_str, abs(val_pre - val_mle)), bare=True)
+            self.stdout.info('{} sigma(guess):        {}'.format(front_str, sigma_guess), bare=True)
+            self.stdout.info('{} par(guess):          {}'.format(front_str, val_guess + corr), bare=True)
+            self.stdout.info('{} best-fit val:        {}'.format(front_str, val_mle), bare=True)
+            self.stdout.info('{} tmu:                 {}'.format(front_str, t_mu), bare=True)
+            self.stdout.info('{} Precision:           {}'.format(front_str, direction*val_guess*precision), bare=True)
+            self.stdout.info('{} Correction:          {}'.format(front_str, -corr), bare=True)
+            self.stdout.info('{} nsigma*sigma(guess): {}'.format(front_str, abs(val_guess-val_mle)), bare=True)
             
             if abs(delta) <= rel_precision:
                 break
         if i >= max_iter:
-            self.stdout.error(f'ERROR: find_sigma failed after {i + 1} iterations')
+            self.stdout.error(f'find_sigma failed after {i + 1} iterations')
             return ROOT.TMath.QuietNan()
         
         err = val_guess - val_mle
         self.stdout.info('{} {} {}sigma = {:.3F} at -2lnL = {:4f} after {} iterations'.format(
-                         front_str, par.GetName(), n_sigma, err, t_mu, i+1))
+                         front_str, par.GetName(), n_sigma, err, t_mu, i+1), bare=True)
         
         return err
     
     def create_profile(self, var:"ROOT.RooRealVar", lo:float, hi:float, n_bins:int):
         map_poi2nll = {}
         
         ROOT.Math.MinimizerOptions.SetDefaultPrintLevel(-1)
```

### Comparing `quickstats-0.6.7.8/quickstats/components/extended_model.py` & `quickstats-0.6.8.1/quickstats/components/extended_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,122 +132,120 @@
         if val is None:
             self._initial_snapshots = []
         elif isinstance(val, str):
             self._initial_snapshots = split_str(val, sep=',', remove_empty=True)
         elif isinstance(val, list):
             self._initial_snapshots = val
         else:
-            raise ValueError("\"initial_snapshots\" must be string or list of strings")
+            raise ValueError('"initial_snapshots" must be string or list of strings')
     
     @semistaticmethod
     def load_extension(self):
         extensions = quickstats.get_workspace_extensions()
         for extension in extensions:
             result = load_macro(extension)
             if (result is not None) and hasattr(ROOT, extension):
-                self.stdout.info(f'INFO: Loaded extension module "{extension}"')
+                self.stdout.info(f'Loaded extension module "{extension}"')
         
     @semistaticmethod
     def modify_interp_codes(self, ws, interp_code, classes=None):
         if classes is None:
             classes = [ROOT.RooStats.HistFactory.FlexibleInterpVar, ROOT.PiecewiseInterpolation]
         for component in ws.components():
             for cls in classes:
                 if (component.IsA() == cls.Class()):
                     component.setAllInterpCodes(interp_code)
                     class_name = cls.Class_Name().split('::')[-1]
-                    self.stdout.info('INFO: {} {} interpolation code set to {}'.format(component.GetName(),
-                                                                            class_name,
-                                                                            interp_code))
+                    self.stdout.info(f'{component.GetName()} {class_name} interpolation code set to {interp_code}')
         return None           
 
     @semistaticmethod
     def activate_binned_likelihood(self, ws):
         for component in ws.components():
             try:
                 # A pdf is binned if it has attribute "BinnedLikelihood" and it is a RooRealSumPdf (or derived class).
                 flag = component.IsA().InheritsFrom(ROOT.RooRealSumPdf.Class())
             except:
                 flag = (component.ClassName() == "RooRealSumPdf")
             if (flag):
                 component.setAttribute('BinnedLikelihood')
-                self.stdout.info('INFO: Activated binned likelihood attribute for {}'.format(component.GetName()))
+                self.stdout.info(f'Activated binned likelihood attribute for {component.GetName()}')
         return None
                           
     @semistaticmethod
     def set_measurement(self, ws, condition):
         for component in ws.components():
             name = component.GetName()
             try:
                 flag = (component.IsA() == ROOT.RooAddPdf.Class())
             except:
                 flag = (component.ClassName() == "RooAddPdf")
             if flag and condition(name):
                 component.setAttribute('MAIN_MEASUREMENT')
-                self.stdout.info('INFO: Activated main measurement attribute for {}'.format(name))
+                self.stdout.info(f'Activated main measurement attribute for {name}')
         return None
     
     @semistaticmethod
     def deactivate_lv2_const_optimization(self, ws, condition):
-        self.stdout.info('INFO: Deactivating level 2 constant term optimization for specified pdfs')
+        self.stdout.info('Deactivating level 2 constant term optimization for specified pdfs')
         for component in ws.components():
             name = component.GetName()
             if (component.InheritsFrom(ROOT.RooAbsPdf.Class()) and condition(name)):
                 component.setAttribute("NOCacheAndTrack")
-                self.stdout.info('INFO: Deactivated level 2 constant term optimization for {}'.format(name))
+                self.stdout.info(f'Deactivated level 2 constant term optimization for {name}')
                 
     def load_snapshots(self, snapshot_names:List[str]):
         for snapshot_name in snapshot_names:
             if self.workspace.getSnapshot(snapshot_name):
                 self.workspace.loadSnapshot(snapshot_name)
-                self.stdout.info(f'INFO: Loaded snapshot "{snapshot_name}"')
+                self.stdout.info(f'Loaded snapshot "{snapshot_name}"')
             else:
-                self.stdout.warning(f'WARNING: Failed to load snapshot "{snapshot_name}"')
+                self.stdout.warning(f'Failed to load snapshot "{snapshot_name}"')
             
     def initialize(self):
         if isinstance(self.fname, str):
             if not os.path.exists(self.fname):
                 raise FileNotFoundError(f'workspace file "{self.fname}" does not exist')
-            self.stdout.info(f'INFO: Opening file "{self.fname}"')
+            self.stdout.info(f'Opening file "{self.fname}"')
             file = ROOT.TFile(self.fname) 
             if (not file):
                 raise RuntimeError(f"Something went wrong while loading the root file: {self.fname}")
             # load workspace
             if self.ws_name is None:
                 ws_names = [i.GetName() for i in file.GetListOfKeys() if i.GetClassName() == 'RooWorkspace']
                 if not ws_names:
                     raise RuntimeError(f"No workspaces found in the root file: {self.fname}")
                 if len(ws_names) > 1:
-                    self.stdout.warning("WARNING: Found multiple workspace instances from the root file: "
+                    self.stdout.warning("Found multiple workspace instances from the root file: "
                                         f"{self.fname}. Available workspaces are \"{','.join(ws_names)}\". "
                                         f"Will choose the first one by default")
                 self.ws_name = ws_names[0]
             ws = file.Get(self.ws_name)
         elif isinstance(self.fname, ROOT.RooWorkspace):
             file = None
             ws = self.fname
         if not ws:
             raise RuntimeError(f'failed to load workspace "{self.ws_name}"')
         self.ws_name = ws.GetName()
-        self.stdout.info(f'INFO: Loaded workspace "{self.ws_name}"')
+        self.stdout.info(f'Loaded workspace "{self.ws_name}"')
         
         # load model config
         if self.mc_name is None:
             mc_names = [i.GetName() for i in ws.allGenericObjects() if 'ModelConfig' in i.ClassName()]
             if not mc_names:
                 raise RuntimeError(f"no ModelConfig object found in the workspace: {ws_name}")
             if len(mc_names) > 1:
-                self.stdout.warning(f"WARNING: Found multiple ModelConfig instances from the workspace: {ws_name}. "
+                self.stdout.warning(f"Found multiple ModelConfig instances from the workspace: {ws_name}. "
                                     f"Available ModelConfigs are \"{','.join(mc_names)}\". "
                                     "Will choose the first one by default")
             self.mc_name = mc_names[0]
         model_config = ws.obj(self.mc_name)
         if not model_config:
             raise RuntimeError(f'failed to load model config "{self.mc_name}"')
-        self.stdout.info(f'INFO: Loaded model config "{self.mc_name}"')
+        self.stdout.info(f'Loaded model config "{self.mc_name}"')
             
         # modify interpolation code
         if self.interpolation_code != -1:
             self.modify_interp_codes(ws, self.interpolation_code,
                                      classes=[ROOT.RooStats.HistFactory.FlexibleInterpVar, ROOT.PiecewiseInterpolation])
         
         # activate binned likelihood
@@ -262,62 +260,62 @@
             self.deactivate_lv2_const_optimization(ws, 
                 condition=lambda name: (name.endswith('_mm') and 'mumu_atlas' in name))
 
         # load pdf
         pdf = model_config.GetPdf()
         if not pdf:
             raise RuntimeError('Failed to load pdf')
-        self.stdout.info(f'INFO: Loaded model pdf "{pdf.GetName()}" from model config')
+        self.stdout.info(f'Loaded model pdf "{pdf.GetName()}" from model config')
              
         # load dataset
         if self.data_name is None:
             data_names = [i.GetName() for i in ws.allData()]
             if not data_names:
                 raise RuntimeError(f"no datasets found in the workspace: {ws.GetName()}")
             self.data_name = data_names[0]
         data = ws.data(self.data_name)
         # in case there is a bug in hash map
         if not data:
             data = [i for i in ws.allData() if i.GetName() == self.data_name]
             if not data:
-                raise RuntimeError(f'failed to load dataset \"{self.data_name}\"')
+                raise RuntimeError(f'failed to load dataset "{self.data_name}"')
             data = data[0]
-        self.stdout.info('INFO: Loaded dataset "{}" from workspace'.format(data.GetName()))
+        self.stdout.info(f'Loaded dataset "{data.GetName()}" from workspace')
                 
         # load nuisance parameters
         nuisance_parameters = model_config.GetNuisanceParameters()
         if not nuisance_parameters:
             #raise RuntimeError('Failed to load nuisance parameters')
-            self.stdout.warning("WARNING: No nuisance parameters found in the workspace. "
+            self.stdout.warning("No nuisance parameters found in the workspace. "
                                 "An empty set will be loaded by default.")
             nuisance_parameters = ROOT.RooArgSet()
             model_config.SetNuisanceParameters(nuisance_parameters)
         else:
-            self.stdout.info('INFO: Loaded nuisance parameters from model config')
+            self.stdout.info('Loaded nuisance parameters from model config')
                 
         # Load global observables
         global_observables = model_config.GetGlobalObservables()
         if not global_observables:
-            self.stdout.warning("WARNING: No global observables found in the workspace. "
+            self.stdout.warning("No global observables found in the workspace. "
                                 "An empty set will be loaded by default.")            
             global_observables = ROOT.RooArgSet()
         else:
-            self.stdout.info('INFO: Loaded global observables from model config')                  
+            self.stdout.info('Loaded global observables from model config')                  
     
         # Load POIs
         pois = model_config.GetParametersOfInterest()
         if not pois:
             raise RuntimeError('Failed to load parameters of interest')
-        self.stdout.info('INFO: Loaded parameters of interest from model config')
+        self.stdout.info('Loaded parameters of interest from model config')
                                   
         # Load observables
         observables = model_config.GetObservables()
         if not observables:
             raise RuntimeError('Failed to load observables')     
-        self.stdout.info('INFO: Loaded observables from model config')
+        self.stdout.info('Loaded observables from model config')
         
         # get categories in case pdf is RooSimultaneous
         if pdf.ClassName() == "RooSimultaneous":
             category = pdf.indexCat()
         else:
             category = None
         """
@@ -351,15 +349,15 @@
                                        source:Optional["ROOT.RooArgSet"]=None,
                                        mode:Union[str, SetValueMode]=SetValueMode.UNCHANGED):
         if source is None:
             source = self.workspace.allVars()
         param_dict = self.parse_param_expr(param_expr)
         parameters = self._set_parameters(source, param_dict, mode=mode)
         if not parameters:
-            self.stdout.warning("WARNING: No parameters are modified from the given fix / profile expression", "red")
+            self.stdout.warning("No parameters are modified from the given fix / profile expression", "red")
         return parameters
         
     def fix_parameters(self, param_expr:Optional[str]=None, source:Optional["ROOT.RooArgSet"]=None):
         return self.set_parameters_with_expression(param_expr, source, mode=SetValueMode.FIX)
     
     def profile_parameters(self, param_expr:Optional[str]=None, source:Optional["ROOT.RooArgSet"]=None):
         return self.set_parameters_with_expression(param_expr, source, mode=SetValueMode.FREE)
@@ -376,33 +374,33 @@
                 selected_params = [sname for sname in source_names if fnmatch.fnmatch(sname, name)]
             if not selected_params:
                 # check the possibility that the parameter is not a variable
                 param = self.workspace.obj(name)
                 if param:
                     selected_params = [param]
                 else:
-                    self.stdout.warning(f'WARNING: Parameter "{name}" does not exist. No modification will be made.', "red")
+                    self.stdout.warning(f'Parameter "{name}" does not exist. No modification will be made.', "red")
             for param in selected_params:
                 if isinstance(param, str):
                     param = source[param]
                 self._set_parameter(param, param_dict[name], mode=mode)
                 selected_parameters.append(param)
         return selected_parameters
 
     def _set_parameter(self, param:"ROOT.RooRealVar", value:Union[float, int, List, Tuple], 
                        mode:Union[str, SetValueMode]=SetValueMode.UNCHANGED):
         mode = SetValueMode.parse(mode)
         name = param.GetName()
         if not isinstance(param, ROOT.RooRealVar):
             if mode == SetValueMode.FIX:
                 param.setConstant(1)
-                self.stdout.info(f"INFO: Fixed object \"{name}\" as constant.")
+                self.stdout.info(f"Fixed object \"{name}\" as constant.")
             elif mode == SetValueMode.FREE:
                 param.setConstant(0)
-                self.stdout.info(f"INFO: Float object \"{name}\".")
+                self.stdout.info(f"Float object \"{name}\".")
             return None
         old_value = param.getVal()
         new_value = old_value
         if isinstance(value, (float, int)):
             new_value = value
         elif isinstance(value, (list, tuple)):
             if len(value) == 3:
@@ -432,23 +430,23 @@
                 if (v_max == 0) and (old_value > 0):
                     new_value = -abs(old_value)
                 param.setMax(v_max)
         if new_value != old_value:
             param.setVal(new_value)
         if mode == SetValueMode.FIX:
             param.setConstant(1)
-            self.stdout.info(f"INFO: Fixed parameter \"{name}\" at value {param.getVal()} "
+            self.stdout.info(f"Fixed parameter \"{name}\" at value {param.getVal()} "
                              f"[{param.getMin()}, {param.getMax()}]")
         elif mode == SetValueMode.FREE:
             param.setConstant(0)
-            self.stdout.info(f"INFO: Float parameter \"{name}\" at value {param.getVal()} "
+            self.stdout.info(f"Float parameter \"{name}\" at value {param.getVal()} "
                              f"[{param.getMin()}, {param.getMax()}]")
         else:
             state_str = "C" if param.isConstant() else "F"
-            self.stdout.info(f"INFO: Set parameter \"{name}\" at value {param.getVal()} "
+            self.stdout.info(f"Set parameter \"{name}\" at value {param.getVal()} "
                              f"[{param.getMin()}, {param.getMax()}] {state_str}")
 
     def set_parameter_defaults(self, source:"ROOT.RooArgSet", value:float=None, error:float=None,
                                constant:bool=None, remove_range:bool=None, target:List[str]=None):
         for param in source:
             if (not target) or (param.GetName() in target):
                 if remove_range:
@@ -561,16 +559,17 @@
                 nuis.setConstant(1)
     
     def get_all_constraints(self, pdf:Optional[ROOT.RooAbsPdf]=None, cache:bool=True):
         if pdf is None:
             pdf = self.pdf
         all_constraints = ROOT.RooArgSet()
         if self.data is not None:
-            cache_name = "CACHE_CONSTR_OF_PDF_{}_FOR_OBS_{}".format(self.pdf.GetName(), 
-                         ROOT.RooNameSet(self.data.get()).content())
+            obs_set = self.data.get()
+            obs_str = ":".join([obs.GetName() for obs in obs_set])
+            cache_name = "CACHE_CONSTR_OF_PDF_{}_FOR_OBS_{}".format(self.pdf.GetName(), obs_str)
         else:
             cache_name = ""
         constr_cache = self.workspace.set(cache_name)
         if constr_cache and cache:
             # retrieve constrains from cache     
             all_constraints.add(constr_cache)
         else:
@@ -623,27 +622,27 @@
                             for server in constraint.servers():
                                 if (server != glob_obs) and (server != nuis):
                                     old_sigma_value = server.getVal()
                                     found_sigma = ROOT.kTRUE
                             if math.isclose(old_sigma_value, 1.0, abs_tol=0.001):
                                 old_sigma_value = 1.0
                             if not found_sigma:
-                                self.stdout.info(f'INFO: Sigma for pdf {constr_name} not found. Uisng 1.0.')
+                                self.stdout.info(f'Sigma for pdf {constr_name} not found. Uisng 1.0.')
                             else:
-                                self.stdout.info(f'INFO: Uisng {old_sigma_value} for sigma of pdf {constr_name}')
+                                self.stdout.info(f'Uisng {old_sigma_value} for sigma of pdf {constr_name}')
 
                             prefit_variation = old_sigma_value
                         elif constraint.IsA() == ROOT.RooPoisson.Class():
                             constraint_type = 'pois'
                             tau = glob_obs.getVal()
-                            self.stdout.info(f'INFO: Found tau {constr_name} of pdf')
+                            self.stdout.info(f'Found tau {constr_name} of pdf')
                             prefit_variation = 1. / math.sqrt(tau)
-                            self.stdout.info(f'INFO: Prefit variation is {prefit_variation}')
+                            self.stdout.info(f'Prefit variation is {prefit_variation}')
                             nuip_nom = 1.0
-                            self.stdout.info(f"INFO: Assume that {nuip_nom} is nominal value of the nuisance parameter")
+                            self.stdout.info(f"Assume that {nuip_nom} is nominal value of the nuisance parameter")
         return prefit_variation, constraint_type, nuip_nom
     
     def create_blind_range(self, blind_range:List[float], categories:Optional[List[str]]=None):
         """Create blind ranges for observables
         
         Arguments
             blind_range: list of float
@@ -674,18 +673,18 @@
             _range_name_SBLo  = f"{range_name_SBLo}_{category}"
             _range_name_Blind = f"{range_name_Blind}_{category}"
             _range_name_SBHi  = f"{range_name_SBHi}_{category}"            
             obs.setRange(_range_name_SBLo, obs_min, blind_min)
             obs.setRange(_range_name_Blind, blind_min, blind_max)
             obs.setRange(_range_name_SBHi, blind_max, obs_max)
             cat_padding = padding + len(category)
-            self.stdout.info(f"INFO: The following ranges are defined for the observable \"{obs_name}\"")
-            self.stdout.info(f"\t{_range_name_SBLo.ljust(cat_padding)}: [{obs_min}, {blind_min}]")
-            self.stdout.info(f"\t{_range_name_Blind.ljust(cat_padding)}: [{blind_min}, {blind_max}]")
-            self.stdout.info(f"\t{_range_name_SBHi.ljust(cat_padding)}: [{blind_max}, {obs_max}]")
+            self.stdout.info(f"The following ranges are defined for the observable \"{obs_name}\"")
+            self.stdout.info(f"\t{_range_name_SBLo.ljust(cat_padding)}: [{obs_min}, {blind_min}]", bare=True)
+            self.stdout.info(f"\t{_range_name_Blind.ljust(cat_padding)}: [{blind_min}, {blind_max}]", bare=True)
+            self.stdout.info(f"\t{_range_name_SBHi.ljust(cat_padding)}: [{blind_max}, {obs_max}]", bare=True)
         return None
     
     def get_sideband_range_name(self):
         """Get sideband range name to be used in RooAbsPdf.createNLL(..., Range(<range_name>))
         """
         range_name_SBLo = self._DEFAULT_NAMES_['range_sideband_low']
         range_name_SBHi = self._DEFAULT_NAMES_['range_sideband_high']
@@ -731,27 +730,27 @@
             obs = self.workspace.var(obs_name)
             obs_range = obs.getRange()
             obs_min = obs_range.first
             obs_max = obs_range.second            
             obs.setRange(range_name_SBLo, obs_min, obs_max)
             obs.setRange(range_name_Blind, obs_min, obs_max)
             obs.setRange(range_name_SBHi, obs_min, obs_max)
-            self.stdout.info(f"INFO: The following ranges are removed from the observable \"{obs_name}\":")
-            self.stdout.info(f"\t{range_name_SBLo}, {range_name_Blind}, {range_name_SBHi}")
+            self.stdout.info(f"The following ranges are removed from the observable \"{obs_name}\":")
+            self.stdout.info(f"\t{range_name_SBLo}, {range_name_Blind}, {range_name_SBHi}", bare=True)
     
     def set_initial_errors(self, source:Optional["ROOT.RooArgSet"]=None):
         if not source:
             source = self.nuisance_parameters
     
         all_constraints = self.get_all_constraints()
         for nuis in source:
             nuis_name = nuis.GetName()
             prefit_variation, constraint_type, _ = self.inspect_constrained_nuisance_parameter(nuis, all_constraints)
             if constraint_type=='gaus':
-                self.stdout.info(f'INFO: Changing error of {nuis_name} from {nuis.getError()} to {prefit_variation}')
+                self.stdout.info(f'Changing error of {nuis_name} from {nuis.getError()} to {prefit_variation}')
                 nuis.setError(prefit_variation)
                 nuis.removeRange()    
         return None
     
     def get_poi(self, poi_name:Optional[str]=None, strict:bool=False):
         """Get POI variable by name
         
@@ -759,36 +758,36 @@
             poi_name: str
                 name of POI to retrieve
             strict: bool
                 require the variable to be defined in the POI list, throw error otherwise
         """
         if poi_name is None:
             poi = self.pois.first()
-            self.stdout.info(f"INFO: POI name not specified. The first POI \"{poi.GetName()}\" is used by default.")
+            self.stdout.info(f'POI name not specified. The first POI "{poi.GetName()}" is used by default.')
         else:
             poi = self.workspace.var(poi_name)
         if not poi:
-            raise RuntimeError(f"workspace does not contain the variable \"{poi_name}\"")
+            raise RuntimeError(f'workspace does not contain the variable "{poi_name}"')
         if strict and (poi not in list(self.pois)):
-            raise RuntimeError(f"workspace variable \"{poi_name}\" is not part of the POIs")
+            raise RuntimeError(f'workspace variable "{poi_name}" is not part of the POIs')
         return poi
     
     def _load_obs_and_weight(self, obs_and_weight:Optional[Union["ROOT.RooArgSet",str]]=None, 
                              weight_var:Optional[Union["ROOT.RooRealVar",str]]=None):
         # get the weight variable
         if weight_var is None:
             weight_name = self._DEFAULT_NAMES_['weight']
             weight_var = self.workspace.var(weight_name)
             if not weight_var:
                 weight_var = ROOT.RooRealVar(weight_name, weight_name, 1)
                 getattr(self.workspace, "import")(weight_var)
         elif isinstance(weight_var, str):
             weight_var = self.workspace.var(weight_var)
             if not weight_var:
-                raise RuntimeError('weight variable "{}" not found in workspace'.format(weight_var))
+                raise RuntimeError(f'weight variable "{weight_var}" not found in workspace')
         elif not isinstance(weight_var, ROOT.RooRealVar):
             raise ValueError('weight variable must be of RooRealVar type')
                 
         # get the obs_and_weight arg set
         if obs_and_weight is None:
             default_name = self._DEFAULT_NAMES_['dataset_args']
             obs_and_weight = self.workspace.set(default_name)
@@ -834,14 +833,15 @@
         pdfmap.keepalive = list()
         for c, d in pdf_dict.items():
             pdfmap.keepalive.append(d)
             pdfmap.insert(pdfmap.begin(), ROOT.std.pair("const string, RooAbsPdf*")(c, d))
         return pdfmap
     
     def generate_asimov_from_pdf(self, name:str="asimovData", pdf:Optional["ROOT.RooAbsPdf"]=None,
+                                 observables:Optional["ROOT.RooArgSet"]=None,
                                  obs_and_weight:Optional[Union["ROOT.RooArgSet",str]]=None, 
                                  weight_var:Optional[Union["ROOT.RooRealVar",str]]=None,
                                  extra_args=None):
         
         pdf = pdf if pdf is not None else self.pdf
         if isinstance(pdf, ROOT.RooSimultaneous):
             raise ValueError("this method should not be called from a simultaneous pdf")
@@ -855,31 +855,32 @@
             if isinstance(extra_args, list):
                 for arg in extra_args:
                     arg_set.add(arg)
             else:
                 arg_set.add(extra_args)
                 
         asimov_data = ROOT.RooDataSet(name, name, arg_set, ROOT.RooFit.WeightVar(weight_var))
-        
+        if observables is None:
+            observables = self.observables
         # generate observables defined by the pdf associated with this state
-        obs = pdf.getObservables(self.observables)
+        obs = pdf.getObservables(observables)
         target_obs = obs.first()
         expected_events = pdf.expectedEvents(obs)
         #print("INFO: Generating Asimov for pdf {}".format(pdf.GetName()))
         for i in range(target_obs.numBins()):
             target_obs.setBin(i)
             norm = pdf.getVal(obs)*target_obs.getBinWidth(i)
             n_events = norm*expected_events
             if n_events <= 0:
-                self.stdout.warning("WARNING: Detected bin with zero expected events ({})! Please check"
-                      "your inputs. Obs = {}, bin = {}".format(n_events, target_obs.GetName(), i))
+                self.stdout.warning("Detected bin with zero expected events ({})! Please check"
+                                    "your inputs. Obs = {}, bin = {}".format(n_events, target_obs.GetName(), i))
             elif (n_events > 0) and (n_events < 1e18):
                 self.stdout.debug("pdf={}, obs={}, bin={}, val={}".format(
                     pdf.GetName(), target_obs.GetName(), i, n_events))
-                asimov_data.add(self.observables, n_events)
+                asimov_data.add(observables, n_events)
             else:
                 raise RuntimeError(f"detected pdf bin with nan (pdf={pdf.GetName()},obs={target_obs.GetName()},bin={i})")
 
         if (asimov_data.sumEntries() != asimov_data.sumEntries()):
             raise RuntimeError("asimov data sum entries is nan")
         return asimov_data
     
@@ -1002,18 +1003,18 @@
         else:
             poi = self.get_poi(poi_name)
         
         # take snapshot of initial states of all variables
         mutable_vars = self.get_variables(WSArgument.MUTABLE)
         ws.saveSnapshot(nom_vars_name, mutable_vars)
         if not ws.getSnapshot(nom_glob_name):
-            self.stdout.info(f'INFO: Saving snapshot "{nom_glob_name}"')
+            self.stdout.info(f'Saving snapshot "{nom_glob_name}"')
             ws.saveSnapshot(nom_glob_name, all_globs)
         if not ws.getSnapshot(nom_nuis_name):
-            self.stdout.info(f'INFO: Saving snapshot "{nom_nuis_name}"')
+            self.stdout.info(f'Saving snapshot "{nom_nuis_name}"')
             ws.saveSnapshot(nom_nuis_name, all_nuis)
         
         if do_fit:
             if dataset is None:
                 dataset = self.data
             minimizer = self.minimizer_cls("Minimizer", self.pdf, dataset, workspace=self.workspace)
             if minimizer_options is None:
@@ -1088,24 +1089,24 @@
                                           ROOT.RooArgSet(obs_and_weight, channel_cat),
                                           ROOT.RooFit.Index(channel_cat),
                                           ROOT.RooFit.Import(dataset_map),
                                           ROOT.RooFit.WeightVar(weight_var))
 
         if do_import:
             if ws.data(asimov_data_name):
-                self.stdout.warning(f"WARNING: Dataset with name {asimov_data_name} already exists in the "
+                self.stdout.warning(f"[WARNING] Dataset with name {asimov_data_name} already exists in the "
                                     "workspace. The newly generated dataset will not overwrite the original "
                                     "dataset.")
             getattr(ws, "import")(asimov_data)
-            self.stdout.info(f'INFO: Generated Asimov Dataset "{asimov_data_name}"')
+            self.stdout.info(f'Generated Asimov Dataset "{asimov_data_name}"')
             
         if asimov_snapshot is not None:
             snapshot_name = asimov_snapshot.format(mu=pretty_value(poi_val),
                                                    mu_cond=pretty_value(poi_profile))
-            self.stdout.info(f'INFO: Saving snapshot "{snapshot_name}"')
+            self.stdout.info(f'Saving snapshot "{snapshot_name}"')
             ws.saveSnapshot(snapshot_name, mutable_vars)
     
         if restore_states == 0:
             # load back a snapshot of all variable's initial states
             ws.loadSnapshot(nom_vars_name)
         elif restore_states == 1:
             # load back a snapshot of the initial global observable states
@@ -1113,14 +1114,33 @@
         elif restore_states == 2:
             pass
         else:
             raise ValueError(f'unsupported restore state option "{restore_states}"')
         
         return asimov_data
     
+    def generate_observed_toys(self, dataset=None, n_toys:int=1, seed:Optional[int]=None,
+                               event_seed:Optional[Dict]=None,
+                               add_ghost:bool=True, do_import:bool=True,
+                               name="toyObsData_{index}"):
+        if dataset is None:
+            dataset = self.data
+        interface = RooDataSet(dataset)
+        generator = interface.generate_toy_dataset(n_toys,
+                                                   seed=seed,
+                                                   add_ghost=add_ghost,
+                                                   event_seed=event_seed,
+                                                   name_fmt=name)
+        toys = []
+        for toy in generator:
+            if do_import:
+                self.workspace.Import(toy)
+            toys.append(toy)
+        return toys
+    
     def generate_toys(self, n_toys:int=1, seed:Union[int, List[int]]=0, 
                       binned:bool=True, randomize_globs:bool=True,
                       do_import:bool=True, name="toyData_{index}_seed_{seed}"):
         if n_toys > 1:
             if seed == 0:
                 seeds = [0] * n_toys
             elif (not isinstance(seed, (list, np.ndarray, range))) or (len(seed) != n_toys):
@@ -1152,15 +1172,15 @@
             toy = self.pdf.generate(*args)
             toy_name = name.format(seed=seeds[i], index=i)
             toy.SetName(toy_name)
             if do_import:
                 if ws.data(toy_name):
                     raise RuntimeError(f"attempt to overwrite existing dataset `{toy_name}`")
                 getattr(ws, "import")(toy)
-                self.stdout.info(f'INFO: Generated toy dataset "{toy_name}"')
+                self.stdout.info(f'Generated toy dataset "{toy_name}"')
             toys.append(toy)
         
         ws.loadSnapshot("tmp")
         
         return toys
     
     def save(self, filename:str, recreate:bool=True, rebuild:bool=True,
@@ -1192,58 +1212,58 @@
             config = {"data_name": None}
             if keep_snapshots is not None:
                 config["snapshot_list"] = keep_snapshots
             else:
                 if (quickstats.root_version >= (6, 26, 0)):
                     config["snapshot_list"] = [i.GetName() for i in self.workspace.getSnapshots()]
                 else:
-                    self.stdout.warning("WARNING: Saving of snapshots not supported with ROOT version < 6.26.0. "
+                    self.stdout.warning("Saving of snapshots not supported with ROOT version < 6.26.0. "
                                         "No snapshots will be saved in the rebuilt workspace.")
                     config["snapshot_list"] = []
             if keep_datasets is not None:
                 config["dataset_list"] = keep_datasets
             modifier = XMLWSModifier(config, verbosity="WARNING")
             modifier.create_modified_workspace(self.workspace, filename,
                                                import_class_code=False,
                                                recreate=recreate)
         else:
             self.workspace.writeToFile(filename, recreate)
     
     @semistaticmethod
     def load_ws(self, fname:str, ws_name:Optional[str]=None, mc_name:Optional[str]=None):
         if not os.path.exists(fname):
-            raise FileNotFoundError('workspace file {} does not exist'.format(fname))
+            raise FileNotFoundError(f'workspace file {fname} does not exist')
         file = ROOT.TFile(fname)
         if (not file):
-            raise RuntimeError("Something went wrong while loading the root file: {}".format(fname))        
+            raise RuntimeError(f"Something went wrong while loading the root file: {fname}")        
         # load workspace
         if ws_name is None:
             ws_names = [i.GetName() for i in file.GetListOfKeys() if i.GetClassName() == 'RooWorkspace']
             if not ws_names:
-                raise RuntimeError("No workspaces found in the root file: {}".format(fname))
+                raise RuntimeError(f"No workspaces found in the root file: {fname}")
             if len(ws_names) > 1:
-                self.stdout.warning("WARNING: Found multiple workspace instances from the root file: {}. Available workspaces"
+                self.stdout.warning("Found multiple workspace instances from the root file: {}. Available workspaces"
                       " are \"{}\". Will choose the first one by default".format(fname, ','.join(ws_names)))
             ws_name = ws_names[0]
         ws = file.Get(ws_name)
         if not ws:
             raise RuntimeError('Failed to load workspace: "{}"'.format(ws_name))
         # load model config
         if mc_name is None:
             mc_names = [i.GetName() for i in ws.allGenericObjects() if 'ModelConfig' in i.ClassName()]
             if not mc_names:
-                raise RuntimeError("no ModelConfig object found in the workspace: {}".format(ws_name))
+                raise RuntimeError(f"no ModelConfig object found in the workspace: {ws_name}")
             if len(mc_names) > 1:
-                self.stdout.warning("WARNING: Found multiple ModelConfig instances from the workspace: {}. "
+                self.stdout.warning("Found multiple ModelConfig instances from the workspace: {}. "
                       "Available ModelConfigs are \"{}\". "
                       "Will choose the first one by default".format(ws_name, ','.join(mc_names)))
             mc_name = mc_names[0]     
         mc = ws.obj(mc_name)
         if not mc:
-            raise RuntimeError('Failed to load model config "{}"'.format(mc_name))
+            raise RuntimeError(f'failed to load model config "{mc_name}"')
         return file, ws, mc
     
     def get_category_map(self, pdf=None):
         if pdf is None:
             pdf = self.pdf
         if not isinstance(pdf, ROOT.RooSimultaneous):
             raise ValueError("input pdf is not a simultaneous pdf")            
@@ -1350,15 +1370,15 @@
                 if  (bins != default_bins):
                     # rebinning
                     from quickstats.maths.statistics import bin_center_to_bin_edge
                     bin_edges = bin_center_to_bin_edge(x)
                     from quickstats.interface.root import TH1
                     pyh = TH1.from_numpy_histogram(y, bin_edges=bin_edges)
                     pyh.rebin(bins)
-                    self.stdout.warning(f"WARNING: Rebinned dataset ({dataset.GetName()}, cat = {cat}) from "
+                    self.stdout.warning(f"Rebinned dataset ({dataset.GetName()}, cat = {cat}) from "
                                         f"nbins = {default_bins} to nbins = {bins}")
                     x = pyh.bin_center
                     y = pyh.bin_content
                 distributions[cat]['x'] = x
                 distributions[cat]['y'] = y
                 is_binned[cat] = True
             else:
@@ -1601,15 +1621,14 @@
             target_distributions.extend(snapshots)
         
         
         if sum_over_category:
             category_map['all_cat'] = ''
             binnings['all_cat'] = combine_dict(binnings[categories[0]])
         
-        categories = list(collected_distributions)
         for i, category in enumerate(categories):
             obs_name = category_map[category]['observable']
             if discriminant is None:
                 xlabel = obs_name
             else:
                 #xlabel = f"{discriminant}_{category}"
                 xlabel = f"{discriminant} (category {category})"
@@ -1796,15 +1815,15 @@
         # snapshots
         if ('snapshot' in items):
             if (quickstats.root_version >= (6, 26, 0)):
                 snapshots = self.workspace.getSnapshots()
                 summary_str += f"Snapshots ({len(snapshots)}):\n"
                 summary_str += "".join([f"\t{snap.GetName()}\n" for snap in snapshots])
             else:
-                self.stdout.warning("WARNING: Snapshot listing is only available after ROOT 6.26/00")
+                self.stdout.warning("Snapshot listing is only available after ROOT 6.26/00")
         # categories
         if 'category' in items:
             if isinstance(self.pdf, ROOT.RooSimultaneous):
                 category_map = self.get_category_map()
                 n_cat = len(category_map)
                 summary_str += f"Categories ({n_cat}):\n"
                 for category in category_map:
@@ -1851,15 +1870,15 @@
                     const_str = "C" if d['is_constant'] else "F"
                     summary_str += f"\t{name} = {value} [{vmin}, {vmax}] {const_str}\n"
             else:
                 for d in data:
                     name = d['name']
                     summary_str += f"\t{name}\n"
         if not suppress_print:
-            self.stdout.info(summary_str)
+            self.stdout.info(summary_str, bare=True)
         if save_as is not None:
             with open(save_as, "w") as f:
                 f.write(summary_str)
                 
     def get_systematics_variations(self, filter_name:Optional[str]=None,
                                    filter_client:Optional[str]=None, fmt:str="pandas"):
         from quickstats.utils.roofit_utils import get_systematics_variations
@@ -1887,35 +1906,51 @@
                               content=content, style=style, fmt="dataframe")
         data_2 = get_str_data(snapshots["right"], fill_classes=False,
                               fill_definitions=True,
                               content=content, style=style, fmt="dataframe")
         data.add(data_1, data_2)
         data.process()
         summary_str = data.get_summary_str(visibility=0b01011, indent="    ")
-        self.stdout.info(summary_str)
+        self.stdout.info(summary_str, bare=True)
     
     def get_gaussian_constraint_attributes(self, fmt:str="pandas"):
         constr_pdfs, _, _ = self.pair_constraints()
         from quickstats.utils.roofit_utils import get_gaussian_pdf_attributes
         return get_gaussian_pdf_attributes(constr_pdfs, fmt=fmt)
    
     def get_poisson_constraint_attributes(self, fmt:str="pandas"):
         constr_pdfs, _, _ = self.pair_constraints()
         from quickstats.utils.roofit_utils import get_poisson_pdf_attributes
         return get_poisson_pdf_attributes(constr_pdfs, fmt=fmt)
     
     
     def get_category_expected_events_over_range(self, category:str, range:List[float],
-                                                normalized:bool=False):
+                                                normalize:bool=False):
         assert len(range) == 2
-        range_name = uuid.uuid4().hex
         pdf_cat = self.pdf.getPdf(category)
         if not pdf_cat:
             raise RuntimeError(f'{category} is not a valid category in the workspace')
-        observables = pdf_cat.getObservables(self.observables)
-        observables.first().setRange(range_name, range[0], range[1])
-        integral = pdf_cat.createIntegral(observables, ROOT.RooFit.NormSet(observables),
-                                          ROOT.RooFit.Range(range_name)).getVal()
-        observables.first().removeRange(range_name)
-        if not normalized:
-            integral *= pdf_cat.expectedEvents(observables)
-        return integral
+        expected_events = RooAbsPdf.get_expected_events_over_range(pdf_cat, self.observables,
+                                                                   range[0], range[1],
+                                                                   normalize=normalize)
+        return expected_events
+    
+    
+    def load_snapshot(self, snapshot_name:Optional[str]=None):
+        if snapshot_name is not None:
+            snapshot = self.workspace.getSnapshot(snapshot_name)
+            if (not snapshot) and ('0x(nil)' in snapshot.__repr__()):
+                self.stdout.warning(f'Snapshot "{snapshot_name}" does not exist.')
+            else:
+                self.workspace.loadSnapshot(snapshot_name)
+                self.stdout.debug(f'Loaded snapshot "{snapshot_name}"')
+                
+    def save_snapshot(self, snapshot_name:Optional[str]=None, 
+                      variables:Optional[Union[ROOT.RooArgSet, str, WSArgument]]=None):
+        if snapshot_name is not None:
+            if variables is None:
+                self.workspace.saveSnapshot(snapshot_name, self.workspace.allVars())
+            else:
+                if isinstance(variables, (str, WSArgument)):
+                    variables = self.get_variables(variables)
+                self.workspace.saveSnapshot(snapshot_name, variables)
+            self.stdout.debug(f'Saved snapshot "{snapshot_name}"')
```

### Comparing `quickstats-0.6.7.8/quickstats/components/extended_rfile.py` & `quickstats-0.6.8.1/quickstats/components/extended_rfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self._cache  = []
         self._components = []        
         
         # initialize from ROOT file
         if isinstance(source, str):
             if not os.path.exists(source):
                 raise FileNotFoundError(f"workspace file {source} does not exist")
-            self.stdout.info('INFO: Opening file "{}"'.format(self.fname))
+            self.stdout.info('Opening file "{}"'.format(self.fname))
             file = ROOT.TFile(source) 
             if self.is_corrupt(file):
                 raise RuntimeError(f"corrupted file: {source}")
             self._file = file
             self.fname = source
             if tree_name is not None:
                 self.set_tree(tree_name)
@@ -96,27 +96,27 @@
     
     def canvas_draw(self):
         self.create_canvas()
         self.canvas.Draw()
     
     def add_tree(self, tree_name:str):
         if tree_name in self._rdf_map:
-            self.stdout.info("INFO: Tree already added to the rdf collection.")
+            self.stdout.info("Tree already added to the rdf collection.")
             return None
         rdf = ROOT.RDataFrame(tree_name, self.fname)
         if not rdf:
             raise RuntimeError(f"failed to load tree \"{tree_name}\"")
         self._rdf_map[tree_name] = rdf
-        self.stdout.info(f"INFO: Added tree \"{tree_name}\" to the rdf collection")
+        self.stdout.info(f"Added tree \"{tree_name}\" to the rdf collection")
         
     def set_tree(self, tree_name:str):
         if tree_name not in self._rdf_map:
             self.add_tree(tree_name)
         self._rdf = self._rdf_map[tree_name]
-        self.stdout.info(f"INFO: Set active tree to \"{tree_name}\"")
+        self.stdout.info(f"Set active tree to \"{tree_name}\"")
     
     def validate(self):
         if self._rdf is None:
             raise RuntimeError("active tree not set")
             
     def get_Histo1D(self, name:str, n_bins:int, xmin:float, xmax:float, column:str, weight:Optional[str]=None,
                     title:Optional[str]=None, pyobject:bool=False, draw:bool=False, draw_option:Optional[str]=None):
@@ -139,19 +139,19 @@
             py_th1 = TH1(r_th1)
             return py_th1
         return r_th1
     
     def append(self, robject:ROOT.TObject):
         if not isinstance(robject, ROOT.TObject):
             raise RuntimeError("only TObject can be added to TFile")
-        self.stdout.info(f"INFO: Added object \"{robject.GetName()}\" to internal components")
+        self.stdout.info(f"Added object \"{robject.GetName()}\" to internal components")
         self._components.append(robject)
     
     def add_cache(self, robject:ROOT.TObject):
-        self.stdout.info(f"INFO: Added object \"{robject.GetName()}\" to cache")
+        self.stdout.info(f"Added object \"{robject.GetName()}\" to cache")
         self._cache.append(robject)
         
     def clear_cache(self):
         self._cache = []
     
     def save_components(self, fname:str, mode:str="RECREATE", components:Optional[List]=None):
         if components is None:
```

### Comparing `quickstats-0.6.7.8/quickstats/components/likelihood.py` & `quickstats-0.6.8.1/quickstats/components/likelihood.py`

 * *Files 4% similar despite different names*

```diff
@@ -132,19 +132,19 @@
         if isinstance(snapshot_name, str):
             snapshot_name = {
                 "uncond": snapshot_name,
                 "cond"  : snapshot_name
             }
         if "uncond" not in snapshot_name:
             snapshot_name["uncond"] = self.kCurrentSnapshotName
-            self.stdout.info(f'INFO: No snapshot given for unconditional fit. The snapshot "{self.kCurrentSnapshotName}" '
+            self.stdout.info(f'No snapshot given for unconditional fit. The snapshot "{self.kCurrentSnapshotName}" '
                              'will be used by default')
         if "cond" not in snapshot_name:
             snapshot_name["cond"] = self.kCurrentSnapshotName
-            self.stdout.info(f'INFO: No snapshot given for conditional fit. The snapshot "{self.kCurrentSnapshotName}" '
+            self.stdout.info(f'No snapshot given for conditional fit. The snapshot "{self.kCurrentSnapshotName}" '
                              'will be used by default')
         if set(snapshot_name.keys()) != set(["uncond", "cond"]):
             raise ValueError('when snapshot name is given as a dictionary, it must be of the '
             'form {"cond": <conditional_fit_snapshot>, "uncond": <unconditional_fit_snapshot>}')
         
         self.load_snapshot(snapshot_name["cond"])
         poi_val = self._parse_poi_val(pois, poi_val)
@@ -165,20 +165,14 @@
         muhat_errlo = {}
         muhat_errhi = {}
         
         # no poi fit
         if mode == FitMode.NOMINAL:
             # restore initial parameter values after each fit
             self.load_snapshot(snapshot_name["cond"])
-            if len(pois) > 0:
-                # fix other pois if they are not studied
-                for poi in self.model.pois:
-                    poi.setConstant(1)
-                for poi in pois:
-                    poi.setConstant(0)
             self.minimizer.create_nll()
             prefit_nll = self.minimizer.nll.getVal()
             fit_status = self.minimizer.minimize()
             roofit_result = self.minimizer.fit_result
             self.save_snapshot("nllFit", WSArgument.MUTABLE)
             postfit_nll = self.minimizer.nll.getVal()
             fit_time = time.time() - start_time
@@ -225,48 +219,48 @@
             fit_status_cond = self.minimizer.minimize()
             roofit_result['cond'] = self.minimizer.fit_result
             self.save_snapshot("condFit", WSArgument.MUTABLE)
             nll_cond = self.minimizer.nll.getVal()
         fit_time_cond = time.time() - fit_time_uncond - start_time
         
         fit_result = {}
-        self.stdout.info("INFO: NLL evaluation completed with")
+        self.stdout.info("NLL evaluation completed with")
         if mode in [FitMode.HYBRID, FitMode.UNCOND, FitMode.NOFIT]:
             best_fit_str = ", ".join([f"{name} = {value:.5f}" for name, value in muhat.items()])
-            self.stdout.info("best fit : ".rjust(15) + f"{best_fit_str}")
-            self.stdout.info("uncond NLL = ".rjust(15) + f"{nll_uncond:.5f}")
+            self.stdout.info("best fit : ".rjust(15) + f"{best_fit_str}", bare=True)
+            self.stdout.info("uncond NLL = ".rjust(15) + f"{nll_uncond:.5f}", bare=True)
             fit_result['uncond_fit'] = {
                 'muhat': muhat,
                 'muhat_errlo': muhat_errlo,
                 'muhat_errhi': muhat_errhi,
                 'nll': nll_uncond,
                 'status': fit_status_uncond,
                 'time': fit_time_uncond
             }
         if mode in [FitMode.HYBRID, FitMode.COND]:
             mu = {name:pretty_value(value) for name, value in poi_val.items()}
             mu_str = ", ".join([f"{name} = {pretty_value(value)}" for name, value in poi_val.items()])
-            self.stdout.info("mu : ".rjust(15) + f"{mu_str}")
+            self.stdout.info("mu : ".rjust(15) + f"{mu_str}", bare=True)
             # also add the best-fit value for profiled POIs
             for name, value in poi_val.items():
                 if value == None:
                     muhat[name] = self.model.workspace.var(name).getVal()
-            self.stdout.info("cond NLL = ".rjust(15)+f"{nll_cond:.5f}")
+            self.stdout.info("cond NLL = ".rjust(15)+f"{nll_cond:.5f}", bare=True)
             fit_result['cond_fit'] = {
                 'mu': mu,
                 'muhat': muhat,
                 'nll': nll_cond,
                 'status': fit_status_cond,
                 'time': fit_time_cond
             }
             
         if mode == FitMode.HYBRID:
             pnll = nll_cond - nll_uncond
             qmu  = 2*pnll
-            self.stdout.info("PNLL = ".rjust(15) + "{:.5f}".format(nll_cond - nll_uncond))
+            self.stdout.info("PNLL = ".rjust(15) + "{:.5f}".format(nll_cond - nll_uncond), bare=True)
             fit_result['pnll'] = pnll
             fit_result['qmu']  = qmu
             
             if (qmu >= 0):
                 ndof = len(pois)
                 if ndof == 1:
                     # ndof = 1 case
@@ -286,20 +280,20 @@
                 fit_result['pvalue'] = pvalue
             else:
                 fit_result['significance'] = None
                 fit_result['pvalue'] = None
                 
         if mode != FitMode.NOMINAL:
             self.stdout.info("time = ".rjust(15) + \
-                             "(uncond_fit) {:.3f}, (cond_fit) {:.3f}".format(fit_time_uncond, fit_time_cond))
+                             "(uncond_fit) {:.3f}, (cond_fit) {:.3f}".format(fit_time_uncond, fit_time_cond), bare=True)
             fit_result['total_time'] = fit_time_uncond + fit_time_cond
         else:
-            self.stdout.info("prefit NLL = ".rjust(18) + f"{prefit_nll:.5f}")
-            self.stdout.info("postfit NLL = ".rjust(18) + f"{postfit_nll:.5f}")
-            self.stdout.info("time = ".rjust(18) + f"{fit_time:.3f}")
+            self.stdout.info("prefit NLL = ".rjust(18) + f"{prefit_nll:.5f}", bare=True)
+            self.stdout.info("postfit NLL = ".rjust(18) + f"{postfit_nll:.5f}", bare=True)
+            self.stdout.info("time = ".rjust(18) + f"{fit_time:.3f}", bare=True)
             fit_result['prefit_nll'] = prefit_nll
             fit_result['postfit_nll'] = postfit_nll
             fit_result['status'] =  fit_status
             fit_result['total_time'] = fit_time
         
         self.roofit_result = roofit_result
```

### Comparing `quickstats-0.6.7.8/quickstats/components/modelling/component_source.py` & `quickstats-0.6.8.1/quickstats/components/modelling/component_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/modelling/data_modelling.py` & `quickstats-0.6.8.1/quickstats/components/modelling/data_modelling.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
             fit_stats = fit_tool.get_fit_stats(n_float_params=n_float_params)
             fit_tool.print_fit_stats(fit_stats)
 
             # free memory
             canvas.Close()
             ROOT.gSystem.ProcessEvents()
             
-        self.stdout.info(f"INFO: Task finished. Total time taken: {t.interval:.3f}s")
+        self.stdout.info(f"Task finished. Total time taken: {t.interval:.3f}s")
         
         param_data = self.get_param_data(model_parameters)
         param_data_value_only = self.get_param_data(model_parameters, value_only=True)
         summary = {"filename"    : filename,
                    "parameters"  : param_data,
                    "fit_options" : copy.deepcopy(fit_options),
                    "stats"       : fit_stats,
```

### Comparing `quickstats-0.6.7.8/quickstats/components/modelling/model_source.py` & `quickstats-0.6.8.1/quickstats/components/modelling/model_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/modelling/parameter_templates.py` & `quickstats-0.6.8.1/quickstats/components/modelling/parameter_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/modelling/pdf_fit_tool.py` & `quickstats-0.6.8.1/quickstats/components/modelling/pdf_fit_tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,15 +63,15 @@
                 Number of floating parameters in the fit. This decreases the number of degrees of freedom
                 used in chi2 calculation.
         """
         return self._get_fit_stats(self.pdf, self.data, n_bins=n_bins, n_float_params=n_float_params)
     
     @semistaticmethod
     def print_fit_stats(self, fit_stats:Dict):
-        self.stdout.info(f"INFO: chi^2/ndf = {fit_stats['chi2/ndf']}, "
+        self.stdout.info(f"chi^2/ndf = {fit_stats['chi2/ndf']}, "
                          f"Number of Floating Parameters + Normalization = {fit_stats['n_float_params'] + 1}, "
                          f"Number of bins = {fit_stats['n_bins']}, "
                          f"ndf = {fit_stats['ndf']}, "
                          f"chi^2 = {fit_stats['chi2']}, "
                          f"p_value = {fit_stats['pvalue']}")
     
     @staticmethod
@@ -91,18 +91,18 @@
         vmax = observable.getMax()
         observable.setRange("fitRange", vmin, vmax)
         
         model_name = self.pdf.GetName()
         data_name  = self.data.GetName()
         obs_name   = observable.GetName()
         
-        self.stdout.info(f"INFO: Begin model fitting...")
-        self.stdout.info(f"      Model : ".rjust(20) + f"{model_name}")
-        self.stdout.info(f"    Dataset : ".rjust(20) + f"{data_name}")
-        self.stdout.info(f" Observable : ".rjust(20) + f"{obs_name}")
+        self.stdout.info(f"Begin model fitting...")
+        self.stdout.info(f"      Model : ".rjust(20) + f"{model_name}", bare=True)
+        self.stdout.info(f"    Dataset : ".rjust(20) + f"{data_name}", bare=True)
+        self.stdout.info(f" Observable : ".rjust(20) + f"{obs_name}", bare=True)
         
         fit_args = [ROOT.RooFit.Range("fitRange"), ROOT.RooFit.PrintLevel(print_level),
                     ROOT.RooFit.Minos(minos), ROOT.RooFit.Hesse(hesse),
                     ROOT.RooFit.Save(), ROOT.RooFit.Strategy(strategy)]
         
         if asymptotic:
             fit_args.append(ROOT.RooFit.AsymptoticError(True))
@@ -113,18 +113,18 @@
             True  : 'SUCCESS',
             False : 'FAIL'
         }
 
         for i in range(1, max_fit + 1):
             fit_result = self.pdf.fitTo(self.data, *fit_args)
             is_success = self.is_fit_success(fit_result)
-            self.stdout.info(f" Fit iteration {i} : ".rjust(20) + f"{status_label[is_success]}")
+            self.stdout.info(f" Fit iteration {i} : ".rjust(20) + f"{status_label[is_success]}", bare=True)
             if i >= min_fit:
                 if is_success:
                     return fit_result
                 elif range_expand_rate is not None:
                     new_vmin = observable.getRange("fitRange").first - range_expand_rate
                     new_vmax = observable.getRange("fitRange").second + range_expand_rate
-                    self.stdout.info(f"INFO: Fit failed to converge, refitting with "
+                    self.stdout.info(f"Fit failed to converge, refitting with "
                                      f"expanded fit range [{new_vmin}, {new_vmax}]")
                     observable.setRange("fitRange", new_vmin, new_vmax)
         return fit_result
```

### Comparing `quickstats-0.6.7.8/quickstats/components/modelling/tree_data_source.py` & `quickstats-0.6.8.1/quickstats/components/modelling/tree_data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         if n_bins is None:
             n_bins = obs.numBins()
         if bin_range is None:
             vmin, vmax = obs.getMin(), obs.getMax()
         else:
             vmin, vmax = bin_range[0], bin_range[1]
         if (vmin == -1e30) and (vmax == 1e30):
-            self.stdout.warning("WARNING: Observable range is unbounded (-1e30, 1e30). "
+            self.stdout.warning("Observable range is unbounded (-1e30, 1e30). "
                                 "The resulting histogram could be buggy.")
         hist = ROOT.TH1D(h_name, h_name, n_bins, vmin, vmax)
         canvas = ROOT.TCanvas(uuid.uuid4().hex)
         if self.weight_name is not None:
             tree.Draw(f"{obs_name} >> {h_name}", self.weight_name)
         else:
             tree.Draw(f"{obs_name} >> {h_name}")
```

### Comparing `quickstats-0.6.7.8/quickstats/components/nuisance_parameter_harmonizer.py` & `quickstats-0.6.8.1/quickstats/components/nuisance_parameter_harmonizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/nuisance_parameter_pull.py` & `quickstats-0.6.8.1/quickstats/components/nuisance_parameter_pull.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/__init__.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from .rooproc_report import RooProcReport
 from .rooproc_export import RooProcExport
 from .rooproc_save_frame import RooProcSaveFrame
 from .rooproc_load_frame import RooProcLoadFrame
 from .rooproc_as_numpy import RooProcAsNumpy
 from .rooproc_if_defined import RooProcIfDefined
 from .rooproc_if_not_defined import RooProcIfNotDefined
+from .rooproc_load_macro import RooProcLoadMacro
 from .auxiliary import *
 
 ACTION_MAP = {
     "TREENAME": RooProcTreeName,
     "DECLARE": RooProcDeclare,
     "GLOBAL": RooProcGlobalVariables,
     "ALIAS": RooProcAlias,
@@ -43,12 +44,13 @@
     "SAVE": RooProcSave,
     "REPORT": RooProcReport,    
     "EXPORT": RooProcExport,
     "SAVE_FRAME": RooProcSaveFrame,
     "LOAD_FRAME": RooProcLoadFrame,
     "AS_NUMPY": RooProcAsNumpy,
     "IFDEF": RooProcIfDefined,
-    "IFNDEF": RooProcIfNotDefined    
+    "IFNDEF": RooProcIfNotDefined,
+    "LOAD_MACRO": RooProcLoadMacro
 }
 
 def get_action(action_name:str):
     return ACTION_MAP.get(action_name, None)
```

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_alias.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_as_numpy.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_as_numpy.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_base_action.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_base_action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from typing import Optional, List, Dict
 import os
 import re
 
 class RooProcBaseAction(object):
+        
     def __init__(self, **params):
         self._params = params
         self.executed = False
         self.status   = None
     
+    @staticmethod
+    def allow_multiline():
+        return False
+    
     def get_formatted_parameters(self, global_vars:Optional[Dict]=None):
         if global_vars is None:
             global_vars = {}
         formatted_parameters = {}
         for k,v in self._params.items():
             if v is None:
                 formatted_parameters[k] = None
```

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_declare.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_define.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from typing import Optional
+import re
 
-from .rooproc_helper_action import RooProcHelperAction
+from .rooproc_rdf_action import RooProcRDFAction
 
-from quickstats.utils.root_utils import declare_expression
-
-class RooProcDeclare(RooProcHelperAction):
+class RooProcDefine(RooProcRDFAction):
     
-    def __init__(self, expression:str, name:Optional[str]=None):
-        super().__init__(expression=expression,
-                         name=name)
+    def __init__(self, name:str, expression:str):
+        super().__init__(name=name, expression=expression)
         
     @classmethod
     def parse(cls, main_text:str, block_text:Optional[str]=None):
-        return cls(expression=main_text)        
-    
-    def _execute(self, processor:"quickstats.RooProcessor", **params):
-        name = params.get("name", None)
+        result = re.search(r"^\s*(\w+)\s*=(.*)", main_text)
+        if not result:
+            raise RuntimeError(f"invalid expression {main_text}")
+        name = result.group(1)
+        expression = result.group(2)
+        return cls(name=name, expression=expression)        
+        
+    def _execute(self, rdf:"ROOT.RDataFrame", **params):
+        name = params['name']
         expression = params['expression']
-        declare_expression(expression, name)
-        return processor
+        rdf_next = rdf.Define(name, expression)
+        return rdf_next
```

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_export.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_export.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_filter.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_filter.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_global_variables.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_global_variables.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_hybrid_action.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_hybrid_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_if_defined.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_if_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_if_not_defined.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_if_not_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_load_frame.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_load_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_nested_action.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_nested_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_report.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_report.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_safe_alias.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_safe_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_save.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_save.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_save_frame.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_save_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_stat.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_stat.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/actions/rooproc_treename.py` & `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_treename.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/builtin_methods.py` & `quickstats-0.6.8.1/quickstats/components/processors/builtin_methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,14 +121,18 @@
                "    return lv_vec.M();\n"
                "}\n"
                "template<typename T>\n"
                "float getE(const LorentzVector<T> &lv_vec){\n"
                "    return lv_vec.E();\n"
                "}\n"
                "template<typename T>\n"
+               "float getRapidity(const LorentzVector<T> &lv_vec){\n"
+               "    return lv_vec.Rapidity();\n"
+               "}\n"
+               "template<typename T>\n"
                "std::vector<T> RVec2Vec(const RVec<T> v){\n"
                "    return std::vector<T>{v.begin(), v.end()};\n"
                "}\n"
                "template <typename T>\n"
                "RVec<typename RVec<T>::size_type> StableArgsortExt(const RVec<T> &v)\n"
                "{\n"
                "   using size_type = typename RVec<T>::size_type;\n"
@@ -137,8 +141,15 @@
                "   std::stable_sort(i.begin(), i.end(), [&v](size_type i1, size_type i2) { return v[i1] < v[i2]; });\n"
                "   return i;\n"
                "}\n"
                "Double_t Phi_mpi_pi(Double_t x)\n"
                "{\n"
                "   return TVector2::Phi_mpi_pi(x);\n"
                "}\n"
+               "template <typename T>\n"
+               "RVec<T> TakeExt(const RVec<T> &v, const RVec<typename RVec<T>::size_type> &index, const int &size, const T &default_val){\n"
+               "    RVec<T> result = Take(v, index);\n"
+               "    for (int i=0; i < size - (int)result.size(); i++)\n"
+               "        result.push_back(default_val);\n"
+               "    return result;\n"
+               "}\n"
 }
```

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/roo_config_parser.py` & `quickstats-0.6.8.1/quickstats/components/processors/roo_config_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,18 @@
             action_tree.current_node = current_node.parent
         else:
             current_node = action_tree.current_node
             action = None
             if current_node.name is not None:
                 action = get_action(current_node.name)
             if action and not issubclass(action, RooProcNestedAction):
-                current_node.data["main_text"] += cline.text
+                if action.allow_multiline():
+                    current_node.data["main_text"] += f'\n{cline.text}'
+                else:
+                    current_node.data["main_text"] += cline.text
             else:
                 tokens = split_str(cline.text)
                 action_name = tokens[0]
                 if len(tokens) > 1:
                     main_text = " ".join(tokens[1:])
                 else:
                     main_text = None
```

### Comparing `quickstats-0.6.7.8/quickstats/components/processors/roo_processor.py` & `quickstats-0.6.8.1/quickstats/components/processors/roo_processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 from quickstats import Timer, AbstractObject, PathManager
 from quickstats.interface.root import TFile
 from quickstats.utils.root_utils import declare_expression, close_all_root_files
 
 class RooProcessor(AbstractObject):
     def __init__(self, config_path:Optional[str]=None,
+                 config_text:Optional[str]=None,
                  flags:Optional[List[str]]=None,
                  multithread:bool=True,
                  cache:bool=False,
                  use_template:bool=False,
                  verbosity:Optional[Union[int, str]]="INFO"):
         super().__init__(verbosity=verbosity)
         self.cache = cache
@@ -36,25 +37,33 @@
         
         self.load_buildin_functions()
         
         if multithread:
             ROOT.EnableImplicitMT()
         
         if config_path is not None:
-            self.load_config(config_path)
+            self.load_config(config_path=config_path)
+        elif config_text is not None:
+            self.load_config(config_text=config_text)
             
     def set_cache(self, cache:bool=True):
         self.cache = cache
             
     def load_buildin_functions(self):
         for name, definition in BUILTIN_METHODS.items():
             declare_expression(definition, name)
     
-    def load_config(self, config_path:Optional[str]=None):
-        action_tree = RooConfigParser.parse_file(config_path)
+    def load_config(self, config_path:Optional[str]=None,
+                    config_text:Optional[str]=None):
+        if config_path is not None:
+            action_tree = RooConfigParser.parse_file(config_path)
+        elif config_text is not None:
+            action_tree = RooConfigParser.parse_text(config_text)
+        else:
+            raise RuntimeError('missing config input')
         action_tree.construct_actions()
         if not action_tree.root_node.has_child:
             raise RuntimeError("no actions found in the process card")
         first_action = action_tree.root_node.first_child.action
         if not isinstance(first_action, RooProcTreeName):
             raise RuntimeError("tree name must be specified at the beginning of the process card")
         self.treename = first_action._params['treename']
@@ -91,15 +100,15 @@
         if not all_files:
             raise FileNotFoundError(f'file "{filename}" does not exist')
         PathManager.check_files(all_files)
         valid_files = []
         for file in all_files:
             rf = ROOT.TFile(file)
             if TFile.is_corrupt(rf):
-                self.stdout.warning(f'WARNING: Found empty/corrupted file "{file}". Skipped.')
+                self.stdout.warning(f'Found empty/corrupted file "{file}". Skipped.')
             else:
                 valid_files.append(file)
         return valid_files
     
     def run_action(self, action:RooProcBaseAction):
         if not self.rdf:
             raise RuntimeError("RDataFrame instance not initialized")
@@ -117,44 +126,44 @@
         return RooProcReturnCode.NORMAL
             
     def run_all_actions(self, consider_child:bool=True):
         if not self.action_tree:
             raise RuntimeError("action tree not initialized")
         node = self.action_tree.get_next(consider_child=consider_child)
         if node is not None:
-            self.stdout.debug(f'DEBUG: Executing node "{node.name}" defined at line {node.data["start_line_number"]}')
+            self.stdout.debug(f'Executing node "{node.name}" defined at line {node.data["start_line_number"]}')
             action = node.action
             return_code = self.run_action(action)
             if return_code == RooProcReturnCode.NORMAL:
                 self.run_all_actions()
             elif return_code == RooProcReturnCode.SKIP_CHILD:
                 self.run_all_actions(consider_child=False)
             else:
                 raise RuntimeError("unknown return code")
         else:
-            self.stdout.debug(f'DEBUG: All node executed')
+            self.stdout.debug(f'All node executed')
             
     def sanity_check(self):
         if not self.action_tree:
             raise RuntimeError("action tree not initialized")        
         if not self.action_tree.root_node.has_child:
-            self.stdout.warning("WARNING: No actions to be performed.")
+            self.stdout.warning("No actions to be performed.")
             return None
         if self.treename is None:
             raise RuntimeError("tree name is undefined")
     
     def run(self, filename:Union[List[str], str]):
         self.sanity_check()
         all_files = self._get_all_files(filename)
         if len(all_files) == 1:
-            self.stdout.info(f'INFO: Processing file "{all_files[0]}".')
+            self.stdout.info(f'Processing file "{all_files[0]}".')
         else:
-            self.stdout.info(f"INFO: Professing files")
+            self.stdout.info(f"Professing files")
             for f in all_files:
-                self.stdout.info(f'\t"{f}"')  
+                self.stdout.info(f'\t"{f}"', bare=True)  
         with Timer() as t:
             self.rdf = ROOT.RDataFrame(self.treename, all_files)
             self.action_tree.reset()
             self.run_all_actions()
             self.cleanup()
             
-        self.stdout.info(f"INFO: Task finished. Total time taken: {t.interval:.3f} s.")
+        self.stdout.info(f"Task finished. Total time taken: {t.interval:.3f} s.")
```

### Comparing `quickstats-0.6.7.8/quickstats/components/pvalue_toys.py` & `quickstats-0.6.8.1/quickstats/components/pvalue_toys.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/roo_inspector.py` & `quickstats-0.6.8.1/quickstats/components/roo_inspector.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             return self._parse_file_expr([file_expr])
         else:
             for expr in file_expr:
                 if os.path.isdir(expr):
                     file_expr = os.path.join(expr, "*.root")
                 fnames_i = glob.glob(expr)
                 if not fnames_i:
-                    self.stdout.warning(f"WARNING: No root files found matching the expression {expr}")
+                    self.stdout.warning(f"No root files found matching the expression {expr}")
                 fnames += fnames_i
         if not fnames:
             raise RuntimeError("no root files found from the given file expression")
         return fnames
     
     def initialise(self, filter_expr:Optional[str]=None):
         self.rdf = ROOT.RDataFrame(self.tree_name, self.fnames)
@@ -73,15 +73,15 @@
         column_types = self.get_column_types(column_names)
         n_columns = len(column_types)
         summary_str += f"Columns of Interest ({n_columns}):\n"
         for cname, ctype in column_types.items():
             ctype_str = "(" + ctype + ")"
             summary_str += f"{ctype_str:<30}{cname}\n"
         if not suppress_print:
-            self.stdout.info(summary_str)
+            self.stdout.info(summary_str, bare=True)
         if save_as is not None:
             with open(save_as, "w") as f:
                 f.write(summary_str)
```

### Comparing `quickstats-0.6.7.8/quickstats/components/root_object.py` & `quickstats-0.6.8.1/quickstats/components/root_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,22 +47,22 @@
             for topic, do_remove in self._roofit_config["RemoveMessage"].items():
                 if not do_remove:
                     continue
                 try:
                     roofit_topic = getattr(ROOT.RooFit, topic)
                     stream.removeTopic(roofit_topic)
                 except:
-                    self.stdout.warning(f'WARNING: Failed to remove RooFit message topic "{topic}".')
+                    self.stdout.warning(f'Failed to remove RooFit message topic "{topic}".')
         if "GlobalKillBelow" in self._roofit_config:
             try:
                 kill_level = self._roofit_config["GlobalKillBelow"]
                 roofit_kill_level = getattr(ROOT.RooFit, kill_level)
                 ROOT.RooMsgService.instance().setGlobalKillBelow(roofit_kill_level)
             except:
-                self.stdout.warning(f'WARNING: Failed to set RooFit global kill below "{kill_level}"')
+                self.stdout.warning(f'Failed to set RooFit global kill below "{kill_level}"')
                 
     def configure_root(self):
         set_batch = self._root_config.get("SetBatch", None)
         if set_batch is not None:
             ROOT.gROOT.SetBatch(set_batch)
         th1_sumw2 = self._root_config.get("TH1Sumw2", None)
         if th1_sumw2 is not None:
@@ -74,8 +74,8 @@
         if self._REQUIRE_CONFIG_["RooFit"]:
             self.configure_roofit()
             
     @semistaticmethod
     def load_extension(self, name:str):
         result = load_macro(name)
         if (result is not None) and hasattr(ROOT, name):
-            self.stdout.info(f'INFO: Loaded extension module "{name}"')            
+            self.stdout.info(f'Loaded extension module "{name}"')
```

### Comparing `quickstats-0.6.7.8/quickstats/components/toy_limit_calculator.py` & `quickstats-0.6.8.1/quickstats/components/toy_limit_calculator.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,23 +57,27 @@
         self.poi.setConstant(False)
         poi_range = [self.poi.getRange()[0], self.poi.getRange()[1]]
         if poi_min is not None:
             poi_range[0] = poi_min
         if poi_max is not None:
             poi_range[1] = poi_max
         self.poi.setRange(poi_range[0], poi_range[1])
-        self.stdout.info("INFO: Using POI \"{}\" with range [{}, {}]".format(self.poi.GetName(),
+        self.stdout.info("Using POI \"{}\" with range [{}, {}]".format(self.poi.GetName(),
                                                                        poi_range[0],
                                                                        poi_range[1]))
-        
+        poi_toy = ROOT.RooArgSet(self.poi)
+        # null hypothesis
         self.model_SB = self.model_base.model_config
+        self.model_SB.SetParametersOfInterest(poi_toy)
         self.poi.setVal(1)
         self.model_SB.SetSnapshot(self.poi)
         
+        # alternative hypothesis
         self.model_B = self.model_base.model_config.Clone("B_only")
+        self.model_B.SetParametersOfInterest(poi_toy)
         self.poi.setVal(0)
         self.model_B.SetSnapshot(self.poi)
         
         self.seed = seed
         self.random_generator = ROOT.RooRandom.randomGenerator()
         self.random_generator.SetSeed(seed)
         
@@ -100,25 +104,26 @@
             self.toy_mc.SetNEventsPerToy(1)        
 
         if mode == 'toy':
             self.calculator = ROOT.RooStats.FrequentistCalculator(self.model_base.data, 
                                                                   self.model_B, 
                                                                   self.model_SB,
                                                                   self.toy_mc)
+            # self.calculator.SetToys(toysNull, toysAlt)
         elif mode == 'asymptotic':
             self.calculator = ROOT.RooStats.AsymptoticCalculator(self.model_base.data, 
                                                                  self.model_B, 
                                                                  self.model_SB)
             self.calculator.SetOneSided(True)
             self.calculator.SetQTilde(True)
             self.calculator.SetPrintLevel(print_level)
             self.calculator.Initialize()
         else:
             raise ValueError("mode must be either `toy` or `asymptotic`")
-
+        
         self.do_coarse_scan = do_coarse_scan
         self.eps            = eps
         self.mode           = mode
         
         self.reset_results()      
         
     def reset_results(self):
@@ -153,37 +158,37 @@
             result["data"]["CLs"].append(scan_result.CLs(i))
             result["data"]["CLsplusb"].append(scan_result.CLsplusb(i))
             result["data"]["CLsplusbError"].append(scan_result.CLsplusbError(i))
         return result
 
     def display_limits(self, scan_result):
         limits = ToyLimitCalculator.scan_result_to_dict(scan_result)['limits']
-        self.stdout.info("Limit Bands")
-        self.stdout.info(f"+2 sigma : {limits[2]}")
-        self.stdout.info(f"+1 sigma : {limits[1]}")
-        self.stdout.info(f"-1 sigma : {limits[-1]}")
-        self.stdout.info(f"-2 sigma : {limits[-2]}")
-        self.stdout.info(f"  Median : {limits[0]}")
+        self.stdout.info("Limit Bands", bare=True)
+        self.stdout.info(f"+2 sigma : {limits[2]}", bare=True)
+        self.stdout.info(f"+1 sigma : {limits[1]}", bare=True)
+        self.stdout.info(f"-1 sigma : {limits[-1]}", bare=True)
+        self.stdout.info(f"-2 sigma : {limits[-2]}", bare=True)
+        self.stdout.info(f"  Median : {limits[0]}", bare=True)
         self.stdout.info("Observed : {}".format(limits["obs"]))
         
     def check_test_statistics(self, scan_min:float, scan_max:float, steps:int):
         poi_val_0 = self.poi.getVal()
-        self.stdout.info("INFO: Checking convergence of test statistics...")
+        self.stdout.info("Checking convergence of test statistics...")
         interval = (scan_max - scan_min) / (steps - 1)
         for i in range(steps):
             mu = scan_min + i * interval
             self._check_test_statistics(mu)
     
     def _check_test_statistics(self, mu:float):
         mu_0  = self.poi.getVal()
         self.poi.setVal(mu)
         test_statistic = self.plr.EvaluateProfileLikelihood(0, 
                                                             self.model_base.data,
                                                             ROOT.RooArgSet(self.poi))
-        self.stdout.info(f"INFO: mu = {mu}, test statistic = {test_statistic}")
+        self.stdout.info(f"mu = {mu}, test statistic = {test_statistic}")
         if test_statistic < 0:
             raise RuntimeError("test statistic failed to converge")
         self.poi.setVal(mu_0)
         return True        
                 
     def append(self, result: Union[ROOT.RooStats.HypoTestInverterResult,
                                    ROOT.RooStats.HypoTestResult]):
@@ -195,24 +200,24 @@
     def run_coarse_scan(self, scan_min:float, scan_max:float):
         
         scale      = 10**(1/3)
         steps      = (math.log(scan_max / scan_min) / math.log(scale)) + 1
         steps_ceil = math.ceil(steps)
         start, end = scan_min, scan_max
         
-        self.stdout.info("INFO: Starting coarse search")
-        self.stdout.info(f"INFO: Evaluating {steps_ceil} logarithmic points from {start} to {end}")
+        self.stdout.info("Starting coarse search")
+        self.stdout.info(f"Evaluating {steps_ceil} logarithmic points from {start} to {end}")
         
         inverter = ROOT.RooStats.HypoTestInverter(self.calculator)
         inverter.SetVerbose(self.inverter_verbose)
         # 95% CLs limits
         inverter.SetConfidenceLevel(0.95) 
         inverter.UseCLs(True)
         
-        self.stdout.info("INFO: Checking for problematic CLs values...")
+        self.stdout.info("Checking for problematic CLs values...")
         
         snapshot_0 = self.freq_calculator.GetNullModel().GetSnapshot()
 
         for i in range(steps_ceil):
             start = math.exp(math.log(scan_min) + i * math.log(scan_max / scan_min) / (steps - 1))
             self.poi.setVal(start)
             self.freq_calculator.GetNullModel().SetSnapshot(self.poi)
@@ -231,17 +236,17 @@
             if (math.isfinite(cls) and cls >= 0.):
                 break
         if start >= end :
             raise RuntimeError("No acceptable points found in coarse scan")
         steps      = math.log(end / start) / math.log(scale) + 1
         steps_ceil = math.ceil(steps)
         self.freq_calculator.GetNullModel().SetSnapshot(snapshot_0)
-        self.stdout.info(f"INFO: Recalculated scan running {steps_ceil} logarithmic points from {start} to {end}")
+        self.stdout.info(f"Recalculated scan running {steps_ceil} logarithmic points from {start} to {end}")
         
-        self.stdout.info("INFO: Running fixed scan")
+        self.stdout.info("Running fixed scan")
         inverter.SetFixedScan(steps, start, end, True)
         result = inverter.GetInterval()
         result.SetInterpolationOption(ROOT.RooStats.HypoTestInverterResult.kLinear)
         
         return result        
 
     def run_scans(self, scan_min:float, scan_max:float, steps:Optional[int]=None, 
@@ -254,66 +259,65 @@
             coarse_result = self.run_coarse_scan(scan_min, scan_max, mode=mode)
             start = coarse_result.minus_2 / 10**(1/3)
             end   = coarse_result.plus_2 / 10**(1/3)
             if (not math.isfinite(start)) or (not math.isfinite(end)):
                 raise RuntimeError("Got non-finite bound from coarse limits")
             if (start < self.poi.getRange()[0]):
                 raise RuntimeError("Got lower bound beyond POI minimum range")
-            self.stdout.info(f"INFO: Bounds for fine search: [{start}, {end}]")
+            self.stdout.info(f"Bounds for fine search: [{start}, {end}]")
             self.display_limits(coarse_result)
         
-        self.stdout.info("INFO: Starting fine search")
+        self.stdout.info("Starting fine search")
         
         if steps is None:
             scale      = 1. + self.eps
             steps      = (math.log(end / start) / math.log(scale)) + 1
             steps_ceil = math.ceil(steps)
             use_log   = True
-            self.stdout.info(f"INFO: Evaluating {steps_ceil} logarithmic points from {start} to {end}")
+            self.stdout.info(f"Evaluating {steps_ceil} logarithmic points from {start} to {end}")
         else:
-            self.stdout.info(f"INFO: Evaluating {steps} points from {start} to {end}")
+            self.stdout.info(f"Evaluating {steps} points from {start} to {end}")
         inverter = ROOT.RooStats.HypoTestInverter(self.calculator)
         inverter.SetVerbose(self.inverter_verbose)
         # 95% CLs limits
         inverter.SetConfidenceLevel(0.95) 
         inverter.UseCLs(True)
         
         if self.mode == 'toy':
             self.check_test_statistics(start, end, steps)
         
-        self.stdout.info("INFO: Running fixed scan")
+        self.stdout.info("Running fixed scan")
         inverter.RunFixedScan(steps, start, end, use_log)
         result = inverter.GetInterval()
         result.SetInterpolationOption(ROOT.RooStats.HypoTestInverterResult.kLinear)
         result.SetName("scan_{}_{}_{}".format(str_encode_value(scan_min, 10),
                                               str_encode_value(scan_max, 10),
                                               steps))
         time_end = time.time()
         
-        self.stdout.info("INFO: Scan finished. Total time taken: {}s".format(time_end-time_start))
+        self.stdout.info("Scan finished. Total time taken: {}s".format(time_end-time_start))
         
         self.display_limits(result)
         
         if append:
             self.append(result)
         
         return result
     
     def run_one_point(self, poi_val:float, append=True):      
         
         poi_val_0 = self.poi.getVal()
         
-        self.stdout.info(f"INFO: Running HypoTest on mu value {poi_val}.")
+        self.stdout.info(f"Running HypoTest on mu value {poi_val}.")
     
         self.poi.setVal(poi_val)
         self.calculator.GetNullModel().SetSnapshot(self.poi)
         result = self.calculator.GetHypoTest()
         result.SetBackgroundAsAlt(True)
         result.SetName(f"{self.poi.GetName()}_{poi_val}")
-        
         self.poi.setVal(poi_val_0)
         
         if append and self.mode == 'toy':
             self.append(result)
         
         return result
     
@@ -326,57 +330,57 @@
         self.poi.setVal(poi_val_0)
         return teststat
     
 
     
     def save_as_root(self, basename:str="toy_result_seed_{seed}.root"):
         if not self.result:
-            self.stdout.warning("WARNING: No result to save.")
+            self.stdout.warning("No result to save.")
             return None
         filename = basename.format(seed=self.seed)
         self.write_to_root(self.result, filename)
             
     def write_to_root(self, result, filename):
         f = ROOT.TFile(filename, "RECREATE")
         f.cd()
         result.Write()
         f.Write()
         f.Close()
-        self.stdout.info(f"INFO: Saved toy limit result as `{filename}`.")
+        self.stdout.info(f"Saved toy limit result as `{filename}`.")
     
     def save(self, filename:str="toy_limit_result.json"):
         
         if (self.result is None) and (self.coarse_result is None) and (self.one_point_result is None):
-            self.stdout.warning("WARNING: No result to save")
+            self.stdout.warning("No result to save")
 
         base_dir = os.path.dirname(filename)
         base_name = os.path.basename(filename)
         extension = os.path.splitext(filename)[1]
             
         if self.coarse_result is not None:
             result = self.scan_result_to_dict(self.coarse_result)
             filename_coarse = os.path.join(base_dir, f"{base_name}_coarse{extension}")
             with open(filename_coarse) as f:
                 json.dump(result, f, indent=2)
-            self.stdout.info(f"INFO: Saved coarse toy limit result as `{filename}`.")
+            self.stdout.info(f"Saved coarse toy limit result as `{filename}`.")
             
         if self.result is not None:
             result = self.scan_result_to_dict(self.result)
             with open(filename) as f:
                 json.dump(result, f, indent=2)
-            self.stdout.info(f"INFO: Saved toy limit result as `{filename}`.")
+            self.stdout.info(f"Saved toy limit result as `{filename}`.")
 
         if self.one_point_result is not None:
             for mu_val in self.one_point_result:
                 mu_str = str_encode_value(mu_val)
                 result = self.scan_result_to_dict(self.one_point_result[mu_val])
                 filename_one_point = os.path.join(base_dir, f"{base_name}_{mu_str}{extension}")
                 with open(filename_one_point) as f:
                     json.dump(result, f, indent=2)
-                self.stdout.info(f"INFO: Saved toy limit result for mu = {mu_val} as `{filename}`.")
+                self.stdout.info(f"Saved toy limit result for mu = {mu_val} as `{filename}`.")
                 
 def evaluate_toy_limits(filename:str, data_name:str, 
                         scan_min:Optional[float]=None, 
                         scan_max:Optional[float]=None, 
                         steps:int=10,
                         mu_val:Optional[float]=None,
                         poi_min:Optional[float]=None, poi_max:Optional[float]=None,
```

### Comparing `quickstats-0.6.7.8/quickstats/components/workspaces/__init__.py` & `quickstats-0.6.8.1/quickstats/components/workspaces/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,8 +4,9 @@
 from .systematics_domain import SystematicsDomain
 from .core_argument_sets import CoreArgumentSets
 from .asimov_handler import AsimovHandler
 from .xml_ws_builder_v1 import XMLWSBuilder as XMLWSBuilderV1
 from .xml_ws_builder_v2 import XMLWSBuilder
 from .xml_ws_modifier import XMLWSModifier
 from .xml_ws_combiner import XMLWSCombiner
-from .ws_comparer import WSComparer, ComparisonData, WSItemType
+from .ws_comparer import WSComparer, ComparisonData, WSItemType
+from .ws_decomposer import WSDecomposer
```

### Comparing `quickstats-0.6.7.8/quickstats/components/workspaces/asimov_handler.py` & `quickstats-0.6.8.1/quickstats/components/workspaces/asimov_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,21 +62,21 @@
                     invalid_setup.append(token)
                     continue
                 else:
                     profile_setup.append(token)
         passed = (len(invalid_setup) == 0) and (len(undefined_setup) == 0)
         if len(invalid_setup) > 0:
             invalid_setup_str = ", ".join([f"`{s}`" for s in invalid_setup])
-            self.stdout.error(f"ERROR: Invalid setup info {invalid_setup_str}.", "red")
+            self.stdout.error(f"Invalid setup info {invalid_setup_str}.", "red")
         if len(undefined_setup) > 0:
             undefined_setup_str = ", ".join([f"`{s}`" for s in undefined_setup])
-            self.stdout.error(f"ERROR: Setup info with undefined variable {undefined_setup_str}.", "red")
+            self.stdout.error(f"Setup info with undefined variable {undefined_setup_str}.", "red")
         if passed:
             if (not fix_setup) and (not profile_setup):
-                self.stdout.info("REGTEST: There is no setup info provided. "
+                self.stdout.info("There is no setup info provided. "
                                  "Proceed with current variable values and ranges.")
             setups = {
                 "fix_param"    : ",".join(fix_setup),
                 "profile_param": ",".join(profile_setup)
             }
             return setups
         return None
@@ -128,20 +128,20 @@
         title_str = format_delimiter_enclosed_text(f"Operation {asimov_name}", "+",
                                                    indent_str=self.title_indent_str)
         self.stdout.info(title_str)
         setup_str = config['setup'].strip()
         if setup_str:
             setup_kwargs = self.parse_setup(setup_str)
             if not setup_kwargs:
-                self.stdout.error(f"\tStop generating Asimov data `{asimov_name}`")
+                self.stdout.error(f"Stop generating Asimov data `{asimov_name}`")
                 return None
             else:
                 self.setup_parameters(**setup_kwargs, update_snapshot=False)
         action_str = config['action'].strip()
-        self.stdout.info(f"REGTEST: Action list ({action_str})")
+        self.stdout.info(f"Action list ({action_str})")
         if not action_str:
             return None
         action_list = action_str.split(":")
         fixed_variables = []
         for action in action_list:
             status = -1
             if action == FIT_ASIMOV_ACTION:
@@ -159,15 +159,15 @@
             elif action == FLOAT_ASIMOV_ACTION:
                 for varname in fixed_variables:
                     if self.model.pois.find(varname):
                         continue
                     else:
                         self.model.workspace.var(varname).setConstant(False)
             elif action == GEN_ASIMOV_ACTION:
-                self.stdout.info(f"REGTEST: Generating Asimov dataset `{asimov_name}`")
+                self.stdout.info(f"Generating Asimov dataset `{asimov_name}`")
                 algorithm = config['algorithm']
                 if algorithm == "roostats":
                     generator = ROOT.RooStats.AsymptoticCalculator.GenerateAsimovData
                     asimov_data = generator(self.model.pdf, self.model.observables)
                     getattr(self.model.workspace, "import")(asimov_data, ROOT.RooFit.Rename(asimov_name))
                 else:
                     asimov_data = self.model.generate_asimov(do_fit=False, modify_globs=False, do_import=True,
@@ -197,14 +197,14 @@
                     'nuis': self.model.nuisance_parameters,
                     'glob': self.model.global_observables,
                     'poi': self.model.pois,
                 }                
                 for param, param_str in param_str_map.items():
                     snapshot_name = config[f"snapshot_{param}"]
                     if snapshot_name != "":
-                        self.stdout.info(f"REGTEST: Saving snapshot {snapshot_name} for current {param_str}")
+                        self.stdout.info(f"Saving snapshot {snapshot_name} for current {param_str}")
                         self.save_snapshot(snapshot_name, param_var_map[param])
                         self.saved_snapshots.append(snapshot_name)
             elif action in self.saved_snapshots:
                 self.load_snapshot(action)
             else:
                 raise RuntimeError(f"unknown action {action}")
```

### Comparing `quickstats-0.6.7.8/quickstats/components/workspaces/core_argument_sets.py` & `quickstats-0.6.8.1/quickstats/components/workspaces/core_argument_sets.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,9 +37,9 @@
             raise RuntimeError('POIs set not initialized')
    
     def define_argsets(self, ws:ROOT.RooWorkspace):
         self.validate()
         for argset, name in [(self.obs_set, OBS_SET), (self.poi_set, POI_SET),
                              (self.nuis_set, NUIS_SET), (self.glob_set, GLOB_SET)]:
             ws.defineSet(name, argset)
-        self.stdout.debug(f'DEBUG: Defined argument set "{name}" for the workspace "{ws.GetName()}".')
+        self.stdout.debug(f'Defined argument set "{name}" for the workspace "{ws.GetName()}".')
```

### Comparing `quickstats-0.6.7.8/quickstats/components/workspaces/sample.py` & `quickstats-0.6.8.1/quickstats/components/workspaces/sample.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/workspaces/settings.py` & `quickstats-0.6.8.1/quickstats/components/workspaces/settings.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/workspaces/systematic.py` & `quickstats-0.6.8.1/quickstats/components/workspaces/systematic.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
                 else:
                     self.errorhi = float(errhi)
                     self.errorlo = -abs(float(errlo))
             else:
                 self.errorhi = errhi
                 self.errorlo = errlo
             if self.get_constr_type() != ConstraintType.Asym:
-                self.stdout.warn(f"WARNING: The systematic {self.name} under domain {self.domain} "
+                self.stdout.warn(f"The systematic {self.name} under domain {self.domain} "
                                  f"will be implemented as an asymmetric uncertainty for now. Please "
                                  f"double-check your config file and use the keyword "
                                  f"{CONSTR_ASYM} for constraint "
                                  f"term type instead of {self.constr_term} if you intend to implement "
                                  f"asymmetric uncertainties.")
     
     def get_tag_name(self):
```

### Comparing `quickstats-0.6.7.8/quickstats/components/workspaces/systematics_domain.py` & `quickstats-0.6.8.1/quickstats/components/workspaces/systematics_domain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/workspaces/ws_comparer.py` & `quickstats-0.6.8.1/quickstats/components/workspaces/ws_comparer.py`

 * *Files 0% similar despite different names*

```diff
@@ -702,21 +702,21 @@
         }
         
         self.target_items = items
         self.visibility_map = visibility_map
         self.data = {}
 
     def set_targets(self, ws_path_1:str, ws_path_2:str):
-        self.stdout.info(f"INFO: Initializing targets...")
+        self.stdout.info(f"Initializing targets...")
         with Timer() as t:
             self.model_1 = ExtendedModel(ws_path_1, data_name=None, verbosity="WARNING")
-        self.stdout.info(f'INFO: Loaded workspace (left) from "{ws_path_1}". Time taken: {t.interval:.3f}s.')
+        self.stdout.info(f'Loaded workspace (left) from "{ws_path_1}". Time taken: {t.interval:.3f}s.')
         with Timer() as t:
             self.model_2 = ExtendedModel(ws_path_2, data_name=None, verbosity="WARNING")
-        self.stdout.info(f'INFO: Loaded workspace (right) from "{ws_path_2}". Time taken: {t.interval:.3f}s.')
+        self.stdout.info(f'Loaded workspace (right) from "{ws_path_2}". Time taken: {t.interval:.3f}s.')
         
     def _parse_items(self, items:Optional[Union[List[str], List[WSItem], WSItem, str]]=None) -> List[WSItem]:
         if items is None:
             parsed_items = list(self.kDefaultItems)
         elif isinstance(items, str):
             item = WSItem.parse(items)
             parsed_items = [item]
@@ -746,25 +746,25 @@
         else:
             items = self._parse_items(items)
             self.target_items = items
             
         if any(item.item_type == WSItemType.VARIABLE for item in items):
             for _item in [WSItem.PDF, WSItem.FUNCTION]:
                 if _item not in items:
-                    self.stdout.info(f'INFO: Added "{_item.title}" to the requested data pool needed for '
+                    self.stdout.info(f'Added "{_item.title}" to the requested data pool needed for '
                                      'inferring renamed and redefined variables.')
                     items.append(_item)
         
         self.clear_data()
-        self.stdout.info("INFO: Loading workspace information...")
+        self.stdout.info("Loading workspace information...")
         with Timer() as t:
             for item in items:
                 item_name = item.name.lower()
                 self.data[item_name] = self.get_item_data(item)
-        self.stdout.info(f"INFO: All requested data have been successfully loaded. Time taken: {t.interval:.3f}s.")        
+        self.stdout.info(f"All requested data have been successfully loaded. Time taken: {t.interval:.3f}s.")        
 
     def _get_workspace_data(self):
         item = WSItem.WORKSPACE
         data = ComparisonData.from_WSItem(item)
         ws_name_1 = self.model_1.workspace.GetName()
         ws_name_2 = self.model_2.workspace.GetName()
         data.add_single(name_1=ws_name_1, name_2=ws_name_2)
@@ -792,15 +792,15 @@
             snapshots_1 = self.model_1.workspace.getSnapshots()
             snapshots_2 = self.model_2.workspace.getSnapshots()
             for snapshot in snapshots_1:
                 data.add_single(name_1=snapshot.GetName())
             for snapshot in snapshots_2:
                 data.add_single(name_2=snapshot.GetName())
         else:
-            self.stdout.warning("WARNING: Snapshot listing is only available after ROOT 6.26/00")
+            self.stdout.warning("Snapshot listing is only available after ROOT 6.26/00")
         return data
      
     def _get_dataset_data(self):
         item = WSItem.DATASET
         data = ComparisonData.from_WSItem(item)
         datasets_1 = self.model_1.workspace.allData()
         datasets_2 = self.model_2.workspace.allData()
@@ -845,15 +845,15 @@
                               content=content, style=style, fmt="dataframe")
         data.add(data_1, data_2)
         return data
     
     def get_item_data(self, item:Union[str, WSItem]):
         item = WSItem.parse(item)
         title = item.title
-        self.stdout.info(f'INFO: Retrieving information for the item: "{title}"')
+        self.stdout.info(f'Retrieving information for the item: "{title}"')
         if item == WSItem.WORKSPACE:
             data = self._get_workspace_data()
         elif item == WSItem.CATEGORY:
             data = self._get_category_data()
         elif item == WSItem.SNAPSHOT:
             data = self._get_snapshot_data()
         elif item == WSItem.DATASET:
@@ -916,17 +916,17 @@
             df.loc[index_2, ['category']] = "renamed"
             df.loc[index_1, ['name_alt']] = names_2[0]
             df.loc[index_2, ['name_alt']] = names_1[0]
     
     def _process_dataset_data(self):
         item = WSItem.DATASET
         item_name = item.name.lower()
-        self.stdout.info(f'INFO: Processing dataset definitions...')
+        self.stdout.info(f'Processing dataset definitions...')
         if item_name not in self.data:
-            self.stdout.warning("WARNING: Dataset data not loaded. Skipping.")
+            self.stdout.warning("Dataset data not loaded. Skipping.")
             return None
         with Timer() as t:
             data = self.data[item_name]
             common_dataset_names = data.get_df("common")['name'].values
             dataset_names_1 = data.get_df("left_only")['name'].values
             dataset_names_2 = data.get_df("right_only")['name'].values
             df = data.df_merge
@@ -948,33 +948,33 @@
                 if len(candidates) == 1:
                     ds_name_2 = candidates[0]
                     df.loc[ds_name_1, ['category']] = "renamed"
                     df.loc[ds_name_1, ['name_alt']] = ds_name_2
                     df.loc[ds_name_2, ['category']] = "renamed"
                     df.loc[ds_name_2, ['name_alt']] = ds_name_1
             df.reset_index(inplace=True)
-        self.stdout.info(f"INFO: Processing finished. Time taken: {t.interval:.3f}s.")
+        self.stdout.info(f"Processing finished. Time taken: {t.interval:.3f}s.")
         
     def _get_combined_mapping_statistics(self):
         pdf_item_name = WSItem.PDF.name.lower()
         function_item_name = WSItem.FUNCTION.name.lower()
         items_to_request = []
         if pdf_item_name not in self.data:
             items_to_request.append(WSItem.PDF)
         if function_item_name not in self.data:
             items_to_request.append(WSItem.FUNCTION)
         
         if len(items_to_request) > 0:
             with Timer() as t:
                 for item in items_to_request:
-                    self.stdout.info(f'INFO: Added "{item.title}" to the requested data pool needed for '
+                    self.stdout.info(f'Added "{item.title}" to the requested data pool needed for '
                                      'inferring renamed and redefined variables.')
                     item_name = item.name.lower()
                     self.data[item_name] = self.get_item_data(item)
-            self.stdout.info(f"INFO: All requested data have been successfully loaded. Time taken: {t.interval:.3f}s.")
+            self.stdout.info(f"All requested data have been successfully loaded. Time taken: {t.interval:.3f}s.")
             return self._get_combined_mapping_statistics()
         
         pdf_mapping_statistics_left = self.data[pdf_item_name].mapping_statistics_left
         function_mapping_statistics_left = self.data[function_item_name].mapping_statistics_left
         pdf_mapping_statistics_right = self.data[pdf_item_name].mapping_statistics_right
         function_mapping_statistics_right = self.data[function_item_name].mapping_statistics_right        
         combined_mapping_left = ComparisonData._get_combined_mapping_statistics([pdf_mapping_statistics_left,
@@ -1018,22 +1018,22 @@
         return relevant_items
 
     def _process_renamed_and_remapped_variables(self):
         
         relevant_items = self._get_items_with_definition()
                 
         if len(relevant_items) > 0:
-            self.stdout.info("INFO: Processing renamed and remapped variables...")
+            self.stdout.info("Processing renamed and remapped variables...")
             with Timer() as t:
                 map_stat_left, map_stat_right = self._get_combined_mapping_statistics()
                 mappings = self._get_mappings(map_stat_left, map_stat_right)
                 for item_str in relevant_items:
                     data = self.data[item_str]
                     data.process_mappings(mappings)
-            self.stdout.info(f"INFO: Processing finished. Time taken: {t.interval:.3f}s")
+            self.stdout.info(f"Processing finished. Time taken: {t.interval:.3f}s")
  
     def process_data(self):
         self._process_workspace_data()
         dataset_item_str = WSItem.DATASET.name.lower()
         if dataset_item_str in self.data:
             self._process_dataset_data()
         self._process_renamed_and_remapped_variables()
@@ -1096,27 +1096,27 @@
             items.append(item)
             instance.data[item_str] = ComparisonData.from_dataframe(item, df)
         instance.target_items = items
         return instance
     
     def save_json(self, filename:str):
         json_data = {}
-        self.stdout.info(f'INFO: Saving comparison result in json format as "{filename}"...')
+        self.stdout.info(f'Saving comparison result in json format as "{filename}"...')
         for item_str, data in self.data.items():
             if data.df_merge is None:
                 data.process()
             # only save items that are requested
             item = WSItem.parse(item_str)
             if item in self.target_items:
                 json_data[item_str] = data.df_merge.to_dict('records')
         with open(filename, "w") as outfile:
             json.dump(json_data, outfile, indent=2)
     
     def save_excel(self, filename:str):
-        self.stdout.info(f'INFO: Saving comparison result in excel format as "{filename}"...')
+        self.stdout.info(f'Saving comparison result in excel format as "{filename}"...')
         import pandas as pd
         writer = pd.ExcelWriter(filename, engine='xlsxwriter')
         for item_str, data in self.data.items():
             if data.df_merge is None:
                 data.process()
             # only save items that are requested
             item = WSItem.parse(item_str)
```

### Comparing `quickstats-0.6.7.8/quickstats/components/workspaces/ws_modifier_config.py` & `quickstats-0.6.8.1/quickstats/components/workspaces/ws_modifier_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_base.py` & `quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,24 +69,24 @@
         elif isinstance(source, str):
             self.basedir = os.path.dirname(source)
         else:
             self.basedir = os.getcwd()
         self.path_manager = PathManager(self.basedir)
         if unlimited_stack:
             set_unlimited_stacksize()
-            self.stdout.info("INFO: Set stack size to unlimited")
+            self.stdout.info("Set stack size to unlimited")
         self.suppress_roofit_message()
         self.custom_classes = {}
 
     def load_extension(self):
         extensions = quickstats.get_workspace_extensions()
         for extension in extensions:
             result = load_macro(extension)
             if (result is not None) and hasattr(ROOT, extension):
-                self.stdout.info(f'INFO: Loaded extension module "{extension}"')
+                self.stdout.info(f'Loaded extension module "{extension}"')
             try:
                 cls = get_macro_TClass(extension)
             except:
                 continue
             self.custom_classes[extension] = cls
     
     @staticmethod
@@ -179,17 +179,17 @@
             if (not ws.arg(object_name)):
                 raise RuntimeError(f"object `{object_name}` does not exist")
             else:
                 return object_name
         # throw error? when attemping to define already existing object
         if check_defined:
             if ws.arg(object_name):
-                self.stdout.debug(f"REGTEST: object {object_name} already exists")
+                self.stdout.debug(f"object {object_name} already exists")
                 return object_name
-        self.stdout.debug(f"REGTEST: Generating {object_type} {object_expr}")
+        self.stdout.debug(f"Generating {object_type} {object_expr}")
         status = ws.factory(object_expr)
         if not status:
             raise RuntimeError(f"object creation from expression `{object_expr}` had failed")
         return object_name
     
     @semistaticmethod
     def get_name_mapping_str(self, old_name:str, new_name:str, width:int=40):
@@ -238,15 +238,15 @@
             # the workspace does not use the extended class, no need to import
             if extension not in all_class:
                 continue
             macro_dir = get_macro_dir(extension)
             ws.addClassDeclImportDir(macro_dir)
             ws.addClassImplImportDir(macro_dir)
             ws.importClassCode(cls)
-            self.stdout.info(f"INFO: Imported class code for \"{cls.GetName()}\".")
+            self.stdout.info(f"Imported class code for \"{cls.GetName()}\".")
         #ws.importClassCode()    
     
     def _generate_asimov(self, ws:ROOT.RooWorkspace, asimov_definitions:List, data_name:str,
                          range_name:Optional[str]=None, minimizer_config:Optional[Dict]=None,
                          title_indent_str:str="\t"):
         from quickstats.components.workspaces import AsimovHandler
         n_asimov = len(asimov_definitions)
```

### Comparing `quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_builder_v1.py` & `quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_builder_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
     def update_paths(self) -> None:
         self.path_manager.set_file("output", self.core_config["output_name"])
         categories = []
         for category, file in self.core_config['input_categories'].items():
             self.path_manager.set_file(f"__Cat_{category}", file)
     
     def parse_core_xml(self, filename:str):
-        self.stdout.info(f"INFO: Parsing file `{filename}`")
+        self.stdout.info(f"Parsing file `{filename}`")
         # load xml file
         core_xml = TXMLTree.load_as_dict(filename)
         # parse core attributes
         attributes = core_xml['attrib']
         core_config = {
             'base_dir'           : os.path.dirname(filename),
             'workspace_name'     : self._get_node_attrib(core_xml, 'WorkspaceName'),
@@ -164,15 +164,15 @@
             'poi_names'          : [],
             'input_categories'   : {},
             'asimov_definitions' : []
         }
         
         if not core_config['output_name'].endswith(".root"):
             core_config['output_name'] = os.path.splitext(core_config['output_name'])[0] + ".root"
-            self.stdout.warning('WARNING: Output file name does not contain ".root" postfix. '
+            self.stdout.warning('Output file name does not contain ".root" postfix. '
                                 'Adding it to avoid confusion.')
         # parse child level attributes
         nodes = core_xml['children']
         for node in nodes:
             tag = node['tag']
             if tag == "Input":
                 file = node['text']
@@ -190,36 +190,36 @@
             else:
                 raise RuntimeError(f"unknown item `{tag}`")
         return core_config
     
     def print_init_summary(self) -> None:
         if not self.core_config:
             raise RuntimeError("core config not set")
-        self.stdout.info("="*74)
-        self.stdout.info("Output file: ".rjust(20) + f"{self.core_config['output_name']}")
-        self.stdout.info("Workspace name: ".rjust(20) + f"{self.core_config['workspace_name']}")
-        self.stdout.info("ModelConfig name: ".rjust(20) + f"{self.core_config['model_config_name']}")
-        self.stdout.info("Dataset name: ".rjust(20) + f"{self.core_config['dataset_name']}")
-        self.stdout.info("Blind analysis: ".rjust(20) + ("True" if self.core_config['do_blind'] else "False"))
-        self.stdout.info("POIs: ".rjust(20) + ", ".join(self.core_config['poi_names']))
-        self.stdout.info("")
-        self.stdout.info("Categories to be included:")
+        self.stdout.info("="*74, bare=True)
+        self.stdout.info("Output file: ".rjust(20) + f"{self.core_config['output_name']}", bare=True)
+        self.stdout.info("Workspace name: ".rjust(20) + f"{self.core_config['workspace_name']}", bare=True)
+        self.stdout.info("ModelConfig name: ".rjust(20) + f"{self.core_config['model_config_name']}", bare=True)
+        self.stdout.info("Dataset name: ".rjust(20) + f"{self.core_config['dataset_name']}", bare=True)
+        self.stdout.info("Blind analysis: ".rjust(20) + ("True" if self.core_config['do_blind'] else "False"), bare=True)
+        self.stdout.info("POIs: ".rjust(20) + ", ".join(self.core_config['poi_names']), bare=True)
+        self.stdout.info("", bare=True)
+        self.stdout.info("Categories to be included:", bare=True)
         input_categories = self.core_config['input_categories']
         for i, input_category in enumerate(input_categories.values()):
-            self.stdout.info(f"XML file {i}: ".rjust(20) + f"{input_category}")
+            self.stdout.info(f"XML file {i}: ".rjust(20) + f"{input_category}", bare=True)
         asimov_definitions = self.core_config['asimov_definitions']
         if asimov_definitions:
-            self.stdout.info("")
-            self.stdout.info("The following asimov dataset(s) will be generated:")
+            self.stdout.info("", bare=True)
+            self.stdout.info("The following asimov dataset(s) will be generated:", bare=True)
             for asimov_def in asimov_definitions:
                 is_gen_asimov = GEN_ASIMOV_ACTION in asimov_def['Action']
                 if is_gen_asimov:
                     asimov_name = asimov_def['Name']
-                    self.stdout.info(f"\t{asimov_name}")
-        self.stdout.info("="*74)
+                    self.stdout.info(f"\t{asimov_name}", bare=True)
+        self.stdout.info("="*74, bare=True)
         
     def get_pdf_name(self, category:str):
         return f"{FINAL_PDF_NAME}_{category}"
     
     def generate_workspace(self):
         t0 = time.time()
         channel_list = ROOT.RooCategory("channellist", "channellist")
@@ -280,15 +280,15 @@
                                           ROOT.RooFit.Index(channel_list),
                                           ROOT.RooFit.Import(dataset_binned_map),
                                           ROOT.RooFit.WeightVar(weight_var))
         self.import_object(self.comb_ws, obs_data, silent=False)
         if (obs_data_binned.numEntries() < obs_data.numEntries()):
             self.import_object(self.comb_ws, obs_data_binned, silent=False)
         else:
-            self.stdout.warning("REGTEST: No need to keep binned dataset, as the "
+            self.stdout.warning("No need to keep binned dataset, as the "
                                 "number of data events is smaller than or equal "
                                 "to the number of bins in all categories", "red")
             self.use_binned = False
         
         # save the original snapshot
         # self.comb_ws.saveSnapshot("nominalNuis", self.model_config.GetNuisanceParameters())
         # self.comb_ws.saveSnapshot("nominalGlobs", self.model_config.GetGlobalObservables())
@@ -328,42 +328,42 @@
         model = ExtendedModel(self.comb_ws, data_name=self.core_config['dataset_name'], verbosity="WARNING")
         pdf = model.pdf
         cat = pdf.indexCat()
         n_cat = len(cat)
         data = model.data
         data_list = data.split(cat, True)
         # start writing summary
-        self.stdout.info("="*70)
+        self.stdout.info("="*70, bare=True)
         title_str = format_delimiter_enclosed_text("Begin summary", "~")
-        self.stdout.info(title_str)
-        self.stdout.info(f"\tThere are {n_cat} sub channels:")
+        self.stdout.info(title_str, bare=True)
+        self.stdout.info(f"\tThere are {n_cat} sub channels:", bare=True)
         for i in range(n_cat):
             cat.setBin(i)
             cat_name = cat.getLabel()
             pdf_i = pdf.getPdf(cat_name)
             data_i = data_list.FindObject(cat_name)
             sum_entries = pretty_value(data_i.sumEntries(), 5)
-            self.stdout.info(f"\t\tIndex: {i}, Pdf: {pdf_i.GetName()}, Data: {data_i.GetName()}, SumEntries: {sum_entries}")
+            self.stdout.info(f"\t\tIndex: {i}, Pdf: {pdf_i.GetName()}, Data: {data_i.GetName()}, SumEntries: {sum_entries}", bare=True)
         title_str = format_delimiter_enclosed_text("POI", "-")
-        self.stdout.info(title_str)
+        self.stdout.info(title_str, bare=True)
         if Verbosity.INFO >= self.stdout.verbosity:
             model.pois.Print("v")
         title_str = format_delimiter_enclosed_text("Dataset", "-")
-        self.stdout.info(title_str)
+        self.stdout.info(title_str, bare=True)
         if Verbosity.INFO >= self.stdout.verbosity:
             for dataset in model.workspace.allData():
                 dataset.Print()
         title_str = format_delimiter_enclosed_text("End Summary", "~")
-        self.stdout.info(title_str)
+        self.stdout.info(title_str, bare=True)
         output_path = self.get_output_path()
-        self.stdout.info(f"Workspace `{ws_name}` has been successfully generated and saved in file `{output_path}`")
+        self.stdout.info(f"Workspace `{ws_name}` has been successfully generated and saved in file `{output_path}`", bare=True)
         #output_plot_path = self.get_output_plot_path()
         #self.stdout.info(f"Plots for each category are summarized in `{output_plot_path}`")
-        self.stdout.info(f"Total time taken: {self.time_taken:.3f}s")
-        self.stdout.info("="*70)
+        self.stdout.info(f"Total time taken: {self.time_taken:.3f}s", bare=True)
+        self.stdout.info("="*70, bare=True)
     
     def get_output_path(self):
         output_name = self.core_config['output_name']
         output_path = self.get_relpath(output_name)
         return output_path
     
     def get_output_plot_path(self):
@@ -372,15 +372,15 @@
         return output_plot_path
                          
     def generate_asimov(self):
         ws = self.comb_ws
         asimov_definitions = self.core_config['asimov_definitions']
         if self.use_binned:
             data_name = self.core_config['dataset_name'] + "binned"
-            self.stdout.warning("REGTEST: Fitting binned dataset.", "red")
+            self.stdout.warning("Fitting binned dataset.", "red")
         else:
             data_name = self.core_config['dataset_name']
         range_name = self.get_fit_range_name()
         self._generate_asimov(ws, asimov_definitions=asimov_definitions,
                               data_name=data_name, range_name=range_name,
                               minimizer_config=self.minimizer_config)
         
@@ -420,15 +420,15 @@
         expected_shape = ROOT.RooArgSet()
         expected_map   = {}
         # load category xml file
         filepath = self.path_manager.get_file(f"__Cat_{category}", check_exist=True)
         cat_xml = TXMLTree.load_as_dict(filepath)
             
         title_str = format_delimiter_enclosed_text(f"Category {category}", "-")
-        self.stdout.info(title_str)
+        self.stdout.info(title_str, bare=True)
         
         self.active_category = category
         category_type = self._get_node_attrib(cat_xml, 'Type').lower()
         luminosity = self._get_node_attrib(cat_xml, "Lumi", required=False,
                                            default="-1", dtype="float")
         
         self.cat_config[category] = {
@@ -466,20 +466,20 @@
         remained_nodes = [node for node in nodes if node['tag'] not in ["Data", "Correlate"]]
         self.read_channel_xml_nodes(remained_nodes, ws_factory)
  
         self._fix_item_priority()
         items_highpriority  = self.cat_config[category]['items_highpriority']
         items_lowpriority   = self.cat_config[category]['items_lowpriority']
         
-        self.stdout.debug("REGTEST: High priority items:")
+        self.stdout.debug("High priority items:")
         for item in items_highpriority:
-            self.stdout.debug(f"\t{item}")
-        self.stdout.debug("REGTEST: Low priority items:")
+            self.stdout.debug(f"\t{item}", bare=True)
+        self.stdout.debug("Low priority items:")
         for item in items_lowpriority:
-            self.stdout.debug(f"\t{item}")
+            self.stdout.debug(f"\t{item}", bare=True)
         # first implement high priority items: common variables 
         # and functions not involving systematic uncertainties
         self.import_expressions(ws_factory, items_highpriority)
 
         systematics = self.cat_config[category]['systematics']
         samples = self.cat_config[category]['samples']
         # secondly implement systematics and import them into the workspace
@@ -518,15 +518,15 @@
             self.import_expression(ws_factory, expr)
         for key, value in expected_map.items():
             expr = self._generate_expr(f"prod::{self.KEYWORDS['expectation_prefix']}{key}(", value)
             self.import_expression(ws_factory, expr)
             
         for sample in samples:
             title_str = format_delimiter_enclosed_text(sample.process, "<", 20)
-            self.stdout.debug(title_str)
+            self.stdout.debug(title_str, bare=True)
             self.import_expressions(ws_factory, sample.shape_factors)
             sample.norm_name = self.KEYWORDS['yield_prefix'] + sample.process
             norm_factor_components = []
             norm_factor_comp = self.import_expressions(ws_factory, sample.norm_factors)
             norm_factor_components.append(norm_factor_comp)
             
             if sample.expected.getSize() > 0:
@@ -549,40 +549,40 @@
                         else:
                             raise RuntimeError(f"unknwon systematic group `{syst_group}` in "
                                                f"Sample `{sample.process}`")
             norm_comp_str = ",".join(norm_factor_components)
             norm_str = f"prod::{sample.norm_name}({norm_comp_str})"
             self.import_expression(ws_factory, norm_str)
             proc_yield = ws_factory.function(sample.norm_name).getVal()
-            self.stdout.info(f"REGTEST: Yield for category `{category}` "
+            self.stdout.info(f"Yield for category `{category}` "
                              f"process `{sample.process}`: {proc_yield}")
             if self.debug_mode:
                 ws_factory.Print()
             
             self.get_model(ws_factory, sample, nuis, constraints, globobs)
         
         if self.debug_mode:
             ws_factory.Print()
         
         # generate the combined pdf
         sum_pdf_components = [f"{sample.norm_name}*{sample.model_name}" for sample in samples]
         sum_pdf_str = f"SUM::{self.KEYWORDS['sum_pdf_name']}({','.join(sum_pdf_components)})"
-        self.stdout.debug(f"REGTEST: Sum pdf expr = {sum_pdf_str}")
+        self.stdout.debug(f"Sum pdf expr = {sum_pdf_str}")
         self.import_expression(ws_factory, sum_pdf_str)
         SB_pdf = ws_factory.pdf(self.KEYWORDS['sum_pdf_name'])
 
         self.implement_blind_range(ws_factory)
         
         self.check_nuisance_parameters(SB_pdf, nuis)
         
         # keep track of correlated variables
         correlated_terms = self.get_correlated_terms(ws_factory, nuis)
         correlated_str = ",".join(correlated_terms)
         
-        self.stdout.debug(f"REGTEST: The following variables will not be renamed: {','.join(correlated_terms)}")
+        self.stdout.debug(f"The following variables will not be renamed: {','.join(correlated_terms)}")
         # import pdf to new workspace, rename objects as appropriate
         self.import_object(ws, ws_factory.pdf(self.KEYWORDS['sum_pdf_name']),
                            ROOT.RooFit.RenameAllNodes(category),
                            ROOT.RooFit.RenameAllVariablesExcept(category, correlated_str))
         
         # import constraint terms
         self.attach_constraints(ws, constraints)
@@ -614,15 +614,15 @@
             blind_sf = 1 - (blind_range[1] - blind_range[0]) / (obs.getMax() - obs.getMin())
         if (dataset.numEntries() > (obs.numBins() * blind_sf)):
             dataset_binned = ROOT.RooDataSet(dataset_binned_name, dataset_binned_name,
                                              ROOT.RooArgSet(obs, weight_var),
                                              ROOT.RooFit.WeightVar(weight_var))
             self._fill_dataset_from_hist(dataset_binned, datahist, obs, weight_var)
         num_events = pretty_value(dataset.sumEntries(), 5)
-        self.stdout.info(f"REGTEST: Number of data events: {num_events}")
+        self.stdout.info(f"Number of data events: {num_events}")
         self.import_object(ws, dataset)
         self.import_object(ws, dataset_binned)
         
         self.datahists[category]       = datahist
         self.datasets[category]        = dataset
         self.datasets_binned[category] = dataset_binned
         
@@ -676,15 +676,15 @@
             datahist.Fill(bin_center, weight)
         #  histogram
         elif (filetype == self.KEYWORDS['histogram']):
             histname = data_config['histname']
             h = self.get_histogram(filename, histname)
             for i in range(1, h.GetNbinsX() + 1):
                 if h.GetBinContent(i) < 0:
-                    self.stdout.warning(f"REGTEST: Input data histogram bin {i} in "
+                    self.stdout.warning(f"Input data histogram bin {i} in "
                                         f"category {category_name} has negative weight. "
                                         f"Will force it to zero.", "red")
                     h.SetBinContent(i, 0)
                     h.SetBinError(i, 0)
             
             self._fill_dataset_from_hist(dataset, h, obs, weight_var, data_scale)
             
@@ -758,15 +758,15 @@
                                    f"{category} has fewer bins ({n_bins}) compared "
                                    f"to observable ({obs_n_bins})")
             if (n_bins > obs_n_bins) and (n_bins % obs_n_bins != 0):
                 raise RuntimeError(f"input data histogram `{histname}` in category "
                                    f"{category} has inconsistent number of bins "
                                    f"({n_bins}) compared to observable ({obs_n_bins})")
             else:
-                self.stdout.warning(f"REGTEST: Rebinning input data histogram "
+                self.stdout.warning(f"Rebinning input data histogram "
                                     f"`{histname}` in category {category} by "
                                     f"{n_bins // obs_n_bins} to match the "
                                     f"binning of observable")
                 h.Rebin(n_bins // obs_n_bins)
                 
     @staticmethod
     def _find_bin(h:ROOT.TH1, low_edge:float):
@@ -834,26 +834,26 @@
                 weight_var.setVal(ghost_weight)
                 dataset.add(ROOT.RooArgSet(obs, weight_var), ghost_weight)
                 # also put the ghost weight in the histograms
                 datahist.SetBinContent(i, ghost_weight)
                 
     def attach_constraints(self, ws:ROOT.RooWorkspace, constraints:ROOT.RooArgSet):
         category_name = self.active_category
-        self.stdout.debug(f"REGTEST: Attaching contraint pdfs to workspace for the category {category_name}")
+        self.stdout.debug(f"Attaching contraint pdfs to workspace for the category {category_name}")
         sum_pdf_name = f"{self.KEYWORDS['sum_pdf_name']}_{category_name}"
         final_pdf_name = f"{self.KEYWORDS['final_pdf_name']}_{category_name}"
         remove_set = ROOT.RooArgSet()
         pdf = ws.pdf(sum_pdf_name)
         if not pdf:
             raise RuntimeError(f"sum pdf `{sum_pdf_name}` not defined")
         for constraint in constraints:
             constr_name = constraint.GetName()
             np_name = constr_name.replace(self.KEYWORDS['constrterm_prefix'], "")
             if not pdf.getVariables().find(np_name):
-                self.stdout.warning(f"WARNING: constraint term {constr_name} with NP "
+                self.stdout.warning(f"constraint term {constr_name} with NP "
                                     f"{np_name} is redundant in the category {category_name}. "
                                     f"It will be removed...", "red")
                 remove_set.add(constraint)
             else:
                 self.import_object(ws, constraint)
         for constraint in remove_set:
             constraints.remove(constraint)
@@ -906,24 +906,24 @@
         if not obs:
             raise RuntimeError("observable variable not initialized")        
         # now handle blinding if needed
         blind_range = cat_config['dataset']['blind_range']
         do_blind = self.core_config["do_blind"]
         if do_blind:
             if blind_range:
-                self.stdout.info(f"REGTEST: Implement blind range [{blind_range[0]}, {blind_range[1]}]")
+                self.stdout.info(f"Implement blind range [{blind_range[0]}, {blind_range[1]}]")
                 sideband_lo_range_name = f"{self.KEYWORDS['sb_lo']}_{category_name}"
                 sideband_hi_range_name = f"{self.KEYWORDS['sb_hi']}_{category_name}"
                 blind_range_name = f"{self.KEYWORDS['blind']}_{category_name}"
                 obs.setRange(sideband_lo_range_name, observable_range[0], blind_range[0])
                 obs.setRange(blind_range_name, blind_range[0], blind_range[1])
                 obs.setRange(sideband_hi_range_name, blind_range[1], observable_range[1])
                 if (blind_range[0] == observable_range[0]) and \
                    (blind_range[1] == observable_range[1]):
-                    self.stdout.info(f"REGTEST: Category `{category_name}` is fully blinded. "
+                    self.stdout.info(f"Category `{category_name}` is fully blinded. "
                                      f"No side-band exists.")
                     cat_config['range_name'] = ""
                 elif (blind_range[1] == observable_range[1]):
                     cat_config['range_name'] = sideband_lo_range_name
                 elif (blind_range[0] == observable_range[0]):
                     cat_config['range_name'] = sideband_hi_range_name
                 else:
@@ -952,19 +952,19 @@
                 items_lowpriority.append(item)
             else:
                 _items_highpriority.append(item)
         cat_config['items_highpriority'] = _items_highpriority
     
     def _item_has_dependent(self, expr:str, reference_list:List[str]):
         _, item_type = self._get_object_name_and_type_from_expr(expr)
-        self.stdout.debug(f"REGTEST: item `{expr}` has type `{item_type}`")
+        self.stdout.debug(f"item `{expr}` has type `{item_type}`")
         if item_type in ['variable', 'defined']:
             return False
         item_list = self._decompose_function_expr(expr)
-        self.stdout.debug(f"REGTEST: Composition of high priority item {expr}: "
+        self.stdout.debug(f"Composition of high priority item {expr}: "
                           f"{', '.join(item_list)}")
         for this_name in item_list:
             for reference in reference_list:
                 that_name, _ = self._get_object_name_and_type_from_expr(reference)
                 if this_name == that_name:
                     return True
         return False
@@ -1107,15 +1107,15 @@
             raise RuntimeError(f"no config info found for the category `{category_name}`")
         cat_config = self.cat_config[category_name]
         return cat_config
         
     def read_systematics_node(self, node:Dict, domain:str):
         cat_config = self.get_active_category_config()
         syst_expr = self._get_node_attrib(node, "Name")
-        self.stdout.debug(f"REGTEST: Reading systematic `{syst_expr}`")
+        self.stdout.debug(f"Reading systematic `{syst_expr}`")
         syst = Systematic()
         syst.name = self._translate_node_attrib(node, "Name", domain)
         # if the process of the systematic is specified, use the 
         # specified process. Otherwise use the default one
         syst.process = self._translate_node_attrib(node, "Process", domain, False, "")
         # common systematics
         if domain == self.KEYWORDS['allproc']:
@@ -1159,15 +1159,15 @@
             syst.errorlo = abs(uncert_val[1]) if (uncert_val[1] is not None) else uncert_expr[1]
             # a RooFit feature noticed by Jared:
             # if one uses FlexibleInterpVar to implement a systematic on a process,
             # then for the same systematic on a different process FlexibleInterpVar 
             # has to be used as well. Otherwise the code will crash.
             if syst.constr_term != self.KEYWORDS['asym']:
                 if syst.errorhi != syst.errorlo:
-                    self.stdout.info(f"INFO: Upper uncert. ({syst.errorhi}) and"
+                    self.stdout.info(f"Upper uncert. ({syst.errorhi}) and"
                                      f" lower uncert. ({syst.errorlo}) for"
                                      f" {syst.constr_term} systematic "
                                      f" {syst.name} are not identical. "
                                      f"Will treat as asymmetric uncertainty "
                                      f"using FlexibleInterpVar with "
                                      f"interpolation code 4. Next time "
                                      f"please use keyword {self.KEYWORDS['asym']} "
@@ -1207,25 +1207,25 @@
             cat_config['items_highpriority'].append(item)
         
     def read_channel_import_node(self, node:Dict, ws:ROOT.RooWorkspace):
         filename = self._translate_node_attrib(node, "FileName")
         filepath = self.get_relpath(filename)
         if not os.path.exists(filepath):
             raise FileNotFoundError(f"import XML file `{filepath}` not found")
-        self.stdout.debug(f"REGTEST: Reading import XML file `{filepath}`")
+        self.stdout.debug(f"Reading import XML file `{filepath}`")
         xml_data = TXMLTree.load_as_dict(filepath)
         nodes = xml_data['children']
         self.read_channel_xml_nodes(nodes, ws)
         
     def read_sample_import_node(self, node:Dict, sample:Sample):
         filename = self._translate_node_attrib(node, "FileName")
         filepath = self.get_relpath(filename)
         if not os.path.exists(filepath):
             raise FileNotFoundError(f"import XML file `{filepath}` not found")
-        self.stdout.info(f"REGTEST: Importing items for `{sample.process}` from {filepath}")
+        self.stdout.info(f"Importing items for `{sample.process}` from {filepath}")
         xml_data = TXMLTree.load_as_dict(filepath)
         nodes = xml_data['children']
         self.read_sample_subnode(nodes, sample)
     
     def read_sample_factor_node(self, node:Dict, sample:Sample, factor_type:str):
         factor = self._translate_node_attrib(node, "Name", sample.process)
         if factor_type == "norm":
@@ -1353,15 +1353,15 @@
             if norm_value != "":
                 norm_name = self.KEYWORDS[f'{key}_name']
                 sample.norm_factors.append(f"{norm_name}_{sample.process}[{norm_value}]")
                 
         sample.share_pdf_group = self._translate_node_attrib(node, "SharePdf", sample.process,
                                                              required=False, default="")
         subnodes = node['children']
-        self.stdout.debug(f"REGTEST: Reading sample `{sample.process}`")
+        self.stdout.debug(f"Reading sample `{sample.process}`")
         self.read_sample_subnode(subnodes, sample)
         self.add_sample_object(sample)
         
     def read_sample_subnode(self, nodes:List, sample:Sample):
         for node in nodes:
             name = node['tag']
             if name == "Systematic":
@@ -1394,15 +1394,15 @@
         if syst.domain != self.KEYWORDS['allproc']:
             var_name += f"_{syst.process}"
         glob_name = self.KEYWORDS['globalobs_prefix'] + syst.name
         constr_name = self.KEYWORDS['constrterm_prefix'] + syst.name
         response_name = self.KEYWORDS['response_prefix'] + var_name
         
         if syst.constr_term == self.KEYWORDS['asym']:
-            self.stdout.debug(f"REGTEST: Set up nuisance parameter {syst.name} as asymmetric uncertainty "
+            self.stdout.debug(f"Set up nuisance parameter {syst.name} as asymmetric uncertainty "
                               f"on the process {syst.process}")
             nuis_var = ROOT.RooRealVar(syst.name, syst.name, 0, -5, 5)
             beta_name = f"beta_{var_name}"
             beta_var = ROOT.RooRealVar(beta_name, beta_name, syst.beta)
             nuis_times_beta_name = f"{var_name}_times_beta"
             nuis_times_beta = ROOT.RooProduct(nuis_times_beta_name, nuis_times_beta_name, 
                                               ROOT.RooArgSet(nuis_var, beta_var))
@@ -1434,15 +1434,15 @@
                 self.import_object(ws, expected_var)
         else:
             nominal_expr = self.import_expression(ws, f"nominal_{var_name}[{syst.nominal}]")
             np_name = self.import_expression(ws, f"{syst.name}[0, -5, 5]", True)
             _buffer = f"prod::{var_name}_times_beta({syst.name}, beta_{var_name}[{syst.beta}])"
             nuis_times_beta_expr = self.import_expression(ws, _buffer)
             uncert_name = self.import_uncert_expr(ws, syst.errorhi, var_name, self.KEYWORDS['uncert_sym_prefix'])
-            self.stdout.debug(f"REGTEST: Set up nuisance parameter {syst.name} as {syst.constr_term} "
+            self.stdout.debug(f"Set up nuisance parameter {syst.name} as {syst.constr_term} "
                               f"uncertainty on process {syst.process}")
             if (syst.constr_term in [self.KEYWORDS['gaussian'], self.KEYWORDS['dfd']]):
                 # the reason we need to keep plain implementation for Gaussian uncertainty is mainly due to spurious signal.
                 # if we use FlexibleInterpVar, the response will be truncated at 0, but we need the response to go negative.
                 uncert_wrapper_expr = f"prod::uncert_{syst.constr_term}_{var_name}({nuis_times_beta_expr}, {uncert_name})"
                 expected_expr = f"sum::{response_name}({nominal_expr}, {uncert_wrapper_expr})"
                 self.import_expression(ws, expected_expr)
@@ -1456,41 +1456,41 @@
                 raise RuntimeError(f"unknown constraint type {syst.constr_term} for NP {syst.name} "
                                    f"in process {syst.process}. Available choices: "
                                    f"{self.KEYWORDS['logn']} (lognormal), "
                                    f"{self.KEYWORDS['gaussian']} (gaussian), "
                                    f"{self.KEYWORDS['asym']} (asymmetric), "
                                    f"{self.KEYWORDS['dfd']} (double-fermi-dirac) ")
         if syst.constr_term == self.KEYWORDS['dfd']:
-            self.stdout.debug(f"REGTEST: Creating DFD constraint term for NP {syst.name}")
+            self.stdout.debug(f"Creating DFD constraint term for NP {syst.name}")
             self.import_expression(ws, f"EXPR::{constr_name}('1/((1+exp(@2*(@0-@3-@1)))*(1+exp(-1*@2*"
                                f"(@0-@3+@1))))', {syst.name}, DFD_e[1], DFD_w[500], {glob_name}[0,-5,5])", True)
         else:
-            self.stdout.debug(f"REGTEST: Creating RooGaussian constraint term for NP {syst.name}")
+            self.stdout.debug(f"Creating RooGaussian constraint term for NP {syst.name}")
             self.import_expression(ws, f"RooGaussian::{constr_name}({syst.name}, {glob_name}[0,-5,5],1)", True)
         nuis.add(ws.var(syst.name), True)
         constraint.add(ws.pdf(constr_name), True)
         globobs.add(ws.var(glob_name), True)
         expected.add(ws.function(response_name), True)
-        self.stdout.debug(f"REGTEST: Finished implementing systematic {syst.name}")
+        self.stdout.debug(f"Finished implementing systematic {syst.name}")
     
     def get_model(self, ws:ROOT.RooWorkspace, sample:Sample, nuis:ROOT.RooArgSet,
                   constraints:ROOT.RooArgSet, globobs:ROOT.RooArgSet):
-        self.stdout.debug("REGTEST: Getting model")
+        self.stdout.debug("Getting model")
         tag_name = sample.get_tag_name()
         sample.model_name = self.KEYWORDS['pdf_prefix'] + tag_name
 
         if ws.pdf(sample.model_name):
             is_shared_pdf = sample.share_pdf_group != ""
             if is_shared_pdf:
                 # use shared pdf
-                self.stdout.debug(f"REGTEST: PDF {sample.model_name} has been created in the workpace.")
+                self.stdout.debug(f"PDF {sample.model_name} has been created in the workpace.")
                 return None
             else:
                 raise RuntimeError(f"PDF {sample.model_name} already exists but the user asks to create it again")
-        self.stdout.debug(sample.model_name)
+        self.stdout.debug(sample.model_name, bare=True)
         cat_config = self.get_active_category_config()
         is_counting = cat_config['category_type'] == self.KEYWORDS['counting']
         obs_name = cat_config['observable']['name']
         if is_counting:
             # in counting experiment we only need a uniform pdf
             self.import_expression(ws, f"RooUniform::{sample.model_name}({obs_name})")
         else:
@@ -1502,15 +1502,15 @@
         filepath = self.get_relpath(filename)
         if not os.path.exists(filepath):
             raise FileNotFoundError(f"model xml file `{filepath}` not found")
         root_node = TXMLTree.load_as_dict(filepath)
         
         model_type = self._get_node_attrib(root_node, "Type").lower()
         if model_type == self.KEYWORDS['userdef']:
-            self.stdout.debug(f"REGTEST: Creating user-defined pdf from `{filepath}`")
+            self.stdout.debug(f"Creating user-defined pdf from `{filepath}`")
             self.build_userdef_model(root_node, ws, sample)
         elif model_type == self.KEYWORDS['external']:
             self.build_external_model(root_node, ws, sample, nuis, constraints, globobs)
         elif model_type == self.KEYWORDS['histogram']:
             self.build_histogram_model(root_node, ws, sample)
         else:
             raise RuntimeError(f"unknown model type: {model_type} . Available choice: "
@@ -1528,15 +1528,15 @@
                 raise RuntimeError("observable not initialized")
             # for the accuracy of Fourier transformation
             obs.setBins(cache_binning, "cache")
         is_success = False
         nodes = root_node['children']
         for node in nodes:
             name = node['tag']
-            self.stdout.debug(f"REGTEST: Reading node `{name}`")
+            self.stdout.debug(f"Reading node `{name}`")
             if name == "Item":
                 expr = self._translate_node_attrib(node, "Name", tag_name)
                 self.import_expression(ws, expr)
             elif name == "ModelItem":
                 factory_str = self._translate_node_attrib(node, "Name", tag_name)
                 str_start = factory_str.find("::")+2
                 str_end   = factory_str.find("(")
@@ -1560,15 +1560,15 @@
             raise FileNotFoundError(f"input file `{filepath}` not found")
         ws_name = self._translate_node_attrib(root_node, "WSName")
         model_name = self._translate_node_attrib(root_node, "ModelName")
         observable_name = self._translate_node_attrib(root_node, "ObservableName")
         tag_name = sample.get_tag_name()
         nodes = root_node['children']
         np_list, glob_list, constr_list = [], [], []
-        self.stdout.debug(f"REGTEST: Use existing PDF `{model_name}` from the workspace `{filename}`")
+        self.stdout.debug(f"Use existing PDF `{model_name}` from the workspace `{filename}`")
         
         f_ext = ROOT.TFile(filename)
         ws_ext = f_ext.Get(ws_name)
         pdf_ext = ws_ext.function(model_name)
         
         name_maps = {}
         do_not_touch = [observable_name]
@@ -1583,15 +1583,15 @@
                 var = ws_ext.var(var_name)
                 if not var:
                     raise RuntimeError(f"no variable named `{var_name}` found im the workspace `{filepath}`")
                 var.setConstant(1)
                 var_val = self._get_node_attrib(node, "Value", False, "")
                 if var_val != "":
                     var.setVal(float(var))
-                self.stdout.debug(f"REGTEST: Fixed variable `{var_name}` at `{var.getVal()}")
+                self.stdout.debug(f"Fixed variable `{var_name}` at `{var.getVal()}")
             elif name == "Rename":
                 # rename the object names in the input workspace
                 old_name = self._translate_node_attrib(node, "OldName", tag_name)
                 new_name = self._translate_node_attrib(node, "NewName", tag_name)
                 do_not_touch.append(old_name)
                 name_maps[old_name] = new_name
             elif name == "ExtSyst":
@@ -1618,32 +1618,32 @@
             ws_temp.Print()
             
         pdf = ws_temp.function(f"{model_name}_{tag_name}")
         obs_ext = ws_temp.var(observable_name)
         if not obs_ext:
             raise RuntimeError(f"observable `{observable_name}` not found in the workspace `{filepath}`")
         if not isinstance(pdf, ROOT.RooAbsPdf):
-            self.stdout.warning(f"WARNING: The object {model_name} is not a p.d.f as seen from RoOFit")
-            self.stdout.warning("REGTEST: Constructing RooRealSumPdf for the pdf from histFactory")
+            self.stdout.warning(f"The object {model_name} is not a p.d.f as seen from RoOFit")
+            self.stdout.warning("Constructing RooRealSumPdf for the pdf from histFactory")
             dummy_pdf = ROOT.RooUniform(f"{sample.model_name}_dummpy_pdf", "for RooRealSumPdf construction",
                                         obs_ext)
             frac = ROOT.RooRealVar(f"{sample.model_name}_real_pdf_frac", "for RooRealSumPdf construction", 1)
             pdf = ROOT.RooRealSumPdf(sample.model_name, "from histFactory", ROOT.RooArgList(pdf, dummy_pdf),
                                      ROOT.RooArgList(frac))
         else:
             name_maps[pdf.GetName()] = sample.model_name
         
         # rename observable (this step should never happen for a HistFactory workspace)
         if observable_name != _observable_name:
             name_maps[observable_name] = _observable_name
-        self.stdout.info("REGTEST: The following variables will be renamed:")
+        self.stdout.info("The following variables will be renamed:")
         old_str = ",".join(name_maps.keys())
         new_str = ",".join(name_maps.values())
-        self.stdout.info(f"REGTEST: Old: {old_str}")
-        self.stdout.info(f"REGTEST: New: {new_str}")
+        self.stdout.info(f"Old: {old_str}")
+        self.stdout.info(f"New: {new_str}")
         
         self.import_object(ws, pdf, ROOT.RooFit.RenameVariable(old_str, new_str),
                            ROOT.RooFit.RecycleConflictNodes())
         # import constraint terms
         for np_name, glob_name, constr_name in zip(np_list, glob_list, constr_list):
             new_np_name = np_name
             # check wheterh NP has been renamed. If yes, update the NP name
@@ -1658,29 +1658,29 @@
                 new_constr_name = self.KEYWORDS['constrterm_prefix'] + new_np_name
                 new_glob_name = self.KEYWORDS['globalobs_prefix'] + new_np_name
                 constr_pdf = ws_ext.pdf(constr_name)
                 old_str = ",".join([constr_name, glob_name, np_name])
                 new_str = ",".join([new_constr_name, new_glob_name, new_np_name])
                 self.import_object(ws, constr_pdf, 
                                    ROOT.RooFit.RenameVariable(old_str, new_str))
-                self.stdout.debug(f"REGTEST: Import systematics {new_np_name} "
+                self.stdout.debug(f"Import systematics {new_np_name} "
                                   f"with constraint term {new_constr_name}")
                 constraints.add(ws.pdf(new_constr_name), True)
                 globobs.add(ws.var(new_glob_name), True)
             ws.var(new_np_name).setConstant(False)
             nuis.add(ws.var(new_np_name), True)
     
     def build_histogram_model(self, root_node:Dict, ws:ROOT.RooWorkspace, sample:Sample):
         cat_config = self.get_active_category_config()
         obs_name = cat_config['observable']['name']
         filename = self._translate_node_attrib(root_node, "Input")
         filepath = self.get_relpath(filename)
         histname = self._translate_node_attrib(root_node, "ModelName")
         rebin = self._get_node_attrib(root_node, "Rebin", False, "-1", dtype="int")
-        self.stdout.debug(f"REGTEST: Creating histogram pdf from `{filepath}`")
+        self.stdout.debug(f"Creating histogram pdf from `{filepath}`")
         h = self.get_histogram(filename, histname)
         if rebin > 0:
             h.Rebin(rebin)
         obs = ws.var(obs_name)
         if not obs:
             raise RuntimeError("observable not initialized")
         h_data = ROOT.RooDataHist("hdata", "hdata", obs, h)
@@ -1692,15 +1692,15 @@
         obs_name = cat_config['observable']['name']        
         var_set = model.getVariables()
         float_set = ROOT.RooArgSet()
         for var in var_set:
             if (not var.isConstant()):
                 if var.getMin() == var.getMax():
                     var_name = var.GetName()
-                    self.stdout.info(f"REGTEST: Fixing {var_name} to constant as it has same upper and loer boundary")
+                    self.stdout.info(f"Fixing {var_name} to constant as it has same upper and loer boundary")
                     var.setConstant(True)
                 else:
                     float_set.add(var)
         poi_obs_names = self.core_config['poi_names'] + [obs_name]
         # reove POI and observable from float set
         for name in poi_obs_names:
             float_var = float_set.find(name)
@@ -1708,22 +1708,22 @@
                 float_set.remove(float_var)
         num_np = len(nuis)
         num_poi = len(self.core_config['poi_names'])
         for var in float_set:
             if not nuis.find(var):
                 nuis.add(var)
                 var_name = var.GetName()
-                self.stdout.info(f"REGTEST: Adding {var_name} to the nuisance parameter set")
+                self.stdout.info(f"Adding {var_name} to the nuisance parameter set")
 
         num_float = len(float_set)
         if num_float < num_np:
-            self.stdout.warning(f"WARNING: There supposed to be {num_poi + num_np} free parameters, "
+            self.stdout.warning(f"There supposed to be {num_poi + num_np} free parameters, "
                                 f"but only seen {num_float} in the category {self.active_category}. "
                                 f"This is in principle not an issue, but please make sure you "
                                 f"understand what you are doing")
             if self.debug_mode:
-                self.stdout.debug("REGTEST: All free parameters: ")
+                self.stdout.debug("All free parameters: ")
                 float_set.Print()
-                self.stdout.debug("REGTEST: All nuisance parameters: ")
+                self.stdout.debug("All nuisance parameters: ")
                 nuis.Print()
         else:
-            self.stdout.info("REGTEST: Number of nuisance parameters looks good!")
+            self.stdout.info("Number of nuisance parameters looks good!")
```

### Comparing `quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_builder_v2.py` & `quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_builder_v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,32 +77,32 @@
         categories = []
         for category, file in self.core_config['input_categories'].items():
             self.path_manager.set_file(f"__Cat_{category}", file)
                                        
     @semistaticmethod
     def set_data_storage_type(self, data_storage_type:Union[str, DataStorageType]="vector") -> None:
         data_storage_type = DataStorageType.parse(data_storage_type)
-        self.stdout.info(f'INFO: Set data storage type to "{data_storage_type.name}"')
+        self.stdout.info(f'Set data storage type to "{data_storage_type.name}"')
         if data_storage_type == DataStorageType.Tree:
             ROOT.RooAbsData.setDefaultStorageType(ROOT.RooAbsData.StorageType.Tree)
         elif data_storage_type == DataStorageType.Vector:
             ROOT.RooAbsData.setDefaultStorageType(ROOT.RooAbsData.StorageType.Vector)
         elif data_storage_type == DataStorageType.Composite:
             ROOT.RooAbsData.setDefaultStorageType(ROOT.RooAbsData.StorageType.Composite)            
         else:
             raise RuntimeError(f'unknown data storage type "{data_storage_type}"')
             
     @semistaticmethod
     def set_integrator(self, integrator:Optional[str]=None) -> None:
         if integrator:
-            self.stdout.warn(f'WARNING: Set default integrator to "{integrator}"')
+            self.stdout.warn(f'Set default integrator to "{integrator}"')
             ROOT.RooAbsReal.defaultIntegratorConfig().method1D().setLabel(integrator)
     
     def parse_core_xml(self, filename:str) -> Dict:
-        self.stdout.info(f'INFO: Parsing file "{filename}"')
+        self.stdout.info(f'Parsing file "{filename}"')
         # load xml file
         core_xml = TXMLTree.load_as_dict(filename)
         # parse core attributes
         attributes = core_xml['attrib']
         core_config = {
             'base_dir'           : os.path.dirname(filename),
             'workspace_name'     : self._get_node_attrib(core_xml, 'WorkspaceName'),
@@ -140,15 +140,15 @@
             }
         else:
             raise FileNotFoundError("directories for importing class code do not exist "
                                     f"(decl = `{class_decl_import_dir}`, impl = `{class_impl_import_dir}`)")
         # make sure output filename has .root extension
         if not core_config['output_name'].endswith(".root"):
             core_config['output_name'] = os.path.splitext(core_config['output_name'])[0] + ".root"
-            self.stdout.warning('WARNING: Output file name does not contain ".root" postfix. '
+            self.stdout.warning('Output file name does not contain ".root" postfix. '
                                 'Adding it to avoid confusion.')
         # parse child level nodes
         nodes = core_xml['children']
         for node in nodes:
             tag = node['tag']
             if tag == "Input":
                 file = node['text']
@@ -166,84 +166,84 @@
             else:
                 raise RuntimeError(f"unknown item `{tag}`")
         return core_config
     
     def print_init_summary(self) -> None:
         if not self.core_config:
             raise RuntimeError("core config not set")
-        self.stdout.info("="*74)
-        self.stdout.info("Output file: ".rjust(20) + f"{self.core_config['output_name']}")
-        self.stdout.info("Workspace name: ".rjust(20) + f"{self.core_config['workspace_name']}")
-        self.stdout.info("ModelConfig name: ".rjust(20) + f"{self.core_config['model_config_name']}")
-        self.stdout.info("Dataset name: ".rjust(20) + f"{self.core_config['dataset_name']}")
-        self.stdout.info("Blind analysis: ".rjust(20) + ("True" if self.core_config['do_blind'] else "False"))
-        self.stdout.info("Generate hist data: ".rjust(20) + ("True" if self.core_config['generate_hist_data'] else "False"))
-        self.stdout.info("Scale lumi: ".rjust(20) + f"{self.core_config['scale_lumi']}")
-        self.stdout.info("POIs: ".rjust(20) + ", ".join(self.core_config['poi_names']))
-        self.stdout.info("")
-        self.stdout.info("Categories to be included:")
+        self.stdout.info("="*74, bare=True)
+        self.stdout.info("Output file: ".rjust(20) + f"{self.core_config['output_name']}", bare=True)
+        self.stdout.info("Workspace name: ".rjust(20) + f"{self.core_config['workspace_name']}", bare=True)
+        self.stdout.info("ModelConfig name: ".rjust(20) + f"{self.core_config['model_config_name']}", bare=True)
+        self.stdout.info("Dataset name: ".rjust(20) + f"{self.core_config['dataset_name']}", bare=True)
+        self.stdout.info("Blind analysis: ".rjust(20) + ("True" if self.core_config['do_blind'] else "False"), bare=True)
+        self.stdout.info("Generate hist data: ".rjust(20) + ("True" if self.core_config['generate_hist_data'] else "False"), bare=True)
+        self.stdout.info("Scale lumi: ".rjust(20) + f"{self.core_config['scale_lumi']}", bare=True)
+        self.stdout.info("POIs: ".rjust(20) + ", ".join(self.core_config['poi_names']), bare=True)
+        self.stdout.info("", bare=True)
+        self.stdout.info("Categories to be included:", bare=True)
         input_categories = self.core_config['input_categories']
         for i, input_category in enumerate(input_categories.values()):
-            self.stdout.info(f"XML file {i}: ".rjust(20) + f"{input_category}")
+            self.stdout.info(f"XML file {i}: ".rjust(20) + f"{input_category}", bare=True)
         asimov_definitions = self.core_config['asimov_definitions']
         if asimov_definitions:
-            self.stdout.info("")
-            self.stdout.info("The following asimov dataset(s) will be generated:")
+            self.stdout.info("", bare=True)
+            self.stdout.info("The following asimov dataset(s) will be generated:", bare=True)
             for asimov_def in asimov_definitions:
                 is_gen_asimov = GEN_ASIMOV_ACTION in asimov_def['Action']
                 if is_gen_asimov:
                     asimov_name = asimov_def['Name']
-                    self.stdout.info(f"\t{asimov_name}")
+                    self.stdout.info(f"\t{asimov_name}", bare=True)
         self.stdout.info("="*74)
 
     def print_final_summary(self) -> None:
         ws_name = self.comb_ws.GetName()
         model = ExtendedModel(self.comb_ws, data_name=self.core_config['dataset_name'], verbosity="WARNING")
         pdf = model.pdf
         cat = pdf.indexCat()
         n_cat = len(cat)
         data = model.data
         data_list = data.split(cat, True)
         # start writing summary
-        self.stdout.info("="*74)
+        self.stdout.info("="*74, bare=True)
         title_str = format_delimiter_enclosed_text("Begin summary", "~")
-        self.stdout.info(title_str)
-        self.stdout.info(f"\tThere are {n_cat} sub channels:")
+        self.stdout.info(title_str, bare=True)
+        self.stdout.info(f"\tThere are {n_cat} sub channels:", bare=True)
         for i in range(n_cat):
             cat.setBin(i)
             cat_name = cat.getLabel()
             pdf_i = pdf.getPdf(cat_name)
             data_i = data_list.FindObject(cat_name)
             sum_entries = pretty_value(data_i.sumEntries(), 5)
-            self.stdout.info(f"\t\tIndex: {i}, Pdf: {pdf_i.GetName()}, Data: {data_i.GetName()}, SumEntries: {sum_entries}")
+            self.stdout.info(f"\t\tIndex: {i}, Pdf: {pdf_i.GetName()}, Data: {data_i.GetName()}, SumEntries: {sum_entries}", bare=True)
         title_str = format_delimiter_enclosed_text("POI", "-")
-        self.stdout.info(title_str)
+        self.stdout.info(title_str, bare=True)
         if Verbosity.INFO >= self.stdout.verbosity:
             model.pois.Print("v")
         title_str = format_delimiter_enclosed_text("Dataset", "-")
-        self.stdout.info(title_str)
+        self.stdout.info(title_str, bare=True)
         if Verbosity.INFO >= self.stdout.verbosity:
             for dataset in model.workspace.allData():
                 dataset.Print()
         title_str = format_delimiter_enclosed_text("End Summary", "~")
-        self.stdout.info(title_str)
+        self.stdout.info(title_str, bare=True)
         output_path = self.path_manager.get_file("output")
-        self.stdout.info(f"Workspace `{ws_name}` has been successfully generated and saved in file `{output_path}`")
+        self.stdout.info(f"Workspace `{ws_name}` has been successfully generated and saved in file `{output_path}`", bare=True)
         #output_plot_path = self.get_output_plot_path()
         #self.stdout.info(f"Plots for each category are summarized in `{output_plot_path}`")
-        self.stdout.info(f"Total time taken: {self.time_taken:.3f}s")
-        self.stdout.info("="*74)
+        self.stdout.info(f"Total time taken: {self.time_taken:.3f}s", bare=True)
+        self.stdout.info("="*74, bare=True)
                          
     def generate_asimov(self, ws:Optional["ROOT.RooWorkspace"]=None) -> None:
         if ws is None:
             ws = self.comb_ws
         asimov_definitions = self.core_config['asimov_definitions']
         if self.use_binned:
             data_name = self.core_config['dataset_name'] + "binned"
-            self.stdout.warning("REGTEST: Fitting binned dataset.", "red")
+            self.stdout.warning("Fitting binned dataset.", "red")
         else:
             data_name = self.core_config['dataset_name']
         range_name = self.get_fit_range_name()
         self._generate_asimov(ws, asimov_definitions=asimov_definitions,
                               data_name=data_name, range_name=range_name,
                               minimizer_config=self.minimizer_config)
         
@@ -281,15 +281,15 @@
         ws_factory = ROOT.RooWorkspace(f"factory_{category}")
         resp_func_map  = {}
         # load category xml file
         filepath = self.path_manager.get_file(f"__Cat_{category}", check_exist=True)
         cat_xml = TXMLTree.load_as_dict(filepath)
             
         title_str = format_delimiter_enclosed_text(f"Category {category}", "-")
-        self.stdout.info(title_str)
+        self.stdout.info(title_str, bare=True)
         
         self.active_category = category
         category_type = self._get_node_attrib(cat_xml, 'Type').lower()
     
         # define luminosity
         if self.core_config['scale_lumi'] > 0:
             lumi_default = 1
@@ -334,20 +334,20 @@
         remained_nodes = [node for node in nodes if node['tag'] not in ["Data", "Correlate"]]
         self.read_channel_xml_nodes(remained_nodes, ws_factory)
  
         self._fix_item_priority()
         items_highpriority  = self.cat_config[category]['items_highpriority']
         items_lowpriority   = self.cat_config[category]['items_lowpriority']
         
-        self.stdout.debug("REGTEST: High priority items:")
+        self.stdout.debug("High priority items:")
         for item in items_highpriority:
-            self.stdout.debug(f"\t{item}")
-        self.stdout.debug("REGTEST: Low priority items:")
+            self.stdout.debug(f"\t{item}", bare=True)
+        self.stdout.debug("Low priority items:")
         for item in items_lowpriority:
-            self.stdout.debug(f"\t{item}")
+            self.stdout.debug(f"\t{item}", bare=True)
         # first implement high priority items: common variables 
         # and functions not involving systematic uncertainties
         self.import_expressions(ws_factory, items_highpriority)
         
         # secondly implement systematics and import them into the workspace
         self.implement_systematics(ws_factory)
 
@@ -371,15 +371,15 @@
         
         self.check_nuisance_parameters(sum_pdf, core_argsets.nuis_set)
         
         # keep track of correlated variables
         correlated_terms = self.get_correlated_terms(ws_factory, core_argsets.nuis_set)
         correlated_str = ",".join(correlated_terms)
         
-        self.stdout.debug(f"REGTEST: The following variables will not be renamed: {correlated_str}")
+        self.stdout.debug(f"The following variables will not be renamed: {correlated_str}")
         # import pdf to new workspace, rename objects as appropriate
         self.import_object(ws, ws_factory.pdf(SUM_PDF_NAME),
                            ROOT.RooFit.RenameAllNodes(category),
                            ROOT.RooFit.RenameAllVariablesExcept(category, correlated_str))
         
         # import constraint terms
         self.attach_constraints(ws, core_argsets.constr_set)
@@ -389,15 +389,15 @@
         core_argsets.poi_set = core_argsets.get_argset_by_names(ws, poi_names)
         core_argsets.define_argsets(ws)
         
         if self.debug_mode:
             ws.Print()
             
         obs = self.get_observable(ws)
-        weight_var = ROOT.RooRealVar("wt", "wt", 1)
+        weight_var = ROOT.RooRealVar("weight", "weight", 1)
         dataset, datahist = self.generate_dataset(obs, weight_var)
     
         # prepare binned data
         dataset_binned_name = f"{OBS_DATASET_NAME}binned"
         dataset_binned = dataset.Clone(dataset_binned_name)
         
         # consider that blinded analysis the number of bins will reduce
@@ -412,15 +412,15 @@
         if (dataset.numEntries() > (obs.numBins() * blind_sf)):
             dataset_binned = ROOT.RooDataSet(dataset_binned_name, dataset_binned_name,
                                              ROOT.RooArgSet(obs, weight_var),
                                              ROOT.RooFit.WeightVar(weight_var))
             RooDataSet.fill_from_TH1(dataset_binned, datahist, blind_range=blind_range,
                                      min_bin_value=self.EPSILON / 1000.)
         num_events = pretty_value(dataset.sumEntries(), 5)
-        self.stdout.info(f"REGTEST: Number of data events: {num_events}")
+        self.stdout.info(f"Number of data events: {num_events}")
         self.import_object(ws, dataset)
         self.import_object(ws, dataset_binned)
         
         if self.core_config['generate_hist_data']:
             datahist_name = f"{OBS_DATASET_NAME}hist"
             rdatahist = ROOT.RooDataHist(datahist_name, datahist_name, ROOT.RooArgSet(obs), datahist)
             ws.Import(rdatahist)
@@ -432,24 +432,24 @@
         return ws
     
     def implement_sum_pdf(self, ws:ROOT.RooWorkspace):
         cat_config = self.get_active_category_config()
         samples = cat_config['samples']
         sum_pdf_components = [f"{sample.norm_name}*{sample.model_name}" for _, sample in samples.items()]
         sum_pdf_str = f"SUM::{SUM_PDF_NAME}({','.join(sum_pdf_components)})"
-        self.stdout.debug(f"REGTEST: Sum pdf expr = {sum_pdf_str}")
+        self.stdout.debug(f"Sum pdf expr = {sum_pdf_str}")
         self.import_expression(ws, sum_pdf_str)
         
     def implement_samples(self, ws:ROOT.RooWorkspace):
         category = self.active_category
         cat_config = self.get_active_category_config()
         resp_func_map = cat_config['resp_func_map']
         samples = cat_config['samples']
         for _, sample in samples.items():
-            self.stdout.debug(f'DEBUG: Implementing sample for the process "{sample.process}"')
+            self.stdout.debug(f'Implementing sample for the process "{sample.process}"')
             self.import_expressions(ws, sample.shape_factors)
             sample.norm_name = YIELD_PREFIX + sample.process
             norm_factor_components = []
             sample_norm_factors = self.import_expressions(ws, sample.norm_factors)
             norm_factor_components.append(sample_norm_factors)
             # common systematics: only add if exist
             for syst_domain in sample.syst_domains:
@@ -463,15 +463,15 @@
                     continue
                 else:
                     raise RuntimeError(f"unknown systematic domain {syst_domain} in sample {sample.process}")
             norm_factor_components_str = ",".join(norm_factor_components)
             norm_factor_expr = f"prod::{sample.norm_name}({norm_factor_components_str})"
             self.import_expression(ws, norm_factor_expr)
             proc_yield = ws.function(sample.norm_name).getVal()
-            self.stdout.info(f'INFO: Yield for category "{category}" '
+            self.stdout.info(f'Yield for category "{category}" '
                              f'process "{sample.process}": {proc_yield}')
             if self.debug_mode:
                 ws.Print()
             self.implement_sample_model(ws, sample)      
     
     def implement_systematics(self, ws:ROOT.RooWorkspace):
         cat_config = self.get_active_category_config()
@@ -537,44 +537,49 @@
             datahist.Fill(bin_center, weight)
         #  histogram
         elif (filetype == DATA_SOURCE_HISTOGRAM):
             histname = data_config['histname']
             h = self.get_histogram(filename, histname)
             neg_bin_indices, _ = TH1.remove_negative_bins(h)
             for i in neg_bin_indices:
-                self.stdout.warning(f"REGTEST: Input data histogram bin {i} in "
+                self.stdout.warning(f"Input data histogram bin {i} in "
                                     f"category {category_name} has negative weight. "
                                     f"Will force it to zero.", "red")
             if blind_range:
                 TH1.apply_blind_range(h, blind_range)
             RooDataSet.fill_from_TH1(dataset, h,
                                      blind_range=blind_range,
                                      min_bin_value=self.EPSILON / 1000.,
                                      weight_scale=data_scale)
             rebin_ratio = TH1.rebin_to_variable(h, obs, tol=self.EPSILON)
             if rebin_ratio != 1:
-                self.stdout.warning(f"REGTEST: Rebinning input data histogram "
+                self.stdout.warning(f"Rebinning input data histogram "
                                     f"`{histname}` in category {category_name} by "
                                     f"{rebin_ratio} to match the binning of the observable")
             TH1.copy_histogram_in_effective_range(h, datahist, tol=self.EPSILON,
                                                   weight_scale=data_scale)
         else:
             if filetype == DATA_SOURCE_ASCII:
                 filepath = self.path_manager.get_relpath(filename)
-                dataset_tmp = self.get_dataset_from_ascii_file(filepath, obs, weight_var)
+                dataset_name = f"{OBS_DATASET_NAME}_tmp"
+                dataset_tmp = RooDataSet.get_dataset_from_txt_file(filepath, obs,
+                                                                   weight_var, dataset_name)
             else:
-                cut      = data_config['cut']
-                treename = data_config['treename']
-                varname  = data_config['varname']
-                chain, _ = self.get_chain_and_branch(filepath, treename, varname, cut)
-                x_tree = ROOT.RooRealVar(varname, varname, obs.getMin(), obs.getMax())
-                _dataset_name = f"{OBS_DATASET_NAME}_tmp"
-                dataset_tmp = ROOT.RooDataSet(_dataset_name, _dataset_name,
-                                              ROOT.RooArgSet(x_tree),
-                                              ROOT.RooFit.Import(chain))
+                filepaths = [self.path_manager.get_relpath(filename) for filename in filename.split(',')]
+                kwargs = {
+                    'filenames'         : filepaths,
+                    'observable'        : obs,
+                    'treename'          : data_config['treename'],
+                    'branchname'        : data_config['varname'],
+                    'weight_branchname' : data_config['weightname'],
+                    'cut'               : data_config['cut'],
+                    'weight_var'        : weight_var,
+                    'dataset_name'      : f"{OBS_DATASET_NAME}_tmp"
+                }
+                dataset_tmp = RooDataSet.get_dataset_from_root_files(**kwargs)
             xdata_tmp = dataset_tmp.get().first()          
             for i in range(dataset_tmp.numEntries()):
                 dataset_tmp.get(i)
                 x_val = xdata_tmp.getVal()
                 obs.setVal(x_val)
                 weight = dataset_tmp.weight() * data_scale
                 weight_var.setVal(weight)
@@ -592,70 +597,29 @@
         if self.debug_mode:
             dataset.Print("v")
         # inject ghost
         if data_config['inject_ghost']:
             RooDataSet.add_ghost_weights(dataset, blind_range=blind_range, ghost_weight=self.EPSILON / 1000.)
             TH1.add_ghost_weights(datahist, blind_range=blind_range, ghost_weight=self.EPSILON / 1000.)
         return dataset, datahist
-    
-    def get_dataset_from_ascii_file(self, file:str, obs:ROOT.RooRealVar, weight_var:ROOT.RooRealVar):
-        cat_config = self.get_active_category_config()
-        weighted_data = cat_config['weighted_data']
-        if weighted_data:
-            dataset_name = f"{OBS_DATASET_NAME}_tmp"
-            dataset = ROOT.RooDataSet(dataset_name, dataset_name,
-                                      ROOT.RooArgSet(obs, weight_var),
-                                      ROOT.RooFit.WeightVar(weight_var))
-            try:
-                data = np.loadtxt(file)
-            except:
-                raise RuntimeError('invalid ascii file format')
-            assert (data.ndim == 2) and (data.shape[1] == 2)
-            for data_i in data:
-                obs.setVal(data_i[0])
-                weight.setVal(data_i[1])
-                dataset.add(ROOT.RooArgSet(obs, weight), weight)
-        else:
-            dataset = ROOT.RooDataSet.read(file, ROOT.RooArgList(obs))
-            if not dataset:
-                raise FileNotFoundError(f"data file {file} does not exist")
-        return dataset    
-        
-    def release_ghost(self, dataset:ROOT.RooDataSet, datahist:ROOT.RooDataHist,
-                      obs:ROOT.RooRealVar, weight_var:ROOT.RooRealVar, ghost_weight:float):
-        do_blind = self.core_config['do_blind']
-        cat_config = self.get_active_category_config()
-        blind_range = cat_config['dataset']['blind_range']
-        n_bins = datahist.GetNbinsX()
-        for i in range(1, n_bins + 1):
-            if datahist.GetBinContent(i) == 0:
-                bin_center = datahist.GetBinCenter(i)
-                if (do_blind and blind_range) and \
-                   (bin_center > blind_range[0]) and (bin_center < blind_range[1]):
-                    continue
-                obs.setVal(bin_center)
-                weight_var.setVal(ghost_weight)
-                dataset.add(ROOT.RooArgSet(obs, weight_var), ghost_weight)
-                # also put the ghost weight in the histograms
-                datahist.SetBinContent(i, ghost_weight)
                 
     def attach_constraints(self, ws:ROOT.RooWorkspace, constraints:ROOT.RooArgSet):
         category_name = self.active_category
-        self.stdout.debug(f"REGTEST: Attaching contraint pdfs to workspace for the category {category_name}")
+        self.stdout.debug(f"Attaching contraint pdfs to workspace for the category {category_name}")
         sum_pdf_name = f"{SUM_PDF_NAME}_{category_name}"
         final_pdf_name = f"{FINAL_PDF_NAME}_{category_name}"
         remove_set = ROOT.RooArgSet()
         pdf = ws.pdf(sum_pdf_name)
         if not pdf:
             raise RuntimeError(f"sum pdf `{sum_pdf_name}` not defined")
         for constraint in constraints:
             constr_name = constraint.GetName()
             np_name = constr_name.replace(CONSTRTERM_PREFIX, "")
             if not pdf.getVariables().find(np_name):
-                self.stdout.warning(f"WARNING: constraint term {constr_name} with NP "
+                self.stdout.warning(f"constraint term {constr_name} with NP "
                                     f"{np_name} is redundant in the category {category_name}. "
                                     f"It will be removed...", "red")
                 remove_set.add(constraint)
             else:
                 self.import_object(ws, constraint)
         for constraint in remove_set:
             constraints.remove(constraint)
@@ -713,24 +677,24 @@
         obs = self.get_observable(ws)
         obs_range = [obs.getMin(), obs.getMax()]
         # now handle blinding if needed
         do_blind = self.core_config["do_blind"]
         if do_blind:
             blind_range = cat_config['dataset']['blind_range']
             if blind_range:
-                self.stdout.info(f"REGTEST: Implement blind range [{blind_range[0]}, {blind_range[1]}]")
+                self.stdout.info(f"Implement blind range [{blind_range[0]}, {blind_range[1]}]")
                 sideband_lo_range_name = f"{RANGE_NAME_SB_LO}_{category}"
                 sideband_hi_range_name = f"{RANGE_NAME_SB_HI}_{category}"
                 blind_range_name = f"{RANGE_NAME_BLIND}_{category}"
                 obs.setRange(sideband_lo_range_name, obs_range[0], blind_range[0])
                 obs.setRange(blind_range_name, blind_range[0], blind_range[1])
                 obs.setRange(sideband_hi_range_name, blind_range[1], obs_range[1])
                 if (blind_range[0] == obs_range[0]) and \
                    (blind_range[1] == obs_range[1]):
-                    self.stdout.info(f"REGTEST: Category `{category}` is fully blinded. "
+                    self.stdout.info(f"Category `{category}` is fully blinded. "
                                      f"No side-band exists.")
                     cat_config['range_name'] = ""
                 elif (blind_range[1] == obs_range[1]):
                     cat_config['range_name'] = sideband_lo_range_name
                 elif (blind_range[0] == obs_range[0]):
                     cat_config['range_name'] = sideband_hi_range_name
                 else:
@@ -760,19 +724,19 @@
                 items_lowpriority.append(item)
             else:
                 _items_highpriority.append(item)
         cat_config['items_highpriority'] = _items_highpriority
     
     def _item_has_dependent(self, expr:str, reference_list:List[str]):
         _, item_type = self._get_object_name_and_type_from_expr(expr)
-        self.stdout.debug(f"REGTEST: item `{expr}` has type `{item_type}`")
+        self.stdout.debug(f"Item `{expr}` has type `{item_type}`")
         if item_type in ['variable', 'defined']:
             return False
         item_list = self._decompose_function_expr(expr)
-        self.stdout.debug(f"REGTEST: Composition of high priority item {expr}: "
+        self.stdout.debug(f"Composition of high priority item {expr}: "
                           f"{', '.join(item_list)}")
         for this_name in item_list:
             for reference in reference_list:
                 that_name, _ = self._get_object_name_and_type_from_expr(reference)
                 if this_name == that_name:
                     return True
         return False
@@ -854,15 +818,15 @@
         if cut != "":
             chain = chain.CopyTree(cut)
         branch = chain.FindBranch(varname)
         if not branch:
             raise RuntimeError(f"cannot find TBranch `{varname}` in TTree `{treename}` "
                                f"in data file `{filename}`")
         if check_only:
-            return Nones
+            return None
         return chain, branch
     
     def get_histogram(self, filename:str, histname:str, check_only:bool=False):
         filepath = self.path_manager.get_relpath(filename)
         if not os.path.exists(filepath):
             raise FileNotFoundError(f"input data file `{filepath}` not found")
         f = ROOT.TFile(filepath)
@@ -916,15 +880,15 @@
         cat_config = self.cat_config[category_name]
         return cat_config
         
     def read_systematics_node(self, node:Dict, domain:str):
         # Read XML config file. Domain name is also passed in some cases, and will replace the :process: keyword in case it is there
         cat_config = self.get_active_category_config()
         syst_expr = self._get_node_attrib(node, "Name")
-        self.stdout.debug(f"REGTEST: Reading systematic `{syst_expr}`")
+        self.stdout.debug(f"Reading systematic `{syst_expr}`")
         syst = Systematic()
         syst.name = self._translate_node_attrib(node, "Name", domain)
         # if the process of the systematic is specified, use the 
         # specified process. Otherwise it is set to empty
         syst.process = self._translate_node_attrib(node, "Process", domain, False, "")
         syst.whereto = self._get_node_attrib(node, "WhereTo")
         syst.nominal = self._get_node_attrib(node, "CentralValue", dtype="float")
@@ -965,25 +929,25 @@
             cat_config['items_highpriority'].append(item)
         
     def read_channel_import_node(self, node:Dict, ws:ROOT.RooWorkspace):
         filename = self._translate_node_attrib(node, "FileName")
         filepath = self.path_manager.get_relpath(filename)
         if not os.path.exists(filepath):
             raise FileNotFoundError(f"import XML file `{filepath}` not found")
-        self.stdout.debug(f"REGTEST: Reading import XML file `{filepath}`")
+        self.stdout.debug(f"Reading import XML file `{filepath}`")
         xml_data = TXMLTree.load_as_dict(filepath)
         nodes = xml_data['children']
         self.read_channel_xml_nodes(nodes, ws)
         
     def read_sample_import_node(self, node:Dict, sample:Sample):
         filename = self._translate_node_attrib(node, "FileName")
         filepath = self.path_manager.get_relpath(filename)
         if not os.path.exists(filepath):
             raise FileNotFoundError(f"import XML file `{filepath}` not found")
-        self.stdout.info(f"REGTEST: Importing items for `{sample.process}` from {filepath}")
+        self.stdout.info(f"Importing items for `{sample.process}` from {filepath}")
         xml_data = TXMLTree.load_as_dict(filepath)
         nodes = xml_data['children']
         self.read_sample_subnode(nodes, sample)
     
     def read_sample_factor_node(self, node:Dict, sample:Sample):
         """Parse Norm/Shape factors from a Sample Node
         
@@ -1049,14 +1013,16 @@
             data_config['histname'] = self._translate_node_attrib(node, ["HistName", "HistoName"])
         # reading from root ntuples
         else:
             data_config['treename'] = self._translate_node_attrib(node, "TreeName")
             data_config['varname'] = self._translate_node_attrib(node, "VarName")
             data_config['cut'] = self._translate_node_attrib(node, "Cut", "",
                                                              required=False, default="")
+            data_config['weightname'] = self._get_node_attrib(node, "WeightName", required=False,
+                                                              default=None)
 
         inject_ghost = self._get_node_attrib(node, "InjectGhost", required=False,
                                              default=False, dtype="bool")
         data_config['inject_ghost'] = inject_ghost
         if (is_counting and data_filename == ""):
             data_config['num_data'] = self._get_node_attrib(node, "NumData", dtype="int")
         else:
@@ -1129,15 +1095,15 @@
                                                      required=False, default="")
             if norm_value != "":
                 sample.norm_factors.append(f"{prefix}_{sample.process}[{norm_value}]")
                 
         sample.share_pdf_group = self._translate_node_attrib(node, "SharePdf", sample.process,
                                                              required=False, default="")
         subnodes = node['children']
-        self.stdout.debug(f"REGTEST: Reading sample `{sample.process}`")
+        self.stdout.debug(f"Reading sample `{sample.process}`")
         self.read_sample_subnode(subnodes, sample)    
         self.add_sample_object(sample)
         
     def read_sample_subnode(self, nodes:List, sample:Sample):
         for node in nodes:
             name = node['tag']
             if name == "Systematic":
@@ -1170,38 +1136,38 @@
         resp_func = syst_domain.get_response_function()
         ws.Import(resp_func, ROOT.RooFit.RecycleConflictNodes())
         if (not syst_domain.is_shape):
             resp_func_map[syst_domain.domain] = syst_domain.get_response_name()
         for i in range(syst_domain.nuis_list.size()):
             np_name, glob_name, constr_name = syst_domain.get_np_glob_constr_names(i)
             if syst_domain.constr_term_list[i] == CONSTR_DFD:
-                self.stdout.debug(f"REGTEST: Creating DFD constraint term for NP {np_name}")
+                self.stdout.debug(f"Creating DFD constraint term for NP {np_name}")
                 constr_expr = (f"EXPR::{constr_name}('1/((1+exp(@2*(@0-@3-@1)))*(1+exp(-1*@2*(@0-@3+@1))))', "
                                f"{np_name}, DFD_e[1], DFD_w[500], {glob_name}[0,-5,5])")
                 self.import_expression(ws, constr_expr, True)
             else:
-                self.stdout.debug(f"REGTEST: Creating RooGaussian constraint term for NP {np_name}")
+                self.stdout.debug(f"Creating RooGaussian constraint term for NP {np_name}")
                 constr_expr = f"RooGaussian::{constr_name}({np_name},{glob_name}[0,-5,5],1)"
             self.import_expression(ws, constr_expr, True)
             core_argsets.nuis_set.add(ws.var(np_name), True)
             core_argsets.glob_set.add(ws.var(glob_name), True)
             core_argsets.constr_set.add(ws.pdf(constr_name), True)
-            self.stdout.debug(f"REGTEST: Finished implementing the systematic {np_name}")
+            self.stdout.debug(f"Finished implementing the systematic {np_name}")
             
     def implement_sample_model(self, ws:ROOT.RooWorkspace, sample:Sample):
-        self.stdout.debug("REGTEST: Getting model")
+        self.stdout.debug("Getting model")
         sample.update_model_name()
         if ws.pdf(sample.model_name):
             if is_shared_pdf:
                 # use shared pdf
-                self.stdout.debug(f"REGTEST: PDF {sample.model_name} has been created in the workpace.")
+                self.stdout.debug(f"PDF {sample.model_name} has been created in the workpace.")
                 return None
             else:
                 raise RuntimeError(f"PDF {sample.model_name} already exists but the user asks to create it again")
-        self.stdout.debug(sample.model_name)
+        self.stdout.debug(sample.model_name, bare=True)
         cat_config = self.get_active_category_config()
         is_counting = cat_config['category_type'] == DATA_SOURCE_COUNTING
         if is_counting:
             # in counting experiment we only need a uniform pdf
             obs_name = cat_config['observable']['name']
             self.import_expression(ws, f"RooUniform::{sample.model_name}({obs_name})")
         else:
@@ -1213,15 +1179,15 @@
         filepath = self.path_manager.get_relpath(filename)
         if not os.path.exists(filepath):
             raise FileNotFoundError(f'model xml file "{filepath}" does not exist')
         root_node = TXMLTree.load_as_dict(filepath)
         
         model_type = self._get_node_attrib(root_node, "Type").lower()
         if model_type == USERDEF_MODEL:
-            self.stdout.debug(f'REGTEST: Creating user-defined pdf from "{filepath}"')
+            self.stdout.debug(f'Creating user-defined pdf from "{filepath}"')
             self.build_userdef_model(root_node, ws, sample)
         elif model_type == EXTERNAL_MODEL:
             self.build_external_model(root_node, ws, sample)
         elif model_type == HISTOGRAM_MODEL:
             self.build_histogram_model(root_node, ws, sample)
         else:
             raise RuntimeError(f"unknown model type: {model_type} . Available choice: "
@@ -1239,15 +1205,15 @@
                 raise RuntimeError("observable not initialized")
             # for the accuracy of Fourier transformation
             obs.setBins(cache_binning, "cache")
         is_success = False
         nodes = root_node['children']
         for node in nodes:
             name = node['tag']
-            self.stdout.debug(f"REGTEST: Reading node `{name}`")
+            self.stdout.debug(f"Reading node `{name}`")
             if name == "Item":
                 expr = self._translate_node_attrib(node, "Name", tag_name)
                 self.import_expression(ws, expr)
             elif name == "ModelItem":
                 factory_str = self._translate_node_attrib(node, "Name", tag_name)
                 str_start = factory_str.find("::")+2
                 str_end   = factory_str.find("(")
@@ -1271,15 +1237,15 @@
             raise FileNotFoundError(f'input file "{filepath}" not found')
         ws_name = self._translate_node_attrib(root_node, "WSName")
         model_name = self._translate_node_attrib(root_node, "ModelName")
         observable_name = self._translate_node_attrib(root_node, "ObservableName")
         tag_name = sample.get_tag_name()
         nodes = root_node['children']
         np_list, glob_list, constr_list = [], [], []
-        self.stdout.debug(f"REGTEST: Use existing PDF `{model_name}` from the workspace `{filename}`")
+        self.stdout.debug(f"Use existing PDF `{model_name}` from the workspace `{filename}`")
         
         f_ext = ROOT.TFile(filename)
         ws_ext = f_ext.Get(ws_name)
         pdf_ext = ws_ext.function(model_name)
         
         name_maps = {}
         do_not_touch = [observable_name]
@@ -1294,15 +1260,15 @@
                 var = ws_ext.var(var_name)
                 if not var:
                     raise RuntimeError(f"no variable named `{var_name}` found im the workspace `{filepath}`")
                 var.setConstant(1)
                 var_val = self._get_node_attrib(node, "Value", False, "")
                 if var_val != "":
                     var.setVal(float(var))
-                self.stdout.debug(f"REGTEST: Fixed variable `{var_name}` at `{var.getVal()}")
+                self.stdout.debug(f"Fixed variable `{var_name}` at `{var.getVal()}")
             elif name == "Rename":
                 # rename the object names in the input workspace
                 old_name = self._translate_node_attrib(node, "OldName", tag_name)
                 new_name = self._translate_node_attrib(node, "NewName", tag_name)
                 do_not_touch.append(old_name)
                 name_maps[old_name] = new_name
             elif name == "ExtSyst":
@@ -1329,32 +1295,32 @@
             ws_temp.Print()
             
         pdf = ws_temp.function(f"{model_name}_{tag_name}")
         obs_ext = ws_temp.var(observable_name)
         if not obs_ext:
             raise RuntimeError(f"observable `{observable_name}` not found in the workspace `{filepath}`")
         if not isinstance(pdf, ROOT.RooAbsPdf):
-            self.stdout.warning(f"WARNING: The object {model_name} is not a p.d.f as seen from RoOFit")
-            self.stdout.warning("REGTEST: Constructing RooRealSumPdf for the pdf from histFactory")
+            self.stdout.warning(f"The object {model_name} is not a p.d.f as seen from RoOFit")
+            self.stdout.warning("Constructing RooRealSumPdf for the pdf from histFactory")
             dummy_pdf = ROOT.RooUniform(f"{sample.model_name}_dummpy_pdf", "for RooRealSumPdf construction",
                                         obs_ext)
             frac = ROOT.RooRealVar(f"{sample.model_name}_real_pdf_frac", "for RooRealSumPdf construction", 1)
             pdf = ROOT.RooRealSumPdf(sample.model_name, "from histFactory", ROOT.RooArgList(pdf, dummy_pdf),
                                      ROOT.RooArgList(frac))
         else:
             name_maps[pdf.GetName()] = sample.model_name
         
         # rename observable (this step should never happen for a HistFactory workspace)
         if observable_name != _observable_name:
             name_maps[observable_name] = _observable_name
-        self.stdout.info("REGTEST: The following variables will be renamed:")
+        self.stdout.info("The following variables will be renamed:")
         old_str = ",".join(name_maps.keys())
         new_str = ",".join(name_maps.values())
-        self.stdout.info(f"REGTEST: Old: {old_str}")
-        self.stdout.info(f"REGTEST: New: {new_str}")
+        self.stdout.info(f"Old: {old_str}")
+        self.stdout.info(f"New: {new_str}")
         
         self.import_object(ws, pdf, ROOT.RooFit.RenameVariable(old_str, new_str),
                            ROOT.RooFit.RecycleConflictNodes())
         # import constraint terms
         for np_name, glob_name, constr_name in zip(np_list, glob_list, constr_list):
             new_np_name = np_name
             # check wheterh NP has been renamed. If yes, update the NP name
@@ -1369,29 +1335,29 @@
                 new_constr_name = CONSTRTERM_PREFIX + new_np_name
                 new_glob_name = GLOBALOBS_PREFIX + new_np_name
                 constr_pdf = ws_ext.pdf(constr_name)
                 old_str = ",".join([constr_name, glob_name, np_name])
                 new_str = ",".join([new_constr_name, new_glob_name, new_np_name])
                 self.import_object(ws, constr_pdf, 
                                    ROOT.RooFit.RenameVariable(old_str, new_str))
-                self.stdout.debug(f"REGTEST: Import systematics {new_np_name} "
+                self.stdout.debug(f"Import systematics {new_np_name} "
                                   f"with constraint term {new_constr_name}")
                 constraints.add(ws.pdf(new_constr_name), True)
                 globobs.add(ws.var(new_glob_name), True)
             ws.var(new_np_name).setConstant(False)
             nuis.add(ws.var(new_np_name), True)
     
     def build_histogram_model(self, root_node:Dict, ws:ROOT.RooWorkspace, sample:Sample):
         cat_config = self.get_active_category_config()
         obs_name = cat_config['observable']['name']
         filename = self._translate_node_attrib(root_node, "Input")
         filepath = self.path_manager.get_relpath(filename)
         histname = self._translate_node_attrib(root_node, "ModelName")
         rebin = self._get_node_attrib(root_node, "Rebin", False, "-1", dtype="int")
-        self.stdout.debug(f"REGTEST: Creating histogram pdf from `{filepath}`")
+        self.stdout.debug(f"Creating histogram pdf from `{filepath}`")
         h = self.get_histogram(filename, histname)
         if rebin > 0:
             h.Rebin(rebin)
         obs = ws.var(obs_name)
         if not obs:
             raise RuntimeError("observable not initialized")
         h_data = ROOT.RooDataHist("hdata", "hdata", obs, h)
@@ -1403,15 +1369,15 @@
         obs_name = cat_config['observable']['name']        
         var_set = model.getVariables()
         float_set = ROOT.RooArgSet()
         for var in var_set:
             if (not var.isConstant()):
                 if var.getMin() == var.getMax():
                     var_name = var.GetName()
-                    self.stdout.info(f"REGTEST: Fixing {var_name} to constant as it has same upper and loer boundary")
+                    self.stdout.info(f"Fixing {var_name} to constant as it has same upper and loer boundary")
                     var.setConstant(True)
                 else:
                     float_set.add(var)
         poi_obs_names = self.core_config['poi_names'] + [obs_name]
         # reove POI and observable from float set
         for name in poi_obs_names:
             float_var = float_set.find(name)
@@ -1419,29 +1385,29 @@
                 float_set.remove(float_var)
         num_np = len(nuis)
         num_poi = len(self.core_config['poi_names'])
         for var in float_set:
             if not nuis.find(var):
                 nuis.add(var)
                 var_name = var.GetName()
-                self.stdout.info(f"REGTEST: Adding {var_name} to the nuisance parameter set")
+                self.stdout.info(f"Adding {var_name} to the nuisance parameter set")
 
         num_float = len(float_set)
         if num_float < num_np:
-            self.stdout.warning(f"WARNING: There supposed to be {num_poi + num_np} free parameters, "
+            self.stdout.warning(f"There supposed to be {num_poi + num_np} free parameters, "
                                 f"but only seen {num_float} in the category {self.active_category}. "
                                 f"This is in principle not an issue, but please make sure you "
                                 f"understand what you are doing")
             if self.debug_mode:
-                self.stdout.debug("REGTEST: All free parameters: ")
+                self.stdout.debug("All free parameters: ")
                 float_set.Print()
-                self.stdout.debug("REGTEST: All nuisance parameters: ")
+                self.stdout.debug("All nuisance parameters: ")
                 nuis.Print()
         else:
-            self.stdout.info("REGTEST: Number of nuisance parameters looks good!")
+            self.stdout.info("Number of nuisance parameters looks good!")
   
     def get_pdf_name(self, category:str):
         return f"{FINAL_PDF_NAME}_{category}"
     
     def implement_model_config_and_sets(self, ws:"ROOT.RooWorkspace",
                                         mc:"ROOT.RooStats.ModelConfig",
                                         obs:ROOT.RooArgSet, pois:ROOT.RooArgSet,
@@ -1489,30 +1455,30 @@
             obs.add(ws_cat.set(OBS_SET), True)
             pois.add(ws_cat.set(POI_SET), True)
             nuis.add(ws_cat.set(NUIS_SET), True)
             globs.add(ws_cat.set(GLOB_SET), True)
             if self.debug_mode:
                 ws_i.Print()
                 
-        self.stdout.info("REGTEST: Making combined workspace")
+        self.stdout.info("Making combined workspace")
                 
         # implement main pdf
         self.import_object(self.comb_ws, combined_pdf)
         
         # implement model config
         self.implement_model_config_and_sets(self.comb_ws, self.model_config,
                                              obs, pois, nuis, globs)
         
-        weight_var = ROOT.RooRealVar("wt", "wt", 1)
+        weight_var = ROOT.RooRealVar("weight", "weight", 1)
         args = ROOT.RooArgSet()
         args.add(obs)
         args.add(weight_var)
         
-        dataset_map = ExtendedModel.get_dataset_map(self.datasets)
-        dataset_binned_map = ExtendedModel.get_dataset_map(self.datasets_binned)
+        dataset_map = RooDataSet.get_dataset_map(self.datasets)
+        dataset_binned_map = RooDataSet.get_dataset_map(self.datasets_binned)
         
         dataset_name = self.core_config['dataset_name']
         obs_data = ROOT.RooDataSet(dataset_name, "Combined data", args,
                                    ROOT.RooFit.Index(channel_list),
                                    ROOT.RooFit.Import(dataset_map),
                                    ROOT.RooFit.WeightVar(weight_var))
         obs_data_binned = ROOT.RooDataSet(dataset_name + "binned", 
@@ -1520,30 +1486,30 @@
                                           ROOT.RooFit.Index(channel_list),
                                           ROOT.RooFit.Import(dataset_binned_map),
                                           ROOT.RooFit.WeightVar(weight_var))
         self.import_object(self.comb_ws, obs_data, silent=False)
         if (obs_data_binned.numEntries() < obs_data.numEntries()):
             self.import_object(self.comb_ws, obs_data_binned, silent=False)
         else:
-            self.stdout.warning("REGTEST: No need to keep binned dataset, as the "
+            self.stdout.warning("No need to keep binned dataset, as the "
                                 "number of data events is smaller than or equal "
                                 "to the number of bins in all categories", "red")
             self.use_binned = False
         
         # save the original snapshot
         # self.comb_ws.saveSnapshot("nominalNuis", self.model_config.GetNuisanceParameters())
         # self.comb_ws.saveSnapshot("nominalGlobs", self.model_config.GetGlobalObservables())
         
         # generate asimov datasets
         self.generate_asimov()
         
         # import class code
         class_code_dirs = self.core_config["class_code_dirs"]
         if (class_code_dirs["decl"] is not None) and (class_code_dirs["impl"] is not None):
-            self.stdout.warning("REGTEST: Importing class code")            
+            self.stdout.warning("Importing class code")            
             self.comb_ws.addClassDeclImportDir(class_code_dirs["decl"])
             self.comb_ws.addClassImplImportDir(class_code_dirs["impl"])
             self.comb_ws.importClassCode()
             
         # save final workspace
         self.path_manager.makedir_for_files("output")
         output_path = self.path_manager.get_file("output")
```

### Comparing `quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_combiner.py` & `quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_combiner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ###############################################################################
 ### This is a reimplementation of workspaceCombiner library in python
-### original author: Hongtao Yang
+### original author: Hongtao Yang, Haoshuang Ji
 ###############################################################################
 import os
 import re
 import json
 from typing import Optional, Union, List, Dict
 
 try:
@@ -122,15 +122,15 @@
         return model
     
     def _exception_check(self, msg:str, strict_mode:bool=False) -> None:
         if strict_mode:
             raise RuntimeError(msg)
         else:
             msg = msg[0].capitalize() + msg[1:]
-            self.stdout.warning(f"WARNING: {msg}. Skipped.")
+            self.stdout.warning(f"{msg}. Skipped.")
     
     def _channel_check(self, channel:str, check_poi_map:bool=False):
         if channel not in self.channel_config:
             raise RuntimeError(f"channel \"{channel}\" not initialized")
         if check_poi_map and ("poi_map" not in self.channel_config[channel]):
             raise RuntimeError(f'missing poi definition for the channel "{channel}"')
             
@@ -144,15 +144,15 @@
     def load_cache_ws(self, ws_type:str):
         if ws_type == "rename":
             filename = self._get_tmp_ws_path()
         elif ws_type == "combine":
             filename = self._get_comb_ws_path()
         else:
             raise ValueError(f"invalid cache workspace type: {ws_type}")
-        self.stdout.info(f'INFO: Reading temporary workspace file from "{filename}"')
+        self.stdout.info(f'Reading temporary workspace file from "{filename}"')
         if not os.path.exists(filename):
             raise FileNotFoundError(f'temporary workspace file "{filename}" does not exist')
         file = ROOT.TFile(filename)
         if is_corrupt(file):
             raise RuntimeError(f'temporary workspace file "{filename}" is corrupted')
         workspace_name = self.combination_config["workspace_name"]
         workspace = file.Get(workspace_name)
@@ -255,28 +255,28 @@
             raise RuntimeError(f"the channel \"{channel}\" is included more than once")
         self.channel_config[channel] = channel_config
         self.channel_config[channel]['rename_map'] = {
             "pdf"  : {},
             "var"  : {}
         }
         self.channel_config[channel]['renamed_constraint'] = {}
-        self.stdout.info(f"INFO: Checking XML input for the channel \"{channel}\".")
+        self.stdout.info(f"Checking XML input for the channel \"{channel}\".")
         # walk through child nodes
         child_nodes = node["children"]
         for child_node in child_nodes:
             tag = child_node['tag']
             if tag == "RenameMap":
                 self.read_channel_rename_node(channel, child_node)
             elif tag == "POIList":
                 self.read_channel_poi_node(channel, child_node)
             elif tag == "ArgSetList":
                 self.read_channel_argset_node(channel, child_node)
             else:
                 raise RuntimeError(f"unknown item `{tag}`")
-        self.stdout.info(f"INFO: Successfully validated XML input for the channel \"{channel}\".")
+        self.stdout.info(f"Successfully validated XML input for the channel \"{channel}\".")
     
     def read_channel_rename_node(self, channel:str, node:Dict) -> None:
         ext_file = self._get_node_attrib(node, "InputFile", required=False)
         if ext_file is not None:
             node = TXMLTree.load_as_dict(ext_file)
         child_nodes = node['children']
         for child_node in child_nodes:
@@ -292,15 +292,15 @@
         argset_strict = self._get_node_attrib(node, "Strict", required=False,
                                               default="True", dtype="bool")
         self.channel_config[channel]['argset_list'] = argset_list
         self.channel_config[channel]['argset_strict'] = argset_strict
                 
     def validate_channel_input(self, channel:str):
         self._channel_check(channel)
-        self.stdout.info(f"INFO: Checking input workspace for the channel \"{channel}\".")
+        self.stdout.info(f"Checking input workspace for the channel \"{channel}\".")
         channel_config = self.channel_config[channel]
         model = self._get_channel_model(channel_config)
         strict_mode = self.combination_config["strict"]
         ws_filename = model.fname
         renamed_pdfs = list(channel_config["rename_map"]["pdf"])
         renamed_vars = list(channel_config["rename_map"]["var"])
         renamed_pois = list(channel_config["poi_map"].values())
@@ -364,19 +364,19 @@
         argset_list = channel_config["argset_list"]
         for argset in argset_list:
             argset_obj = model.workspace.obj(argset)
             if not argset_obj:
                 if channel_config["argset_strict"]:
                     raise RuntimeError(f'Argument set "{argset}" does not exist in the channel "{channel}"')
                 else:
-                    self.stdout.warning(f'WARNING: Argument set "{argset}" does not exist in the channel "{channel}". Skipped.')
+                    self.stdout.warning(f'Argument set "{argset}" does not exist in the channel "{channel}". Skipped.')
                     continue
             if not isinstance(argset_obj, ROOT.RooArgSet):
                 raise RuntimeError(f'Argument set "{argset}" from the channel "{channel}" is an instance of RooArgSet object')
-        self.stdout.info(f"INFO: Successfully validated input workspace for the channel \"{channel}\".")
+        self.stdout.info(f"Successfully validated input workspace for the channel \"{channel}\".")
         
     def read_rename_syst_node(self, channel:str, node:Dict) -> None:
         self._channel_check(channel)
         channel_config = self.channel_config[channel]
         old_name = self._get_node_attrib(node, "OldName", required=True)
         new_name = self._get_node_attrib(node, "NewName", required=True)
         if not old_name:
@@ -445,15 +445,15 @@
         if ignore_list is None:
             ignore_list = []
         for arg in args:
             arg_name = arg.GetName()
             if arg_name in ignore_list:
                 continue
             arg.SetName(f"{arg_name}_{channel}")
-            self.stdout.debug(f'DEBUG: Appended channel suffix "{channel}" to the {arg_type} '
+            self.stdout.debug(f'Appended channel suffix "{channel}" to the {arg_type} '
                               f'"{arg_name}"')
     
     def _get_tmp_ws_path(self):
         basename = os.path.splitext(self.combination_config["output_file"])[0]
         filename = f"{basename}_{self.KEYWORDS['rename_save_suffix']}.root"
         return filename
     
@@ -523,21 +523,21 @@
         summary_text += title
         poi_table = self.get_poi_table()
         summary_text += poi_table
         return summary_text
     
     def print_input_summary(self) -> None:
         summary_text = self.get_summary_text()
-        self.stdout.info(summary_text)
+        self.stdout.info(summary_text, bare=True)
         
     def rename_channel(self, channel:str) -> None:
         self._channel_check(channel, check_poi_map=True)
         channel_config = self.channel_config[channel]
         simplified_import = channel_config["simplified_import"]
-        self.stdout.info(f'INFO: Renaming objects for the channel "{channel}"')
+        self.stdout.info(f'Renaming objects for the channel "{channel}"')
         # do not reuse model
         model = self._get_channel_model(channel_config)
         workspace = model.workspace
         variables = workspace.allVars()
         pdfs = workspace.allPdfs()
         functions = workspace.allFunctions()
         ignore_list = []
@@ -547,47 +547,47 @@
         rename_map = channel_config["rename_map"]
         # rename pdf
         for old_name, new_name in rename_map["pdf"].items():
             old_pdf = workspace.pdf(old_name)
             if not simplified_import:
                 pdfs.remove(old_pdf)
             if old_name == new_name:
-                self.stdout.debug(f'DEBUG: Found redundant renaming of the pdf "{old_name}". Skipped.')
+                self.stdout.debug(f'Found redundant renaming of the pdf "{old_name}". Skipped.')
                 continue
             old_pdf.SetName(new_name)
-            self.stdout.debug(f'DEBUG: Renamed pdf from "{old_name}" to "{new_name}"')
+            self.stdout.debug(f'Renamed pdf from "{old_name}" to "{new_name}"')
         # rename variable
         for old_name, new_name in rename_map["var"].items():
             old_var = workspace.var(old_name)
             if not simplified_import:
                 variables.remove(old_var)
             else:
                 ignore_list.append(new_name)
             if old_name == new_name:
-                self.stdout.debug(f'DEBUG: Found redundant renaming of the variable "{old_name}". Skipped.')
+                self.stdout.debug(f'Found redundant renaming of the variable "{old_name}". Skipped.')
                 continue
             old_var.SetName(new_name)
-            self.stdout.debug(f'DEBUG: Renamed variable from "{old_name}" to "{new_name}"')
+            self.stdout.debug(f'Renamed variable from "{old_name}" to "{new_name}"')
         # rename pois
         poi_map = channel_config['poi_map']
         for comb_poi_name, channel_poi_name in poi_map.items():
             if channel_poi_name == self.KEYWORDS['dummy']:
                 continue
             poi = workspace.var(channel_poi_name)
             if not simplified_import:
                 variables.remove(poi)
             else:
                 ignore_list.append(comb_poi_name)
             if comb_poi_name == channel_poi_name:
-                self.stdout.debug(f'DEBUG: Found redundant renaming of the poi "{channel_poi_name}". Skipped.')
+                self.stdout.debug(f'Found redundant renaming of the poi "{channel_poi_name}". Skipped.')
                 continue
             poi.SetName(comb_poi_name)
-            self.stdout.debug(f'DEBUG: Renamed poi from "{channel_poi_name}" to "{comb_poi_name}"')
+            self.stdout.debug(f'Renamed poi from "{channel_poi_name}" to "{comb_poi_name}"')
         if simplified_import:
-            self.stdout.info(f'INFO: Simplified import requested for the channel "{channel}". '
+            self.stdout.info(f'Simplified import requested for the channel "{channel}". '
                              'Only unspecified constraint PDFs, nuisance parameters, '
                              'global observables and POIs will be renamed.')
             global_observables = model.global_observables
             nuisance_parameters = model.nuisance_parameters
             pois = model.pois
             constr_pdfs = ROOT.RooArgSet()
             # get the relevant constraint pdfs
@@ -618,19 +618,19 @@
         else:
             # remove observables
             observables = ROOT.RooArgSet(model.observables)
             variables.remove(observables)
             
             # add channel suffix to functions
             self._append_channel_suffix_to_args(channel, functions, "function")
-            self.stdout.debug(f'DEBUG: All functions in channel "{channel}" have been renamed')
+            self.stdout.debug(f'All functions in channel "{channel}" have been renamed')
             self._append_channel_suffix_to_args(channel, pdfs, "PDF")
-            self.stdout.debug(f'DEBUG: All PDFs in channel "{channel}" have been renamed')
+            self.stdout.debug(f'All PDFs in channel "{channel}" have been renamed')
             self._append_channel_suffix_to_args(channel, variables, "variable")
-            self.stdout.debug(f'DEBUG: All variables in channel "{channel}" have been renamed')
+            self.stdout.debug(f'All variables in channel "{channel}" have been renamed')
         
         # rename key objects
         pdf  = model.pdf
         data = model.data
         if not isinstance(pdf, ROOT.RooSimultaneous):
             raise RuntimeError(f'main pdf of the channel "{channel}" does not belong to the RooSimultaneous class')
         cat = pdf.indexCat()
@@ -671,29 +671,29 @@
                 raise RuntimeError(f'duplicated ArgSet object "{new_argset_name}"')
             argset_map[new_argset_name] = components
         self.argsets.update(argset_map)
     
     def rename(self, save_rename_ws:bool=True) -> None:
         title = format_delimiter_enclosed_text(f"Rename PDFs, functions and variables",
                                                delimiter="-", indent_str="")
-        self.stdout.info(title)
+        self.stdout.info(title, bare=True)
         self.reset_tmp_ws()
         for channel in self.channel_config:
             self.rename_channel(channel)
         if save_rename_ws:
             self.tmp_ws.defineSet(self.KEYWORDS['comb_nuis_name'], self.tmp_nuis, True);
             self.tmp_ws.defineSet(self.KEYWORDS['comb_glob_name'], self.tmp_glob, True);
             filename = self._get_tmp_ws_path()
-            self.stdout.info(f'INFO: Saving temporary workspace to "{filename}"')
+            self.stdout.info(f'Saving temporary workspace to "{filename}"')
             self.tmp_ws.writeToFile(filename, True)
             
     def combine_channel(self, channel:str):
         title = format_delimiter_enclosed_text(f"Channel {channel}",
                                                delimiter="+", indent_str="")
-        self.stdout.info(title)
+        self.stdout.info(title, bare=True)
         channel_pdf_name = f"{self.KEYWORDS['comb_pdf_name']}_{channel}"
         channel_data_name = f"{self.KEYWORDS['comb_data_name']}_{channel}"
         channel_cat_name = f"{self.KEYWORDS['comb_cat_name']}_{channel}"
         channel_pdf = self.tmp_ws.pdf(channel_pdf_name)
         if not channel_pdf:
             raise RuntimeError(f'missing pdf "{channel_pdf_name}" in the channel "{channel}"')
         channel_cat = channel_pdf.indexCat()
@@ -704,15 +704,15 @@
         channel_data_list = channel_data.split(channel_cat, True)
         
         n_cat = channel_cat.size()
         for i in range(n_cat):
             channel_cat.setBin(i)
             cat_name_i = channel_cat.getLabel()
             new_cat_name_i = f"{channel_cat_name}_{cat_name_i}"
-            self.stdout.info(f"Category {i+1}: {cat_name_i} --> {new_cat_name_i}")
+            self.stdout.info(f"Category {i+1}: {cat_name_i} --> {new_cat_name_i}", bare=True)
             pdf_i = channel_pdf.getPdf(cat_name_i)
             data_i = channel_data_list.FindObject(cat_name_i)
             observables_i = pdf_i.getObservables(data_i)
             obs_and_weight, weight_var = self._get_obs_and_weight(observables_i)
             # create new dataset
             new_data_i = ROOT.RooDataSet(f"{new_cat_name_i}_data", f"{new_cat_name_i}_data",
                                          obs_and_weight, ROOT.RooFit.WeightVar(self.KEYWORDS['weight_name']))
@@ -724,57 +724,57 @@
             self.comb_pdf.addPdf(pdf_i, new_cat_name_i)
             self.comb_data_map[new_cat_name_i] = new_data_i
             self.comb_obs.add(observables_i.snapshot(), True)
             
     def combine(self, load_rename_ws:bool=True, save_combine_ws:bool=True) -> None:
         title = format_delimiter_enclosed_text(f"Create Combined Pdf and Dataset",
                                                delimiter="-", indent_str="")
-        self.stdout.info(title)
+        self.stdout.info(title, bare=True)
         if load_rename_ws:
             self.load_cache_ws("rename")
         
         self.reset_comb_ws()
         for channel in self.channel_config:
             self.combine_channel(channel)
         
         pdf_name  = self.KEYWORDS['comb_pdf_name']
         data_name = self.combination_config["data_name"]
-        self.stdout.info(f'INFO: Generating combined pdf "{pdf_name}"')
+        self.stdout.info(f'Generating combined pdf "{pdf_name}"')
         self.comb_ws.Import(self.comb_pdf)
-        self.stdout.info(f'INFO: Generating combined dataset "{data_name}"')
+        self.stdout.info(f'Generating combined dataset "{data_name}"')
         self.comb_obs.add(self.comb_cat)
         obs_and_weight, weight_var = self._get_obs_and_weight(self.comb_obs)
         dataset_map = ExtendedModel.get_dataset_map(self.comb_data_map)
         comb_data = ROOT.RooDataSet(data_name, data_name, obs_and_weight,
                                     ROOT.RooFit.Index(self.comb_cat),
                                     ROOT.RooFit.Import(dataset_map),
                                     ROOT.RooFit.WeightVar(weight_var))
         self.comb_ws.Import(comb_data)
-        self.stdout.info(f'INFO: Defining variable set "{self.KEYWORDS["comb_nuis_name"]}"')
+        self.stdout.info(f'Defining variable set "{self.KEYWORDS["comb_nuis_name"]}"')
         self.comb_ws.defineSet(self.KEYWORDS["comb_nuis_name"], self.tmp_nuis, True)
-        self.stdout.info(f'INFO: Defining variable set "{self.KEYWORDS["comb_glob_name"]}"')
+        self.stdout.info(f'Defining variable set "{self.KEYWORDS["comb_glob_name"]}"')
         self.comb_ws.defineSet(self.KEYWORDS["comb_glob_name"], self.tmp_glob, True)
-        self.stdout.info(f'INFO: Defining variable set "{self.KEYWORDS["comb_obs_name"]}"')
+        self.stdout.info(f'Defining variable set "{self.KEYWORDS["comb_obs_name"]}"')
         self.comb_ws.defineSet(self.KEYWORDS["comb_obs_name"], self.comb_obs, True)
         self.define_argsets(self.comb_ws)    
         if save_combine_ws:
             filename = self._get_comb_ws_path()
-            self.stdout.info(f'INFO: Saving temporary workspace to "{filename}"')
+            self.stdout.info(f'Saving temporary workspace to "{filename}"')
             self.comb_ws.writeToFile(filename, True)
             
     def define_argsets(self, ws:ROOT.RooWorkspace):
         for argset_name, arg_names in self.argsets.items():
             argset = ROOT.RooArgSet()
             for arg_name in arg_names:
                 arg = ws.obj(arg_name)
                 if not arg:
                     raise RuntimeError(f'failed to locate object "{arg_name}" from the combined workspace when '
                                        f'defining the ArgSet "{argset_name}"')
                 argset.add(arg)
-            self.stdout.info(f'INFO: Defining argument set "{argset_name}"')
+            self.stdout.info(f'Defining argument set "{argset_name}"')
             ws.Import(argset, argset_name, True)
         
     def get_combined_model_config(self) -> None:
         pois = ROOT.RooArgSet()
         if "poi_definition" not in self.combination_config:
             raise RuntimeError("Combined POIs not initialized")        
         poi_definitions = self.combination_config["poi_definition"]
@@ -788,15 +788,15 @@
                     poi.setConstant(True)
                 else:
                     poi.setRange(poi_min, poi_max)
                     if (poi_value is not None) and ((poi_value > poi_min) and (poi_value < poi_max)):
                         poi.setVal(poi_value)
                 pois.add(poi)
             else:
-                self.stdout.warning(f'WARNING: The POI "{poi_name}" does not exist in the combined model')
+                self.stdout.warning(f'The POI "{poi_name}" does not exist in the combined model')
         mc_name = self.combination_config["model_config_name"]
         model_config = ROOT.RooStats.ModelConfig(mc_name, self.comb_ws)
         #model_config.SetWorkspace(self.com_ws)
         pdf_name  = self.KEYWORDS['comb_pdf_name']
         data_name = self.combination_config["data_name"]
         pdf = self.comb_ws.pdf(pdf_name)
         data = self.comb_ws.data(data_name)
@@ -848,37 +848,37 @@
         
     def finalize(self, load_combine_ws:bool=True, save_final_ws:bool=True,
                  import_class_code:bool=True) -> None:
         if load_combine_ws:
             self.load_cache_ws("combine")
         
         # create model config
-        self.stdout.info(f'INFO: Creating ModelConfig "{self.combination_config["model_config_name"]}"')
+        self.stdout.info(f'Creating ModelConfig "{self.combination_config["model_config_name"]}"')
         model_config = self.get_combined_model_config()
         self.comb_ws.Import(model_config)
         if import_class_code:
             self.import_class_code(self.comb_ws)
         
         title = format_delimiter_enclosed_text(f"Generate Asimov Dataset",
                                                delimiter="-", indent_str="")
-        self.stdout.info(title)
+        self.stdout.info(title, bare=True)
         
         # generate asimov dataset
         self.generate_asimov()
             
         title = format_delimiter_enclosed_text(f"Workspace Summary",
                                                delimiter="-", indent_str="")
-        self.stdout.info(title)
+        self.stdout.info(title, bare=True)
         
         mc_summary = self.get_model_config_summary()
-        self.stdout.info(mc_summary)
+        self.stdout.info(mc_summary, bare=True)
         
         if save_final_ws:
             filename = self.combination_config["output_file"]
-            self.stdout.info(f'INFO: Saving final combined workspace to "{filename}"')
+            self.stdout.info(f'Saving final combined workspace to "{filename}"')
             self.comb_ws.writeToFile(filename, True)
             
     def reset_combination(self):
         self.argsets = {}
     
     def create_combined_workspace(self, infiles:Optional[Dict[str, str]]=None,
                                   outfile:Optional[str]=None,
@@ -900,8 +900,8 @@
             for channel in self.channel_config:
                 self.validate_channel_input(channel)
             self.print_input_summary()
             self.rename(save_rename_ws=save_rename_ws)
             self.combine(load_rename_ws=save_rename_ws, save_combine_ws=save_combine_ws)
             self.finalize(load_combine_ws=save_combine_ws, save_final_ws=save_final_ws,
                           import_class_code=import_class_code)
-        self.stdout.info(f"INFO: Total time taken: {t.interval:.3f}s")
+        self.stdout.info(f"Total time taken: {t.interval:.3f}s")
```

### Comparing `quickstats-0.6.7.8/quickstats/components/workspaces/xml_ws_modifier.py` & `quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_modifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             "dataset_list"       : source.pop("dataset_list", None),
             "fix_parameters"     : source.pop("fix_parameters", None),
             "profile_parameters" : source.pop("profile_parameters", None),
             "strict"             : source.pop("strict", True)
         }
         if source:
             unknown_attributes = list(source)
-            self.stdout.warning(f"WARNING: The following unrecognized configuration attribute(s) will be ignored: "
+            self.stdout.warning(f"The following unrecognized configuration attribute(s) will be ignored: "
                                 f"{', '.join(unknown_attributes)}")
         actions = {
             "map"        : _actions.pop("map", []),
             "define"     : _actions.pop("define", []),
             "redefine"   : _actions.pop("redefine", []),
             "asimov"     : _actions.pop("asimov", []),
             "constraint" : [],
@@ -128,19 +128,19 @@
             "model_config" : _rename.pop("model_config", {}),
             "dataset"      : _rename.pop("dataset", {}),
             "variable"     : _rename.pop("variable", {})
         }
         actions["rename"] = rename
         if _actions:
             unknown_attributes = list(_actions)
-            self.stdout.warning(f"WARNING: Unknown action type: {', '.join(unknown_attributes)}. "
+            self.stdout.warning(f"Unknown action type: {', '.join(unknown_attributes)}. "
                                 "Ignoring...")
         if _rename:
             unknown_attributes = list(_rename)
-            self.stdout.warning(f"WARNING: Unknown object type in rename: {', '.join(unknown_attributes)}. "
+            self.stdout.warning(f"Unknown object type in rename: {', '.join(unknown_attributes)}. "
                                 "Ignoring...")
         
         self.config = config
         self.actions = actions
     
     def parse_config_json(self, filename:str):
         with open(filename, 'r') as f:
@@ -275,54 +275,54 @@
             if infile is None:
                 infile = self.config['input_file']
             # override path to the output workspace
             if outfile is None:
                 outfile = self.config['output_file']
             ws_name  = self.config['workspace_name']
             mc_name  = self.config['model_config_name']
-            self.stdout.info(f"INFO: Begin modification of the workspace \"{infile}\".")
+            self.stdout.info(f"Begin modification of the workspace \"{infile}\".")
             model    = ExtendedModel(infile, ws_name=ws_name, mc_name=mc_name,
                                      data_name=None, verbosity="WARNING")
             ws_orig  = model.workspace
             mc_orig  = model.model_config
             ws_name  = ws_orig.GetName()
             mc_name  = mc_orig.GetName()
 
             # create temporary workspace
             ws_tmp = ROOT.RooWorkspace(ws_name)
 
             title_str = format_delimiter_enclosed_text("Step 1: Redefine objects", "-")
-            self.stdout.info(title_str)
+            self.stdout.info(title_str, bare=True)
             flag = self.redefine_objects(ws_orig, ws_tmp)
             # nothing is done
             if not flag:
-                self.stdout.info("INFO: No objects are redefined.")
+                self.stdout.info("No objects are redefined.")
 
             title_str = format_delimiter_enclosed_text("Step 2: Create new objects", "-")
-            self.stdout.info(title_str)
+            self.stdout.info(title_str, bare=True)
             flag = self.implement_external_pdfs(ws_tmp)
             flag |= self.implement_objects(ws_tmp)
             # nothing is done
             if not flag:
-                self.stdout.info("INFO: No new objects are defined.")
+                self.stdout.info("No new objects are defined.")
             
             dataset_list = self.config['dataset_list']
             # need to import datasets first so the variables are also imported into the workspace
             self.import_datasets(ws_orig, ws_tmp, dataset_list)
 
             title_str = format_delimiter_enclosed_text("Step 3: Rename variables", "-")
-            self.stdout.info(title_str)
+            self.stdout.info(title_str, bare=True)
             rename_map = self.get_rename_map(ws_orig, ws_tmp)
             actual_rename_map = self.get_actual_rename_map(rename_map, ws_orig, ws_tmp)
             self.rename_variables(mc_orig, ws_tmp, rename_map)
             if not rename_map:
-                self.stdout.info("INFO: No variables are renamed.")
+                self.stdout.info("No variables are renamed.")
 
             title_str = format_delimiter_enclosed_text("Step 4: Making output workspace", "-")
-            self.stdout.info(title_str)
+            self.stdout.info(title_str, bare=True)
 
             # create final workspace
             if len(self.actions['constraint']) > 0:
                 ws_final = ROOT.RooWorkspace(ws_name)
                 sim_pdf = self.remake_simultaneous_pdf(mc_orig, ws_tmp)
                 self.import_object(ws_final, sim_pdf)
                 self.import_datasets(ws_orig, ws_final, dataset_list)
@@ -349,31 +349,31 @@
             self.setup_parameters(ws_final)
 
             outdir  = os.path.dirname(outfile)
             if outdir and (not os.path.exists(outdir)):
                 os.makedirs(outdir)
 
             ws_final.writeToFile(outfile, recreate)
-            self.stdout.info(f'INFO: Saved output workspace as "{outfile}".')
-        self.stdout.info(f"INFO: Total time taken: {t.interval:.3f}s")
+            self.stdout.info(f'Saved output workspace as "{outfile}".')
+        self.stdout.info(f"Total time taken: {t.interval:.3f}s")
     
     def post_process_workspace(self, ws:ROOT.RooWorkspace):
         self.add_product_terms(ws)
     
     def add_product_terms(self, ws:ROOT.RooWorkspace):
         for target_name, extra_terms in self.actions["add_product_terms"].items():
             prod_var = self.get_workspace_arg(ws, target_name, strict=True)
             if not isinstance(prod_var, ROOT.RooProduct):
                 class_name = prod_var.ClassName()
                 raise RuntimeError(f"failed to add product term to the variable \"{target_name}\": "
                                    f"expect a RooProduct instance but {class_name} received")
             for extra_term in extra_terms:
                 member_var = self.get_workspace_arg(ws, extra_term, strict=True)
                 prod_var.addTerm(member_var)
-            self.stdout.info(f"INFO: The following product terms are added to the variable {target_name}: "
+            self.stdout.info(f"The following product terms are added to the variable {target_name}: "
                              f"{', '.join(extra_terms)}")
     
     def setup_parameters(self, ws:ROOT.RooWorkspace):
         data_name = self.config['data_name']
         model = ExtendedModel(ws, data_name=data_name, verbosity="WARNING")
         model.stdout.verbosity = self.stdout.verbosity
         if self.config["fix_parameters"] is not None:
@@ -407,38 +407,38 @@
         for variable in variables:
             name = variable.GetName()
             if name in rename_map:
                 new_name = rename_map[name]
                 # note only renaming of RooRealVar instance will be considered
                 new_variable = new_ws.var(new_name)
                 if not new_variable:
-                    self.stdout.warning(f'WARNING: The argset variable "{name}" not found in the new workspace. Skipped.')
+                    self.stdout.warning(f'The argset variable "{name}" not found in the new workspace. Skipped.')
                 # avoid modifying the original value
                 copied_variable = self.copy_variable(variable, new_variable)
                 renamed_variables_old.add(variable)
                 renamed_variables_new.add(copied_variable)
         variables.remove(renamed_variables_old)
         variables.add(renamed_variables_new)
                                
     def copy_snapshot_variables(self, old_ws:ROOT.RooWorkspace, old_mc:ROOT.RooStats.ModelConfig,
                                 new_ws:ROOT.RooWorkspace, new_mc:ROOT.RooStats.ModelConfig,
                                 snapshot_name:str, variable_type:Optional[Union[WSArgument, str]]=None,
                                 rename_map:Optional[Dict]=None):
         snapshot = old_ws.getSnapshot(snapshot_name)
         if not snapshot:
-            self.stdout.warning(f"WARNING: Snapshot {snapshot_name} not found in the original workspace")
+            self.stdout.warning(f"Snapshot {snapshot_name} not found in the original workspace")
         # get variables from orginal workspace, make sure to make a clone
         if variable_type is None:
             variables = snapshot.Clone()
         else:
             target_variables = self.get_variables(old_mc, variable_type)
             variables = snapshot.Clone().selectCommon(target_variables)
         if rename_map is None:
             rename_map = {}
-        self.stdout.info(f"INFO: Copying snapshot \"{snapshot_name}\" from the original workspace "
+        self.stdout.info(f"Copying snapshot \"{snapshot_name}\" from the original workspace "
                          "to the new workspace")
         self.copy_variables(variables, new_ws, rename_map)
         # important: the third argument decide whether to take values from the argset or from the workspace
         new_ws.saveSnapshot(snapshot_name, variables, True)
         
     def get_variables(self, mc:ROOT.RooStats.ModelConfig, variable_type:Union[WSArgument, str]):
         _variable_type = WSArgument.parse(variable_type)
@@ -492,18 +492,18 @@
         # only create objects of type RooArgSet
         generic_objects = [obj for obj in generic_objects if isinstance(obj, ROOT.RooArgSet)]
         if rename_map is None:
             rename_map = {}
         for generic_object in generic_objects:
             name = generic_object.GetName()
             if not name:
-                self.stdout.warning('WARNING: Found generic object without name. '
+                self.stdout.warning('Found generic object without name. '
                                     'The object will not be imported to the new workspace')
                 continue
-            self.stdout.info(f'INFO: Copying generic object "{name}" from the original workspace to the new workspace"')
+            self.stdout.info(f'Copying generic object "{name}" from the original workspace to the new workspace"')
             if all(isinstance(obj, ROOT.RooRealVar) for obj in generic_object):
                 argset = generic_object.Clone()
                 self.copy_variables(argset, new_ws, rename_map)
             else:
                 argset = self.recreate_argset(generic_object, new_ws, rename_map)
             new_ws.Import(argset, name, True)
             
@@ -552,18 +552,18 @@
             poi_names = [rename_map.get(poi_name, poi_name) for poi_name in poi_names]
         for poi_name in poi_names:
             poi = self._get_relevant_variable(poi_name, new_ws, pdf)
             if not poi:
                 if strict:
                     raise RuntimeError(f"POI {poi_name} does not exist")
                 else:
-                    self.stdout.warning(f"WARNING: POI {poi_name} does not exist. Skipping.")
+                    self.stdout.warning(f"POI {poi_name} does not exist. Skipping.")
                     continue
             pois.add(poi)
-            self.stdout.info(f"INFO: Added POI \"{poi_name}\".")
+            self.stdout.info(f"Added POI \"{poi_name}\".")
         mc.SetParametersOfInterest(pois)
         
         # nuisance parameters and global observables from original workspace
         old_nuis = old_mc.GetNuisanceParameters()
         if old_nuis:
             nuis_names = [nuis.GetName() for nuis in old_nuis]
             nuis_names = [rename_map.get(nuis, nuis) for nuis in nuis_names]
@@ -585,47 +585,47 @@
             glob_names += item['glob']
             
         # additional (unconstrained) nuisance parameters
         extra_nuis = self.actions['add_syst']
         nuis_names += extra_nuis
         
         if len(new_nuis) > 0:
-            self.stdout.info("INFO: The following newly defined nuisance parameter(s) will be added to ModelConfig")
+            self.stdout.info("The following newly defined nuisance parameter(s) will be added to ModelConfig")
             for nuis_name in new_nuis:
-                self.stdout.info(f"    {nuis_name}")
+                self.stdout.info(f"    {nuis_name}", bare=True)
         if len(extra_nuis) > 0:
-            self.stdout.info("INFO: The following additional nuisance parameter(s) will be added to ModelConfig")
+            self.stdout.info("The following additional nuisance parameter(s) will be added to ModelConfig")
             for nuis_name in extra_nuis:
-                self.stdout.info(f"    {nuis_name}")
+                self.stdout.info(f"    {nuis_name}", bare=True)
         
         nuis_names = remove_list_duplicates(nuis_names)
         # set nuisance parameters
         nuisance_parameters = ROOT.RooArgSet()
         for nuis_name in nuis_names:
             nuis = self._get_relevant_variable(nuis_name, new_ws, pdf)
             if not nuis:
-                self.stdout.warning(f"WARNING: The nuisance parameter {nuis_name} no longer exists in "
+                self.stdout.warning(f"The nuisance parameter {nuis_name} no longer exists in "
                                     "the new workspace. It will be removed from the new ModelConfig.")
                 continue
             if nuis.isConstant():
-                self.stdout.warning(f"WARNING: The nuisace parameter {nuis_name} is initialized as a constant. "
+                self.stdout.warning(f"The nuisace parameter {nuis_name} is initialized as a constant. "
                                     "It will be floated in the new workspace.")
                 nuis.setConstant(False)
             nuisance_parameters.add(nuis)
                 
         # set global observables
         global_observables = ROOT.RooArgSet()
         for glob_name in glob_names:
             glob = self._get_relevant_variable(glob_name, new_ws, pdf)
             if not glob:
-                self.stdout.warning(f"WARNING: The global observable {glob_name} no longer exists in "
+                self.stdout.warning(f"The global observable {glob_name} no longer exists in "
                                     "the new workspace. It will be removed from the new ModelConfig.")
                 continue
             if not glob.isConstant():
-                self.stdout.warning(f"WARNING: The global observable {glob_name} is initialized as a floating "
+                self.stdout.warning(f"The global observable {glob_name} is initialized as a floating "
                                     "parameter. It will be set to constant in the new workspace.")
 
                 glob.setConstant(True)
             global_observables.add(glob)
 
         # set observables
         observables = ROOT.RooArgSet()
@@ -649,47 +649,47 @@
         for variable in variables:
             variable_name = variable.GetName()
             extracted_variable = ws.arg(variable_name)
             if not extracted_variable:
                 if strict:
                     raise RuntimeError(f"missing variable {variable_name} in the workspace {ws.GetName()}")
                 else:
-                    self.stdout.warning(f"WARNING: No variable {variable_name} found in the workspace {ws.GetName()}")
+                    self.stdout.warning(f"No variable {variable_name} found in the workspace {ws.GetName()}")
                     continue
             extracted_variables.add(extracted_variable, True)
         return extracted_variables
 
     def rename_variables(self, old_mc:ROOT.RooStats.ModelConfig, new_ws:ROOT.RooWorkspace, rename_map:Dict):
         old_var_expr = ",".join(list(rename_map.keys()))
         new_var_expr = ",".join(list(rename_map.values()))
         getattr(new_ws, "import")(old_mc.GetPdf(),
                                   ROOT.RooFit.RenameVariable(old_var_expr, new_var_expr),
                                   ROOT.RooFit.RecycleConflictNodes())
         if rename_map:
-            self.stdout.info("INFO: Renamed variables\n")
+            self.stdout.info("Renamed variables\n")
             rename_table = "\n".join(self.get_name_mapping_str_arrays(rename_map))
-            self.stdout.info(rename_table)
+            self.stdout.info(rename_table, bare=True)
         
     def rename_objects(self, ws:ROOT.RooWorkspace, mc:ROOT.RooStats.ModelConfig):
         if len(self.actions['rename']['workspace']) > 0:
-            self.stdout.info("INFO: Renamed workspace\n")
+            self.stdout.info("Renamed workspace\n")
             rename_map = {}
             for old_name, new_name in self.actions['rename']['workspace'].items():
                 rename_map[ws.GetName()] = new_name
                 ws.SetName(new_name)
             rename_table = "\n".join(self.get_name_mapping_str_arrays(rename_map))
-            self.stdout.info(rename_table)
+            self.stdout.info(rename_table, bare=True)
         if len(self.actions['rename']['model_config']) > 0:
-            self.stdout.info("INFO: Renamed model config\n")
+            self.stdout.info("Renamed model config\n")
             rename_map = {}
             for old_name, new_name in self.actions['rename']['model_config'].items():
                 rename_map[mc.GetName()] = new_name
                 mc.SetName(new_name)
             rename_table = "\n".join(self.get_name_mapping_str_arrays(rename_map))
-            self.stdout.info(rename_table)
+            self.stdout.info(rename_table, bare=True)
         if len(self.actions['rename']['dataset']) > 0:
             rename_map = {}            
             for old_name, new_name in self.actions['rename']['dataset'].items():
                 if old_name == new_name:
                     continue
                 dataset = ws.data(old_name)
                 if not dataset:
@@ -697,44 +697,44 @@
                 check_dataset = ws.data(new_name)
                 if check_dataset:
                     raise RuntimeError(f"cannot rename dataset from \"{old_name}\" to \"{new_name}\": "
                                        f"the dataset \"{new_name}\" already exists in the original workspace")
                 rename_map[old_name] = new_name
                 dataset.SetName(new_name)
             if rename_map:
-                self.stdout.info("INFO: Renamed dataset\n")
+                self.stdout.info("Renamed dataset\n")
                 rename_table = "\n".join(self.get_name_mapping_str_arrays(rename_map))
-                self.stdout.info(rename_table)                
+                self.stdout.info(rename_table, bare=True)                
         
     def import_datasets(self, old_ws:ROOT.RooWorkspace, new_ws:ROOT.RooWorkspace,
                         dataset_names:Optional[List[str]]=None):
         if dataset_names is None:
             datasets = old_ws.allData()
         else:
             datasets = []
             for dataset_name in dataset_names:
                 dataset = old_ws.data(dataset_name)
                 if not dataset:
                     raise RuntimeError(f"dataset {dataset_name} does not exist in the original workspace")
                 datasets.append(dataset)
         for dataset in datasets:
             getattr(new_ws, "import")(dataset)
-            self.stdout.info(f"INFO: Imported dataset \"{dataset.GetName()}\".")
+            self.stdout.info(f"Imported dataset \"{dataset.GetName()}\".")
             
     def redefine_objects(self, old_ws:ROOT.RooWorkspace, new_ws:ROOT.RooWorkspace):
         flag = False
         for i, expr in enumerate(self.actions['redefine']):
-            self.stdout.info(f"INFO: (Item {i}) {expr}")
+            self.stdout.info(f"(Item {i}) {expr}")
             obj_name, obj_type = self._get_object_name_and_type_from_expr(expr)
             arg = old_ws.arg(obj_name)
             if not arg:
                 if self.config['strict']:
                     raise RuntimeError(f"object {obj_name} does not exist in the original workspace")
                 else:
-                    self.stdout.warning(f"WARNING: object {obj_name} does not exist in the original workspace")
+                    self.stdout.warning(f"object {obj_name} does not exist in the original workspace")
                     continue
             if obj_type == WSObjectType.VARIABLE:
                 result = re.search(r"\[(.+)\]", expr)
                 if not result:
                     raise RuntimeError(f"invalid variable expression {expr}")
                 self.import_expression(new_ws, expr)
                 new_var = new_ws.var(obj_name)
@@ -754,15 +754,15 @@
                 self.import_expression(new_ws, expr)
             flag = True
         return flag
         
     def implement_objects(self, ws:ROOT.RooWorkspace):
         flag = False
         for i, expr in enumerate(self.actions['define']):
-            self.stdout.info(f"INFO: (Item {i}) {expr}")
+            self.stdout.info(f"(Item {i}) {expr}")
             if "FlexibleInterpVar" in expr:
                 self.implement_flexible_interp_var(ws, expr)
             elif "RooMultiVarGaussian" in expr:
                 self.implement_multi_var_gaussian(ws, expr)
             else:
                 self.import_expression(ws, expr)
             flag = True
@@ -771,15 +771,15 @@
     def implement_external_pdfs(self, ws:ROOT.RooWorkspace):
         flag = False
         for i, item in enumerate(self.actions['constraint']):
             pdf_name = item['pdf']
             file = item['file']
             if file is not None:
                 self.load_external_pdf(file, pdf_name, ws)
-                self.stdout.info(f"INFO: Loaded external pdf {pdf_name} from {file}")
+                self.stdout.info(f"Loaded external pdf {pdf_name} from {file}")
                 flag = True
         return flag
                 
     def load_external_pdf(self, ext_rfile:str, pdf_name:str, ws:ROOT.RooWorkspace):
         model = ExtendedModel(ext_rfile, data_name=None, verbosity="WARNING")
         pdf = model.workspace.pdf(pdf_name)
         if not pdf:
@@ -851,15 +851,15 @@
         nuisance_parameters = self.extract_ws_variables(new_ws, old_mc.GetNuisanceParameters(), False)
 
         pdf_map = {}
         
         for i in range(n_cat):
             category.setBin(i)
             category_name = category.getLabel()
-            self.stdout.info(f"INFO: Creating new pdf for the category {category_name}")
+            self.stdout.info(f"Creating new pdf for the category {category_name}")
             pdf_i = pdf.getPdf(category_name)
             
             base_components = ROOT.RooArgSet()
             obs_terms = ROOT.RooArgList()
             dis_constraints = ROOT.RooArgList()
             ROOT.RooStats.FactorizePdf(observables, pdf_i, obs_terms, dis_constraints)
             base_components.add(obs_terms)
@@ -877,15 +877,15 @@
                 glob_names = item['glob']
                 independent = item['independent']
                 new_pdf = new_ws.pdf(pdf_name)
                 if not new_pdf:
                     raise RuntimeError(f"pdf {pdf_name} does not exist in the new workspace")
                 if independent:
                     base_components.add(new_pdf)
-                    self.stdout.info(f"INFO: Adding independent constraint pdf \"{pdf_name}\" to "
+                    self.stdout.info(f"Adding independent constraint pdf \"{pdf_name}\" to "
                                      f"\"{new_pdf_name}\"")
                     continue
                 # check whether the current category depends on the constraint pdf
                 for nuis_name in nuis_names:
                     nuis_var = self._get_relevant_variable(nuis_name, new_ws, pdf_i)
                     if (nuis_var is not None):
                         base_components.add(new_pdf)
@@ -899,19 +899,19 @@
         return sim_pdf
     
     @staticmethod
     def _get_relevant_variable(var_name:str, ws:ROOT.RooWorkspace, pdf:ROOT.RooAbsPdf, warn:bool=False):
         var = ws.var(var_name)
         if not var:
             if warn:
-                self.stdout.warning(f"WARNING: Variable {var_name} does not exist in the new workspace")
+                self.stdout.warning(f"Variable {var_name} does not exist in the new workspace")
             return None
         if not pdf.dependsOn(var):
             if warn:
-                self.stdout.warning(f"WARNING: Variable {var_name} exists in the new workspace but is "
+                self.stdout.warning(f"Variable {var_name} exists in the new workspace but is "
                                     f"not part of the provided pdf {pdf.GetName()}")
             return None
         return var
         
     def implement_flexible_interp_var(self, ws:ROOT.RooWorkspace, expr:str):
         # parse attributes
         expr = re.sub('\s+', '', expr)
@@ -936,16 +936,16 @@
         nuis_arglist = ROOT.RooArgList()
         nuis = self.get_workspace_arg(ws, nuis_name)
         nuis_arglist.add(nuis)
         
         function = ROOT.RooStats.HistFactory.FlexibleInterpVar(response_name, response_name, nuis_arglist,
                                                                nominal, sigma_var_low, sigma_var_high, code)
         self.import_object(ws, function)
-        self.stdout.info(f"INFO: Implemented FlexibleInterpVar \"{response_name}\"")
-        self.stdout.info(str(py_V))
+        self.stdout.info(f"Implemented FlexibleInterpVar \"{response_name}\"")
+        self.stdout.info(str(py_V), bare=True)
 
     
     def implement_multi_var_gaussian(self, ws:ROOT.RooWorkspace, expr:str):
         # parse attributes
         expr = re.sub('\s+', '', expr)
         program = re.compile(r"RooMultiVarGaussian::(?P<name>[\w]+)\({(?P<obsList>[\w,]+)}:"
                              r"{(?P<meanList>[\w,]+)}:{(?P<uncertList>[\w,]+)}:"
@@ -990,9 +990,9 @@
                     V[i, j] = v
                     V[j, i] = v
                     py_V[i, j] = v
                     py_V[j, i] = v
                     index += 1
         function = RooMultiVarGaussian(function_name, function_name, obs_arglist, mean_arglist, V)
         self.import_object(ws, function)
-        self.stdout.info(f"INFO: Implemented RooMultiVarGaussian \"{function_name}\" with correlation matrix")
-        self.stdout.info(str(py_V))
+        self.stdout.info(f"Implemented RooMultiVarGaussian \"{function_name}\" with correlation matrix")
+        self.stdout.info(str(py_V), bare=True)
```

### Comparing `quickstats-0.6.7.8/quickstats/concurrent/abstract_runner.py` & `quickstats-0.6.8.1/quickstats/concurrent/abstract_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         pass
         
     def run_instance(self, kwargs:Dict[str, Any]):
         self._prerun_instance(**kwargs)
         outname = kwargs.get("outname", None)
         
         if outname and (self.config['cache'] and os.path.exists(outname) and is_valid_file(outname)):
-            self.stdout.info(f"INFO: Cached output from {outname}")
+            self.stdout.info(f"Cached output from {outname}")
             return self._cached_return(outname)
         
         log_path = kwargs.get("log_path", None)
         if (outname and self.config['save_log']) and (not log_path):
             log_path = os.path.splitext(outname)[0] + ".log"
         if self.config['save_log']:
             with standard_log(log_path) as logger:
@@ -68,12 +68,12 @@
         t0 = time.time()
         self._prerun_batch()
         raw_result = execute_multi_tasks(self.run_instance, argument_list, parallel=parallel)
         results = self.postprocess(raw_result, auxiliary_args)
         t1 = time.time()
         dt = t1 - t0        
         if self.config['timed']:
-            self.stdout.info('INFO: All jobs have finished. Total time taken: {:.3f} s'.format(dt))
+            self.stdout.info('All jobs have finished. Total time taken: {:.3f} s'.format(dt))
         return results
     
     def postprocess(self, raw_result, auxiliary_args:Optional[Dict]=None):
         return raw_result
```

### Comparing `quickstats-0.6.7.8/quickstats/concurrent/logging.py` & `quickstats-0.6.8.1/quickstats/concurrent/logging.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/concurrent/parameterised_asymptotic_cls.py` & `quickstats-0.6.8.1/quickstats/concurrent/parameterised_asymptotic_cls.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     
     @semistaticmethod
     def _prerun_instance(self, filename:str, parameters:Optional[Dict[str, Any]]=None, **kwargs):
         if parameters:
             param_str = "("+ParamParser.val_encode_parameters(parameters)+")"
         else:
             param_str = ""
-        self.stdout.info(f"INFO: Evaluating limit for the workspace {filename} {param_str}")
+        self.stdout.info(f"Evaluating limit for the workspace {filename} {param_str}")
     
     @semistaticmethod
     def _cached_return(self, outname:str):
         with open(outname, 'r') as f:
             limits = json_load(f)
             return limits
```

### Comparing `quickstats-0.6.7.8/quickstats/concurrent/parameterised_likelihood.py` & `quickstats-0.6.8.1/quickstats/concurrent/parameterised_likelihood.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,26 +39,26 @@
             'outname': outname
         }
         
         self.attributes['poi_names'] = ParamParser._get_param_str_attributes(param_expr)
 
     def _prerun_batch(self):
         self.stdout.info("TIPS: When running likelihood scan on an Asimov dataset, remember to restore the global "
-                         "observables to their Asimov values by loading the appropriate snapshot.")
+                         "observables to their Asimov values by loading the appropriate snapshot.", bare=True)
         outdir = self.attributes['outdir']
         cache_dir = self.get_cache_dir()
         batch_makedirs([outdir, cache_dir])
     
     @semistaticmethod
     def _prerun_instance(self, filename:str, mode:int, poi_val:Optional[Union[float, Dict[str, float]]]=None, **kwargs):
         if mode == 2:
             param_str = "("+ParamParser.val_encode_parameters(poi_val)+")"
-            self.stdout.info(f"INFO: Evaluating conditional NLL {param_str} for the workspace {filename}")
+            self.stdout.info(f"Evaluating conditional NLL {param_str} for the workspace {filename}")
         elif mode == 1:
-            self.stdout.info(f"INFO: Evaluating unconditional NLL for the workspace {filename}")
+            self.stdout.info(f"Evaluating unconditional NLL for the workspace {filename}")
     
     @semistaticmethod
     def _cached_return(self, outname:str):
         with open(outname, 'r') as f:
             result = json.load(f)
             processed_result = self._process_result(result)
         return processed_result
```

### Comparing `quickstats-0.6.7.8/quickstats/concurrent/parameterised_runner.py` & `quickstats-0.6.8.1/quickstats/concurrent/parameterised_runner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/core/abstract_object.py` & `quickstats-0.6.8.1/quickstats/core/abstract_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/core/configs.py` & `quickstats-0.6.8.1/quickstats/core/configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,20 +365,20 @@
             text = bullet + node_label + "\n"
             text += component.get_explain_text(linebreak=linebreak)
         else:
             text = traverse_node(self.config_format, write=node_label=="",
                                  filter_labels=required_labels)
         if not text:
             if required_only:
-                self.stdout.critical('ERROR: No required components matches the requested scope. '
+                self.stdout.critical('No required components matches the requested scope. '
                                      'Try using "required_only=False" instead.')
             elif node_label:
-                self.stdout.critical(f'ERROR: Config node "{node_label}" does not exist.')
+                self.stdout.critical(f'Config node "{node_label}" does not exist.')
             else:
-                self.stdout.critical(f'ERROR: Config format is empty.')                
+                self.stdout.critical(f'Config format is empty.')                
         return text
     
     def explain(self, node_label:Optional[str]="",
                 required_only:bool=False,
                 indent:str="    ",
                 bullet:str="=>",
                 linebreak:int=100):
@@ -407,15 +407,15 @@
             raise ValueError(f'found unsupported format in the config component "{label}"')
         return component_map
     
     def parse_config(self, config:Union[Dict, str]):
         if isinstance(config, str):
             extension = os.path.splitext(config)[-1]
             if not self.disable_message:
-                self.stdout.info(f'INFO: Reading configuration file "{config}".')
+                self.stdout.info(f'Reading configuration file "{config}".')
             if extension == ".json":
                 import json
                 with open(config, "r") as file:
                     config = json.load(file)
             elif extension == ".yaml":
                 import yaml
                 with open(config, "r") as file:
@@ -465,16 +465,16 @@
                     for config_key in extra_keys:
                         config[config_key] = component.validate(config[config_key])
                 else:
                     # only fill default if component is strictly required
                     if component.required_strict:
                         config[key] = component.validate(MISSING)
                         if not self.disable_message:
-                            self.stdout.info(f'INFO: Auto-filled missing config component "{config_label}" with '
-                                         f'default value "{config[key]}".')
+                            self.stdout.info(f'Auto-filled missing config component "{config_label}" with '
+                                             f'default value "{config[key]}".')
             else:
                 if key == "*":
                     config_keys = extra_keys
                 else:
                     if key not in config:
                         config[key] = {}
                     config_keys = [key]
```

### Comparing `quickstats-0.6.7.8/quickstats/core/configurable_object.py` & `quickstats-0.6.8.1/quickstats/core/configurable_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/core/dataclass_object.py` & `quickstats-0.6.8.1/quickstats/core/dataclass_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/core/decorators.py` & `quickstats-0.6.8.1/quickstats/core/decorators.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
 def cls_method_timer(func):
     def wrapper(self, *args, **kwargs):
         t1 = time.time()
         result = func(self, *args, **kwargs)
         t2 = time.time()
         method_name = f"{type(self).__name__}::{func.__name__}"
-        self.stdout.info(f'INFO: Task {method_name!r} executed in {(t2-t1):.4f}s')
+        self.stdout.info(f'Task {method_name!r} executed in {(t2-t1):.4f}s')
         return result
     return wrapper 
 
 class Timer:    
     def __enter__(self):
         self.start = time.time()
         return self
```

### Comparing `quickstats-0.6.7.8/quickstats/core/enums.py` & `quickstats-0.6.8.1/quickstats/core/enums.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/core/methods.py` & `quickstats-0.6.8.1/quickstats/core/methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/core/path_manager.py` & `quickstats-0.6.8.1/quickstats/core/path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/core/virtual_trees.py` & `quickstats-0.6.8.1/quickstats/core/virtual_trees.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/interface/cppyy/core.py` & `quickstats-0.6.8.1/quickstats/interface/cppyy/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/interface/cppyy/vectorize.py` & `quickstats-0.6.8.1/quickstats/interface/cppyy/vectorize.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/interface/root/RooAbsData.py` & `quickstats-0.6.8.1/quickstats/interface/root/RooAbsData.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/interface/root/RooCategory.py` & `quickstats-0.6.8.1/quickstats/interface/root/RooCategory.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/interface/root/RooDataSet.py` & `quickstats-0.6.8.1/quickstats/interface/root/RooDataSet.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 from typing import Dict, Union, List, Optional, Tuple
+import os
 
 import numpy as np
 
 from quickstats import semistaticmethod, AbstractObject
 from quickstats.interface.cppyy.vectorize import as_np_array
 from quickstats.maths.statistics import (dataset_is_binned, fill_missing_bins,
                                          rebin_dataset, bin_edge_to_bin_center)
 
 class RooDataSet(AbstractObject):
     
+    GHOST_THRESHOLD = 1e-8
+    GHOST_WEIGHT    = 1e-9
+    
     def __init__(self, dataset:"ROOT.RooDataSet",
+                 remove_ghost:bool=False,
+                 ghost_threshold:Optional[float]=None,
+                 ghost_weight:Optional[float]=None,
                  verbosity:Optional[Union[int, str]]=None):
         super().__init__(verbosity=verbosity)
-        self.parse(dataset)
-        self.ghost_threshold = 1e-8
+        if ghost_threshold is None:
+            self.ghost_threshold = self.GHOST_THRESHOLD
+        else:
+            self.ghost_threshold = ghost_threshold
+        if ghost_weight is None:
+            self.ghost_weight = self.GHOST_WEIGHT
+        else:
+            self.ghost_weight = ghost_weight            
         self.bin_precision = 8
         self.error_option = 'poisson'
+        self.parse(dataset, remove_ghost=remove_ghost)
         
-    def parse(self, dataset:"ROOT.RooDataSet"):
+    def parse(self, dataset:"ROOT.RooDataSet", remove_ghost:bool=False):
         category = self.get_dataset_category(dataset)
         if not category:
             raise RuntimeError('no category defined in the dataset')
         self.set_category_variable(category)
         observables = self.get_dataset_observables(dataset)
         self.set_observable_variables(observables)
-        self.data = self.to_numpy(dataset, copy=True, rename_columns=False,
-                                  category_label=False)
+        self.data = self.to_numpy(dataset, copy=True,
+                                  rename_columns=False,
+                                  category_label=False,
+                                  remove_ghost=remove_ghost)
         self.name = dataset.GetName()
         self.title = dataset.GetTitle()
         self.set_weight_variable(dataset.weightVar())
         
         obs_cat_pairing = self.pair_category_and_observable(dataset)
         category_map = {}
         for pairing in obs_cat_pairing:
@@ -38,15 +54,16 @@
                 'category_index': pairing['category_index']
             }
         self.category_map = category_map
             
     @semistaticmethod
     def to_numpy(self, dataset:"ROOT.RooDataSet", copy:bool=True,
                  rename_columns:bool=True, category_label:bool=True,
-                 split_category:bool=False):
+                 split_category:bool=False, sort:bool=True,
+                 remove_ghost:bool=False):
         # use ROOT's built-in method if available
         if hasattr(dataset, "to_numpy"):
             data = dataset.to_numpy(copy=copy)
         # just copy the implementation from ROOT
         else:
             import ROOT
 
@@ -96,123 +113,164 @@
             if category_col is not None:
                 data['category_index'] = data.pop(category_col)
                 category_col = 'category_index'
                 
         if label_values is not None:
             data['category_label'] = label_values
             
-        if split_category and (category is not None):
+        if remove_ghost and (weight_col is not None):
+            mask = data[weight_col] > self.GHOST_THRESHOLD
+            for key in data:
+                data[key] = data[key][mask]
+            
+        if split_category:
+            if category is None:
+                raise RuntimeError(f'cannot split dataset by category: no category '
+                                   'defined in the dataset')
             cat_obs_info_list = self.pair_category_and_observable(dataset)
             cat_data = {}
             for cat_obs_info in cat_obs_info_list:
                 cat_label = cat_obs_info['category_label']
                 cat_index = cat_obs_info['category_index']
                 observable = cat_obs_info['observable']
                 mask = data[category_col] == cat_index
+                obs_values = data[observable][mask]
+                wt_values  = data[weight_col][mask]
+                if sort:
+                    sort_idx = np.argsort(obs_values)
+                    obs_values = obs_values[sort_idx]
+                    wt_values = wt_values[sort_idx]
                 cat_data[cat_label] = {
-                    observable: data[observable][mask],
-                    weight_col: data[weight_col][mask]
+                    observable: obs_values,
+                    weight_col: wt_values
                 }
             return cat_data
             
         return data
     
     @staticmethod
-    def from_numpy(data:Dict[str, "numpy.ndarray"],
-                   variables:"ROOT.RooArgSet",
-                   name:str=None, title:str=None,
-                   weight_name:str=None, clip_to_limits=True):
+    def from_numpy(data, variables, name=None, title=None, weight_name=None):
         import ROOT
-        if name is None:
-            name = ""
-        if title is None:
-            title = ""
-            
-        if weight_name is None:
-            dataset = ROOT.RooDataSet(name, title, variables)
+        # use ROOT's built-in method
+        if hasattr(ROOT.RooDataSet, "from_numpy"):
+            dataset = ROOT.RooDataSet.from_numpy(data, variables,
+                                                 name=name,
+                                                 title=title,
+                                                 weight_name=weight_name)
         else:
-            dataset = ROOT.RooDataSet(name, title, variables, weight_name)
-            
-        real_variables = {}
-        cat_variables = {}
-        for v in variables:
-            var_name = v.GetName()
-            class_name = v.ClassName()
-            if var_name == weight_name:
-                continue
-            if var_name not in data:
-                if (class_name == "RooCategory") and ("category_index" in data):
-                    var_name = "category_index"
-                else:
-                    raise RuntimeError(f"missing data for the variable `{var_name}`")
-            if class_name == "RooCategory":
-                cat_variables[var_name] = v
-            else:
-                real_variables[var_name] = v
-                if clip_to_limits:
-                    data[var_name] = np.clip(data[var_name], 
-                                             a_min=v.getMin(),
-                                             a_max=v.getMax())
-        if weight_name not in data:
-            if "weight" in data:
-                weight_name = "weight"
-            else:
-                raise RuntimeError(f"missing data for the variable `{weight_name}`")
-                
-        data_sizes = [len(data[k]) for k in data]
-        if len(set(data_sizes)) > 1:
-            raise RuntimeError("data has inconsistent sizes")
-        if weight_name is None:
-            for i in range(data_sizes[0]):
-                for name, variable in real_variables.items():
-                    variable.setVal(data[name][i])
-                for name, variable in cat_variables.items():
-                    variable.setIndex(data[name][i])
-                dataset.add(variables, 1.)
-        else:
-            for i in range(data_sizes[0]):
-                for name, variable in real_variables.items():
-                    variable.setVal(data[name][i])
-                for name, variable in cat_variables.items():
-                    variable.setIndex(int(data[name][i]))
-                weight = data[weight_name][i]
-                dataset.add(variables, weight)
-            
+            raise NotImplementedError
         return dataset
     
     @semistaticmethod
     def to_pandas(self, dataset:"ROOT.RooDataSet", copy:bool=True,
                   rename_columns:bool=True, category_label:bool=True,
-                  split_category:bool=False):
+                  split_category:bool=False, sort:bool=True,
+                  remove_ghost:bool=False):
         numpy_data = self.to_numpy(dataset, copy=copy,
                                    rename_columns=rename_columns,
                                    category_label=category_label,
-                                   split_category=split_category)
+                                   split_category=split_category,
+                                   sort=sort,
+                                   remove_ghost=remove_ghost)
         import pandas as pd
         if split_category:
             df_cat = {}
             for category, category_data in numpy_data.items():
                 df_cat[category] = pd.DataFrame(category_data)
             return df_cat
         df = pd.DataFrame(numpy_data)
         return df
     
     to_dataframe = to_pandas
     
     @staticmethod
+    def from_pandas(df, variables, name=None, title=None, weight_name=None):
+        import ROOT
+        # use ROOT's built-in method
+        if hasattr(ROOT.RooDataSet, "from_pandas"):
+            dataset = ROOT.RooDataSet.from_pandas()
+        else:
+            raise NotImplementedError
+        return dataset
+    
+    @staticmethod
     def get_dataset_map(dataset_dict:Dict):
         import ROOT
         dsmap = ROOT.std.map('string, RooDataSet*')()
         dsmap.keepalive = list()
         for c, d in dataset_dict.items():
             dsmap.keepalive.append(d)
             dsmap.insert(dsmap.begin(), ROOT.std.pair("const string, RooDataSet*")(c, d))
         return dsmap
     
     @staticmethod
+    def from_category_data(data, variables, name=None, title=None, weight_name=None,
+                           add_ghost:bool=False, ghost_weight:float=GHOST_WEIGHT):
+        import ROOT
+        
+        if name is None:
+            name = "dataset"
+        if title is None:
+            title = name
+
+        def get_category_observable(columns:List[str], category:str):
+            candidates = [column for column in columns if variables.find(column)]
+            if weight_name is not None:
+                candidates = [column for column in columns if column != weight_name]
+            if len(candidates) != 1:
+                raise RuntimeError(f'failed to deduce observable name for the category "{category}"')
+            return variables.find(candidates[0])
+        
+        dataset_map = {}
+        for category, cat_data in data.items():
+            cat_variables = ROOT.RooArgSet()
+            columns = list(cat_data.keys())
+            cat_observable = get_category_observable(columns, category)
+            cat_variables.add(cat_observable)
+            if weight_name is not None:
+                weight_var = ROOT.RooRealVar(weight_name, weight_name, 1)
+                cat_variables.add(weight_var)
+            cat_name = f"{name}_{category}"
+            cat_title = f"{title}_{category}"
+            cat_dataset = RooDataSet.from_numpy(cat_data, cat_variables,
+                                                name=cat_name, title=cat_title,
+                                                weight_name=weight_name)
+            if add_ghost:
+                RooDataSet.add_ghost_weights(cat_dataset,
+                                             ghost_weight=ghost_weight)
+            dataset_map[category] = cat_dataset
+
+        # not needed by newer version of ROOT
+        c_dataset_map = RooDataSet.get_dataset_map(dataset_map)
+        cat_var = [v for v in variables if v.ClassName() == "RooCategory"]
+        _variables = ROOT.RooArgSet(variables)
+        if not cat_var:
+            cat_var = ROOT.RooCategory('category', 'category')
+            for category in data:
+                cat_var.defineType(category)
+        else:
+            cat_var = cat_var[0]
+            _variables.remove(cat_var)
+
+        if weight_name is not None:
+            weight_var = _variables.find(weight_name)
+            if not weight_var:
+                weight_var = ROOT.RooRealVar(weight_name, weight_name, 1)
+                _variables.add(weight_var)
+            dataset = ROOT.RooDataSet(name, title, _variables,
+                                      ROOT.RooFit.Index(cat_var),
+                                      ROOT.RooFit.Import(dataset_map),
+                                      ROOT.RooFit.WeightVar(weight_var))
+        else:
+            dataset = ROOT.RooDataSet(name, title, _variables,
+                                      ROOT.RooFit.Index(cat_var),
+                                      ROOT.RooFit.Import(dataset_map))
+        return dataset
+    
+    @staticmethod
     def from_RooDataHist(source:"ROOT.RooDataHist", pdf:"ROOT.RooAbsPdf",
                          name:Optional[str]=None):
         import ROOT
         if name is None:
             name = source.GetName()
         parameters = source.get()
         category = None
@@ -367,38 +425,14 @@
             if n_bins_data != n_bins:
                 raise RuntimeError(f"the observable has `{n_bins}` bins but data has `{n_bins_data}`")
             for j in range(n_bins_data):
                 observable.setBin(j)
                 dataset.add(variables, data_i[j])
         return dataset
     
-    @semistaticmethod
-    def to_category_data(self, dataset:"ROOT.RooDataSet",
-                         pdf:"ROOT.RooAbsPdf"):
-        cat_and_obs = self.get_category_and_observables(dataset)
-        cat_variable = cat_and_obs['category']
-        if cat_variable is None:
-            raise RuntimeError('no category defined in the dataset')
-        n_cat = cat_variable.size()
-        data = self.to_numpy(dataset)
-        result = {}
-        for i in range(n_cat):
-            cat_variable.setIndex(i)
-            cat_name = cat_variable.getLabel()
-            pdf_cat = pdf.getPdf(cat_name)
-            obs = pdf_cat.getObservables(variables)
-            cat_obs = obs.first()
-            obs_name = cat_obs.GetName()
-            mask = (data['index'] == i)
-            bin_value = data[obs_name][mask]
-            ind = np.argsort(bin_value)
-            bin_weight = data['weight'][mask][ind]
-            result[cat_name] = bin_weight
-        return result
-    
     @staticmethod
     def fill_from_TH1(dataset:"ROOT.RooDataSet", hist:"ROOT.TH1",
                       skip_out_of_range:bool=True,
                       blind_range:Optional[List[float]]=None,
                       min_bin_value:float=0,
                       weight_scale:float=1):
         import ROOT
@@ -461,26 +495,26 @@
                 continue
             hist.Fill(x_val, weight)
         return hist
     
     @staticmethod
     def add_ghost_weights(dataset:"ROOT.RooDataSet",
                           blind_range:Optional[List[float]]=None,
-                          ghost_weight:float=1e-9):
+                          ghost_weight:float=GHOST_WEIGHT):
         x, weight_var = RooDataSet.get_x_and_weight(dataset)
-        xmin = x.getMin()
-        xmax = x.getMax()
+        xmin, xmax = x.getMin(), x.getMax()
         n_bins = x.getBins()
         bin_width = (xmax - xmin) / n_bins
         data = RooDataSet.to_numpy(dataset)
         x_data = data[x.GetName()]
         weight_data = data["weight"]
         hist, bin_edges = np.histogram(x_data, bins=n_bins, range=(xmin, xmax), weights=weight_data)
         from quickstats.maths.statistics import bin_edge_to_bin_center
         bin_centers = bin_edge_to_bin_center(bin_edges)
+        # to be optimized
         import ROOT
         for bin_val, bin_center in zip(hist, bin_centers):
             if (bin_val != 0):
                 continue
             if (blind_range and (bin_center > blind_range[0]) and (bin_center < blind_range[1])):
                 continue
             x.setVal(bin_center)
@@ -599,37 +633,70 @@
         for category, scale_factor in scale_factors.items():
             if category not in self.category_map:
                 raise ValueError(f'dataset has no category "{category}"')
             category_index = self.category_map[category]['category_index']
             mask = self.data[category_name] == category_index
             self.data[weight_name][mask] *= scale_factor
     
-    def get_category_data(self, category:str):
+    def get_category_data(self, category:str, sort:bool=True,
+                          remove_ghost:bool=False):
         category_name = self.category.name
         weight_name = self.weight.name
         category_index = self.category_map[category]['category_index']
         observable_name = self.category_map[category]['observable']
         mask = self.data[category_name] == category_index
+        obs_values = self.data[observable_name][mask]
+        wt_values = self.data[weight_name][mask]
+        if sort:
+            sort_idx = np.argsort(obs_values)
+            obs_values = obs_values[sort_idx]
+            wt_values = wt_values[sort_idx]
+        if remove_ghost:
+            mask = wt_values > self.ghost_threshold
+            obs_values = obs_values[mask]
+            wt_values = wt_values[mask]
         category_data = {
-            observable_name: self.data[observable_name][mask],
-            weight_name: self.data[weight_name][mask]
+            observable_name: obs_values,
+            weight_name: wt_values
         }
         return category_data
     
+    def get_category_histogram(self, category:str, histname:str='hist',
+                               histtitle:Optional[str]=None,
+                               nbins:Optional[int]=None,
+                               bin_range:Optional[Tuple[float]]=None,
+                               weight_scale:Optional[float]=None,
+                               include_error:bool=True):
+        distribution = self.get_category_distribution(category, nbins=nbins,
+                                                      bin_range=bin_range,
+                                                      weight_scale=weight_scale,
+                                                      include_error=False)
+        if include_error:
+            bin_error, _ = self.get_weight_error(distribution['y'], error_option='sumw2')
+        else:
+            bin_error = None
+        from quickstats.interface.root import TH1
+        from quickstats.maths.statistics import bin_center_to_bin_edge
+        bin_edges = bin_center_to_bin_edge(distribution['x'])
+        hist = TH1.from_numpy_histogram(distribution['y'],
+                                        bin_edges=bin_edges,
+                                        bin_error=bin_error)
+        roohist = hist.to_ROOT(histname, histtitle)
+        return roohist
+        
+    
     def get_category_distribution(self, category:str, nbins:Optional[int]=None,
                                   bin_range:Optional[Tuple[float]]=None,
                                   weight_scale:Optional[float]=None,
                                   include_error:bool=True):
-        data = self.get_category_data(category)
+        data = self.get_category_data(category, sort=True)
         observable_name = self.category_map[category]['observable']
         weight_name = self.weight.name
         x, y = data[observable_name], data[weight_name]
-        idx = np.argsort(x)
-        x, y = x[idx], y[idx]
-        observable = [v for v in self.observables if v.name == observable_name]
+        observable = [obs for obs in self.observables if obs.name == observable_name]
         assert len(observable) == 1
         observable = observable[0]
         default_nbins = observable.n_bins
         if nbins is None:
             nbins = default_nbins
         if bin_range is None:
             bin_range = observable.range
@@ -647,15 +714,15 @@
             x, y = fill_missing_bins(x, y, xlow=bin_range[0],
                                      xhigh=bin_range[1],
                                      nbins=default_nbins,
                                      bin_precision=self.bin_precision)
         # rebin binned dataset
         if binned_dataset and (nbins != default_nbins):
             x, y = rebin_dataset(x, y, nbins)
-            self.stdout.warning(f"WARNING: Rebinned dataset ({self.name}, category = {category}) "
+            self.stdout.warning(f"Rebinned dataset ({self.name}, category = {category}) "
                                 f"from nbins = {default_nbins} to nbins = {nbins}")
         if not binned_dataset:
             non_ghost_mask = (y > self.ghost_threshold)
             if non_ghost_mask.all():
                 x_non_ghost = x
                 y_non_ghost = y
             else:
@@ -665,15 +732,15 @@
                                            range=(bin_range[0], bin_range[1]),
                                            density=False, weights=y_non_ghost)
             bin_centers = bin_edge_to_bin_center(bin_edges)
             x = bin_centers
             y = hist
 
         if include_error:
-            yerrlo, yerrhi = self.get_weight_error(y)
+            yerrlo, yerrhi = self.get_weight_error(y, self.error_option)
         else:
             yerrlo, yerrhi = None, None
             
         if weight_scale is not None:
             y *= weight_scale
             if (yerrlo is not None) and (yerrhi is not None):
                 yerrlo *= weight_scale
@@ -684,15 +751,15 @@
         }
         if (yerrlo is not None) and (yerrhi is not None):
             result["yerrlo"] = yerrlo
             result["yerrhi"] = yerrhi
         return result
     
     def create_binned_dataset(self, binnings:Optional[Union[Dict[str, int], int]]=None) -> "RooDataSet":
-        pass
+        raise NotImplementedError
     
     def get_merged_distribution(self, categories:Optional[List[str]]=None,
                                 nbins:Optional[int]=None,
                                 bin_range:Optional[Tuple[float]]=None,
                                 include_error:bool=True,
                                 weight_scales:Optional[Union[float, Dict[str, float]]]=None):
         if categories is None:
@@ -728,21 +795,22 @@
             'y': y
         }
         if (yerrlo is not None) and (yerrhi is not None):
             result["yerrlo"] = np.sqrt(yerrlo)
             result["yerrhi"] = np.sqrt(yerrhi)
         return result
     
-    def get_weight_error(self, weight:np.ndarray):
-        if self.error_option == "poisson":
+    @semistaticmethod
+    def get_weight_error(self, weight:np.ndarray, error_option:str='sumw2'):
+        if error_option == "poisson":
             from quickstats.interface.root import TH1
             weight_error = TH1.GetPoissonError(weight)
             return weight_error['lo'], weight_error['hi']
-        elif self.error_option == "sumw2":
-            weight_error = np.sqrt(y)
+        elif error_option == "sumw2":
+            weight_error = np.sqrt(weight)
             return weight_error, weight_error
         else:
             raise RuntimeError(f'unknown error option: {self.error_option}')
     
     def new(self) -> "ROOT.RooDataSet":
         import ROOT
         variables = ROOT.RooArgSet()
@@ -756,8 +824,165 @@
         else:
             weight_name = None
         dataset = ROOT.RooDataSet.from_numpy(self.data, variables,
                                              name=self.name,
                                              title=self.title,
                                              weight_name=weight_name)
         return dataset
-    
+    
+    @staticmethod
+    def get_dataset_from_txt_file(filename:str, observable:"ROOT.RooRealVar",
+                                  weight_var:Optional["ROOT.RooRealVar"]=None,
+                                  dataset_name:str="dataset"):
+        if not os.path.exists(filename):
+            raise FileNotFoundError(f'file does not exist: {filename}')
+        try:
+            data = np.loadtxt(filename)
+        except:
+            raise RuntimeError(f'failed to read data from text file: {filename}')
+        import ROOT
+        if weight_var is None:
+            weight_var = ROOT.RooRealVar("weight", "weight", 1)
+        dataset = ROOT.RooDataSet(dataset_name, dataset_name,
+                                  ROOT.RooArgSet(observable, weight_var),
+                                  ROOT.RooFit.WeightVar(weight_var))
+        if (data.ndim == 1):
+            ROOT.RFUtils.FillDataSetValues(dataset, observable, data.data,
+                                           data.shape[0])
+        elif (data.ndim == 2) and (data.shape[1] == 2):
+            ROOT.RFUtils.FillWeightedDataSetValues(dataset, observable,
+                                                   data.flatten().data,
+                                                   data.shape[0],
+                                                   weight_var)
+        else:
+            raise RuntimeError('invalid file format')
+        return dataset
+    
+    @staticmethod
+    def get_dataset_from_root_files(filenames:Union[str, List[str]],
+                                    observable:"ROOT.RooRealVar",
+                                    treename:str, branchname:str,
+                                    weight_var:Optional["ROOT.RooRealVar"]=None,
+                                    weight_branchname:Optional[str]=None,
+                                    cut:str="",
+                                    dataset_name:str="dataset"):
+        import ROOT
+        chain = ROOT.TChain(treename)
+        if isinstance(filenames, str):
+            filenames = filenames.split(",")
+        for filename in filenames:
+            if not os.path.exists(filename):
+                raise FileNotFoundError(f"file does not exist: {filename}")
+            status = chain.AddFile(filename, -1)
+            if not status:
+                raise RuntimeError(f'cannot find tree "{treename}" in file "{filename}"')
+        if cut:
+            chain = chain.CopyTree(cut)
+        branch = chain.FindBranch(branchname)
+        if not branch:
+            raise RuntimeError(f'cannot find branch "{branchname}" in tree "{treename}"')
+        x = ROOT.RooRealVar(branchname, branchname, observable.getMin(), observable.getMax())
+        if weight_branchname is not None:
+            weight_branch = chain.FindBranch(weight_branchname)
+            if not weight_branch:
+                raise RuntimeError(f'cannot find branch "{weight_branchname}" in tree "{treename}"')
+            w = ROOT.RooRealVar(weight_branchname, weight_branchname, 1)
+            dataset = ROOT.RooDataSet(dataset_name, dataset_name,
+                                      ROOT.RooArgSet(x, w),
+                                      ROOT.RooFit.Import(chain),
+                                      ROOT.RooFit.WeightVar(w))
+            if weight_var is not None:
+                dataset.weightVar().SetName(weight_var.GetName())
+        else:
+            dataset = ROOT.RooDataSet(dataset_name, dataset_name,
+                                      ROOT.RooArgSet(x),
+                                      ROOT.RooFit.Import(chain))
+        dataset.get().first().SetName(observable.GetName())
+        return dataset
+    
+    def filter_categories(self, categories:List[str]):
+        cat_indices = []
+        excluded_categories = []
+        excluded_obs  = []
+        for category in categories:
+            if category not in self.category_map:
+                raise ValueError(f'dataset does not contain the category "{category}"')
+            cat_index = self.category_map[category]['category_index']
+            cat_indices.append(cat_index)
+        for category in self.category_map:
+            if category not in categories:
+                excluded_categories.append(category)
+                obs_label = self.category_map[category]['observable']
+                excluded_obs.append(obs_label)
+        cat_column = self.category.name
+        mask = np.isin(self.data[cat_column], cat_indices)
+        # clean up observable and category information
+        for key in self.data:
+            self.data[key] = self.data[key][mask]
+        self.observables = [obs for obs in self.observables if obs.name not in excluded_obs]       
+        for category in excluded_categories:
+            self.category_map.pop(category)
+        self.category.category_labels = list(categories)
+        # reset category index
+        index_map = {}
+        for new_index, category in enumerate(categories):
+            old_index = self.category_map[category]['category_index']
+            index_map[old_index] = new_index
+            self.category_map[category]['category_index'] = new_index
+        self.data[cat_column] = np.vectorize(index_map.get)(self.data[cat_column])
+        
+            
+    def generate_toy_dataset(self, n_toys:int=1,
+                             seed:Optional[int]=None,
+                             event_seed:Optional[Dict]=None,
+                             add_ghost:bool=True,
+                             name_fmt:str="{name}_toy_{index}",
+                             title_fmt:str="{title}_toy_{index}"):
+        from quickstats.maths.statistics_jitted import random_poisson_elementwise_seed
+        import ROOT
+        cat_data = {}
+        weight_name = self.weight.name
+        for category in self.category_map:
+            cat_data[category] = self.get_category_data(category,
+                                                        remove_ghost=True,
+                                                        sort=True)
+            unbinned = (cat_data[category][weight_name] == 1).all()
+            if not unbinned:
+                raise RuntimeError('cannot generate toy dataset from binned data')
+        variables = ROOT.RooArgSet()
+        for observable in self.observables:
+            variables.add(observable.new())
+        variables.add(self.category.new())
+        
+        if seed is not None:
+            np.random.seed(seed)
+        
+        for i in range(n_toys):
+            toy_data = {}
+            for category in self.category_map:
+                toy_data[category] = {}
+                obs_name = self.category_map[category]['observable']
+                obs_values = cat_data[category][obs_name]
+                if event_seed is not None:
+                    if category not in event_seed:
+                        raise ValueError(f'no event seed defined for the category: {category}')
+                    cat_event_seed = np.array(event_seed[category])
+                    if cat_event_seed.shape != obs_values.shape:
+                        raise ValueError(f'number of event seeds in a category must match '
+                                         f'the number of events in the category dataset')
+                    cat_event_seed = cat_event_seed + i
+                    pois_weights = random_poisson_elementwise_seed(cat_event_seed, 1).flatten()
+                else:
+                    pois_weights = np.random.poisson(size=cat_data[category][weight_name].shape)
+                toy_data[category][obs_name] = np.repeat(obs_values, pois_weights)
+                toy_data[category][weight_name] = np.ones(toy_data[category][obs_name].shape)
+            name  = name_fmt.format(name=self.name, index=(i+1))
+            if title_fmt is None:
+                title = name
+            else:
+                title = title_fmt.format(title=self.title, index=(i+1))
+            toy_dataset_i = self.from_category_data(toy_data, variables,
+                                                    name=name, title=title,
+                                                    weight_name=weight_name,
+                                                    add_ghost=add_ghost,
+                                                    ghost_weight=self.ghost_weight)
+            yield toy_dataset_i
```

### Comparing `quickstats-0.6.7.8/quickstats/interface/root/RooMsgService.py` & `quickstats-0.6.8.1/quickstats/interface/root/RooMsgService.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/interface/root/RooRealVar.py` & `quickstats-0.6.8.1/quickstats/interface/root/RooRealVar.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             self.value  = obj.getVal()
             self.n_bins = obj.getBins()
             self.unit   = obj.getUnit()
             _range = obj.getRange()
             self.range = [_range[0], _range[1]]
             named_ranges = {}
             for name in obj.getBinningNames():
-                if str(name) == "":
+                if str(name) in ["", "cache"]:
                     continue
                 _range = obj.getRange(name)
                 named_ranges[name] = [_range[0], _range[1]]
             self.named_ranges = named_ranges
         
     @staticmethod
     def _parse_named_ranges(named_ranges:Optional[Dict[str, List[float]]]=None):
```

### Comparing `quickstats-0.6.7.8/quickstats/interface/root/TF1.py` & `quickstats-0.6.8.1/quickstats/interface/root/TF1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/interface/root/TFile.py` & `quickstats-0.6.8.1/quickstats/interface/root/TFile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/interface/root/TH1.py` & `quickstats-0.6.8.1/quickstats/interface/root/TH1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/interface/root/TH2.py` & `quickstats-0.6.8.1/quickstats/interface/root/TH2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 import array
 import numpy as np
 
+from quickstats import semistaticmethod
 from quickstats.interface.root import TObject, TArrayData
 from quickstats.interface.cppyy.vectorize import c_array_to_np_array
 
 class TH2(TObject):
     
+    DTYPE_MAP = {
+        "TH2I": "int",
+        "TH2F": "float",
+        "TH2D": "double"
+    }
+    
     def __init__(self, h:"ROOT.TH2", underflow_bin:bool=False, overflow_bin:bool=False):
+        import ROOT
         dtype_map = {
             ROOT.TH2I: "int",
             ROOT.TH2F: "float",
             ROOT.TH2D: "double"
         }
         self.dtype = dtype_map.get(type(h), "double")
         self.underflow_bin = underflow_bin
@@ -93,24 +101,25 @@
     def GetXBinLowEdgeArray(h:"ROOT.TH2", dtype:str='double', underflow_bin:int=0, overflow_bin:int=0):
         return TH2.GetAxisBinLowEdgeArray(h.GetXaxis(), dtype, underflow_bin, overflow_bin)
     
     @staticmethod
     def GetYBinLowEdgeArray(h:"ROOT.TH2", dtype:str='double', underflow_bin:int=0, overflow_bin:int=0):
         return TH2.GetAxisBinLowEdgeArray(h.GetYaxis(), dtype, underflow_bin, overflow_bin)
     
-    @staticmethod
-    def correlationHist_to_dataframe(h:"ROOT.TH2"):
-        dtype = TH2.DTYPE_MAP.get(type(h), "double")
-        data = TH2.GetBinContentArray(h, dtype)
-        xlabels = TH2.GetXLabelArray(h)
-        ylabels = TH2.GetYLabelArray(h)
+    @semistaticmethod
+    def correlationHist_to_dataframe(self, h:"ROOT.TH2"):
+        dtype = self.DTYPE_MAP.get(h.ClassName(), "double")
+        data = self.GetBinContentArray(h, dtype)
+        xlabels = self.GetXLabelArray(h)
+        ylabels = self.GetYLabelArray(h)
         if not np.array_equal(xlabels, ylabels):
             raise RuntimeError("invalid correlation histogram: labels along x-axis and y-axis do not match")
         if (data.shape[0] != len(xlabels)) or (data.shape[1] != len(ylabels)):
             raise RuntimeError("invaiid correlation histogram: size of matrix does not match number of labels")
         _data = {}
         for i, label in enumerate(xlabels):
             _data[label] = data[:, i]
         import pandas as pd
         df = pd.DataFrame(_data)
         df.index = ylabels[::-1]
+        df = df.loc[df.index[::-1]]
         return df
```

### Comparing `quickstats-0.6.7.8/quickstats/interface/root/TObject.py` & `quickstats-0.6.8.1/quickstats/interface/root/TObject.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/interface/root/__init__.py` & `quickstats-0.6.8.1/quickstats/interface/root/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/interface/root/helper.py` & `quickstats-0.6.8.1/quickstats/interface/root/helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/interface/root/inspection.py` & `quickstats-0.6.8.1/quickstats/interface/root/inspection.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/interface/root/roofit_extension.py` & `quickstats-0.6.8.1/quickstats/interface/root/roofit_extension.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx` & `quickstats-0.6.8.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h` & `quickstats-0.6.8.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx` & `quickstats-0.6.8.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h` & `quickstats-0.6.8.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx` & `quickstats-0.6.8.1/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/macros/QuickStatsCore/RooFitExt.cxx` & `quickstats-0.6.8.1/quickstats/macros/QuickStatsCore/RooFitExt.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/macros/QuickStatsCore/RooFitExt.h` & `quickstats-0.6.8.1/quickstats/macros/QuickStatsCore/RooFitExt.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/macros/ResponseFunction/ResponseFunction.cxx` & `quickstats-0.6.8.1/quickstats/macros/ResponseFunction/ResponseFunction.cxx`

 * *Files 3% similar despite different names*

```diff
@@ -165,15 +165,15 @@
 //_____________________________________________________________________________
 double ResponseFunction::PolyInterpValue(int i, double x) const
 {
   // If this is running for first time
   if (!_logInit)
   {
     // Create polynomial array
-    const unsigned int n = (unsigned int)_lowList.getSize();
+    const unsigned int n = _lowList.getSize();
     assert(n == (unsigned int)_highList.getSize());
     _polCoeff.resize(n * 6);
     // cache the polynomial coefficient values
     // which do not dpened on x but on the boundaries values
     for (unsigned j = 0; j < n; j++)
       cacheCoef(j);
     _logInit = kTRUE;
@@ -211,15 +211,15 @@
   // Calculate and return value of polynomial
 
   Double_t total = 1;
 
   RooAbsReal *param;
   int i = 0;
 
-  for (size_t i=0; i < (size_t)_paramList.getSize(); i++) {
+  for (size_t i=0; i < _paramList.getSize(); i++) {
     const auto& param = static_cast<RooAbsReal&>(_paramList[i]);
     const auto& low = static_cast<RooAbsReal&>(_lowList[i]);
     const auto& high = static_cast<RooAbsReal&>(_highList[i]);
 
     Int_t icode = _interpCode[i];
 
     double highVar = fabs(high.getVal());
@@ -277,15 +277,15 @@
   RooAbsReal::printMultiline(os, contents, verbose, indent);
   os << indent << "--- ResponseFunction ---" << std::endl;
   printResponseFunctions(os);
 }
 
 void ResponseFunction::printResponseFunctions(std::ostream &os) const
 {
-  for (size_t i = 0; i < (size_t)_paramList.getSize(); i++)
+  for (size_t i = 0; i < _paramList.getSize(); i++)
   {
     const auto& param = static_cast<RooAbsReal&>(_paramList[i]);
     const auto& low = static_cast<RooAbsReal&>(_lowList[i]);
     const auto& high = static_cast<RooAbsReal&>(_highList[i]);
     os << std::setw(36) << param.GetName() << ": "
        << std::setw(7) << _nominal.at(i) << "  "
        << std::setw(7) << low.getVal() << "  "
@@ -330,63 +330,48 @@
   coeff[1] = 1. / (8 * x0 * x0) * (-24 + 24 * S0 - 9 * x0 * A1 + x0 * x0 * S2);
   coeff[2] = 1. / (4 * pow(x0, 3)) * (-5 * A0 + 5 * x0 * S1 - x0 * x0 * A2);
   coeff[3] = 1. / (4 * pow(x0, 4)) * (12 - 12 * S0 + 7 * x0 * A1 - x0 * x0 * S2);
   coeff[4] = 1. / (8 * pow(x0, 5)) * (+3 * A0 - 3 * x0 * S1 + x0 * x0 * A2);
   coeff[5] = 1. / (8 * pow(x0, 6)) * (-8 + 8 * S0 - 5 * x0 * A1 + x0 * x0 * S2);
 }
 
-#if ROOT_VERSION_CODE >= ROOT_VERSION(6,26,0)
+#if ROOT_VERSION_CODE >= ROOT_VERSION(6,29,0)
 
 #include <RooFitHS3/RooJSONFactoryWSTool.h>
-#include <RooFitHS3/JSONInterface.h>
+#include <RooFit/Detail/JSONInterface.h>
+#include <RooFitHS3/JSONIO.h>
 #include <RooWorkspace.h>
 
-using namespace RooFit::Experimental;
+using namespace RooFit::Detail;
 
 namespace {
-class ResponseFunctionStreamer : public RooJSONFactoryWSTool::Exporter {
+  class ResponseFunctionStreamer : public RooFit::JSONIO::Exporter {
 public:
   virtual const std::string& key() const override {
     static const std::string _key = "resonse";
     return _key;
   }
   
   virtual bool exportObject(RooJSONFactoryWSTool *, const RooAbsArg *func, JSONNode &elem) const override
   {
     const ResponseFunction *pip = static_cast<const ResponseFunction *>(func);
     elem["type"] << key();
-    elem["interpolationCodes"] << pip->interpolationCodes();
-    auto &vars = elem["vars"];
-    vars.set_seq();
-    for (const auto &v : pip->parameters()) {
-      vars.append_child() << v->GetName();
-    }
-
-    auto &nom = elem["nom"];
-    nom << pip->nominal();
-
-    auto &high = elem["high"];
-    high.set_seq();
-    for (const auto &v : pip->high()) {
-      high.append_child() << v->GetName();
-    }
-
-    auto &low = elem["low"];
-    low.set_seq();
-    for (const auto &v : pip->low()) {
-      low.append_child() << v->GetName();
-    }
+    elem["interpolationCodes"].fill_seq(pip->interpolationCodes());
+    elem["vars"].fill_seq(pip->parameters(), [](auto const &f) { return f->GetName(); });    
+    elem["nom"].fill_seq(pip->nominal());
+    elem["high"].fill_seq(pip->high(), [](auto const &f) { return f->GetName(); });
+    elem["low"].fill_seq(pip->low(), [](auto const &f) { return f->GetName(); });    
     return true;
   }
 };
 } // namespace
 
 
 namespace {
-class ResponseFunctionFactory : public RooJSONFactoryWSTool::Importer {
+class ResponseFunctionFactory : public RooFit::JSONIO::Importer {
 public:
    virtual bool importFunction(RooJSONFactoryWSTool *tool, const JSONNode &p) const override
    {
       std::string name(RooJSONFactoryWSTool::name(p));
       if (!p.has_child("vars")) {
          RooJSONFactoryWSTool::error("no vars of '" + name + "'");
       }
@@ -434,15 +419,15 @@
    }
 };
 } // namespace
 
 
 namespace {
   int register_serializations(){
-    RooJSONFactoryWSTool::registerImporter("response", std::make_unique<ResponseFunctionFactory>());
-    RooJSONFactoryWSTool::registerExporter(ResponseFunction::Class(), std::make_unique<ResponseFunctionStreamer>());
+    RooFit::JSONIO::registerImporter("response", std::make_unique<ResponseFunctionFactory>());
+    RooFit::JSONIO::registerExporter(ResponseFunction::Class(), std::make_unique<ResponseFunctionStreamer>());
     return 1;
   }
   int _dummy = register_serializations();
 }
 
 #endif
```

### Comparing `quickstats-0.6.7.8/quickstats/macros/ResponseFunction/ResponseFunction.h` & `quickstats-0.6.8.1/quickstats/macros/ResponseFunction/ResponseFunction.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx` & `quickstats-0.6.8.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h` & `quickstats-0.6.8.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/maths/interpolation.py` & `quickstats-0.6.8.1/quickstats/maths/interpolation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/maths/numerics.py` & `quickstats-0.6.8.1/quickstats/maths/numerics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/maths/statistics.py` & `quickstats-0.6.8.1/quickstats/maths/statistics.py`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,16 @@
         Arguments:
             data: np.ndarray
                 Array containing the event number in each bin.
             n_simg: float
                 Number of sigma to use for the Poisson interval.
     """
     from quickstats.interface.root import TH1
-    return TH1.GetPoissonError(data, n_sigma)
+    result = TH1.GetPoissonError(data, n_sigma)
+    return result
 
 def get_counting_significance(s:float, b:float, sigma_b:float=0, leading_order:bool=False):
     """
         Asimov approximation for the median significance in a counting experiment.
         
         Arguments:
         -------------------------------------------------------------------------------
@@ -184,15 +185,15 @@
         Z_combined = np.sqrt(np.sum(Z2))
     return Z_combined
 
 def bin_edge_to_bin_center(bin_edge:np.ndarray):
     return 0.5 * (bin_edge[1:] + bin_edge[:-1])
 
 def bin_center_to_bin_edge(bin_center:np.ndarray):
-    bin_widths = np.diff(bin_center)
+    bin_widths = np.round(np.diff(bin_center), 8)
     if len(np.unique(bin_widths)) != 1:
         raise ValueError("can not deduce bin edges from bin centers of irregular bin widths")
     bin_width = bin_widths[0]
     bin_edges = np.concatenate([bin_center - bin_width / 2, [bin_center[-1] + bin_width/2]])
     return bin_edges
 
 def min_max_to_range(min_val:Optional[float]=None, max_val:Optional[float]=None):
@@ -252,27 +253,27 @@
            The bin errors of the histogram.
     """
     x = np.array(x)
     
     if weights is None:
         weights = np.ones(x.shape)
     else:
-        weights = np.array(weights)
+        # fix overflow bugs
+        weights = np.array(weights, dtype=float)
         
     if normalize:
         if clip_weight and (bin_range is not None):
             first_edge, last_edge = bin_range
             norm_factor = weights[(x >= first_edge) & (x <= last_edge)].sum()
         else:
             norm_factor = weights.sum()
     else:
         norm_factor = 1
         
     bin_content, bin_edges = np.histogram(x, bins=bins, range=bin_range, weights=weights)
-        
     if evaluate_error:
         error_option = BinErrorOption.parse(error_option)
         if error_option == BinErrorOption.AUTO:
             unit_weight = np.allclose(weights, np.ones(weights.shape))
             error_option = BinErrorOption.POISSON if unit_weight else BinErrorOption.SUMW2
         if error_option == BinErrorOption.POISSON:
             pois_interval = get_poisson_interval(bin_content)
@@ -346,25 +347,48 @@
                                    bins=bins, bin_range=bin_range,
                                    normalize=normalize,
                                    clip_weight=clip_weight,
                                    evaluate_error=yerr,
                                    error_option=error_option)
     x = bin_edge_to_bin_center(bin_edges)
     if xerr:
-        xerr = np.diff(bin_edges) / 2
+        # todo do not hard-code number of digits to keep
+        xerr = np.round(np.diff(bin_edges) / 2, 5)
     else:
         xerr = None
     hist_data = {
         "x": x,
         "y": y,
         "xerr": xerr,
         "yerr": yerr
     }
     return hist_data
 
+def get_stacked_hist_data(x:List[np.ndarray],
+                          weights:List[Optional[np.ndarray]]=None,
+                          bins:Union[int, Sequence]=10,
+                          bin_range:Optional[Sequence]=None,
+                          normalize:bool=True,
+                          clip_weight:bool=False,
+                          xerr:bool=True,
+                          yerr:bool=True,
+                          error_option:Union[BinErrorOption, str]="auto"):
+    x = np.concatenate(x)
+    if weights is not None:
+        weights = np.concatenate(weights)
+        assert x.shape == weights.shape
+    if bin_range is None:
+        bin_range = (np.min(x), np.max(x))
+    return get_hist_data(x=x, weights=weights,
+                         bins=bins, bin_range=bin_range,
+                         normalize=normalize,
+                         clip_weight=clip_weight,
+                         xerr=xerr, yerr=yerr,
+                         error_option=error_option)
+
 def get_sumw2(weights:np.ndarray):
     return np.sqrt(np.sum(weights ** 2))
 
 def get_hist_mean(x:np.ndarray, y:np.ndarray):
     return np.sum(x * y) / np.sum(y)
 
 def get_hist_std(x:np.ndarray, y:np.ndarray):
@@ -402,14 +426,19 @@
 def get_bin_centers_from_range(xlow:float, xhigh:float, nbins:int, bin_precision:int=8):
     bin_width = (xhigh - xlow) / nbins
     low_bin_center  = xlow + bin_width / 2
     high_bin_center = xhigh - bin_width /2
     bins = np.around(np.linspace(low_bin_center, high_bin_center, nbins), bin_precision)
     return bins
 
+def pvalue_to_significance(pvalue:float):
+    import ROOT
+    significance = ROOT.RooStats.PValueToSignificance(pvalue)
+    return significance
+
 def dataset_is_binned(x:np.ndarray, y:np.ndarray, xlow:float, xhigh:float, nbins:int,
                       ghost_threshold:float=1e-8, bin_precision:int=8):
     bin_centers = get_bin_centers_from_range(xlow, xhigh, nbins, bin_precision=bin_precision)
     x = np.around(x, bin_precision)
     same_nbins = len(x) == len(bin_centers)
     if same_nbins and np.allclose(bin_centers, x):
         return True
@@ -455,15 +484,15 @@
 
 def get_hist_comparison_data(reference_data, target_data,
                              mode:Union[HistComparisonMode, str]="ratio"):
     mode = HistComparisonMode.parse(mode)
     if not np.allclose(target_data['x'], reference_data['x']):
         raise RuntimeError("cannot compare two distributions with different binnings")
     comparison_data = {}
-    comparison_data['x']    = reference_data['x']
+    comparison_data['x'] = reference_data['x']
     source_data = {}
     all_zero = {}
     # fill zero error if not given
     for key, data in [('reference', reference_data), 
                  ('target', target_data)]:
         source_data[key] = {}
         all_zero[key] = {}
@@ -487,36 +516,47 @@
         allclose = all(np.allclose(source_data['reference']['xerr'][i],
                                    source_data['target']['xerr'][i]) \
                        for i in [0, 1])
     else:
         allclose = np.allclose(source_data['reference']['xerr'],
                                source_data['target']['xerr'])
     if not allclose:
-        raise RuntimeError('xerr of the reference and target distributions must match')
+        if (all_zero['reference']['xerr'] or all_zero['target']['xerr']):
+            if not all_zero['reference']['xerr']:
+                comparison_xerr = source_data['reference']['xerr']
+            else:
+                comparison_xerr = source_data['target']['xerr']
+        else:
+            raise RuntimeError('xerr of the reference and target distributions must match')
+    else:
+        comparison_xerr = source_data['reference']['xerr']
     
     if not (all_zero['reference']['xerr'] and all_zero['target']['xerr']):
-        comparison_data['xerr'] = source_data['reference']['xerr']
+        comparison_data['xerr'] = comparison_xerr
     else:
         comparison_data['xerr'] = np.zeros(comparison_data['x'].shape)
+        
+    if mode == HistComparisonMode.RATIO:
+        comparison_data['y'] = safe_div(target_data['y'], reference_data['y'], True)
+    elif mode == HistComparisonMode.DIFFERENCE:
+        comparison_data['y'] = target_data['y'] - reference_data['y']
     
-    if not (all_zero['reference']['xerr'] and all_zero['target']['xerr']):
+    if not (all_zero['reference']['yerr'] and all_zero['target']['yerr']):
         yerr_ref, yerr_tgt = source_data['reference']['yerr'], source_data['target']['yerr']
         if mode == HistComparisonMode.RATIO:
-            comparison_data['y'] = safe_div(target_data['y'], reference_data['y'], True)
             if isinstance(yerr_ref, tuple):
                 errlo = np.sqrt(safe_div(yerr_ref[0], reference_data['y'], True)**2 + 
                                 safe_div(yerr_tgt[0], target_data['y'], True)**2)
                 errhi = np.sqrt(safe_div(yerr_ref[1], reference_data['y'], True)**2 + 
                                 safe_div(yerr_tgt[1], target_data['y'], True)**2)
                 comparison_data['yerr'] = (errlo, errhi)
             else:
                 comparison_data['yerr'] = np.sqrt(safe_div(yerr_ref, reference_data['y'], True)**2 + 
                                                   safe_div(yerr_tgt, target_data['y'], True)**2)
         elif mode == HistComparisonMode.DIFFERENCE:
-            comparison_data['y'] = target_data['y'] - reference_data['y']
             if isinstance(yerr_ref, tuple):
                 errlo = np.sqrt(yerr_ref[0]**2 + yerr_tgt[0]**2)
                 errhi = np.sqrt(yerr_ref[1]**2 + yerr_tgt[1]**2)
                 comparison_data['yerr'] = (errlo, errhi)
             else:
                 comparison_data['yerr'] = np.sqrt(yerr_ref**2 + yerr_tgt**2)
     else:
```

### Comparing `quickstats-0.6.7.8/quickstats/maths/statistics_jitted.py` & `quickstats-0.6.8.1/quickstats/maths/statistics_jitted.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,13 +81,13 @@
             rounded -= 1
         rounded /= np.power(10, dummy)
     return rounded  
 
 @jit(nopython=True)
 def random_poisson_elementwise_seed(seeds, size):
     n_seed = seeds.shape[0]
-    poisson_weights = np.zeros((size, n_seed))
+    poisson_weights = np.zeros((size, n_seed), dtype=int64)
     for i, seed in enumerate(seeds):
-        np.random.seed(seed)
+        np.random.seed(seed % 4294967296)
         for j in range(size):
             poisson_weights[j, i] = np.random.poisson()
     return poisson_weights
```

### Comparing `quickstats-0.6.7.8/quickstats/maths/symbolics.py` & `quickstats-0.6.8.1/quickstats/maths/symbolics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/parsers/param_parser.py` & `quickstats-0.6.8.1/quickstats/parsers/param_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import copy
 import glob
 import fnmatch
 import itertools
 from functools import partial
 
 import numpy as np
+import pandas as pd
 
 from quickstats import semistaticmethod, DescriptiveEnum
 from quickstats.maths.numerics import pretty_float, str_encode_value, str_decode_value, to_string, to_rounded_float
 from quickstats.utils.string_utils import remove_whitespace, split_str
 
 signature_regex = {
     'F': r"\d+[.]?\d*",
@@ -148,22 +149,24 @@
         return attribute_parser
     
     @staticmethod
     def _get_param_str_attributes(param_str:Optional[str]=None):
         if param_str is None:
             return []
         attributes = []
-        param_expr_list = split_str(param_str, sep=',', remove_empty=True)
-        for expr in param_expr_list:
-            tokens = split_str(expr, sep='=')
-            if len(tokens) not in [1, 2]:
-                raise ValueError('invalid expression for parameterisation')
-            attribute = tokens[0]
-            if attribute not in attributes:
-                attributes.append(attribute)
+        idp_param_strs = split_str(param_str, sep=';', remove_empty=True)
+        for idp_param_str in idp_param_strs:
+            param_expr_list = split_str(idp_param_str, sep=',', remove_empty=True)
+            for expr in param_expr_list:
+                tokens = split_str(expr, sep='=')
+                if len(tokens) not in [1, 2]:
+                    raise ValueError('invalid expression for parameterisation')
+                attribute = tokens[0]
+                if attribute not in attributes:
+                    attributes.append(attribute)
         return attributes
     
     @semistaticmethod
     def _get_format_str_attributes(self, format_str:Optional[str]=None):
         if format_str is None:
             return []
         attribute_parser = self.get_attribute_parser(format_str)
@@ -171,14 +174,15 @@
 
     @staticmethod
     def parse_param_str(param_str:Optional[str]=None):
         if param_str is None:
             return {}
         param_points = []
         idp_param_strs = split_str(param_str, sep=';', remove_empty=True)
+        all_combinations = []
         for idp_param_str in idp_param_strs:
             param_values = {}
             param_expr_list = split_str(idp_param_str, sep=',', remove_empty=True)
             for expr in param_expr_list:
                 tokens = expr.split('=')
                 # floating poi
                 if len(tokens) == 1:
@@ -214,18 +218,19 @@
             # convert to numpy arrays
             combinations = [np.array(param_values[param_name]) for param_name in param_names]
             # take care of rounding errors and negative zeros
             combinations = [(arr.round(decimals=8) + 0.0) if arr[0] is not None else arr for arr in combinations]
             # take care of duplicate ploints
             combinations = [np.unique(arr) for arr in combinations]
             combinations = itertools.product(*combinations)
-
-            for combination in combinations:
-                param_point = {k:v for k,v in zip(param_names, combination)}
-                param_points.append(param_point)
+            all_combinations.extend(list(combinations))
+        all_combinations = pd.unique(all_combinations)
+        for combination in all_combinations:
+            param_point = {k:v for k,v in zip(param_names, combination)}
+            param_points.append(param_point)
         return param_points
     
     @staticmethod
     def val_encode_parameters(parameters:Dict):
         tokens = []
         for param, value in parameters.items():
             if value is None:
```

### Comparing `quickstats-0.6.7.8/quickstats/plots/__init__.py` & `quickstats-0.6.8.1/quickstats/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/abstract_plot.py` & `quickstats-0.6.8.1/quickstats/plots/abstract_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,16 +229,14 @@
         xlim = list(ax.get_xlim())
         ylim = list(ax.get_ylim())
         if xmin is not None:
             xlim[0] = xmin
         if xmax is not None:
             xlim[1] = xmax
         if ypad is not None:
-            if (ymax is not None):
-                raise ValueError('can not use both "ypad" and "ymax" when setting axis range')
             if ypad < 0 or ypad > 1:
                 raise ValueError('"ypad" must be between 0 and 1')
             ylim[1] = ylim[1] / (1 - ypad)
         if ymin is not None:
             ylim[0] = ymin
         if ymax is not None:
             ylim[1] = ymax                
@@ -265,14 +263,15 @@
         error_format = ErrorDisplayFormat.parse(error_format)
         handle, error_handle = None, None
         
         x, y = data['x'], data['y']
         xerr, yerr = data.get('xerr', 0), data.get('yerr', 0)
         
         if draw_data:
+            styles = combine_dict(self.styles['errorbar'], styles)
             if plot_format == PlotFormat.ERRORBAR:
                 if (not draw_error) or (error_format != ErrorDisplayFormat.ERRORBAR):
                     handle = ax.errorbar(x, y, **styles)
                 else:
                     handle = ax.errorbar(**data, **styles)
             else:
                 raise RuntimeError(f'unsupported plot format: {plot_format.name}')
```

### Comparing `quickstats-0.6.7.8/quickstats/plots/bidirectional_bar_chart.py` & `quickstats-0.6.8.1/quickstats/plots/bidirectional_bar_chart.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/collective_data_plot.py` & `quickstats-0.6.8.1/quickstats/plots/collective_data_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/color_schemes.py` & `quickstats-0.6.8.1/quickstats/plots/color_schemes.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/core.py` & `quickstats-0.6.8.1/quickstats/plots/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,22 +97,22 @@
     from matplotlib.colors import ListedColormap
     from matplotlib.cm import register_cmap
     for name, colors in listed_colors.items():
         cmap = ListedColormap(colors, name=name)
         register_cmap(name=name, cmap=cmap, override_builtin=True)
         
 def get_cmap(source:Optional[Union[List, str]], name:Optional[str]="from_list", size:Optional[int]=None, resample:bool=True):
-    from matplotlib.colors import ListedColormap
+    from matplotlib.colors import ListedColormap, LinearSegmentedColormap
     if isinstance(source, str):
         from matplotlib.cm import get_cmap as gcm
         cmap = gcm(source)
         return get_cmap(cmap, size=size, resample=resample)
-    elif isinstance(source, ListedColormap):
+    elif isinstance(source, (ListedColormap, LinearSegmentedColormap)):
         if size is None:
-            return source
+            return source.copy()
         if resample or (size >= source.N):
             return source.resampled(size)
         else:
             cmap_rgba = source(range(source.N))[:size]
             return get_cmap(cmap_rgba, name=source.name)
     else:
         return ListedColormap(source, name=name, N=size)
```

### Comparing `quickstats-0.6.7.8/quickstats/plots/general_1D_plot.py` & `quickstats-0.6.8.1/quickstats/plots/general_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/general_distribution_plot.py` & `quickstats-0.6.8.1/quickstats/plots/general_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/histo_1D_plot.py` & `quickstats-0.6.8.1/quickstats/plots/histo_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/hypotest_inverter_plot.py` & `quickstats-0.6.8.1/quickstats/plots/hypotest_inverter_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/likelihood_1D_plot.py` & `quickstats-0.6.8.1/quickstats/plots/likelihood_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/likelihood_2D_plot.py` & `quickstats-0.6.8.1/quickstats/plots/likelihood_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/np_ranking_plot.py` & `quickstats-0.6.8.1/quickstats/plots/np_ranking_plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,21 +442,20 @@
         text_options = {
             'fontsize'  : styles['label']['fontsize'],
         }
         
         extra_texts = []
         
         if extra_text:
-            extra_texts.append(extra_texts)
+            extra_texts.extend(extra_text.split('//'))
             
         if ranking_label:
             rank_text = 'Rank {} to {}'.format(r_start, r_end)
             extra_texts.append(rank_text)
-        
-        
+
         draw_options = {
             'axis': axis,
             'loc': (x_logo, -height),
             'fontsize': fontsize_logo,
             'status': status,
             'extra_text': "//".join(extra_texts),
             'dy': dy,
```

### Comparing `quickstats-0.6.7.8/quickstats/plots/pdf_distribution_plot.py` & `quickstats-0.6.8.1/quickstats/plots/pdf_distribution_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,26 @@
                 else:
                     x = pdata['x']
                     y = pdata['y']
                     xerr = pdata['xerr']
                     yerr = pdata['yerr']
                 if not show_error:
                     error_format = None
+                y_nonzero = np.where(y != 0)
+                x, y = x[y_nonzero], y[y_nonzero]
+                if (xerr is not None):
+                    if isinstance(xerr, tuple):
+                        xerr = (xerr[0][y_nonzero], xerr[1][y_nonzero])
+                    else:
+                        xerr = xerr[y_nonzero]
+                if (yerr is not None):
+                    if isinstance(yerr, tuple):
+                        yerr = (yerr[0][y_nonzero], yerr[1][y_nonzero])
+                    else:
+                        yerr = yerr[y_nonzero]
                 handle = self._draw_data(ax, x, y, xerr, yerr,
                                          plot_options=combined_options,
                                          error_format=error_format,
                                          error_styles=error_styles)
             elif plot_type == "hist":
                 x = pdata['x']
                 y = pdata['y']
@@ -286,14 +298,15 @@
              yerr_tgt = pdata_tgt['yerr']
         if mode == "ratio":
             vmode = 0
         elif mode in ["diff", "difference"]:
             vmode = 1
         else:
             raise ValueError(f"unsupported mode \"{mode}\", choose between \"ratio\" and \"difference\"")
+        valid_mask = (pdata_tgt['y'] > 0) & (pdata_ref['y'] > 0)
         if vmode == 0:
             pdata_comp['y'] = pdata_tgt['y'] / pdata_ref['y']
             if isinstance(yerr_ref, tuple):
                 errlo = np.sqrt((yerr_ref[0]/pdata_ref['y'])**2 + (yerr_tgt[0]/pdata_tgt['y'])**2)
                 errhi = np.sqrt((yerr_ref[1]/pdata_ref['y'])**2 + (yerr_tgt[1]/pdata_tgt['y'])**2)
                 pdata_comp['yerr'] = (errlo, errhi)
             else:
@@ -310,24 +323,20 @@
         combined_options = combine_dict(plot_options)
         if combined_options.get('markersize', None) is None:
             nbins = len(pdata_comp['x'])
             combined_options['markersize'] = suggest_markersize(nbins)
             
         draw_blind = blind_range is not None
         if draw_blind:
-            x = pdata_comp['x'][pdata_ref['sideband']]
-            y = pdata_comp['y'][pdata_ref['sideband']]
-            xerr = self._get_selected_err(pdata_comp['xerr'], pdata_ref['sideband'])
-            yerr = self._get_selected_err(pdata_comp['yerr'], pdata_ref['sideband'])
-        else:
-            x = pdata_comp['x']
-            y = pdata_comp['y']
-            xerr = pdata_comp['xerr']
-            yerr = pdata_comp['yerr']
-            
+            valid_mask &= pdata_ref['sideband']
+        x = pdata_comp['x'][valid_mask]
+        y = pdata_comp['y'][valid_mask]
+        xerr = self._get_selected_err(pdata_comp['xerr'], valid_mask)
+        yerr = self._get_selected_err(pdata_comp['yerr'], valid_mask)
+        
         if not show_error:
             error_format = None
         handle = self._draw_data(ax, x, y, xerr, yerr,
                                  plot_options=combined_options,
                                  error_format=error_format,
                                  error_styles=error_styles)
```

### Comparing `quickstats-0.6.7.8/quickstats/plots/sample_purity_plot.py` & `quickstats-0.6.8.1/quickstats/plots/sample_purity_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/score_distribution_plot.py` & `quickstats-0.6.8.1/quickstats/plots/score_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/stat_plot_config.py` & `quickstats-0.6.8.1/quickstats/plots/stat_plot_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/template.py` & `quickstats-0.6.8.1/quickstats/plots/template.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/test_statistic_distribution_plot.py` & `quickstats-0.6.8.1/quickstats/plots/test_statistic_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/upper_limit_1D_plot.py` & `quickstats-0.6.8.1/quickstats/plots/upper_limit_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/upper_limit_2D_plot.py` & `quickstats-0.6.8.1/quickstats/plots/upper_limit_2D_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -158,14 +158,15 @@
         if styles is None:
             styles = self.config['highlight_styles']
         handle = ax.plot(data['x'], data['y'], label=data['label'], **styles)
         self.update_legend_handles({'highlight': handle[0]}, idx=0)
         
     def draw_single_data(self, ax, data, scale_factor=None,
                          log:bool=False, 
+                         draw_expected:bool=True,
                          draw_observed:bool=True,
                          color_pallete:Optional[Dict]=None,
                          labels:Optional[Dict]=None,
                          sigma_band_hatch:Optional[str]=None,
                          draw_errorband:bool=True,
                          idx:int=0):
         
@@ -207,51 +208,56 @@
  
         if draw_observed:
             obs_limits = data['obs'].values * scale_factor
             handle_observed = draw_fn(indices, obs_limits, color=color_pallete['observed'], 
                                       label=labels['observed'], 
                                       **self.config["observed_plot_styles"])
             handles_map['observed'] = handle_observed[0]
-            
-        handle_expected = draw_fn(indices, exp_limits, color=color_pallete['expected'],
-                                  label=labels['expected'],
-                                  **self.config["expected_plot_styles"])
-        handles_map['expected'] = handle_expected[0]
+        
+        if draw_expected:
+            handle_expected = draw_fn(indices, exp_limits, color=color_pallete['expected'],
+                                      label=labels['expected'],
+                                      **self.config["expected_plot_styles"])
+            handles_map['expected'] = handle_expected[0]
 
         self.update_legend_handles(handles_map, idx=idx)
         
     def add_data(self, data:pd.DataFrame, color_pallete:Optional[Dict]=None,
-                 labels:Optional[Dict]=None, draw_observed:bool=False,
+                 labels:Optional[Dict]=None, draw_expected:bool=True,
+                 draw_observed:bool=False,
                  draw_errorband:bool=False):
         config = {
             "data": data,
             "color_pallete": combine_dict(self.COLOR_PALLETE_EXTRA, color_pallete),
             "labels": combine_dict(self.LABELS_EXTRA, labels),
             "draw_observed": draw_observed,
+            "draw_expected": draw_expected,
             "draw_errorband": draw_errorband
         }
         self.additional_data.append(config)
             
     def draw(self, xlabel:str="", ylabel:str="", ylim=None, xlim=None,
-             log:bool=False, draw_observed:bool=True, draw_errorband:bool=True,
+             log:bool=False, draw_expected:bool=True,
+             draw_observed:bool=True, draw_errorband:bool=True,
              draw_sec_errorband:bool=False, draw_hatch:bool=True):
         
         ax = self.draw_frame()
         
         if len(self.additional_data) > 0:
             if draw_hatch:
                 sigma_band_hatch = self.config['secondary_hatch']
                 alpha = self.config['secondary_alpha']
             else:
                 sigma_band_hatch = None
                 alpha = 1.
             for idx, config in enumerate(self.additional_data):
                 self.draw_single_data(ax, config["data"],
                                       scale_factor=self.scale_factor,
-                                      log=log, 
+                                      log=log,
+                                      draw_expected=config["draw_expected"],
                                       draw_observed=config["draw_observed"],
                                       color_pallete=config["color_pallete"],
                                       labels=config["labels"],
                                       sigma_band_hatch=sigma_band_hatch,
                                       draw_errorband=config["draw_errorband"],
                                       idx=idx + 1)
             if draw_hatch:
@@ -261,15 +267,16 @@
                 sigma_band_hatch = None
                 alpha = 1.
         else:
             sigma_band_hatch = None
             alpha = 1.
         self.draw_single_data(ax, self.data,
                               scale_factor=self.scale_factor,
-                              log=log, 
+                              log=log,
+                              draw_expected=draw_expected,
                               draw_observed=draw_observed,
                               color_pallete=self.color_pallete,
                               labels=self.labels,
                               sigma_band_hatch=sigma_band_hatch,
                               draw_errorband=draw_errorband,
                               idx=0)
```

### Comparing `quickstats-0.6.7.8/quickstats/plots/upper_limit_3D_plot.py` & `quickstats-0.6.8.1/quickstats/plots/upper_limit_3D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/upper_limit_benchmark_plot.py` & `quickstats-0.6.8.1/quickstats/plots/upper_limit_benchmark_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/plots/variable_distribution_plot.py` & `quickstats-0.6.8.1/quickstats/plots/variable_distribution_plot.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,54 +10,60 @@
 
 from quickstats.plots import AbstractPlot, get_color_cycle
 from quickstats.plots.template import ratio_frames, suggest_markersize, centralize_axis
 from quickstats.utils.common_utils import combine_dict
 from quickstats.maths.numerics import safe_div
 from quickstats.maths.statistics import (HistComparisonMode,
                                          min_max_to_range, get_hist_data,
+                                         get_stacked_hist_data,
                                          get_hist_comparison_data)
 
 from .core import PlotFormat, ErrorDisplayFormat
 
 class VariableDistributionPlot(AbstractPlot):
     
     COLOR_CYCLE = "simple_contrast"
     
     STYLES = {
+        "legend": {
+            "handletextpad": 0.3
+        },
         "hist": {
             'histtype' : 'step',
             'linestyle': '-'
         },
         "bar": {
             'linewidth' : 0,
             'alpha'     : 0.5
         },
         "fill_between": {
             'alpha' : 0.5
         },
         'errorbar': {
             "marker": 'o',
             "markersize": None,
+            'linestyle': 'none',
             "linewidth": 0,
             "elinewidth": 1,
-            "capsize": 3,
-            "capthick": 1
+            "capsize": 0,
+            "capthick": 0
         },        
     }
     
     CONFIG = {
         'ratio_line_styles':{
             'color': 'gray',
             'linestyle': '--',
             'zorder': 0
         },
         'plot_format': 'hist',
         'error_format': 'shade',
         'error_label_format': r'{label} $\pm \sigma$',
-        'show_xerr': True
+        'show_xerr': True,
+        'stacked_label': ':stacked_{index}:'
     }
     
     def __init__(self, data_map:Union["pandas.DataFrame", Dict[str, "pandas.DataFrame"]],
                  plot_options:Optional[Dict]=None,
                  label_map:Optional[Dict]=None,
                  color_cycle:Optional[Union[List, str, "ListedColorMap"]]=None,
                  styles:Optional[Union[Dict, str]]=None,
@@ -73,26 +79,41 @@
                 {<sample_name>: <pandas.DataFrame>}
             plot_options: dicionary
                 A dictionary containing the plot options for various group of samples.
                 It should be of the form
                 { <sample_group>:
                   {
                     "samples": <list of sample names>,
+                    "weight_scale": <scale factor>,
                     "styles" : <options in mpl.hist or mpl.errorbar>,
-                    "error_styles": <options in mpl.bar>
+                    "error_styles": <options in mpl.bar>,
+                    "plot_format": "hist" or "errorbar",
+                    "stack_index": <stack index>
                   }
                 }
                 where "styles" should match the options available in mpl.hist if
-                `plot_format` = "hist" or mpl.errorbar if `plot_format` = "errorbar";
+                `plot_format` = "hist" or mpl.errorbar if `plot_format` = "errorbar"
+                
+                (optional) "weight_scale" is used to scale the weights of the given
+                group of samples by the given factor
+                
                 "error_styles" should match the options available in mpl.errorbar if
-                `error_format` = "errorbar", mpl.bar if `plot_format` = "shade" or
+                `error_format` = "errorbar", mpl.bar if `error_format` = "shade" or
                 mpl.fill_between if `error_format` = "fill"
+                
+                (optional) "stack_index" is be used when multiple stacked plots are made;
+                sample groups with the same stack index will be stacked; this option
+                is only used when `plot_format` = "hist" and the draw method is called
+                with the `stack` option set to True; by default a stack index of 0 will
+                be assigned
+                
                 Note: If both `plot_format` and `error_format` are errorbar, "styles"
                 will be used instead of "error_styles" for the error styles.
                 
+                
         """
         self.load_data(data_map)
         self.plot_options = plot_options
         self.label_map = label_map
         super().__init__(color_cycle=color_cycle,
                          styles=styles,
                          analysis_label_options=analysis_label_options,
@@ -138,29 +159,47 @@
         for target in targets:
             options = combine_dict(plot_options.get(target, {}))
             # use default styles if not specified
             if 'styles' not in options:
                 options['styles'] = combine_dict(self.get_styles(plot_format.mpl_method))
             if 'color' not in options['styles']:
                 if color_i == n_colors:
-                    self.stdout.warning("WARNING: Number of targets is more than the number of colors "
+                    self.stdout.warning("Number of targets is more than the number of colors "
                                         "available in the color map. The colors will be repeated.")
                 options['styles']['color'] = colors[color_i % n_colors]
                 color_i += 1
             if 'label' not in options['styles']:
-                options['styles']['label'] = label_map.get(target, target)
+                label = label_map.get(target, target)
+                if label is None:
+                    label = 'None'
+                options['styles']['label'] = label
             if 'samples' not in options:
                 options['samples'] = [target]
             if 'error_styles' not in options:
                 options['error_styles'] = combine_dict(self.get_styles(error_format.mpl_method))
             if 'color' not in options['error_styles']:
                 options['error_styles']['color'] = options['styles']['color']
             if 'label' not in options['error_styles']:
                 fmt = self.config['error_label_format']
                 options['error_styles']['label'] = fmt.format(label=options['styles']['label'])
+            if 'plot_format' not in options:
+                options['plot_format'] = PlotFormat.parse(self.config['plot_format'])
+            else:
+                options['plot_format'] = PlotFormat.parse(options['plot_format'])
+            if 'error_format' not in options:
+                if options['plot_format'] == PlotFormat.ERRORBAR:
+                    options['error_format'] = ErrorDisplayFormat.ERRORBAR
+                else:
+                    options['error_format'] = ErrorDisplayFormat.parse(self.config['error_format'])
+            else:
+                options['error_format'] = ErrorDisplayFormat.parse(options['error_format'])
+            if 'stack_index' not in options:
+                options['stack_index'] = 0
+            if 'weight_scale' not in options:
+                options['weight_scale'] = None
             final_plot_options[target] = options
         return final_plot_options
     
     def resolve_comparison_options(self, comparison_options:Optional[Dict]=None,
                                    plot_options:Optional[Dict]=None):
         if comparison_options is None:
             return None
@@ -210,27 +249,28 @@
             component['mode'] = comparison_options['mode']
         comparison_options['components'] = components
         return comparison_options
     
     def decorate_comparison_axis(self, ax, xlabel:str="", ylabel:str="", 
                                  mode:Union[HistComparisonMode, str]="ratio",
                                  ylim:Optional[Sequence]=None,
+                                 ypad:Optional[float]=0.1,
                                  draw_ratio_line:bool=True):
         mode = HistComparisonMode.parse(mode)
         if ylim is not None:
             ax.set_ylim(ylim)
         do_centralize_axis = ylim is None
         if mode == HistComparisonMode.RATIO:
             if do_centralize_axis:
-                centralize_axis(ax, which="y", ref_value=1)
+                centralize_axis(ax, which="y", ref_value=1, padding=ypad)
             if draw_ratio_line:
                 ax.axhline(1, **self.config['ratio_line_styles'])
         elif mode == HistComparisonMode.DIFFERENCE:
             if do_centralize_axis:
-                centralize_axis(ax, which="y", ref_value=0)
+                centralize_axis(ax, which="y", ref_value=0, padding=ypad)
             if draw_ratio_line:
                 ax.axhline(0, **self.config['ratio_line_styles'])
         # set default ylabel if not given
         if not ylabel:
             if mode == HistComparisonMode.RATIO:
                 ylabel = "Ratio"
             elif mode == HistComparisonMode.DIFFERENCE:
@@ -265,54 +305,109 @@
         if ylim[1] < np.max(y):
             ylim[1] = np.max(y)
         ax.set_ylim(ylim)
         
         return handle, error_handle
     
     def deduce_bin_range(self, samples:List[str], column_name:str,
-                         rescale_by:Optional[float]=None):
+                         variable_scale:Optional[float]=None):
         xmin = None
         xmax = None
         for sample in samples:
             df = self.data_map[sample]
             x = df[column_name].values
-            if rescale_by is not None:
-                x = x * rescale_by
+            if variable_scale is not None:
+                x = x * variable_scale
             if xmin is None:
                 xmin = np.min(x)
             else:
                 xmin = min(xmin, np.min(x))
             if xmax is None:
                 xmax = np.max(x)
             else:
                 xmax = min(xmax, np.max(x))
         return (xmin, xmax)
     
     def get_sample_data(self, samples:List[str],
                         column_name:str,
-                        rescale_by:Optional[float]=None,
+                        variable_scale:Optional[float]=None,
+                        weight_scale:Optional[float]=None,
                         weight_name:Optional[str]=None):
         df = pd.concat([self.data_map[sample] for sample in samples], ignore_index=True)
         x = df[column_name].values
-        if rescale_by is not None:
-            x = x * rescale_by
+        if variable_scale is not None:
+            x = x * variable_scale
         if weight_name is not None:
             weights = df[weight_name]
         else:
             weights = np.ones(x.shape)
+        if weight_scale is not None:
+            weights = weights * weight_scale            
         return x, weights
     
+    def draw_stacked(self, ax, plot_options:Dict,
+                     column_name:str, weight_name:Optional[str]=None,
+                     bins:Union[int, Sequence]=25,
+                     bin_range:Optional[Sequence]=None,
+                     normalize:bool=True,
+                     show_error:bool=False,
+                     variable_scale:Optional[float]=None):
+        stacked_data = {
+            'x'       : [],
+            'weights' : [],
+            'color'   : [],
+            'label'   : [],
+        }
+
+        stacked_styles = []
+        for target, options in plot_options.items():
+            samples, styles = options['samples'], options['styles']
+            label, color = styles['label'], styles['color']
+            weight_scale = options['weight_scale']
+            x, weights = self.get_sample_data(samples, column_name,
+                                              variable_scale=variable_scale,
+                                              weight_scale=weight_scale,
+                                              weight_name=weight_name)
+            stacked_data['x'].append(x)
+            stacked_data['weights'].append(weights)
+            stacked_data['color'].append(color)
+            stacked_data['label'].append(label)
+            stacked_styles.append(styles)
+        if normalize:
+            norm_factor = np.sum([np.sum(weights) for weights in stacked_data['weights']])
+            stacked_data['weights'] = [weights / norm_factor for weights in stacked_data['weights']]
+        stacked_styles = {k:v for k,v in stacked_styles[0].items() if k not in ['color', 'label']}
+        hist_y, bin_edges, handle = ax.hist(**stacked_data,
+                                            bins=bins,
+                                            range=bin_range,
+                                            stacked=True,
+                                            **stacked_styles)
+        for i, target in enumerate(plot_options):
+            self.update_legend_handles({target:handle[i]})
+        bin_edges = np.histogram_bin_edges(np.concatenate(stacked_data['x']).flatten(),
+                                           bins=bins, range=bin_range)
+        hist_data = get_stacked_hist_data(stacked_data['x'], stacked_data['weights'],
+                                          normalize=normalize,
+                                          bin_range=bin_range, bins=bins,
+                                          clip_weight=False,
+                                          xerr=show_error and self.config['show_xerr'],
+                                          yerr=show_error,
+                                          error_option='auto')
+        return bin_edges, hist_data
+            
     def draw(self, column_name:str, weight_name:Optional[str]=None,
              targets:Optional[List[str]]=None,
              xlabel:str="", ylabel:str="Fraction of Events / {bin_width:.2f}",
              bins:Union[int, Sequence]=25, bin_range:Optional[Sequence]=None,
              normalize:bool=True, show_error:bool=False, show_error_legend:bool=False,
              stacked:bool=False, xmin:Optional[float]=None, xmax:Optional[float]=None,
-             ypad:float=0.3, rescale_by:Optional[float]=None, logy:bool=False,
-             comparison_options:Optional[Union[Dict, List[Dict]]]=None):
+             ymin:Optional[float]=None, ymax:Optional[float]=None, ypad:float=0.3,
+             variable_scale:Optional[float]=None, logy:bool=False,
+             comparison_options:Optional[Union[Dict, List[Dict]]]=None,
+             legend_order:Optional[List[str]]=None):
         """
         
         Arguments:
             column_name: string
                 Name of the variable in the dataframe(s).
             weight_name: (optional) string
                 If specified, weight the histogram by the "weight_name" variable
@@ -338,129 +433,131 @@
                 Whether to display data error.
             show_error_legend: bool, default = False
                 Whether to include legend for the error artists.
             xmin: (optional) float
                 Minimum range of x-axis.
             xmax: (optional) float
                 Maximum range of x-axis.
+            ymin: (optional) float
+                Minimum range of y-axis.
+            ymax: (optional) float
+                Maximum range of y-axis.
             ypad: float, default = 0.4
-                Fraction of the y-axis that should be padded.
-            rescale_by: (optional) float
+                Fraction of the y-axis that should be padded. This options will be
+                ignored if ymax is set.
+            variable_scale: (optional) float
                 Rescale variable values by a factor.
             logy: bool, default = False
                 Use log scale for y-axis.
             comparison_options: (optional) dict or list of dict
                 One or multiple dictionaries containing instructions on
-                making comparison plots.                
+                making comparison plots.
+            legend_order: (optional) list of str
+                Order of legend labels. The same order as targets will be used by default.
         """
         plot_options = self.resolve_plot_options(self.plot_options, targets=targets)
         comparison_options = self.resolve_comparison_options(comparison_options,
                                                              plot_options)
-        plot_format  = PlotFormat.parse(self.config['plot_format'])
-        error_format = ErrorDisplayFormat.parse(self.config['error_format'])
+        if legend_order is not None:
+            self.legend_order = list(legend_order)
+        else:
+            self.legend_order = list(plot_options)
+        if show_error_legend and (not stacked):
+            self.legend_order.extend([f"{target}_error" for target in self.legend_order])
+                
         if comparison_options is not None:
             ax, ax_ratio = self.draw_frame(ratio_frames, logy=logy,
                                            **self.styles["ratio_frames"])
         else:
             ax = self.draw_frame(logy=logy)
         if bin_range is None:
             relevant_samples = [sample for options in plot_options.values() \
                                 for sample in options['samples']]
-            bin_range = self.deduce_bin_range(relevant_samples, column_name, rescale_by=rescale_by)
-            self.stdout.info(f"INFO: Using deduced bin range ({bin_range[0]:.3f}, {bin_range[1]:.3f})")
+            bin_range = self.deduce_bin_range(relevant_samples, column_name, variable_scale=variable_scale)
+            self.stdout.info(f"Using deduced bin range ({bin_range[0]:.3f}, {bin_range[1]:.3f})")
+
+        binned_data   = {}
+        target_bin_edges = {}
+        
+        stacked_plot_options = {}
         if stacked:
-            if plot_format != PlotFormat.HIST:
-                raise RuntimeError('stacked plot is only available for hist format')
-            if show_error:
-                self.stdout.warning('WARNING: No error will be drawn for stacked plot')
-            stack_x = []
-            stack_weight = []
-            stack_color = []
-            stack_label = []
-            stack_styles = []
-            for target, options in plot_options.items():
-                samples, styles = options['samples'], options['styles']
-                label, color = styles['label'], styles['color']
-                x, weights = self.get_sample_data(samples, column_name,
-                                                  rescale_by=rescale_by,
-                                                  weight_name=weight_name)
-                stack_x.append(x)
-                stack_weight.append(weights)
-                stack_color.append(color)
-                stack_label.append(label)
-                stack_styles.append(styles)
-            if normalize:
-                norm_factor = np.sum([np.sum(weights) for weights in stack_weight])
-                stack_weight = [weights / norm_factor for weights in stack_weight]
-            styles = {k:v for k,v in stack_styles[0].items() if k not in ['color', 'label']}
-            hist_y, bin_edges, handle = ax.hist(stack_x, bins, range=bin_range,
-                                                weights=stack_weight,
-                                                color=stack_color,
-                                                label=stack_label,
-                                                stacked=True,
-                                                **styles)
-            binned_data = None
-            target_bin_edges = None
-            for i, target in enumerate(plot_options):
-                self.update_legend_handles({target:handle[i]})
-        else:
-            binned_data   = {}
-            target_bin_edges = {}
-            for target, options in plot_options.items():
-                samples, styles, error_styles = options['samples'], options['styles'], options['error_styles']
-                label = styles['label']
-                x, weights = self.get_sample_data(samples, column_name,
-                                                  rescale_by=rescale_by,
-                                                  weight_name=weight_name)
-                bin_edges = np.histogram_bin_edges(x, bins=bins, range=bin_range)
-                hist_data = get_hist_data(x, weights, normalize=normalize,
-                                          bin_range=bin_range, bins=bins,
-                                          clip_weight=False,
-                                          xerr=show_error and self.config['show_xerr'],
-                                          yerr=show_error,
-                                          error_option='auto')
-                binned_data[target] = hist_data
-                target_bin_edges[target] = bin_edges
-                if plot_format == PlotFormat.HIST:
-                    if normalize:
-                        weights /= weights.sum()
-                    hist_y, _, handle = ax.hist(x, bins, range=bin_range,
-                                                weights=weights, **styles)
-                    assert np.allclose(hist_data['y'], hist_y)
-                    _, error_handle = self.draw_binned_data(ax, hist_data,
-                                                            bin_edges=bin_edges,
-                                                            draw_data=False,
-                                                            draw_error=show_error,
-                                                            error_format=error_format,
-                                                            error_styles=error_styles)
-                elif plot_format == PlotFormat.ERRORBAR:
-                    handle, error_handle = self.draw_binned_data(ax, hist_data,
-                                                                 bin_edges=bin_edges,
-                                                                 styles=styles,
-                                                                 draw_error=show_error,
-                                                                 error_format=error_format,
-                                                                 error_styles=error_styles)
-                self.update_legend_handles({target:handle})
-                if error_handle is not None:
-                    self.update_legend_handles({f"{target}_error": error_handle})
+            stack_targets = [target for target, options in plot_options.items() if \
+                             options['plot_format'] == PlotFormat.HIST]
+            if not stack_targets:
+                raise RuntimeError('no histograms to be stacked')
+            for target in stack_targets:
+                options = plot_options.pop(target)
+                stack_index = options['stack_index']
+                if stack_index not in stacked_plot_options:
+                    stacked_plot_options[stack_index] = {}
+                stacked_plot_options[stack_index][target] = options
+            for stack_index, stacked_plot_options_i in stacked_plot_options.items():
+                bin_edges, hist_data = self.draw_stacked(ax, stacked_plot_options_i,
+                                                         column_name=column_name,
+                                                         weight_name=weight_name,
+                                                         bins=bins, bin_range=bin_range,
+                                                         normalize=normalize,
+                                                         variable_scale=variable_scale)
+                label = self.config['stacked_label'].format(index=stack_index)
+                binned_data[label] = hist_data
+                target_bin_edges[label] = bin_edges
+
+        for target, options in plot_options.items():
+            samples, styles, error_styles = options['samples'], options['styles'], options['error_styles']
+            label = styles['label']
+            weight_scale = options['weight_scale']
+            plot_format, error_format = options['plot_format'], options['error_format']
+            x, weights = self.get_sample_data(samples, column_name,
+                                              variable_scale=variable_scale,
+                                              weight_scale=weight_scale,
+                                              weight_name=weight_name)
+            bin_edges = np.histogram_bin_edges(x, bins=bins, range=bin_range)
+            hist_data = get_hist_data(x, weights, normalize=normalize,
+                                      bin_range=bin_range, bins=bins,
+                                      clip_weight=False,
+                                      xerr=show_error and self.config['show_xerr'],
+                                      yerr=show_error,
+                                      error_option='auto')
+            binned_data[target] = hist_data
+            target_bin_edges[target] = bin_edges
+            if plot_format == PlotFormat.HIST:
+                if normalize:
+                    weights /= weights.sum()
+                hist_y, _, handle = ax.hist(x, bins, range=bin_range,
+                                            weights=weights, **styles)
+                assert np.allclose(hist_data['y'], hist_y)
+                _, error_handle = self.draw_binned_data(ax, hist_data,
+                                                        bin_edges=bin_edges,
+                                                        draw_data=False,
+                                                        draw_error=show_error,
+                                                        error_format=error_format,
+                                                        error_styles=error_styles)
+            elif plot_format == PlotFormat.ERRORBAR:
+                handle, error_handle = self.draw_binned_data(ax, hist_data,
+                                                             bin_edges=bin_edges,
+                                                             styles=styles,
+                                                             draw_error=show_error,
+                                                             error_format=error_format,
+                                                             error_styles=error_styles)
+            self.update_legend_handles({target:handle})
+            if error_handle is not None:
+                self.update_legend_handles({f"{target}_error": error_handle})
                     
         # propagate bin width to ylabel if needed
         if isinstance(bins, int):
             bin_width = (bin_range[1] - bin_range[0]) / bins
             ylabel = ylabel.format(bin_width=bin_width)
         
         self.draw_axis_components(ax, xlabel=xlabel, ylabel=ylabel)
-        self.set_axis_range(ax, xmin=xmin, xmax=xmax, ypad=ypad)
-
-        if not self.legend_order:
-            self.legend_order = list(plot_options)
-            if show_error_legend and (not stacked):
-                self.legend_order.extend([f"{target}_error" for target in self.legend_order])
-        handles, labels = self.get_legend_handles_labels()
-        ax.legend(handles=handles, labels=labels, **self.styles['legend'])
+        self.set_axis_range(ax, xmin=xmin, xmax=xmax,
+                            ymin=ymin, ymax=ymax, ypad=ypad)
+                
+        if not self.is_single_data():
+            handles, labels = self.get_legend_handles_labels()
+            ax.legend(handles=handles, labels=labels, **self.styles['legend'])
         
         if comparison_options is not None:
             components = comparison_options.pop('components')
             for component in components:
                 reference = component.pop('reference')
                 target    = component.pop('target')
                 bin_edges = target_bin_edges[target]
```

### Comparing `quickstats-0.6.7.8/quickstats/root_checker.py` & `quickstats-0.6.8.1/quickstats/root_checker.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/utils/common_utils.py` & `quickstats-0.6.8.1/quickstats/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/utils/data_conversion.py` & `quickstats-0.6.8.1/quickstats/utils/data_conversion.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/utils/hep_utils.py` & `quickstats-0.6.8.1/quickstats/utils/hep_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/utils/roofit_utils.py` & `quickstats-0.6.8.1/quickstats/utils/roofit_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -580,8 +580,22 @@
     raise ValueError(f'invalid output format "{fmt}" (choose between "dict" or "pandas")')
     
 def get_gaussian_pdf_attributes(pdfs:"ROOT.RooArgSet", fmt:str="pandas"):
     return get_pdf_attributes(pdfs, ["X", "Mean", "Sigma"], ROOT.RooGaussian, fmt=fmt)
 
 def get_poisson_pdf_attributes(pdfs:"ROOT.RooArgSet", fmt:str="pandas"):
     return get_pdf_attributes(pdfs, ["X", "Mean"], pdf_class=ROOT.RooPoisson, fmt=fmt)
-    
+    
+    
+def get_sim_pdf_ndof(pdf:"ROOT.RooSimultaneous", observables:"ROOT.RooArgSet", exclude_syst:bool=True):
+    import ROOT
+    if not isinstance(pdf, ROOT.RooSimultaneous):
+        raise RuntimeError('not a simultaneous pdf')
+    params = pdf.getVariables()
+    nuis_pdf = ROOT.RooStats.MakeNuisancePdf(pdf, observables, "nuisancePdf")
+    ndof = 0
+    for param in params:
+        param_name = param.GetName()
+        if ((not param.isConstant()) and (not observables.find(param_name))
+            and (exclude_syst and not nuis_pdf.dependsOn(ROOT.RooArgSet(param)))):
+            ndof += 1
+    return ndof
```

### Comparing `quickstats-0.6.7.8/quickstats/utils/roostats_utils.py` & `quickstats-0.6.8.1/quickstats/utils/roostats_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats/utils/root_utils.py` & `quickstats-0.6.8.1/quickstats/utils/root_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,27 +272,27 @@
     for source_file in source_files:
         files = glob.glob(source_file)
         if not files:
             raise FileNotFoundError(f"file \"{source_file}\" does not exist")
         rfiles += files
     # now all rfiles are guaranteed to exist
     for i, rfile in enumerate(rfiles):
-        stdout.info(f"Source {i+1}: {rfile}")
+        stdout.info(f"Source {i+1}: {rfile}", bare=True)
         if is_corrupt(rfile):
             raise RuntimeError(f"the root file \"{rfile}\" is corrupted")
     if not rfiles:
         raise RuntimeError("no source files found")
     if treename is None:
         f = ROOT.TFile(rfiles[0])
         treenames = get_tree_names(f)
         if len(treenames) > 1:
             raise RuntimeError("unable to deduce tree name from source files: "
                                "multiple trees are present")
         treename = treenames[0]
-        stdout.info("INFO: No tree name specified for merging. Will use "
+        stdout.info("No tree name specified for merging. Will use "
                     f"the auto-detected tree name \"{treename}\".")
         
     # configure multi-threading setting
     multithread_orig_state = ROOT.IsImplicitMTEnabled()
     if multithread and (not multithread_orig_state) and (not keep_order):
         ROOT.EnableImplicitMT()
     if keep_order and multithread_orig_state:
@@ -305,27 +305,27 @@
             rdf = ROOT.RDataFrame(treename, rfile)
             columns = set([str(i) for i in rdf.GetColumnNames()])
             all_columns.update(columns)
             column_map[rfile] = columns
         for fname, columns in column_map.items():
             if columns != all_columns:
                 missing_columns = list(all_columns - columns)
-                stdout.warning(f"WARNING: The root file \"{rfile}\" is missing the following column(s): "
+                stdout.warning(f"The root file \"{rfile}\" is missing the following column(s): "
                                f"{','.join(missing_columns)}. The missing column(s) will not be saved.")
         columns_to_keep = list(set.intersection(*column_map.values()))
         rdf = ROOT.RDataFrame(treename, rfiles)
-        stdout.info(f"Target path: {target_file}")
+        stdout.info(f"Target path: {target_file}", bare=True)
         if use_template:
             snapshot = templated_rdf_snapshot(rdf, columns_to_keep)
         else:
             snapshot = rdf.Snapshot
         snapshot(treename, target_file, columns_to_keep)
     else:
         rdf = ROOT.RDataFrame(treename, rfiles)
-        stdout.info(f"Target path: {target_file}")
+        stdout.info(f"Target path: {target_file}", bare=True)
         if use_template:
             snapshot = templated_rdf_snapshot(rdf, columns_to_keep)
         else:
             snapshot = rdf.Snapshot
         snapshot(treename, target_file)
    
     # restore multi-threading setting
```

### Comparing `quickstats-0.6.7.8/quickstats/utils/string_utils.py` & `quickstats-0.6.8.1/quickstats/utils/string_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional, Callable
 import re
 
 whitespace_trans = str.maketrans('', '', " \t\r\n\v")
+newline_trans = str.maketrans('', '', "\r\n")
 
 def split_lines(string:str, comment_string:Optional[str]="#", remove_blank:bool=True,
                 with_line_number:bool=False, keepends:bool=False):
     lines = string.splitlines(keepends=keepends)
     # remove comments
     lines = [l.split(comment_string)[0] for l in lines]
     # remove blank lines
@@ -28,8 +29,11 @@
         # remove empty tokens
         tokens = [s for s in tokens if s]
     if cast is not None:
         tokens = [cast(s) for s in tokens]
     return tokens
 
 def remove_whitespace(string:str):
-    return string.translate(whitespace_trans)
+    return string.translate(whitespace_trans)
+
+def remove_newline(string:str):
+    return string.translate(newline_trans)
```

### Comparing `quickstats-0.6.7.8/quickstats/utils/xml_tools.py` & `quickstats-0.6.8.1/quickstats/utils/xml_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.7.8/quickstats.egg-info/PKG-INFO` & `quickstats-0.6.8.1/quickstats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.7.8
+Version: 0.6.8.1
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.7.8/quickstats.egg-info/SOURCES.txt` & `quickstats-0.6.8.1/quickstats.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 quickstats/components/processors/actions/rooproc_filter.py
 quickstats/components/processors/actions/rooproc_global_variables.py
 quickstats/components/processors/actions/rooproc_helper_action.py
 quickstats/components/processors/actions/rooproc_hybrid_action.py
 quickstats/components/processors/actions/rooproc_if_defined.py
 quickstats/components/processors/actions/rooproc_if_not_defined.py
 quickstats/components/processors/actions/rooproc_load_frame.py
+quickstats/components/processors/actions/rooproc_load_macro.py
 quickstats/components/processors/actions/rooproc_max.py
 quickstats/components/processors/actions/rooproc_mean.py
 quickstats/components/processors/actions/rooproc_min.py
 quickstats/components/processors/actions/rooproc_nested_action.py
 quickstats/components/processors/actions/rooproc_rdf_action.py
 quickstats/components/processors/actions/rooproc_redefine.py
 quickstats/components/processors/actions/rooproc_report.py
@@ -94,14 +95,15 @@
 quickstats/components/workspaces/asimov_handler.py
 quickstats/components/workspaces/core_argument_sets.py
 quickstats/components/workspaces/sample.py
 quickstats/components/workspaces/settings.py
 quickstats/components/workspaces/systematic.py
 quickstats/components/workspaces/systematics_domain.py
 quickstats/components/workspaces/ws_comparer.py
+quickstats/components/workspaces/ws_decomposer.py
 quickstats/components/workspaces/ws_modifier_config.py
 quickstats/components/workspaces/xml_ws_base.py
 quickstats/components/workspaces/xml_ws_builder_v1.py
 quickstats/components/workspaces/xml_ws_builder_v2.py
 quickstats/components/workspaces/xml_ws_combiner.py
 quickstats/components/workspaces/xml_ws_modifier.py
 quickstats/concurrent/__init__.py
```

### Comparing `quickstats-0.6.7.8/setup.py` & `quickstats-0.6.8.1/setup.py`

 * *Files identical despite different names*

