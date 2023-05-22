# Comparing `tmp/permit-1.2.2.tar.gz` & `tmp/permit-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permit-1.2.2.tar", last modified: Thu May 11 14:38:10 2023, max compression
+gzip compressed data, was "permit-2.0.0.tar", last modified: Mon May 22 06:46:16 2023, max compression
```

## Comparing `permit-1.2.2.tar` & `permit-2.0.0.tar`

### file list

```diff
@@ -1,224 +1,58 @@
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.039020 permit-1.2.2/
--rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-1.2.2/MANIFEST.in
--rw-r--r--   0 asafc      (501) staff       (20)      453 2023-05-11 14:38:10.038899 permit-1.2.2/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     7297 2022-10-01 21:14:31.000000 permit-1.2.2/README.md
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.021269 permit-1.2.2/permit/
--rw-r--r--   0 asafc      (501) staff       (20)      700 2022-10-01 21:14:31.000000 permit-1.2.2/permit/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.022236 permit-1.2.2/permit/api/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/api/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)    15873 2023-05-11 14:37:27.000000 permit-1.2.2/permit/api/client.py
--rw-r--r--   0 asafc      (501) staff       (20)     7362 2023-05-11 14:06:27.000000 permit-1.2.2/permit/api/client_sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.022336 permit-1.2.2/permit/cache/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.2/permit/cache/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     2884 2023-05-11 14:06:27.000000 permit-1.2.2/permit/client.py
--rw-r--r--   0 asafc      (501) staff       (20)     2170 2023-05-11 14:06:27.000000 permit-1.2.2/permit/config.py
--rw-r--r--   0 asafc      (501) staff       (20)       42 2023-04-04 20:50:12.000000 permit-1.2.2/permit/constants.py
--rw-r--r--   0 asafc      (501) staff       (20)      866 2023-05-11 14:06:27.000000 permit-1.2.2/permit/elements.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.022585 permit-1.2.2/permit/enforcement/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.2/permit/enforcement/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     6798 2023-05-11 14:06:27.000000 permit-1.2.2/permit/enforcement/enforcer.py
--rw-r--r--   0 asafc      (501) staff       (20)      742 2022-10-01 21:14:31.000000 permit-1.2.2/permit/enforcement/interfaces.py
--rw-r--r--   0 asafc      (501) staff       (20)     1495 2023-05-11 14:06:31.000000 permit-1.2.2/permit/exceptions.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.022677 permit-1.2.2/permit/instrument/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.2/permit/instrument/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.022851 permit-1.2.2/permit/mutations/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.2/permit/mutations/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)    13857 2023-05-11 14:06:27.000000 permit-1.2.2/permit/mutations/client.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.023131 permit-1.2.2/permit/openapi/
--rw-r--r--   0 asafc      (501) staff       (20)      101 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.023330 permit-1.2.2/permit/openapi/api/
--rw-r--r--   0 asafc      (501) staff       (20)       47 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.023709 permit-1.2.2/permit/openapi/api/api_keys/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/api_keys/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      726 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/api_keys/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     2900 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/api_keys/get_api_key_scope.py
--rw-r--r--   0 asafc      (501) staff       (20)     5029 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/api_keys/get_environment_api_key.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.023876 permit-1.2.2/permit/openapi/api/authentication/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/authentication/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     3595 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/authentication/elements_login_as.py
--rw-r--r--   0 asafc      (501) staff       (20)      341 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/base.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.024464 permit-1.2.2/permit/openapi/api/environments/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/environments/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     5109 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/environments/create_environment.py
--rw-r--r--   0 asafc      (501) staff       (20)     5105 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/environments/delete_environment.py
--rw-r--r--   0 asafc      (501) staff       (20)     5415 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/environments/get_environment.py
--rw-r--r--   0 asafc      (501) staff       (20)     6456 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/environments/list_environments.py
--rw-r--r--   0 asafc      (501) staff       (20)     5781 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/environments/update_environment.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.024917 permit-1.2.2/permit/openapi/api/opal_data/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/opal_data/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4979 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/opal_data/get_all_data.py
--rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/opal_data/get_data_for_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/opal_data/get_data_for_user.py
--rw-r--r--   0 asafc      (501) staff       (20)     5028 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/opal_data/get_pdp_info.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.025494 permit-1.2.2/permit/openapi/api/organizations/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/organizations/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4647 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/organizations/create_organization.py
--rw-r--r--   0 asafc      (501) staff       (20)     4437 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/organizations/delete_organization.py
--rw-r--r--   0 asafc      (501) staff       (20)     4932 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/organizations/get_organization.py
--rw-r--r--   0 asafc      (501) staff       (20)     5991 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/organizations/list_organizations.py
--rw-r--r--   0 asafc      (501) staff       (20)     5097 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/organizations/update_organization.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.026045 permit-1.2.2/permit/openapi/api/projects/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/projects/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4267 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/projects/create_project.py
--rw-r--r--   0 asafc      (501) staff       (20)     4305 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/projects/delete_project.py
--rw-r--r--   0 asafc      (501) staff       (20)     4547 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/projects/get_project.py
--rw-r--r--   0 asafc      (501) staff       (20)     5658 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/projects/list_projects.py
--rw-r--r--   0 asafc      (501) staff       (20)     4881 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/projects/update_project.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.026587 permit-1.2.2/permit/openapi/api/resource_actions/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_actions/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     7170 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_actions/create_resource_action.py
--rw-r--r--   0 asafc      (501) staff       (20)     7011 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_actions/delete_resource_action.py
--rw-r--r--   0 asafc      (501) staff       (20)     7069 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_actions/get_resource_action.py
--rw-r--r--   0 asafc      (501) staff       (20)     8107 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_actions/list_resource_actions.py
--rw-r--r--   0 asafc      (501) staff       (20)     8069 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_actions/update_resource_action.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.027137 permit-1.2.2/permit/openapi/api/resource_attributes/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_attributes/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     7433 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_attributes/create_resource_attribute.py
--rw-r--r--   0 asafc      (501) staff       (20)     7334 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_attributes/delete_resource_attribute.py
--rw-r--r--   0 asafc      (501) staff       (20)     7231 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_attributes/get_resource_attribute.py
--rw-r--r--   0 asafc      (501) staff       (20)     8173 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_attributes/list_resource_attributes.py
--rw-r--r--   0 asafc      (501) staff       (20)     8428 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_attributes/update_resource_attribute.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.028121 permit-1.2.2/permit/openapi/api/resource_roles/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     9926 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/add_parent_resource_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     7966 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/assign_permissions_to_resource_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     7588 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/create_resource_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     6901 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/delete_resource_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     6961 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/get_resource_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     8063 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/list_resource_roles.py
--rw-r--r--   0 asafc      (501) staff       (20)     9533 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/remove_parent_resource_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     8017 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/remove_permissions_from_resource_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     8271 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resource_roles/update_resource_role.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.028754 permit-1.2.2/permit/openapi/api/resources/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resources/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     8399 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resources/create_resource.py
--rw-r--r--   0 asafc      (501) staff       (20)     5917 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resources/delete_resource.py
--rw-r--r--   0 asafc      (501) staff       (20)     6068 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resources/get_resource.py
--rw-r--r--   0 asafc      (501) staff       (20)     8202 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resources/list_resources.py
--rw-r--r--   0 asafc      (501) staff       (20)     8438 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resources/replace_resource.py
--rw-r--r--   0 asafc      (501) staff       (20)     6861 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/resources/update_resource.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.029120 permit-1.2.2/permit/openapi/api/role_assignments/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/role_assignments/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     6767 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/role_assignments/assign_role.py
--rw-r--r--   0 asafc      (501) staff       (20)    11048 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/role_assignments/list_role_assignments.py
--rw-r--r--   0 asafc      (501) staff       (20)     6772 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/role_assignments/unassign_role.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.030062 permit-1.2.2/permit/openapi/api/roles/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     8630 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/add_parent_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     6989 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/assign_permissions_to_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     6371 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/create_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     6013 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/delete_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     5880 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/get_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     6999 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/list_roles.py
--rw-r--r--   0 asafc      (501) staff       (20)     8237 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/remove_parent_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     7040 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/remove_permissions_from_role.py
--rw-r--r--   0 asafc      (501) staff       (20)     7093 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/roles/update_role.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.030768 permit-1.2.2/permit/openapi/api/tenants/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/tenants/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     6768 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/tenants/create_tenant.py
--rw-r--r--   0 asafc      (501) staff       (20)     5842 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/tenants/delete_tenant.py
--rw-r--r--   0 asafc      (501) staff       (20)     6023 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/tenants/get_tenant.py
--rw-r--r--   0 asafc      (501) staff       (20)     8279 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/tenants/list_tenant_users.py
--rw-r--r--   0 asafc      (501) staff       (20)     7150 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/tenants/list_tenants.py
--rw-r--r--   0 asafc      (501) staff       (20)     6738 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/tenants/update_tenant.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.031677 permit-1.2.2/permit/openapi/api/users/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1371 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/api.py
--rw-r--r--   0 asafc      (501) staff       (20)     7226 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/assign_role_to_user.py
--rw-r--r--   0 asafc      (501) staff       (20)     7523 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/create_user.py
--rw-r--r--   0 asafc      (501) staff       (20)     5768 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/delete_user.py
--rw-r--r--   0 asafc      (501) staff       (20)     5905 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/get_user.py
--rw-r--r--   0 asafc      (501) staff       (20)     7671 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/list_users.py
--rw-r--r--   0 asafc      (501) staff       (20)     7392 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/unassign_role_from_user.py
--rw-r--r--   0 asafc      (501) staff       (20)     6573 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/api/users/update_user.py
--rw-r--r--   0 asafc      (501) staff       (20)     1660 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/client.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.037242 permit-1.2.2/permit/openapi/models/
--rw-r--r--   0 asafc      (501) staff       (20)     3996 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      476 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/action_block_editable.py
--rw-r--r--   0 asafc      (501) staff       (20)      647 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/action_block_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      483 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/add_role_permissions.py
--rw-r--r--   0 asafc      (501) staff       (20)      230 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/api_key_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      691 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/api_key_scope_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      609 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/attribute_block.py
--rw-r--r--   0 asafc      (501) staff       (20)      149 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/attribute_type.py
--rw-r--r--   0 asafc      (501) staff       (20)      635 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/environment_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     1452 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/environment_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      671 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/environment_update.py
--rw-r--r--   0 asafc      (501) staff       (20)      317 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/full_data.py
--rw-r--r--   0 asafc      (501) staff       (20)      255 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/http_validation_error.py
--rw-r--r--   0 asafc      (501) staff       (20)      684 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/organization_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     1173 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/organization_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      706 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/organization_update.py
--rw-r--r--   0 asafc      (501) staff       (20)      420 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/paginated_result_user_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      148 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/pdp_info_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      764 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/project_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     1407 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/project_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      800 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/project_update.py
--rw-r--r--   0 asafc      (501) staff       (20)      130 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/relations_block.py
--rw-r--r--   0 asafc      (501) staff       (20)      469 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/remove_role_permissions.py
--rw-r--r--   0 asafc      (501) staff       (20)      651 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_action_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     1949 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_action_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      457 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_action_update.py
--rw-r--r--   0 asafc      (501) staff       (20)      849 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_attribute_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     2224 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_attribute_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      635 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_attribute_update.py
--rw-r--r--   0 asafc      (501) staff       (20)     2117 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     3074 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_read.py
--rw-r--r--   0 asafc      (501) staff       (20)     1895 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_replace.py
--rw-r--r--   0 asafc      (501) staff       (20)     1153 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_role_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     2252 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_role_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      949 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_role_update.py
--rw-r--r--   0 asafc      (501) staff       (20)     1930 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/resource_update.py
--rw-r--r--   0 asafc      (501) staff       (20)      646 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_assignment_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     1517 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_assignment_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      652 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_assignment_remove.py
--rw-r--r--   0 asafc      (501) staff       (20)      852 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_block.py
--rw-r--r--   0 asafc      (501) staff       (20)     1145 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_create.py
--rw-r--r--   0 asafc      (501) staff       (20)      181 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_data.py
--rw-r--r--   0 asafc      (501) staff       (20)     2090 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      941 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/role_update.py
--rw-r--r--   0 asafc      (501) staff       (20)      126 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/roles_block.py
--rw-r--r--   0 asafc      (501) staff       (20)      832 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/tenant_create.py
--rw-r--r--   0 asafc      (501) staff       (20)     2072 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/tenant_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      655 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/tenant_update.py
--rw-r--r--   0 asafc      (501) staff       (20)     1171 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_create.py
--rw-r--r--   0 asafc      (501) staff       (20)      327 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_data.py
--rw-r--r--   0 asafc      (501) staff       (20)      369 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_login_request.py
--rw-r--r--   0 asafc      (501) staff       (20)      837 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_login_response.py
--rw-r--r--   0 asafc      (501) staff       (20)     1869 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_read.py
--rw-r--r--   0 asafc      (501) staff       (20)      317 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_role.py
--rw-r--r--   0 asafc      (501) staff       (20)      470 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_role_create.py
--rw-r--r--   0 asafc      (501) staff       (20)      472 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_role_remove.py
--rw-r--r--   0 asafc      (501) staff       (20)      798 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/user_update.py
--rw-r--r--   0 asafc      (501) staff       (20)      258 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/models/validation_error.py
--rw-r--r--   0 asafc      (501) staff       (20)      939 2023-05-11 14:06:27.000000 permit-1.2.2/permit/openapi/types.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.037605 permit-1.2.2/permit/resources/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.2/permit/resources/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1014 2023-04-04 20:50:12.000000 permit-1.2.2/permit/resources/interfaces.py
--rw-r--r--   0 asafc      (501) staff       (20)     6402 2022-10-01 21:14:31.000000 permit-1.2.2/permit/resources/registry.py
--rw-r--r--   0 asafc      (501) staff       (20)     6398 2022-10-01 21:14:31.000000 permit-1.2.2/permit/resources/reporter.py
--rw-r--r--   0 asafc      (501) staff       (20)     1496 2022-10-01 21:14:31.000000 permit-1.2.2/permit/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.037966 permit-1.2.2/permit/utils/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.2/permit/utils/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      848 2022-10-01 21:14:31.000000 permit-1.2.2/permit/utils/context.py
--rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-1.2.2/permit/utils/dicts.py
--rw-r--r--   0 asafc      (501) staff       (20)      926 2023-05-11 14:06:27.000000 permit-1.2.2/permit/utils/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.021942 permit-1.2.2/permit.egg-info/
--rw-r--r--   0 asafc      (501) staff       (20)      453 2023-05-11 14:38:09.000000 permit-1.2.2/permit.egg-info/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     7955 2023-05-11 14:38:10.000000 permit-1.2.2/permit.egg-info/SOURCES.txt
--rw-r--r--   0 asafc      (501) staff       (20)        1 2023-05-11 14:38:09.000000 permit-1.2.2/permit.egg-info/dependency_links.txt
--rw-r--r--   0 asafc      (501) staff       (20)       55 2023-05-11 14:38:09.000000 permit-1.2.2/permit.egg-info/requires.txt
--rw-r--r--   0 asafc      (501) staff       (20)       13 2023-05-11 14:38:09.000000 permit-1.2.2/permit.egg-info/top_level.txt
--rw-r--r--   0 asafc      (501) staff       (20)       55 2023-05-11 14:06:27.000000 permit-1.2.2/requirements.txt
--rw-r--r--   0 asafc      (501) staff       (20)       38 2023-05-11 14:38:10.039055 permit-1.2.2/setup.cfg
--rw-r--r--   0 asafc      (501) staff       (20)      767 2023-05-11 14:37:27.000000 permit-1.2.2/setup.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.038315 permit-1.2.2/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-1.2.2/tests/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-11 14:38:10.038733 permit-1.2.2/tests/api/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-11 14:06:27.000000 permit-1.2.2/tests/api/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      742 2023-05-11 14:06:27.000000 permit-1.2.2/tests/api/conftest.py
--rw-r--r--   0 asafc      (501) staff       (20)     8431 2023-05-11 14:06:27.000000 permit-1.2.2/tests/api/test_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     8489 2023-05-11 14:06:27.000000 permit-1.2.2/tests/api/test_client_sync.py
--rw-r--r--   0 asafc      (501) staff       (20)      532 2022-10-01 21:14:31.000000 permit-1.2.2/tests/conftest.py
--rw-r--r--   0 asafc      (501) staff       (20)     4429 2023-05-11 14:06:27.000000 permit-1.2.2/tests/test_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     4348 2023-05-11 14:06:27.000000 permit-1.2.2/tests/test_sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 06:46:16.451383 permit-2.0.0/
+-rw-r--r--   0 asafc      (501) staff       (20)    11357 2023-05-22 06:43:35.000000 permit-2.0.0/LICENSE
+-rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-2.0.0/MANIFEST.in
+-rw-r--r--   0 asafc      (501) staff       (20)      478 2023-05-22 06:46:16.451267 permit-2.0.0/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)      268 2023-05-22 06:43:35.000000 permit-2.0.0/README.md
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 06:46:16.447027 permit-2.0.0/permit/
+-rw-r--r--   0 asafc      (501) staff       (20)      373 2023-05-22 06:43:35.000000 permit-2.0.0/permit/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 06:46:16.449668 permit-2.0.0/permit/api/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     4185 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/api_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9692 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/base.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3601 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/condition_set_rules.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5424 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/condition_sets.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3534 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/context.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6793 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/deprecated.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1927 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/elements.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8821 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/environments.py
+-rw-r--r--   0 asafc      (501) staff       (20)   137541 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/models.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5098 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/projects.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5378 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/resource_action_groups.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6010 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/resource_actions.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6310 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/resource_attributes.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5971 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/resources.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5397 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/role_assignments.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6647 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/roles.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/sync_api_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6705 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/tenants.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8862 2023-05-22 06:43:35.000000 permit-2.0.0/permit/api/users.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2039 2023-05-22 06:43:35.000000 permit-2.0.0/permit/config.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 06:46:16.449939 permit-2.0.0/permit/enforcement/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.0/permit/enforcement/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7073 2023-05-22 06:43:35.000000 permit-2.0.0/permit/enforcement/enforcer.py
+-rw-r--r--   0 asafc      (501) staff       (20)      742 2022-10-01 21:14:31.000000 permit-2.0.0/permit/enforcement/interfaces.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2859 2023-05-22 06:43:35.000000 permit-2.0.0/permit/exceptions.py
+-rw-r--r--   0 asafc      (501) staff       (20)      212 2023-05-22 06:43:35.000000 permit-2.0.0/permit/logger.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3116 2023-05-22 06:43:35.000000 permit-2.0.0/permit/permit.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2494 2023-05-22 06:43:35.000000 permit-2.0.0/permit/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 06:46:16.450586 permit-2.0.0/permit/utils/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.0/permit/utils/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      836 2023-05-22 06:43:35.000000 permit-2.0.0/permit/utils/context.py
+-rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-2.0.0/permit/utils/dicts.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1496 2023-05-22 06:43:35.000000 permit-2.0.0/permit/utils/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 06:46:16.447504 permit-2.0.0/permit.egg-info/
+-rw-r--r--   0 asafc      (501) staff       (20)      478 2023-05-22 06:46:16.000000 permit-2.0.0/permit.egg-info/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)     1142 2023-05-22 06:46:16.000000 permit-2.0.0/permit.egg-info/SOURCES.txt
+-rw-r--r--   0 asafc      (501) staff       (20)        1 2023-05-22 06:46:16.000000 permit-2.0.0/permit.egg-info/dependency_links.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 06:46:16.000000 permit-2.0.0/permit.egg-info/requires.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       13 2023-05-22 06:46:16.000000 permit-2.0.0/permit.egg-info/top_level.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 06:43:35.000000 permit-2.0.0/requirements.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       38 2023-05-22 06:46:16.451418 permit-2.0.0/setup.cfg
+-rw-r--r--   0 asafc      (501) staff       (20)      793 2023-05-22 06:43:35.000000 permit-2.0.0/setup.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-05-22 06:46:16.451129 permit-2.0.0/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.0/tests/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1191 2023-05-22 06:43:35.000000 permit-2.0.0/tests/conftest.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9232 2023-05-22 06:43:35.000000 permit-2.0.0/tests/test_abac_e2e.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8745 2023-05-22 06:43:35.000000 permit-2.0.0/tests/test_rbac_e2e.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8666 2023-05-22 06:43:35.000000 permit-2.0.0/tests/test_rbac_e2e_sync.py
+-rw-r--r--   0 asafc      (501) staff       (20)      323 2023-05-22 06:43:35.000000 permit-2.0.0/tests/utils.py
```

### Comparing `permit-1.2.2/permit/config.py` & `permit-2.0.0/permit/config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,62 @@
 from typing import List
 
 from pydantic import BaseModel, Field
 
