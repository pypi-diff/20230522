# Comparing `tmp/snowflake_cli_labs-0.2.8.tar.gz` & `tmp/snowflake_cli_labs-0.2.9.tar.gz`

## Comparing `snowflake_cli_labs-0.2.8.tar` & `snowflake_cli_labs-0.2.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/LEGAL.md
--rw-r--r--   0        0        0    11607 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/README.md
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/requirements-dev.txt
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/requirements.txt
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/snowcli.spec
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/tox.ini
--rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/docs/images/coverage_1.png
--rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/docs/images/coverage_2.png
--rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/docs/images/coverage_3.png
--rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/docs/images/coverage_4.png
--rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/docs/images/coverage_5.png
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/__init__.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/config.py
--rw-r--r--   0        0        0    16558 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/snow_connector.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/snowsql_config.py
--rw-r--r--   0        0        0    21769 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/utils.py
--rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/__init__.py
--rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/connection.py
--rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/function.py
--rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/package.py
--rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/procedure.py
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/render.py
--rw-r--r--   0        0        0    20029 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/snowpark_shared.py
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/sql.py
--rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/stage.py
--rw-r--r--   0        0        0    10105 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/streamlit.py
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/warehouse.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/procedure_coverage/__init__.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/procedure_coverage/clear.py
--rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/cli/procedure_coverage/report.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/python_templates/environment.yml.jinja
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/python_templates/snowpark_coverage.py.jinja
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/python_templates/streamlit_app_launcher.py.jinja
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/call_procedure.sql
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/create_function.sql
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/create_procedure.sql
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/create_stage.sql
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/create_streamlit.sql
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/describe_function.sql
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/describe_procedure.sql
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/describe_streamlit.sql
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/drop_function.sql
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/drop_procedure.sql
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/drop_stage.sql
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/drop_streamlit.sql
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/execute_function.sql
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/get_stage.sql
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/get_streamlit_url.sql
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/list_functions.sql
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/list_procedures.sql
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/list_stage.sql
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/list_stages.sql
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/list_streamlits.sql
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/put_stage.sql
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/remove_from_stage.sql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/set_procedure_comment.sql
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/share_streamlit.sql
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/snowcli/sql/show_warehouses.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_function/.gitignore
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_function/app.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_function/app.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_function/requirements.txt
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_procedure/.gitignore
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_procedure/app.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_procedure/app.toml
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_procedure/local_connection.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/src/templates/default_procedure/requirements.txt
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/tests/conftest.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/tests/test_main.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/tests/test_render.py
--rw-r--r--   0        0        0    14849 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/tests/test_snow_connector.py
--rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/tests/test_sql.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/tests/__snapshots__/test_snow_connector.ambr
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/LICENSE
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/LEGAL.md
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/requirements-dev.txt
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/requirements.txt
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/snowcli.spec
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/tox.ini
+-rw-r--r--   0        0        0    13022 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/docs/images/coverage_1.png
+-rw-r--r--   0        0        0    24318 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/docs/images/coverage_2.png
+-rw-r--r--   0        0        0    12852 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/docs/images/coverage_3.png
+-rw-r--r--   0        0        0    24441 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/docs/images/coverage_4.png
+-rw-r--r--   0        0        0    14955 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/docs/images/coverage_5.png
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/__init__.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/config.py
+-rw-r--r--   0        0        0    16911 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/snow_connector.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/snowsql_config.py
+-rw-r--r--   0        0        0    21769 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/utils.py
+-rw-r--r--   0        0        0     4270 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/__init__.py
+-rw-r--r--   0        0        0     2256 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/connection.py
+-rw-r--r--   0        0        0     6362 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/function.py
+-rw-r--r--   0        0        0     5199 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/package.py
+-rw-r--r--   0        0        0     7118 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/procedure.py
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/render.py
+-rw-r--r--   0        0        0    20029 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/snowpark_shared.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/sql.py
+-rw-r--r--   0        0        0     4630 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/stage.py
+-rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/streamlit.py
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/warehouse.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/procedure_coverage/__init__.py
+-rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/procedure_coverage/clear.py
+-rw-r--r--   0        0        0     5797 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/cli/procedure_coverage/report.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/python_templates/environment.yml.jinja
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/python_templates/snowpark_coverage.py.jinja
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/python_templates/streamlit_app_launcher.py.jinja
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/call_procedure.sql
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/create_function.sql
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/create_procedure.sql
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/create_stage.sql
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/create_streamlit.sql
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/describe_function.sql
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/describe_procedure.sql
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/describe_streamlit.sql
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/drop_function.sql
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/drop_procedure.sql
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/drop_stage.sql
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/drop_streamlit.sql
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/execute_function.sql
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/get_stage.sql
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/get_streamlit_url.sql
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/list_functions.sql
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/list_procedures.sql
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/list_stage.sql
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/list_stages.sql
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/list_streamlits.sql
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/put_stage.sql
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/remove_from_stage.sql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/set_procedure_comment.sql
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/share_streamlit.sql
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/snowcli/sql/show_warehouses.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/__init__.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_function/.gitignore
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_function/app.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_function/app.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_function/requirements.txt
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_procedure/.gitignore
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_procedure/app.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_procedure/app.toml
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_procedure/local_connection.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/src/templates/default_procedure/requirements.txt
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/tests/conftest.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/tests/test_main.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/tests/test_render.py
+-rw-r--r--   0        0        0    15880 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/tests/test_snow_connector.py
+-rw-r--r--   0        0        0     3329 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/tests/test_sql.py
+-rw-r--r--   0        0        0     7104 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/tests/__snapshots__/test_snow_connector.ambr
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/LICENSE
+-rw-r--r--   0        0        0    11607 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/README.md
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    12603 2020-02-02 00:00:00.000000 snowflake_cli_labs-0.2.9/PKG-INFO
```

### Comparing `snowflake_cli_labs-0.2.8/.pre-commit-config.yaml` & `snowflake_cli_labs-0.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/README.md` & `snowflake_cli_labs-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/snowcli.spec` & `snowflake_cli_labs-0.2.9/snowcli.spec`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/docs/images/coverage_1.png` & `snowflake_cli_labs-0.2.9/docs/images/coverage_1.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/docs/images/coverage_2.png` & `snowflake_cli_labs-0.2.9/docs/images/coverage_2.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/docs/images/coverage_3.png` & `snowflake_cli_labs-0.2.9/docs/images/coverage_3.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/docs/images/coverage_4.png` & `snowflake_cli_labs-0.2.9/docs/images/coverage_4.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/docs/images/coverage_5.png` & `snowflake_cli_labs-0.2.9/docs/images/coverage_5.png`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/config.py` & `snowflake_cli_labs-0.2.9/src/snowcli/config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/snow_connector.py` & `snowflake_cli_labs-0.2.9/src/snowcli/snow_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,22 @@
 from snowflake.connector.cursor import SnowflakeCursor
 
 from snowcli.snowsql_config import SnowsqlConfig
 
 TEMPLATES_PATH = Path(__file__).parent / "sql"
 
 
