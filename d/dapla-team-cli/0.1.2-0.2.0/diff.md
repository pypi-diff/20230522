# Comparing `tmp/dapla_team_cli-0.1.2.tar.gz` & `tmp/dapla_team_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_team_cli-0.1.2.tar", max compression
+gzip compressed data, was "dapla_team_cli-0.2.0.tar", max compression
```

## Comparing `dapla_team_cli-0.1.2.tar` & `dapla_team_cli-0.2.0.tar`

### file list

```diff
@@ -1,53 +1,89 @@
--rw-r--r--   0        0        0     1099 2023-03-02 08:01:11.495973 dapla_team_cli-0.1.2/LICENSE
--rw-r--r--   0        0        0     2917 2023-03-02 08:01:11.495973 dapla_team_cli-0.1.2/README.md
--rw-r--r--   0        0        0     2905 2023-03-02 08:01:26.451970 dapla_team_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      433 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/__init__.py
--rw-r--r--   0        0        0     2464 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/__main__.py
--rw-r--r--   0        0        0       50 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/api/__init__.py
--rw-r--r--   0        0        0       43 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/api/models/__init__.py
--rw-r--r--   0        0        0     1111 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/api/models/group.py
--rw-r--r--   0        0        0      157 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/api/models/link.py
--rw-r--r--   0        0        0     1417 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/api/models/team.py
--rw-r--r--   0        0        0      873 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/api/models/user.py
--rw-r--r--   0        0        0     1351 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/api/utils.py
--rw-r--r--   0        0        0       27 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/auth/__init__.py
--rw-r--r--   0        0        0     2263 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/auth/cmd.py
--rw-r--r--   0        0        0       47 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/auth/services/__init__.py
--rw-r--r--   0        0        0      407 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/auth/services/expiry.py
--rw-r--r--   0        0        0     2284 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/auth/services/get_token.py
--rw-r--r--   0        0        0     1299 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/auth/services/set_token.py
--rw-r--r--   0        0        0     1493 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/config.py
--rw-r--r--   0        0        0       44 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/doctor/__init__.py
--rw-r--r--   0        0        0      708 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/doctor/check.py
--rw-r--r--   0        0        0     1398 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/doctor/cmd.py
--rw-r--r--   0        0        0     3483 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/doctor/gcloud.py
--rw-r--r--   0        0        0     1296 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/doctor/keycloak.py
--rw-r--r--   0        0        0     2060 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/gcp/__init__.py
--rw-r--r--   0        0        0   230022 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/gcp/project_roles.json
--rw-r--r--   0        0        0     1477 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/github.py
--rw-r--r--   0        0        0       35 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/groups/__init__.py
--rw-r--r--   0        0        0      357 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/groups/cmd.py
--rw-r--r--   0        0        0       35 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/groups/list_members/__init__.py
--rw-r--r--   0        0        0     2891 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/groups/list_members/cmd.py
--rw-r--r--   0        0        0       49 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/groups/services/__init__.py
--rw-r--r--   0        0        0       22 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/secrets/__init__.py
--rw-r--r--   0        0        0     2851 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/secrets/cmd.py
--rw-r--r--   0        0        0     2405 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/secrets/services.py
--rw-r--r--   0        0        0     3353 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/team.py
--rw-r--r--   0        0        0       37 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/tf/__init__.py
--rw-r--r--   0        0        0      345 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/tf/cmd.py
--rw-r--r--   0        0        0      414 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/__init__.py
--rw-r--r--   0        0        0     2962 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/auth_groups.py
--rw-r--r--   0        0        0     3727 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/buckets.py
--rw-r--r--   0        0        0    13631 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/cmd.py
--rw-r--r--   0        0        0     3174 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/configs.py
--rw-r--r--   0        0        0      434 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/environments.py
--rw-r--r--   0        0        0     3339 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/expiry.py
--rw-r--r--   0        0        0     1631 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/project_roles.py
--rw-r--r--   0        0        0     1021 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/templates/buckets-iam.jinja
--rw-r--r--   0        0        0      112 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/templates/iam-bindings-git-commit-msg.jinja
--rw-r--r--   0        0        0      977 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/templates/projects-iam.jinja
--rw-r--r--   0        0        0     6232 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/terraform.py
--rw-r--r--   0        0        0     1994 2023-03-02 08:01:11.511973 dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/utilities.py
--rw-r--r--   0        0        0     4836 1970-01-01 00:00:00.000000 dapla_team_cli-0.1.2/setup.py
--rw-r--r--   0        0        0     4772 1970-01-01 00:00:00.000000 dapla_team_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-22 12:39:51.129940 dapla_team_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2915 2023-05-22 12:39:51.129940 dapla_team_cli-0.2.0/README.md
+-rw-r--r--   0        0        0     3015 2023-05-22 12:40:08.098262 dapla_team_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      433 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/__init__.py
+-rw-r--r--   0        0        0     2629 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/__main__.py
+-rw-r--r--   0        0        0       50 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/api/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/api/models/__init__.py
+-rw-r--r--   0        0        0     1111 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/api/models/group.py
+-rw-r--r--   0        0        0      157 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/api/models/link.py
+-rw-r--r--   0        0        0     1417 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/api/models/team.py
+-rw-r--r--   0        0        0      873 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/api/models/user.py
+-rw-r--r--   0        0        0     1351 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/api/utils.py
+-rw-r--r--   0        0        0       27 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/auth/__init__.py
+-rw-r--r--   0        0        0     2263 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/auth/cmd.py
+-rw-r--r--   0        0        0       47 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/auth/services/__init__.py
+-rw-r--r--   0        0        0      407 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/auth/services/expiry.py
+-rw-r--r--   0        0        0     2284 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/auth/services/get_token.py
+-rw-r--r--   0        0        0     1299 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/auth/services/set_token.py
+-rw-r--r--   0        0        0     1496 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/config.py
+-rw-r--r--   0        0        0       44 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/doctor/__init__.py
+-rw-r--r--   0        0        0      708 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/doctor/check.py
+-rw-r--r--   0        0        0     1398 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/doctor/cmd.py
+-rw-r--r--   0        0        0     3483 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/doctor/gcloud.py
+-rw-r--r--   0        0        0     1296 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/doctor/keycloak.py
+-rw-r--r--   0        0        0     2060 2023-05-22 12:39:51.141940 dapla_team_cli-0.2.0/src/dapla_team_cli/gcp/__init__.py
+-rw-r--r--   0        0        0   230022 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/gcp/project_roles.json
+-rw-r--r--   0        0        0     4296 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/github.py
+-rw-r--r--   0        0        0       35 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/groups/__init__.py
+-rw-r--r--   0        0        0      357 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/groups/cmd.py
+-rw-r--r--   0        0        0       35 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/groups/list_members/__init__.py
+-rw-r--r--   0        0        0     2891 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/groups/list_members/cmd.py
+-rw-r--r--   0        0        0       49 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/groups/services/__init__.py
+-rw-r--r--   0        0        0       37 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/approve/__init__.py
+-rw-r--r--   0        0        0     1657 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/approve/approve.py
+-rw-r--r--   0        0        0      359 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/approve/cmd.py
+-rw-r--r--   0        0        0       36 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/atlantis_apply/__init__.py
+-rw-r--r--   0        0        0     2795 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/atlantis_apply/atlantis_apply_all.py
+-rw-r--r--   0        0        0      833 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/atlantis_apply/cmd.py
+-rw-r--r--   0        0        0       35 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/atlantis_plan/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/atlantis_plan/atlantis_plan_all.py
+-rw-r--r--   0        0        0      490 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/atlantis_plan/cmd.py
+-rw-r--r--   0        0        0      675 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/batch_handler.py
+-rw-r--r--   0        0        0     1191 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/cmd.py
+-rw-r--r--   0        0        0     1809 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/const.py
+-rw-r--r--   0        0        0       29 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/janitor/__init__.py
+-rw-r--r--   0        0        0     2030 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/janitor/close_all.py
+-rw-r--r--   0        0        0      694 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/janitor/cmd.py
+-rw-r--r--   0        0        0       31 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/merge/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/merge/cmd.py
+-rw-r--r--   0        0        0     2592 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/merge/merge_all.py
+-rw-r--r--   0        0        0       34 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/open/__init__.py
+-rw-r--r--   0        0        0     2591 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/open/cmd.py
+-rw-r--r--   0        0        0     3917 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/open/open_prs.py
+-rw-r--r--   0        0        0       37 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/probe/__init__.py
+-rw-r--r--   0        0        0      880 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/probe/cmd.py
+-rw-r--r--   0        0        0     1851 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/probe/probe_atlantis_apply.py
+-rw-r--r--   0        0        0     3659 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/probe/probe_workflows.py
+-rw-r--r--   0        0        0      434 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/prompt_utils.py
+-rw-r--r--   0        0        0       82 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/ready/__init__.py
+-rw-r--r--   0        0        0      775 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/ready/cmd.py
+-rw-r--r--   0        0        0     2332 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/ready/generate_state.py
+-rw-r--r--   0        0        0     1225 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/rich_check.py
+-rw-r--r--   0        0        0       54 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/state/__init__.py
+-rw-r--r--   0        0        0      967 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/state/cmd.py
+-rw-r--r--   0        0        0     3639 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/state/state_commands.py
+-rw-r--r--   0        0        0     4426 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/state/state_utils.py
+-rw-r--r--   0        0        0       35 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/validate/__init__.py
+-rw-r--r--   0        0        0      135 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/pr/validate/cmd.py
+-rw-r--r--   0        0        0       22 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/secrets/__init__.py
+-rw-r--r--   0        0        0     2851 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/secrets/cmd.py
+-rw-r--r--   0        0        0     2405 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/secrets/services.py
+-rw-r--r--   0        0        0     3353 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/team.py
+-rw-r--r--   0        0        0       37 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/tf/__init__.py
+-rw-r--r--   0        0        0      345 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/tf/cmd.py
+-rw-r--r--   0        0        0      414 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/__init__.py
+-rw-r--r--   0        0        0     2962 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/auth_groups.py
+-rw-r--r--   0        0        0     3727 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/buckets.py
+-rw-r--r--   0        0        0    13631 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/cmd.py
+-rw-r--r--   0        0        0     3174 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/configs.py
+-rw-r--r--   0        0        0      434 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/environments.py
+-rw-r--r--   0        0        0     3339 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/expiry.py
+-rw-r--r--   0        0        0     1631 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/project_roles.py
+-rw-r--r--   0        0        0     1021 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/templates/buckets-iam.jinja
+-rw-r--r--   0        0        0      112 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/templates/iam-bindings-git-commit-msg.jinja
+-rw-r--r--   0        0        0      977 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/templates/projects-iam.jinja
+-rw-r--r--   0        0        0     6232 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/terraform.py
+-rw-r--r--   0        0        0     1994 2023-05-22 12:39:51.145940 dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/utilities.py
+-rw-r--r--   0        0        0     4796 1970-01-01 00:00:00.000000 dapla_team_cli-0.2.0/PKG-INFO
```

### Comparing `dapla_team_cli-0.1.2/LICENSE` & `dapla_team_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/README.md` & `dapla_team_cli-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 <!-- this anchor is linked to, so avoid renaming it -->
 
 ## Installation
 
 Install with [pipx]:
 
 ```console
-$ pipx install dapla-team-cli
+pipx install dapla-team-cli
 ```
 
 (Be patient, installation can take some time.)
 
 ## Features
 
 - Assign bucket access and GCP roles to members for a limited amount of time