-from permit.constants import DEFAULT_PDP_URL
+from .api.context import ApiContext
 
 
 class LoggerConfig(BaseModel):
-    level: str = Field("info", description="logging level")
-    label: str = Field("Permit.io", description="label added to logs")
+    enable: bool = Field(
+        False, description="Whether or not to enable logging from the Permit library"
+    )
+    level: str = Field(
+        "info", description="Sets the log level configured for the Permit SDK Logger."
+    )
+    label: str = Field(
+        "Permit",
+        description="Sets the label configured for logs emitted by the Permit SDK Logger.",
+    )
     log_as_json: bool = Field(
         False,
         alias="json",
-        description="When logging - dump full data to console as JSON",
-    )
-
-
-class AutoMappingConfig(BaseModel):
-    enable: bool = Field(
-        False,
-        description="Should the module automatically plugin to map frameworks on load",
-    )
-    ignored_url_prefixes: List[str] = Field(
-        [],
-        description="if auto mapping is on, ignore these prefixes when analyzing url paths",
+        description="Sets whether the SDK log output should be in JSON format.",
     )
-    review_mode: bool = Field(False, description="Print review and do nothing active")
 
 
 class MultiTenancyConfig(BaseModel):
     default_tenant: str = Field(
-        "default", description="the tenant key of the default tenant"
+        "default",
+        description="the key of the default tenant to be used if use_default_tenant_if_empty == True",
     )
     use_default_tenant_if_empty: bool = Field(
         True,
-        description="if resource tenant was not specified, should we assume the default tenant?",
+        description="whether or not the SDK should automatically associate a resource with the defaultTenant "
+        + "if the resource provided in permit.check() was not associated with a tenant (i.e: undefined tenant).",
     )
 
 
 class PermitConfig(BaseModel):