+def get_standard_stage_name(name: str) -> str:
+    # Handle embedded stages
+    if name.startswith("snow://"):
+        return name
+
+    return f"@{name}"
+
+
 class SnowflakeConnector:
     """Initialize a connection from a snowsql-formatted config"""
 
     def __init__(
         self,
         snowsql_config: SnowsqlConfig,
         connection_name: str,
@@ -272,14 +280,16 @@
         database,
         schema,
         role,
         warehouse,
         name,
         like="%%",
     ) -> SnowflakeCursor:
+        name = get_standard_stage_name(name)
+
         return self.runSql(
             "list_stage",
             {
                 "database": database,
                 "schema": schema,
                 "role": role,
                 "warehouse": warehouse,
@@ -293,14 +303,16 @@
         database,
         schema,
         role,
         warehouse,
         name,
         path,
     ) -> SnowflakeCursor:
+        name = get_standard_stage_name(name)
+
         return self.runSql(
             "get_stage",
             {
                 "database": database,
                 "schema": schema,
                 "role": role,
                 "warehouse": warehouse,
@@ -343,14 +355,16 @@
         role,
         warehouse,
         name,
         path,
         overwrite: bool = False,
         parallel: int = 4,
     ) -> SnowflakeCursor:
+        name = get_standard_stage_name(name)
+
         return self.runSql(
             "put_stage",
             {
                 "database": database,
                 "schema": schema,
                 "role": role,
                 "warehouse": warehouse,
@@ -360,14 +374,16 @@
                 "parallel": parallel,
             },
         )
 
     def removeFromStage(
         self, database, schema, role, warehouse, name, path
     ) -> SnowflakeCursor:
+        name = get_standard_stage_name(name)
+
         return self.runSql(
             "remove_from_stage",
             {
                 "database": database,
                 "schema": schema,
                 "role": role,
                 "warehouse": warehouse,
@@ -510,24 +526,26 @@
         self,
         database="",
         schema="",
         role="",
         warehouse="",
         name="",
         file="",
+        from_stage_command="",
     ) -> SnowflakeCursor:
         return self.runSql(
             "create_streamlit",
             {
                 "database": database,
                 "schema": schema,
                 "role": role,
                 "warehouse": warehouse,
                 "name": name,
                 "file_name": file,
+                "from_stage_command": from_stage_command,
             },
         )
 
     def shareStreamlit(
         self,
         database="",
         schema="",
@@ -551,45 +569,42 @@
     def dropStreamlit(
         self,
         database="",
         schema="",
         role="",
         warehouse="",
         name="",
-        drop_stage: bool = True,
     ) -> SnowflakeCursor:
-
-        drop_command = f'drop stage "{name}_STAGE";' if drop_stage else ""
-
         return self.runSql(
             "drop_streamlit",
             {
                 "database": database,
                 "schema": schema,
                 "role": role,
                 "warehouse": warehouse,
                 "name": name,
-                "drop_command": drop_command,
             },
         )
 
     def deployStreamlit(
         self,
         name,
         file_path,
         stage_path,
         role,
         database,
         schema,
         overwrite,
     ):
+        stage_name = f"snow://streamlit/{database}.{schema}.{name}/default_checkout"
+
         """Upload main python file to stage and return url of streamlit"""
         self.uploadFileToStage(
             file_path,
-            f"{name}_stage",
+            stage_name,
             stage_path,
             role,
             database,
             schema,
             overwrite,
         )
 
@@ -629,15 +644,14 @@
 
     def runSql(
         self,
         command,
         context,
         show_exceptions=True,
     ) -> SnowflakeCursor:
-
         env = Environment(loader=FileSystemLoader(TEMPLATES_PATH))
         template = env.get_template(f"{command}.sql")
         sql = template.render(**context)
         try:
             if os.getenv("DEBUG"):
                 print(f"Executing sql:\n{sql}")
             results = self.ctx.execute_stream(StringIO(sql))
```

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/snowsql_config.py` & `snowflake_cli_labs-0.2.9/src/snowcli/snowsql_config.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/utils.py` & `snowflake_cli_labs-0.2.9/src/snowcli/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/cli/__init__.py` & `snowflake_cli_labs-0.2.9/src/snowcli/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/cli/connection.py` & `snowflake_cli_labs-0.2.9/src/snowcli/cli/connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/cli/function.py` & `snowflake_cli_labs-0.2.9/src/snowcli/cli/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         "--return-type",
         "-r",
         help="Return type",
     ),
     replace: bool = typer.Option(
         False,
         "--replace-always",
-        "-r",
+        "-a",
         help="Replace function, even if no detected changes to metadata",
     ),
 ):
     snowpark_package(
         pypi_download,  # type: ignore[arg-type]
         check_anaconda_for_pypi_deps,
         package_native_libraries,  # type: ignore[arg-type]
```

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/cli/package.py` & `snowflake_cli_labs-0.2.9/src/snowcli/cli/package.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/cli/procedure.py` & `snowflake_cli_labs-0.2.9/src/snowcli/cli/procedure.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/cli/render.py` & `snowflake_cli_labs-0.2.9/src/snowcli/cli/render.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/cli/snowpark_shared.py` & `snowflake_cli_labs-0.2.9/src/snowcli/cli/snowpark_shared.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/cli/sql.py` & `snowflake_cli_labs-0.2.9/src/snowcli/cli/sql.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/cli/stage.py` & `snowflake_cli_labs-0.2.9/src/snowcli/cli/stage.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/cli/streamlit.py` & `snowflake_cli_labs-0.2.9/src/snowcli/cli/streamlit.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,22 @@
     CheckAnacondaForPyPiDependancies,
     PackageNativeLibrariesOption,
     PyPiDownloadOption,
     snowpark_package,
 )
 
 
+def get_standard_stage_name(name: str) -> str:
+    # Handle embedded stages
+    if name.startswith("snow://"):
+        return name
+
+    return f"@{name}"
+
+
 @app.command("list")
 def streamlit_list(
     environment: str = EnvironmentOption,
     only_cols: List[str] = typer.Option(list, help="Only show these columns"),
     show_header: bool = typer.Option(
         True,
         help="Show column headers",
@@ -91,34 +99,51 @@
     file: Path = typer.Option(
         "streamlit_app.py",
         exists=True,
         readable=True,
         file_okay=True,
         help="Path to streamlit file",
     ),
+    from_stage: Optional[str] = typer.Option(
+        None,
+        help="Stage name to copy streamlit file from",
+    ),
     use_packaging_workaround: bool = typer.Option(
         False,
         help="Set this flag to package all code and dependencies into a zip file. "
         + "This should be considered a temporary workaround until native support is available.",
     ),
 ):
     """
     Create a streamlit app named NAME.
     """
     env_conf = AppConfig().config.get(environment)
 
     if config.isAuth():
         config.connectToSnowflake()
+        if from_stage:
+            if "." in from_stage:
+                full_stage_name = from_stage
+            else:
+                full_stage_name = (
+                    f"{env_conf.get('database')}.{env_conf.get('schema')}.{from_stage}"
+                )
+            standard_page_name = get_standard_stage_name(full_stage_name)
+            from_stage_command = f"FROM {standard_page_name}"
+        else:
+            from_stage_command = ""
+
         results = config.snowflake_connection.createStreamlit(
             database=env_conf.get("database"),
             schema=env_conf.get("schema"),
             role=env_conf.get("role"),
             warehouse=env_conf.get("warehouse"),
             name=name,
             file="streamlit_app_launcher.py" if use_packaging_workaround else file.name,
+            from_stage_command=from_stage_command,
         )
         print_db_cursor(results)
 
 
 @app.command("share")
 def streamlit_share(
     environment: str = EnvironmentOption,
@@ -145,33 +170,28 @@
         print_db_cursor(results)
 
 
 @app.command("drop")
 def streamlit_drop(
     environment: str = EnvironmentOption,
     name: str = typer.Argument(..., help="Name of streamlit to be deleted."),
-    drop_stage: bool = typer.Option(
-        True,
-        help="Drop the stage associated with the streamlit app",
-    ),
 ):
     """
     Create a streamlit app named NAME.
     """
     env_conf = AppConfig().config.get(environment)
 
     if config.isAuth():
         config.connectToSnowflake()
         results = config.snowflake_connection.dropStreamlit(
             database=env_conf.get("database"),
             schema=env_conf.get("schema"),
             role=env_conf.get("role"),
             warehouse=env_conf.get("warehouse"),
             name=name,
-            drop_stage=drop_stage,
         )
         print_db_cursor(results)
 
 
 @app.command("deploy")
 def streamlit_deploy(
     environment: str = EnvironmentOption,
```

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/cli/warehouse.py` & `snowflake_cli_labs-0.2.9/src/snowcli/cli/warehouse.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/cli/procedure_coverage/clear.py` & `snowflake_cli_labs-0.2.9/src/snowcli/cli/procedure_coverage/clear.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/cli/procedure_coverage/report.py` & `snowflake_cli_labs-0.2.9/src/snowcli/cli/procedure_coverage/report.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/python_templates/snowpark_coverage.py.jinja` & `snowflake_cli_labs-0.2.9/src/snowcli/python_templates/snowpark_coverage.py.jinja`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/python_templates/streamlit_app_launcher.py.jinja` & `snowflake_cli_labs-0.2.9/src/snowcli/python_templates/streamlit_app_launcher.py.jinja`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/snowcli/sql/create_procedure.sql` & `snowflake_cli_labs-0.2.9/src/snowcli/sql/create_procedure.sql`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/templates/default_procedure/app.py` & `snowflake_cli_labs-0.2.9/src/templates/default_procedure/app.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/src/templates/default_procedure/local_connection.py` & `snowflake_cli_labs-0.2.9/src/templates/default_procedure/local_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/tests/test_render.py` & `snowflake_cli_labs-0.2.9/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/tests/test_snow_connector.py` & `snowflake_cli_labs-0.2.9/tests/test_snow_connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import textwrap
 from unittest import mock
 
+import pytest
 from snowcli.snow_connector import SnowflakeConnector
 
 
 # Used as a solution to syrupy having some problems with comparing multilines string
 class custom_str(str):
     def __repr__(self):
         return str(self)
@@ -171,46 +172,52 @@
         warehouse="warehouseValue",
         like="likeValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
+@pytest.mark.parametrize(
+    "stage_name", [("namedStageValue"), ("snow://embeddedStageValue")]
+)
 @mock.patch("snowflake.connector")
-def test_listStage(_, snapshot):
+def test_listStage(_, snapshot, stage_name):
     connector = SnowflakeConnector(
         connection_name="foo", snowsql_config=mock.MagicMock()
     )
     connector.ctx.execute_stream.return_value = (None, None)
 
     connector.listStage(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
-        name="nameValue",
+        name=stage_name,
         like="likeValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
+@pytest.mark.parametrize(
+    "stage_name", [("namedStageValue"), ("snow://embeddedStageValue")]
+)
 @mock.patch("snowflake.connector")
-def test_getStage(_, snapshot):
+def test_getStage(_, snapshot, stage_name):
     connector = SnowflakeConnector(
         connection_name="foo", snowsql_config=mock.MagicMock()
     )
     connector.ctx.execute_stream.return_value = (None, None)
 
     connector.getStage(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
-        name="nameValue",
+        name=stage_name,
         path="pathValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
@@ -231,49 +238,55 @@
         show_exceptions="show_exceptionsValue",
         comment="commentValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
+@pytest.mark.parametrize(
+    "stage_name", [("namedStageValue"), ("snow://embeddedStageValue")]
+)
 @mock.patch("snowflake.connector")
-def test_putStage(_, snapshot):
+def test_putStage(_, snapshot, stage_name):
     connector = SnowflakeConnector(
         connection_name="foo", snowsql_config=mock.MagicMock()
     )
     connector.ctx.execute_stream.return_value = (None, None)
 
     connector.putStage(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
-        name="nameValue",
+        name=stage_name,
         path="pathValue",
         overwrite=True,
         parallel="parallelValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert textwrap.dedent(query.getvalue()) == snapshot
 
 
+@pytest.mark.parametrize(
+    "stage_name", [("namedStageValue"), ("snow://embeddedStageValue")]
+)
 @mock.patch("snowflake.connector")
-def test_removeFromStage(_, snapshot):
+def test_removeFromStage(_, snapshot, stage_name):
     connector = SnowflakeConnector(
         connection_name="foo", snowsql_config=mock.MagicMock()
     )
     connector.ctx.execute_stream.return_value = (None, None)
 
     connector.removeFromStage(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
-        name="nameValue",
-        path="pathValue",
+        name=stage_name,
+        path="/pathValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
 def test_createStage(_, snapshot):
@@ -416,14 +429,34 @@
         file="fileValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
+def test_createStreamlitFromStage(_, snapshot):
+    connector = SnowflakeConnector(
+        connection_name="foo", snowsql_config=mock.MagicMock()
+    )
+    connector.ctx.execute_stream.return_value = (None, None)
+
+    connector.createStreamlit(
+        database="databaseValue",
+        schema="schemaValue",
+        role="roleValue",
+        warehouse="warehouseValue",
+        name="nameValue",
+        file="fileValue",
+        from_stage_command="FROM @stageValue",
+    )
+    query, *_ = connector.ctx.execute_stream.call_args.args
+    assert query.getvalue() == snapshot
+
+
+@mock.patch("snowflake.connector")
 def test_shareStreamlit(_, snapshot):
     connector = SnowflakeConnector(
         connection_name="foo", snowsql_config=mock.MagicMock()
     )
     connector.ctx.execute_stream.return_value = (None, None)
 
     connector.shareStreamlit(
@@ -447,15 +480,14 @@
 
     connector.dropStreamlit(
         database="databaseValue",
         schema="schemaValue",
         role="roleValue",
         warehouse="warehouseValue",
         name="nameValue",
-        drop_stage="drop_stageValue",
     )
     query, *_ = connector.ctx.execute_stream.call_args.args
     assert query.getvalue() == snapshot
 
 
 @mock.patch("snowflake.connector")
 def test_deployStreamlit(_, snapshot):
```

### Comparing `snowflake_cli_labs-0.2.8/tests/test_sql.py` & `snowflake_cli_labs-0.2.9/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `snowflake_cli_labs-0.2.8/tests/__snapshots__/test_snow_connector.ambr` & `snowflake_cli_labs-0.2.9/tests/__snapshots__/test_snow_connector.ambr`

 * *Files 12% similar despite different names*

```diff
@@ -46,23 +46,41 @@
 # name: test_createStreamlit
   '''
   use role roleValue;
   use database databaseValue;
   use schema schemaValue;
   use warehouse warehouseValue;
   
-  create or replace stage nameValue_stage;
+  create streamlit nameValue
+    
+    MAIN_FILE = 'fileValue'
+    QUERY_WAREHOUSE = warehouseValue;
+  
+  show streamlits;
+  describe streamlit nameValue;
+  
+  alter streamlit nameValue checkout;
+  '''
+# ---
+# name: test_createStreamlitFromStage
+  '''
+  use role roleValue;
+  use database databaseValue;
+  use schema schemaValue;
+  use warehouse warehouseValue;
   
   create streamlit nameValue
-    ROOT_LOCATION = @databaseValue.schemaValue.nameValue_stage
-    MAIN_FILE = '/fileValue'
+    FROM @stageValue
+    MAIN_FILE = 'fileValue'
     QUERY_WAREHOUSE = warehouseValue;
   
   show streamlits;
   describe streamlit nameValue;
+  
+  alter streamlit nameValue checkout;
   '''
 # ---
 # name: test_deployStreamlit
   '''
   use database databaseValue;
   use schema schemaValue;
   use role roleValue;
@@ -123,20 +141,18 @@
   use schema schemaValue;
   
   drop stage nameValue;
   '''
 # ---
 # name: test_dropStreamlit
   '''
+  use role roleValue;
   use database databaseValue;
   use schema schemaValue;
   use warehouse warehouseValue;
-  
-  drop stage "nameValue_STAGE";
-  
   drop streamlit "nameValue";
   '''
 # ---
 # name: test_executeFunction
   '''
   use role roleValue;
   use warehouse warehouseValue;
@@ -150,22 +166,32 @@
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   call procedureValue;
   '''
 # ---
-# name: test_getStage
+# name: test_getStage[namedStageValue]
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  get @namedStageValue file://pathValue/
+  '''
+# ---
+# name: test_getStage[snow://embeddedStageValue]
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
-  get @nameValue file://pathValue/
+  get snow://embeddedStageValue file://pathValue/
   '''
 # ---
 # name: test_listFunctions
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
@@ -180,21 +206,30 @@
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   show user procedures like 'likeValue';
   select "name", "created_on", "arguments" from table(result_scan(last_query_id()));
   '''
 # ---
-# name: test_listStage
+# name: test_listStage[namedStageValue]
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  ls @namedStageValue;
+  '''
+# ---
+# name: test_listStage[snow://embeddedStageValue]
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
-  ls @nameValue;
+  ls snow://embeddedStageValue;
   '''
 # ---
 # name: test_listStages
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
@@ -207,32 +242,52 @@
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   show streamlits;
   '''
 # ---
-# name: test_putStage
+# name: test_putStage[namedStageValue]
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  put file://pathValue @namedStageValue auto_compress=false parallel=parallelValue overwrite=True;
+  '''
+# ---
+# name: test_putStage[snow://embeddedStageValue]
+  '''
+  use role roleValue;
+  use warehouse warehouseValue;
+  use database databaseValue;
+  use schema schemaValue;
+  
+  put file://pathValue snow://embeddedStageValue auto_compress=false parallel=parallelValue overwrite=True;
+  '''
+# ---
+# name: test_removeFromStage[namedStageValue]
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
-  put file://pathValue @nameValue auto_compress=false parallel=parallelValue overwrite=True;
+  remove @namedStageValue/pathValue
   '''
 # ---
-# name: test_removeFromStage
+# name: test_removeFromStage[snow://embeddedStageValue]
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
   use schema schemaValue;
   
-  remove @nameValuepathValue
+  remove snow://embeddedStageValue/pathValue
   '''
 # ---
 # name: test_setProcedureComment
   '''
   use role roleValue;
   use warehouse warehouseValue;
   use database databaseValue;
```

### Comparing `snowflake_cli_labs-0.2.8/LICENSE` & `snowflake_cli_labs-0.2.9/LICENSE`

 * *Files identical despite different names*