```

### Comparing `dapla_team_cli-0.1.2/pyproject.toml` & `dapla_team_cli-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-team-cli"
-version = "0.1.2"
+version = "0.2.0"
 description = "CLI for working with Dapla Teams"
 authors = ["Kenneth Leine Schulstad <kls@rdck.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-team-cli"
 repository = "https://github.com/statisticsnorway/dapla-team-cli"
 documentation = "https://statisticsnorway.github.io/dapla-team-cli"
@@ -14,36 +14,38 @@
     "Typing :: Typed",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/statisticsnorway/dapla-team-cli/releases"
 
 [tool.poetry.dependencies]
-python = "^3.8.0"
-click = ">=8.1.3"
-devtools = "^0.9.0"
+python = ">=3.10.0,<4.0"
+click = "^8.1.3"
+devtools = "^0.11.0"
 questionary = "^1.10.0"
 pendulum = "^2.1.2"
-rich = "^12.5.1"
-pydantic = "^1.9.1"
+rich = "^13.3.5"
+pydantic = "^1.10.7"
 python-tfvars = "^0.1.0"
 Jinja2 = "^3.1.2"
-GitPython = "^3.1.27"
-azure-cli = "^2.43.0"
-google-cloud-secret-manager = "^2.12.4"
-twine = "^4.0.1"
+GitPython = "^3.1.31"
+azure-cli = "^2.48.1"
+google-cloud-secret-manager = "^2.16.1"
+twine = "^4.0.2"
 click-configfile = "^0.2.3"
 click-config-file = "^0.6.0"
-jupyterhub = "^3.0.0"
-requests = "^2.28.1"
-typer = "^0.6.1"
-SQLAlchemy = "2.0.0b1"
-returns = "^0.19.0"
-python-hcl2 = "^4.3.0"
-typeguard = "^2.13.3"
+jupyterhub = "^4.0.0"
+requests = "^2.30.0"
+typer = "^0.9.0"
+SQLAlchemy = "^2.0.13"
+returns = "^0.20.0"
+python-hcl2 = "^4.3.1"
+typeguard = "^3.0.2"
+google-cloud-storage = "^2.9.0"
+types-google-cloud-ndb = "^2.1.0.7"
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 coverage = {extras = ["toml"], version = ">=6.2"}
 darglint = ">=1.8.1"
 isort = ">=5.10.1"
 mypy = ">=0.930"
@@ -51,24 +53,24 @@
 pre-commit = ">=2.16.0"
 pre-commit-hooks = ">=4.1.0"
 pytest = ">=6.2.5"
 pyupgrade = ">=2.29.1"
 safety = ">=1.10.3"
 typeguard = ">=2.13.3"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
-mkdocstrings = "^0.19.0"
-mkdocstrings-python = "^0.7.1"
-mkdocs = "^1.3.1"
-mkdocs-material = "^8.3.9"
-mkdocs-gen-files = "^0.3.5"
-mkdocs-literate-nav = "^0.4.1"
-mkdocs-section-index = "^0.3.4"
-mkdocs-typer = "^0.0.2"
-black = "^22.6.0"
-pylint = "^2.14.5"
+mkdocstrings = ">=0.19.0"
+mkdocstrings-python = ">=0.7.1"
+mkdocs = ">=1.3.1"
+mkdocs-material = ">=8.3.9"
+mkdocs-gen-files = ">=0.3.5"
+mkdocs-literate-nav = ">=0.4.1"
+mkdocs-section-index = ">=0.3.4"
+mkdocs-typer = ">=0.0.2"
+black = ">=22.6.0"
+pylint = ">=2.14.5"
 
 [tool.poetry.scripts]
 dpteam = "dapla_team_cli.__main__:main"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
@@ -86,14 +88,15 @@
 force_single_line = true
 lines_after_imports = 2
 
 [tool.black]
 line-length = 132
 
 [tool.mypy]
+implicit_reexport = true
 strict = true
 warn_unreachable = true
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 show_error_context = true
 # Need to apply this globally until mypy fixes this issue: https://github.com/python/mypy/issues/10757
```

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/__main__.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,23 +10,25 @@
     ´iam-bindings´ is the actual command
 
 Command groups must be mounted here to become available.
 
 Each sub-command's modules should be grouped into a separate python package.
 """
 import logging
+import os
 from enum import Enum
 from importlib.metadata import version
 from typing import Optional
 
 import typer
 
 import dapla_team_cli.auth.cmd as auth
 import dapla_team_cli.doctor.cmd as doctor
 import dapla_team_cli.groups.cmd as groups
+import dapla_team_cli.pr.cmd as pr
 import dapla_team_cli.secrets.cmd as secrets
 import dapla_team_cli.tf.cmd as tf
 
 
 app = typer.Typer(no_args_is_help=True, pretty_exceptions_show_locals=False)
 logging.basicConfig()
 
@@ -83,11 +85,15 @@
 
 
 app.add_typer(tf.app)
 app.add_typer(groups.app)
 app.add_typer(secrets.app)
 app.add_typer(auth.app)
 
+if os.getenv("NB_USER") != "jovyan":  # Batch update should only be used outside of Jupyter
+    app.add_typer(pr.app)
+
+
 app.command()(doctor.doctor)
 
 if __name__ == "__main__":
     main()
```

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/api/models/group.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/api/models/group.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/api/models/team.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/api/models/team.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/api/models/user.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/api/models/user.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/api/utils.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/api/utils.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/auth/cmd.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/auth/cmd.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/auth/services/get_token.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/auth/services/get_token.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/auth/services/set_token.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/auth/services/set_token.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/config.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """
     if platform in ("linux", "darwin"):
         config_folder_path = Path.home() / ".config/dapla-team-cli"
     elif platform == "win32":
         username = os.getlogin()
         config_folder_path = Path(rf"C:\Users\{username}\AppData\dapla-team-cli")
     else:
-        raise Exception("Unknown platform. The CLI only supports Unix and Windows based platforms.")
+        raise RuntimeError("Unknown platform. The CLI only supports Unix and Windows based platforms.")
 
     if not os.path.exists(config_folder_path):
         os.makedirs(config_folder_path)
 
     if tmp:
         return str(config_folder_path / "tmp/")
```

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/doctor/check.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/doctor/check.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/doctor/cmd.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/doctor/cmd.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/doctor/gcloud.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/doctor/gcloud.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/doctor/keycloak.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/doctor/keycloak.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/gcp/__init__.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/gcp/project_roles.json` & `dapla_team_cli-0.2.0/src/dapla_team_cli/gcp/project_roles.json`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/groups/list_members/cmd.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/groups/list_members/cmd.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/secrets/cmd.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/secrets/cmd.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/secrets/services.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/secrets/services.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/team.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/team.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/auth_groups.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/auth_groups.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/buckets.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/buckets.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/cmd.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/cmd.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/configs.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/configs.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/expiry.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/expiry.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/project_roles.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/project_roles.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/templates/buckets-iam.jinja` & `dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/templates/buckets-iam.jinja`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/templates/projects-iam.jinja` & `dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/templates/projects-iam.jinja`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/terraform.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/terraform.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/src/dapla_team_cli/tf/iam_bindings/utilities.py` & `dapla_team_cli-0.2.0/src/dapla_team_cli/tf/iam_bindings/utilities.py`

 * *Files identical despite different names*

### Comparing `dapla_team_cli-0.1.2/PKG-INFO` & `dapla_team_cli-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 Metadata-Version: 2.1
 Name: dapla-team-cli
-Version: 0.1.2
+Version: 0.2.0
 Summary: CLI for working with Dapla Teams
 Home-page: https://github.com/statisticsnorway/dapla-team-cli
 License: MIT
 Author: Kenneth Leine Schulstad
 Author-email: kls@rdck.no
-Requires-Python: >=3.8.0,<4.0.0
+Requires-Python: >=3.10.0,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
-Requires-Dist: GitPython (>=3.1.27,<4.0.0)
+Requires-Dist: GitPython (>=3.1.31,<4.0.0)
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: SQLAlchemy (==2.0.0b1)
-Requires-Dist: azure-cli (>=2.43.0,<3.0.0)
-Requires-Dist: click (>=8.1.3)
+Requires-Dist: SQLAlchemy (>=2.0.13,<3.0.0)
+Requires-Dist: azure-cli (>=2.48.1,<3.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-config-file (>=0.6.0,<0.7.0)
 Requires-Dist: click-configfile (>=0.2.3,<0.3.0)
-Requires-Dist: devtools (>=0.9.0,<0.10.0)
-Requires-Dist: google-cloud-secret-manager (>=2.12.4,<3.0.0)
-Requires-Dist: jupyterhub (>=3.0.0,<4.0.0)
+Requires-Dist: devtools (>=0.11.0,<0.12.0)
+Requires-Dist: google-cloud-secret-manager (>=2.16.1,<3.0.0)
+Requires-Dist: google-cloud-storage (>=2.9.0,<3.0.0)
+Requires-Dist: jupyterhub (>=4.0.0,<5.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
-Requires-Dist: pydantic (>=1.9.1,<2.0.0)
-Requires-Dist: python-hcl2 (>=4.3.0,<5.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: python-hcl2 (>=4.3.1,<5.0.0)
 Requires-Dist: python-tfvars (>=0.1.0,<0.2.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: returns (>=0.19.0,<0.20.0)
-Requires-Dist: rich (>=12.5.1,<13.0.0)
-Requires-Dist: twine (>=4.0.1,<5.0.0)
-Requires-Dist: typeguard (>=2.13.3,<3.0.0)
-Requires-Dist: typer (>=0.6.1,<0.7.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: returns (>=0.20.0,<0.21.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
+Requires-Dist: twine (>=4.0.2,<5.0.0)
+Requires-Dist: typeguard (>=3.0.2,<4.0.0)
+Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: types-google-cloud-ndb (>=2.1.0.7,<3.0.0.0)
 Project-URL: Changelog, https://github.com/statisticsnorway/dapla-team-cli/releases
 Project-URL: Documentation, https://statisticsnorway.github.io/dapla-team-cli
 Project-URL: Repository, https://github.com/statisticsnorway/dapla-team-cli
 Description-Content-Type: text/markdown
 
 # Dapla Team CLI
 
@@ -74,15 +74,15 @@
 <!-- this anchor is linked to, so avoid renaming it -->
 
 ## Installation
 
 Install with [pipx]:
 
 ```console
-$ pipx install dapla-team-cli
+pipx install dapla-team-cli
 ```
 
 (Be patient, installation can take some time.)
 
 ## Features
 
 - Assign bucket access and GCP roles to members for a limited amount of time
```