+    token: str = Field(
+        ...,
+        description="The token (API Key) used for authorization against the PDP and the Permit REST API.",
+    )
+    pdp: str = Field(
+        "http://localhost:7766",
+        description="Configures the Policy Decision Point (PDP) url.",
+    )
     api_url: str = Field(
-        "https://api.permit.io", description="The url of Permit.io API"
+        "https://api.permit.io", description="The url of Permit REST API"
     )
-    token: str = Field(
-        "", description="Your PDP token, used to authenticate to the PDP"
+    log: LoggerConfig = Field(
+        LoggerConfig(), description="the logger configuration used by the SDK"
+    )
+    multi_tenancy: MultiTenancyConfig = Field(
+        MultiTenancyConfig(),
+        description="configuration of default tenant assignment for RBAC",
+    )
+    api_context: ApiContext = Field(
+        ApiContext(), description="represents the current API key authorization level."
     )
-    pdp: str = Field(DEFAULT_PDP_URL, description="Your PDP url")
-    debug_mode: bool = Field(False, description="in debug mode we log more stuff")
-    log: LoggerConfig = Field(LoggerConfig())
-    auto_mapping: AutoMappingConfig = Field(AutoMappingConfig())
-    multi_tenancy: MultiTenancyConfig = Field(MultiTenancyConfig())
-
-
-class ConfigFactory:
-    @staticmethod
-    def build(options: dict) -> PermitConfig:
-        config = PermitConfig(**options)
-        # if no log level was set manually but debug mode is set,
-        # we set the log level to debug/info respectively
-        log_level_option = options.get("log", {}).get("level", None)
-        if log_level_option is None:
-            config.log.level = "debug" if config.debug_mode else "info"
 
-        return config
+    class Config:
+        arbitrary_types_allowed = True
```

### Comparing `permit-1.2.2/permit/enforcement/enforcer.py` & `permit-2.0.0/permit/enforcement/enforcer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
 from typing import Union
 
 import aiohttp
 from loguru import logger
 
-from permit.config import PermitConfig
-from permit.enforcement.interfaces import ResourceInput, UserInput
-from permit.exceptions import PermitConnectionError
-from permit.utils.context import Context, ContextStore
+from ..config import PermitConfig
+from ..exceptions import PermitConnectionError
+from ..utils.context import Context, ContextStore
+from ..utils.sync import SyncClass
+from .interfaces import ResourceInput, UserInput
 
 
 def set_if_not_none(d: dict, k: str, v):
     if v is not None:
         d[k] = v
 
 
@@ -21,15 +22,14 @@
 Action = str
 Resource = Union[dict, str]
 
 
 class Enforcer:
     def __init__(self, config: PermitConfig):
         self._config = config
-        self._logger = logger.bind(name="permit.enforcer")
         self._context_store = ContextStore()
         self._headers = {
             "Content-Type": "application/json",
             "Authorization": f"bearer {self._config.token}",
         }
         self._base_url = self._config.pdp
 
@@ -45,31 +45,39 @@
         self,
         user: User,
         action: Action,
         resource: Resource,
         context: Context = {},
     ) -> bool:
         """
-        usage:
+        Checks if a user is authorized to perform an action on a resource within the specified context.
 
-        user is a unique string identifying the user on the application end.
-        usually it is the `sub` claim (subject claim) present inside a JWT token.
+        Args:
+            user: The user object representing the user.
+            action: The action to be performed on the resource.
+            resource: The resource object representing the resource.
+            context: The context object representing the context in which the action is performed. Defaults to None.
 
-        it can also be dictionary of type UserInput, in case you want to pass
-        more context about the user (user attributes, etc).
+        Returns:
+            bool: True if the user is authorized, False otherwise.
 
-        # can the user close any issue?
-        await permit.check(user, 'close', 'issue')
+        Raises:
+            PermitConnectionError: If an error occurs while sending the authorization request to the PDP.
 
-        # can the user close any issue who's id is 1234?
-        await permit.check(user, 'close', 'issue:1234')
+        Examples:
 
-        # can the user close (any) issues belonging to the 't1' tenant?
-        # (in a multi tenant application)
-        await permit.check(user, 'close', {'type': 'issue', 'tenant': 't1'})
+            # can the user close any issue?
+            await permit.check(user, 'close', 'issue')
+
+            # can the user close any issue who's id is 1234?
+            await permit.check(user, 'close', 'issue:1234')
+
+            # can the user close (any) issues belonging to the 't1' tenant?
+            # (in a multi tenant application)
+            await permit.check(user, 'close', {'type': 'issue', 'tenant': 't1'})
         """
         normalized_user: UserInput = (
             UserInput(key=user) if isinstance(user, str) else UserInput(**user)
         )
         normalized_resource: ResourceInput = self._normalize_resource(
             (
                 self._resource_from_string(resource)
@@ -89,15 +97,15 @@
             try:
                 async with session.post(
                     f"{self._base_url}/allowed",
                     data=json.dumps(input),
                 ) as response:
                     if response.status != 200:
                         error_json: dict = await response.json()
-                        self._logger.error(
+                        logger.error(
                             "error in permit.check({}, {}, {}):\n{}\n{}".format(
                                 normalized_user,
                                 action,
                                 self._resource_repr(normalized_resource),
                                 f"status code: {response.status}",
                                 repr(error_json),
                             )
@@ -105,26 +113,25 @@
                         raise PermitConnectionError(
                             f"Permit SDK got unexpected status code: {response.status}, please check your Permit SDK class init and PDP container are configured correctly. \n\
                             Read more about setting up the PDP at https://docs.permit.io/reference/SDKs/Python/quickstart_python"
                         )
 
                     content: dict = await response.json()
                     decision: bool = bool(content.get("allow", False))
-                    if self._config.debug_mode:
-                        self._logger.info(
-                            "permit.check({}, {}, {}) = {}".format(
-                                normalized_user,
-                                action,
-                                self._resource_repr(normalized_resource),
-                                repr(decision),
-                            )
+                    logger.debug(
+                        "permit.check({}, {}, {}) = {}".format(
+                            normalized_user,
+                            action,
+                            self._resource_repr(normalized_resource),
+                            repr(decision),
                         )
+                    )
                     return decision
             except aiohttp.ClientError as err:
-                self._logger.error(
+                logger.error(
                     "error in permit.check({}, {}, {}):\n{}".format(
                         normalized_user,
                         action,
                         self._resource_repr(normalized_resource),
                         err,
                     )
                 )
@@ -165,7 +172,11 @@
 
     @staticmethod
     def _resource_from_string(resource: str) -> ResourceInput:
         parts = resource.split(RESOURCE_DELIMITER)
         if len(parts) < 1 or len(parts) > 2:
             raise ValueError(f"permit.check() got invalid resource string: {resource}")
         return ResourceInput(type=parts[0], id=(parts[1] if len(parts) > 1 else None))
+
+
+class SyncEnforcer(Enforcer, metaclass=SyncClass):
+    pass
```

### Comparing `permit-1.2.2/permit/enforcement/interfaces.py` & `permit-2.0.0/permit/enforcement/interfaces.py`

 * *Files identical despite different names*

### Comparing `permit-1.2.2/permit/resources/reporter.py` & `permit-2.0.0/permit/api/resource_actions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,172 +1,174 @@
-import json
 from typing import List
 
-import aiohttp
-from loguru import logger
-from pydantic import BaseModel
-
-from permit.config import PermitConfig
-from permit.resources.interfaces import ActionConfig, ResourceConfig, ResourceTypes
-from permit.resources.registry import (
-    ActionDefinition,
-    ResourceDefinition,
-    ResourceRegistry,
-)
-
-
-class SyncObjectResponse(BaseModel):
-    id: str
-
-
-class AbstractResourceReporter:
-    def add_action_to_resource(self, resource_name: str, action_def: ActionDefinition):
-        raise NotImplementedError("abstract class")
-
-
-class ResourceStub:
-    def __init__(self, reporter: AbstractResourceReporter, resource_name: str):
-        self._reporter = reporter
-        self._resource_name = resource_name
-
-    def action(self, config: ActionConfig):
-        action = ActionDefinition(
-            name=config.name,
-            title=config.title,
-            description=config.description,
-            path=config.path,
-            attributes=config.attributes or {},
-        )
-        self._reporter.add_action_to_resource(self._resource_name, action)
+from pydantic import validate_arguments
 
+from .base import BasePermitApi, SimpleHttpClient, ensure_context, pagination_params
+from .context import ApiKeyLevel
+from .models import ResourceActionCreate, ResourceActionRead, ResourceActionUpdate
 
-class ResourceReporter(AbstractResourceReporter):
-    def __init__(self, config: PermitConfig, registry: ResourceRegistry):
-        self._config = config
-        self._registry = registry
-        self._logger = logger.bind(name="permit.resources.reporter")
-        self._headers = {
-            "Authorization": f"Bearer {self._config.token}",
-            "Content-Type": "application/json",
-        }
-        self._base_url = self._config.pdp
-        self._initialized = True  # TODO: remove this
-
-    async def __aenter__(self):
-        await self._sync_resources_to_control_plane()
-        return self
 
-    async def __aexit__(self, exc_type, exc, tb):
+class ResourceActionsApi(BasePermitApi):
+    @property
+    def __actions(self) -> SimpleHttpClient:
+        return self._build_http_client(
+            "/v2/schema/{proj_id}/{env_id}/resources".format(
+                proj_id=self.config.api_context.project,
+                env_id=self.config.api_context.environment,
+            )
+        )
+
+    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @validate_arguments
+    async def list(
+        self, resource_key: str, page: int = 1, per_page: int = 100
+    ) -> List[ResourceActionRead]:
         """
-        Context handler to terminate internal tasks
+        Retrieves a list of actions.
+
+        Args:
+            resource_key: The key of the resource to filter on.
+            page: The page number to fetch (default: 1).
+            per_page: How many items to fetch per page (default: 100).
+
+        Returns:
+            an array of actions.
+
+        Raises:
+            PermitApiError: If the API returns an error HTTP status code.
+            PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        pass
+        return await self.__actions.get(
+            f"/{resource_key}/actions",
+            model=List[ResourceActionRead],
+            params=pagination_params(page, per_page),
+        )
 
-    @property
-    def token(self) -> str:
-        return self._config.token
+    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @validate_arguments
+    async def get(self, resource_key: str, action_key: str) -> ResourceActionRead:
+        """
+        Retrieves a action by its key.
 
-    async def add_resource(self, resource: ResourceDefinition) -> ResourceStub:
-        self._registry.add_resource(resource)
-        await self._maybe_sync_resource(resource)
-        return ResourceStub(self, resource.name)
-
-    async def add_action_to_resource(
-        self, resource_name: str, action_def: ActionDefinition
-    ):
-        action = self._registry.add_action_to_resource(resource_name, action_def)
-        if action is not None:
-            await self._maybe_sync_action(action)
-
-    async def _maybe_sync_resource(self, resource: ResourceDefinition):
-        if self._initialized and not self._registry.is_synced(resource):
-            self._logger.info(f"syncing resource: {repr(resource)}")
-            async with aiohttp.ClientSession(headers=self._headers) as session:
-                try:
-                    async with session.put(
-                        f"{self._base_url}/cloud/resources/{resource.name}",
-                        data=json.dumps(resource.dict()),
-                    ) as response:
-                        content: dict = await response.json()
-                        remote_id: str = content.get("id", None)
-                        if remote_id is not None:
-                            self._registry.mark_as_synced(resource, remote_id=remote_id)
-                except aiohttp.ClientError as err:
-                    self._logger.error(
-                        f"tried to sync resource {resource.name}, got error: {err}"
-                    )
-
-    async def _maybe_sync_action(self, action: ActionDefinition):
-        resource_id = action.resource_id
-        if resource_id is None:
-            return
-
-        if self._initialized and not self._registry.is_synced(action):
-            self._logger.info(f"syncing action: {repr(action)}")
-            async with aiohttp.ClientSession(headers=self._headers) as session:
-                try:
-                    async with session.put(
-                        f"{self._base_url}/cloud/resources/{resource_id}/actions",
-                        data=json.dumps(action.dict()),
-                    ) as response:
-                        content: dict = await response.json()
-                        remote_id: str = content.get("id", None)
-                        if remote_id is not None:
-                            self._registry.mark_as_synced(action, remote_id=remote_id)
-                except aiohttp.ClientError as err:
-                    self._logger.error(
-                        f"tried to sync action {action.name}, got error: {err}"
-                    )
-
-    async def _sync_resources_to_control_plane(self):
-        for resource in self._registry.resources:
-            await self._maybe_sync_resource(resource)
-
-    async def resource(self, config: ResourceConfig) -> ResourceStub:
-        resource = ResourceDefinition(
-            name=config.name,
-            type=config.type,
-            path=config.path,
-            description=config.description,
-            actions=config.actions or [],
-            attributes=config.attributes or {},
+        Args:
+            resource_key: The key of the resource the action belongs to.
+            action_key: The key of the action.
+
+        Returns:
+            the action.
+
+        Raises:
+            PermitApiError: If the API returns an error HTTP status code.
+            PermitContextError: If the configured ApiContext does not match the required endpoint context.
+        """
+        return await self.__actions.get(
+            f"/{resource_key}/actions/{action_key}", model=ResourceActionRead
         )
-        return await self.add_resource(resource)
 
-    def action(self, config: ActionConfig) -> ActionDefinition:
-        return ActionDefinition(
-            name=config.name,
-            title=config.title,
-            description=config.description,
-            path=config.path,
-            attributes=config.attributes or {},
+    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @validate_arguments
+    async def get_by_key(
+        self, resource_key: str, action_key: str
+    ) -> ResourceActionRead:
+        """
+        Retrieves a action by its key.
+        Alias for the get method.
+
+        Args:
+            resource_key: The key of the resource the action belongs to.
+            action_key: The key of the action.
+
+        Returns:
+            the action.
+
+        Raises:
+            PermitApiError: If the API returns an error HTTP status code.
+            PermitContextError: If the configured ApiContext does not match the required endpoint context.
+        """
+        return await self.get(resource_key, action_key)
+
+    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @validate_arguments
+    async def get_by_id(self, resource_id: str, action_id: str) -> ResourceActionRead:
+        """
+        Retrieves a action by its ID.
+        Alias for the get method.
+
+        Args:
+            resource_key: The ID of the resource the action belongs to.
+            action_id: The ID of the action.
+
+        Returns:
+            the action.
+
+        Raises:
+            PermitApiError: If the API returns an error HTTP status code.
+            PermitContextError: If the configured ApiContext does not match the required endpoint context.
+        """
+        return await self.get(resource_id, action_id)
+
+    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @validate_arguments
+    async def create(
+        self, resource_key: str, action_data: ResourceActionCreate
+    ) -> ResourceActionRead:
+        """
+        Creates a new action.
+
+        Args:
+            resource_key: The key of the resource under which the action should be created.
+            action_data: The data for the new action.
+
+        Returns:
+            the created action.
+
+        Raises:
+            PermitApiError: If the API returns an error HTTP status code.
+            PermitContextError: If the configured ApiContext does not match the required endpoint context.
+        """
+        return await self.__actions.post(
+            f"/{resource_key}/actions",
+            model=ResourceActionRead,
+            json=action_data,
         )
 
-    async def sync_resources(self, config: ResourceTypes) -> List[ResourceStub]:
-        stubs: List[ResourceStub] = []
+    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @validate_arguments
+    async def update(
+        self, resource_key: str, action_key: str, action_data: ResourceActionUpdate
+    ) -> ResourceActionRead:
+        """
+        Updates a action.
 
-        for resource in config.resources:
-            actions = []
-            for actionName, action in iter(resource.actions.items()):
-                actions.append(
-                    ActionDefinition(
-                        name=actionName,
-                        title=action.title or actionName,
-                        description=action.description,
-                        path=action.path,
-                        attributes=action.attributes or {},
-                    )
-                )
-
-            stub = await self.add_resource(
-                ResourceDefinition(
-                    name=resource.type,
-                    type="rest",
-                    path=f"/resources/{resource.type}",
-                    description=resource.description,
-                    actions=actions,
-                    attributes=resource.attributes or {},
-                )
-            )
-            stubs.append(stub)
+        Args:
+            resource_key: The key of the resource the action belongs to.
+            action_key: The key of the action.
+            action_data: The updated data for the action.
+
+        Returns:
+            the updated action.
+
+        Raises:
+            PermitApiError: If the API returns an error HTTP status code.
+            PermitContextError: If the configured ApiContext does not match the required endpoint context.
+        """
+        return await self.__actions.patch(
+            f"/{resource_key}/actions/{action_key}",
+            model=ResourceActionRead,
+            json=action_data,
+        )
 
-        return stubs
+    @ensure_context(ApiKeyLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @validate_arguments
+    async def delete(self, resource_key: str, action_key: str) -> None:
+        """
+        Deletes a action.
+
+        Args:
+            resource_key: The key of the resource the action belongs to.
+            action_key: The key of the action to delete.
+
+        Raises:
+            PermitApiError: If the API returns an error HTTP status code.
+            PermitContextError: If the configured ApiContext does not match the required endpoint context.
+        """
+        return await self.__actions.delete(f"/{resource_key}/actions/{action_key}")
```

### Comparing `permit-1.2.2/permit/utils/context.py` & `permit-2.0.0/permit/utils/context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Callable, Dict, List
 
-from permit.utils.dicts import deep_merge
+from .dicts import deep_merge
 
 Context = Dict[str, Any]
 ContextTransform = Callable[[Context], Context]
 
 
 class ContextStore:
     def __init__(self):
```

### Comparing `permit-1.2.2/setup.py` & `permit-2.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,18 +6,19 @@
         env = "-{}".format(env)
     with open("requirements{}.txt".format(env)) as fp:
         return [x.strip() for x in fp.read().split("\n") if not x.startswith("#")]
 
 
 setup(
     name="permit",
-    version="1.2.2",
+    version="2.0.0",
     packages=find_packages(),
     author="Asaf Cohen",
     author_email="asaf@permit.io",
+    license="Apache 2.0",
     python_requires=">=3.7",
     description="Permit.io python sdk",
     install_requires=get_requirements(),
     classifiers=[
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
```

