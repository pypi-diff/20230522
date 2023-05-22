# Comparing `tmp/Pokie-0.3.5.tar.gz` & `tmp/Pokie-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pokie-0.3.5.tar", last modified: Tue Jan 10 17:45:09 2023, max compression
+gzip compressed data, was "Pokie-0.4.1.tar", last modified: Mon May 22 13:14:59 2023, max compression
```

## Comparing `Pokie-0.3.5.tar` & `Pokie-0.4.1.tar`

### file list

```diff
@@ -1,148 +1,151 @@
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1326 2023-01-10 17:45:01.000000 Pokie-0.3.5/LICENSE
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      125 2023-01-10 17:45:01.000000 Pokie-0.3.5/MANIFEST.in
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1866 2023-01-10 17:45:09.769395 Pokie-0.3.5/PKG-INFO
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/Pokie.egg-info/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1866 2023-01-10 17:45:09.000000 Pokie-0.3.5/Pokie.egg-info/PKG-INFO
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3306 2023-01-10 17:45:09.000000 Pokie-0.3.5/Pokie.egg-info/SOURCES.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2023-01-10 17:45:09.000000 Pokie-0.3.5/Pokie.egg-info/dependency_links.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2023-01-10 17:45:09.000000 Pokie-0.3.5/Pokie.egg-info/not-zip-safe
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      157 2023-01-10 17:45:09.000000 Pokie-0.3.5/Pokie.egg-info/requires.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       12 2023-01-10 17:45:09.000000 Pokie-0.3.5/Pokie.egg-info/top_level.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      623 2023-01-10 17:45:01.000000 Pokie-0.3.5/README.md
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       64 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      116 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/__main__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/codegen/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/codegen/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/codegen/pg/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      104 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/codegen/pg/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2044 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/codegen/pg/record.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4238 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/codegen/pg/request.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     4111 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/codegen/pg/spec.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      405 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/codegen/spec.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      590 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/codegen/textfile.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/config/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/config/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1314 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/config/template.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1259 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/constants.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/contrib/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/contrib/auth/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/contrib/auth/cli/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      358 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/cli/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    11700 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/cli/acl.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    10574 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/cli/user.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       80 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/constants.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/contrib/auth/dto/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       48 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/dto/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      654 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/dto/acl.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      384 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/dto/user.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1491 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/module.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/contrib/auth/plugin/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       29 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/plugin/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2719 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/plugin/db.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/contrib/auth/repository/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/repository/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     8672 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/repository/acl.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      989 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/repository/user.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/contrib/auth/service/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       88 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/service/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3396 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/service/acl.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2510 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/service/auth.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2998 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/service/user.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/contrib/auth/sql/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1113 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/sql/001-auth-schema.sql
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/contrib/auth/view/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/view/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1660 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/auth/view/account.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/contrib/base/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/contrib/base/cli/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      255 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/cli/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5275 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/cli/base.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     6330 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/cli/codegen.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     7245 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/cli/db.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2624 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/cli/fixture.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2325 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/cli/job.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      106 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/constants.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.765395 Pokie-0.3.5/pokie/contrib/base/dto/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       51 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/dto/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      329 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/dto/records.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/contrib/base/job/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       26 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/job/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      459 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/job/idle.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1641 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/module.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/contrib/base/repository/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       43 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/repository/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      191 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/repository/fixture.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1985 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/repository/settings.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      807 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/repository/validator.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/contrib/base/service/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      128 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/service/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1025 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/service/autorest.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2098 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/service/fixture.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1125 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/service/settings.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2079 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/service/validator.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/contrib/base/sql/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      210 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/sql/001-settings.sql
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      138 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/sql/002-fixtures.sql
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/contrib/base/validators/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       46 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/validators/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1507 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/base/validators/pk.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/contrib/mail/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/contrib/mail/cli/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       46 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/cli/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1502 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/cli/queue.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       78 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/constants.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/contrib/mail/dto/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       63 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/dto/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      728 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/dto/records.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1466 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/helpers.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/contrib/mail/job/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       32 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/job/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2069 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/job/queue.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      661 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/module.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/contrib/mail/repository/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       76 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/repository/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2809 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/repository/repositories.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/contrib/mail/service/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       84 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/service/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1370 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/service/queue.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      939 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/service/template.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/contrib/mail/sql/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      854 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/contrib/mail/sql/001-mail.sql
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/core/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      139 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/core/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     6491 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/core/application.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      636 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/core/command.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/core/factories/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/core/factories/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      664 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/core/factories/login.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      887 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/core/factories/pgsql.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      848 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/core/factories/redis.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      475 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/core/module.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      813 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/core/signal.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/http/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       96 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/http/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2143 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/http/helpers.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      175 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/http/response.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     3129 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/http/rest.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2165 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/http/routes.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     9506 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/http/view.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/plugins/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/plugins/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      731 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/plugins/auth.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/rest/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       69 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/rest/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      652 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/rest/mixin.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2204 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/rest/service.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/pokie/util/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/util/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      775 2023-01-10 17:45:01.000000 Pokie-0.3.5/pokie/util/cli_args.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1515 2023-01-10 17:45:09.769395 Pokie-0.3.5/setup.cfg
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       39 2023-01-10 17:45:01.000000 Pokie-0.3.5/setup.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:09.769395 Pokie-0.3.5/tests/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2023-01-10 17:45:01.000000 Pokie-0.3.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-22 13:14:26.000000 Pokie-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-22 13:14:26.000000 Pokie-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-22 13:14:59.746138 Pokie-0.4.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.738138 Pokie-0.4.1/Pokie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-22 13:14:59.000000 Pokie-0.4.1/Pokie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-22 13:14:59.000000 Pokie-0.4.1/Pokie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:14:59.000000 Pokie-0.4.1/Pokie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:14:59.000000 Pokie-0.4.1/Pokie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 13:14:59.000000 Pokie-0.4.1/Pokie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 13:14:59.000000 Pokie-0.4.1/Pokie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-22 13:14:26.000000 Pokie-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.738138 Pokie-0.4.1/pokie/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.738138 Pokie-0.4.1/pokie/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/codegen/pg/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/pg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/pg/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/pg/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/pg/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/codegen/textfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/config/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/cli/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/cli/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/dto/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/dto/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/plugin/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8672 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/repository/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/repository/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/service/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/service/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/service/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/sql/001-auth-schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/auth/view/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/view/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/auth/view/account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/base/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/db_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/cli/tpl_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/base/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/dto/records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/base/job/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/job/idle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/base/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/repository/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/repository/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/repository/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.742138 Pokie-0.4.1/pokie/contrib/base/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/service/autorest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/service/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/service/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/service/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/base/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/sql/001-settings.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/sql/002-fixtures.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/base/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/base/validators/pk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/mail/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/mail/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/cli/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/mail/dto/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/dto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/dto/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/mail/job/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/job/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/mail/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/repository/repositories.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/mail/service/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/service/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/service/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/contrib/mail/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/contrib/mail/sql/001-mail.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/core/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/factories/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/factories/pgsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/factories/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/core/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/http/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/http/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/http/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/http/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/http/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/plugins/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/rest/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/rest/service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/pokie/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-22 13:14:26.000000 Pokie-0.4.1/pokie/util/cli_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-22 13:14:59.746138 Pokie-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 13:14:26.000000 Pokie-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:59.746138 Pokie-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:14:26.000000 Pokie-0.4.1/tests/__init__.py
```

### Comparing `Pokie-0.3.5/LICENSE` & `Pokie-0.4.1/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022-2023, João Pinheiro
+Copyright (c) João Pinheiro
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
     1. Redistributions of source code must retain the above copyright notice,
        this list of conditions and the following disclaimer.
```

### Comparing `Pokie-0.3.5/PKG-INFO` & `Pokie-0.4.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: Pokie
-Version: 0.3.5
+Version: 0.4.1
 Summary: A high-level Python REST web framework based on Flask, Rick and RickDb.
-Home-page: https://github.com/oddbit-project/pokie
+Home-page: https://git.oddbit.org/OddBit/pokie
 Author: João Pinheiro
 License: BSD-3-Clause
-Project-URL: Documentation, https://oddbit-project.github.io/pokie/
-Project-URL: Source, https://github.com/oddbit-project/pokie
-Platform: UNKNOWN
+Project-URL: Documentation, https://docs.oddbit.org/pokie/
+Project-URL: Source, https://git.oddbit.org/OddBit/pokie
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -20,23 +19,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Provides-Extra: redis
 Provides-Extra: jwt
 License-File: LICENSE
 
 # Welcome to Pokie
 
+
 [![Tests](https://github.com/oddbit-project/pokie/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/pokie/actions)
 [![pypi](https://img.shields.io/pypi/v/pokie.svg)](https://pypi.org/project/pokie/)
-[![license](https://img.shields.io/pypi/l/pokie.svg)](https://github.com/oddbit-project/pokie/blob/master/LICENSE)
-
-Pokie is a Flask application boilerplate, using [Rick](https://github.com/oddbit-project/rick) and 
-[Rick-db](https://github.com/oddbit-project/rick_db) components.
+[![license](https://img.shields.io/pypi/l/pokie.svg)](https://git.oddbit.org/OddBit/pokie/src/branch/master/LICENSE)
 
-For more information, please check the [Documentation](https://oddbit-project.github.io/pokie/)
 
+Pokie is a Flask application boilerplate, using [Rick](https://git.oddbit.org/OddBit/rick) and 
+[Rick-db](https://git.oddbit.org/OddBit/rick_db) components.
 
+For more information, please check the [Documentation](https://oddbit-project.github.io/pokie/)
```

### Comparing `Pokie-0.3.5/Pokie.egg-info/PKG-INFO` & `Pokie-0.4.1/Pokie.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: Pokie
-Version: 0.3.5
+Version: 0.4.1
 Summary: A high-level Python REST web framework based on Flask, Rick and RickDb.
-Home-page: https://github.com/oddbit-project/pokie
+Home-page: https://git.oddbit.org/OddBit/pokie
 Author: João Pinheiro
 License: BSD-3-Clause
-Project-URL: Documentation, https://oddbit-project.github.io/pokie/
-Project-URL: Source, https://github.com/oddbit-project/pokie
-Platform: UNKNOWN
+Project-URL: Documentation, https://docs.oddbit.org/pokie/
+Project-URL: Source, https://git.oddbit.org/OddBit/pokie
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
@@ -20,23 +19,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Provides-Extra: redis
 Provides-Extra: jwt
 License-File: LICENSE
 
 # Welcome to Pokie
 
+
 [![Tests](https://github.com/oddbit-project/pokie/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/pokie/actions)
 [![pypi](https://img.shields.io/pypi/v/pokie.svg)](https://pypi.org/project/pokie/)
-[![license](https://img.shields.io/pypi/l/pokie.svg)](https://github.com/oddbit-project/pokie/blob/master/LICENSE)
-
-Pokie is a Flask application boilerplate, using [Rick](https://github.com/oddbit-project/rick) and 
-[Rick-db](https://github.com/oddbit-project/rick_db) components.
+[![license](https://img.shields.io/pypi/l/pokie.svg)](https://git.oddbit.org/OddBit/pokie/src/branch/master/LICENSE)
 
-For more information, please check the [Documentation](https://oddbit-project.github.io/pokie/)
 
+Pokie is a Flask application boilerplate, using [Rick](https://git.oddbit.org/OddBit/rick) and 
+[Rick-db](https://git.oddbit.org/OddBit/rick_db) components.
 
+For more information, please check the [Documentation](https://oddbit-project.github.io/pokie/)
```

### Comparing `Pokie-0.3.5/Pokie.egg-info/SOURCES.txt` & `Pokie-0.4.1/Pokie.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 Pokie.egg-info/requires.txt
 Pokie.egg-info/top_level.txt
 pokie/__init__.py
 pokie/__main__.py
 pokie/constants.py
 pokie/codegen/__init__.py
 pokie/codegen/spec.py
+pokie/codegen/template.py
 pokie/codegen/textfile.py
 pokie/codegen/pg/__init__.py
 pokie/codegen/pg/record.py
 pokie/codegen/pg/request.py
 pokie/codegen/pg/spec.py
 pokie/config/__init__.py
 pokie/config/template.py
@@ -44,18 +45,20 @@
 pokie/contrib/auth/view/__init__.py
 pokie/contrib/auth/view/account.py
 pokie/contrib/base/__init__.py
 pokie/contrib/base/constants.py
 pokie/contrib/base/module.py
 pokie/contrib/base/cli/__init__.py
 pokie/contrib/base/cli/base.py
-pokie/contrib/base/cli/codegen.py
 pokie/contrib/base/cli/db.py
+pokie/contrib/base/cli/db_codegen.py
 pokie/contrib/base/cli/fixture.py
 pokie/contrib/base/cli/job.py
+pokie/contrib/base/cli/pytest.py
+pokie/contrib/base/cli/tpl_codegen.py
 pokie/contrib/base/dto/__init__.py
 pokie/contrib/base/dto/records.py
 pokie/contrib/base/job/__init__.py
 pokie/contrib/base/job/idle.py
 pokie/contrib/base/repository/__init__.py
 pokie/contrib/base/repository/fixture.py
 pokie/contrib/base/repository/settings.py
```

### Comparing `Pokie-0.3.5/README.md` & `Pokie-0.4.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Welcome to Pokie
 
+
 [![Tests](https://github.com/oddbit-project/pokie/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/pokie/actions)
 [![pypi](https://img.shields.io/pypi/v/pokie.svg)](https://pypi.org/project/pokie/)
-[![license](https://img.shields.io/pypi/l/pokie.svg)](https://github.com/oddbit-project/pokie/blob/master/LICENSE)
+[![license](https://img.shields.io/pypi/l/pokie.svg)](https://git.oddbit.org/OddBit/pokie/src/branch/master/LICENSE)
+
 
-Pokie is a Flask application boilerplate, using [Rick](https://github.com/oddbit-project/rick) and 
-[Rick-db](https://github.com/oddbit-project/rick_db) components.
+Pokie is a Flask application boilerplate, using [Rick](https://git.oddbit.org/OddBit/rick) and 
+[Rick-db](https://git.oddbit.org/OddBit/rick_db) components.
 
 For more information, please check the [Documentation](https://oddbit-project.github.io/pokie/)
```

### Comparing `Pokie-0.3.5/pokie/codegen/pg/record.py` & `Pokie-0.4.1/pokie/codegen/pg/record.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/codegen/pg/request.py` & `Pokie-0.4.1/pokie/codegen/pg/request.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/codegen/pg/spec.py` & `Pokie-0.4.1/pokie/codegen/pg/spec.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/codegen/textfile.py` & `Pokie-0.4.1/pokie/codegen/textfile.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/constants.py` & `Pokie-0.4.1/pokie/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Version
-POKIE_VERSION = ["0", "3", "5"]
+POKIE_VERSION = ["0", "4", "1"]
 
 
 def get_version():
     return ".".join(POKIE_VERSION)
 
 
 # Http Codes
```

### Comparing `Pokie-0.3.5/pokie/contrib/auth/cli/acl.py` & `Pokie-0.4.1/pokie/contrib/auth/cli/acl.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,14 @@
 class AclUserRoleCmd(AclCommand):
     description = "list roles associated with a given username"
 
     def arguments(self, parser: ArgumentParser):
         parser.add_argument("username", type=str, help="Existing username")
 
     def run(self, args) -> bool:
-
         user = self.svc_user.get_by_username(args.username)
         if user is None:
             self.tty.write(
                 self.tty.colorizer.red(
                     "Error: username '{}' not found".format(args.username)
                 )
             )
```

### Comparing `Pokie-0.3.5/pokie/contrib/auth/cli/user.py` & `Pokie-0.4.1/pokie/contrib/auth/cli/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,14 @@
             "--admin",
             default=False,
             action="store_true",
             help="Create admin (default False)",
         )
 
     def run(self, args) -> bool:
-
         req = UserCreateRequest()
         if not req.is_valid({"username": args.username, "email": args.email}):
             for k, v in req.get_errors().items():
                 self.tty.write(
                     self.tty.colorizer.red("Error in {}: {}".format(k, v["*"]))
                 )
             return False
@@ -107,15 +106,14 @@
         "attributes": "Attributes",
     }
 
     def arguments(self, parser: ArgumentParser):
         parser.add_argument("username", help="User name to search")
 
     def run(self, args) -> bool:
-
         req = UserInfoRequest()
         if not req.is_valid({"username": args.username}):
             for k, v in req.get_errors().items():
                 self.tty.write(
                     self.tty.colorizer.red("Error in {}: {}".format(k, v["*"]))
                 )
             return False
@@ -148,15 +146,14 @@
         )
         parser.add_argument(
             "-d", "--disabled", action="store_true", help="Disable user"
         )
         parser.add_argument("-e", "--enabled", action="store_true", help="Enable user")
 
     def run(self, args) -> bool:
-
         req = UserInfoRequest()
         if not req.is_valid({"username": args.username}):
             for k, v in req.get_errors().items():
                 self.tty.write(
                     self.tty.colorizer.red("Error in {}: {}".format(k, v["*"]))
                 )
             return False
@@ -279,15 +276,14 @@
             "-c", "--count", type=int, help="Records to show", default=0
         )
         parser.add_argument(
             "-i", "--id", action="store_true", help="Sort by id", default=False
         )
 
     def run(self, args) -> bool:
-
         if args.offset < 0:
             self.tty.write(self.tty.colorizer.red("Error: offset cannot be negative"))
             return False
 
         if args.count < 0:
             self.tty.write(self.tty.colorizer.red("Error: count cannot be negative"))
             return False
```

### Comparing `Pokie-0.3.5/pokie/contrib/auth/dto/acl.py` & `Pokie-0.4.1/pokie/contrib/auth/dto/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/auth/module.py` & `Pokie-0.4.1/pokie/contrib/auth/module.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/auth/plugin/db.py` & `Pokie-0.4.1/pokie/contrib/auth/plugin/db.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/auth/repository/acl.py` & `Pokie-0.4.1/pokie/contrib/auth/repository/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/auth/repository/user.py` & `Pokie-0.4.1/pokie/contrib/auth/repository/user.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/auth/service/acl.py` & `Pokie-0.4.1/pokie/contrib/auth/service/acl.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/auth/service/auth.py` & `Pokie-0.4.1/pokie/contrib/auth/service/auth.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/auth/service/user.py` & `Pokie-0.4.1/pokie/contrib/auth/service/user.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/auth/sql/001-auth-schema.sql` & `Pokie-0.4.1/pokie/contrib/auth/sql/001-auth-schema.sql`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     username VARCHAR(200) NOT NULL UNIQUE,
     first_name VARCHAR(100),
     last_name VARCHAR(100),
     email VARCHAR(200),
     password TEXT NOT NULL,
     creation_date timestamp with time zone default NOW(),
     last_login TIMESTAMP WITH TIME ZONE default NULL,
+    external BOOL DEFAULT False,
     attributes JSONB DEFAULT '{}'
 );
 
 CREATE TABLE acl_role(
     id_acl_role SERIAL NOT NULL PRIMARY KEY,
     description VARCHAR(200) NOT NULL UNIQUE
 );
```

### Comparing `Pokie-0.3.5/pokie/contrib/auth/view/account.py` & `Pokie-0.4.1/pokie/contrib/auth/view/account.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/base/cli/base.py` & `Pokie-0.4.1/pokie/contrib/base/cli/base.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/base/cli/codegen.py` & `Pokie-0.4.1/pokie/contrib/base/cli/db_codegen.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from typing import Optional, List
 
 from rick_db.conn import Connection
 from rick_db.sql.dialect import PgSqlDialect
 from rick_db.util.pg import PgInfo
 
 from pokie.codegen.pg import PgTableSpec, RecordGenerator, RequestGenerator
-from pokie.constants import DI_DB, DI_APP
+from pokie.constants import DI_DB
 from pokie.core import CliCommand
 
 
-class CodeGenCommand(CliCommand):
+class DbCodeGenCommand(CliCommand):
     def get_db(self) -> Optional[Connection]:
         result = None
         di = self.get_di()
         if di.has(DI_DB):
             result = di.get(DI_DB)
         return result
 
@@ -50,15 +50,14 @@
                 )
                 return []
             table_list.append(table)
 
         return table_list, schema
 
     def pg_gen_dto(self, db, table_expr, dest_file, camel_case=False) -> bool:
-
         pg = PgTableSpec(db)
         table_list, schema = self.parse_table_list(pg.manager(), table_expr)
         if len(table_list) == 0:
             return False
 
         gen = RecordGenerator()
         first = True
@@ -84,15 +83,14 @@
 
             self.tty.write(self.tty.colorizer.green("success!"))
         return True
 
     def pg_gen_request(
         self, db, table_expr, dest_file, camelcase_id=False, camelcase_cols=False
     ) -> bool:
-
         pg = PgTableSpec(db)
         table_list, schema = self.parse_table_list(pg.manager(), table_expr)
         if len(table_list) == 0:
             return False
 
         gen = RequestGenerator()
         first = True
@@ -124,15 +122,15 @@
             with open(dest_file, "w") as f:
                 f.write("\n".join(result))
 
             self.tty.write(self.tty.colorizer.green("success!"))
         return True
 
 
-class GenDtoCmd(CodeGenCommand):
+class GenDtoCmd(DbCodeGenCommand):
     description = "generate dto class from database table"
 
     def arguments(self, parser: ArgumentParser):
         parser.add_argument(
             "table", type=str, help="source table or view for dto generation"
         )
         parser.add_argument("-f", dest="file", type=str, help="destination file")
@@ -155,15 +153,15 @@
             if dest_file.exists():
                 self.tty.error("destination file already exists")
                 return False
 
         return self.pg_gen_dto(db, args.table, args.file, args.camelcase)
 
 
-class GenRequestRecordCmd(CodeGenCommand):
+class GenRequestRecordCmd(DbCodeGenCommand):
     description = "generate RequestRecord class from database table"
 
     def arguments(self, parser: ArgumentParser):
         parser.add_argument(
             "table", type=str, help="source table or view for request record generation"
         )
         parser.add_argument("-f", dest="file", type=str, help="destination file")
```

### Comparing `Pokie-0.3.5/pokie/contrib/base/cli/db.py` & `Pokie-0.4.1/pokie/contrib/base/cli/db.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/base/cli/fixture.py` & `Pokie-0.4.1/pokie/contrib/base/cli/fixture.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,14 @@
     def arguments(self, parser: ArgumentParser):
         parser.add_argument("name", type=str, help="fixture name(s) to run", nargs="*")
 
     def valid_name(self, name: str) -> bool:
         return name.find(".") > -1
 
     def run(self, args) -> bool:
-
         existing = []
         all = self.svc_fixture.scan() if len(args.name) == 0 else args.name
 
         for r in self.svc_fixture.list():
             existing.append(r.name)
 
         for name in all:
@@ -56,17 +55,29 @@
         return True
 
 
 class CheckFixtureCmd(FixtureCmd):
     description = "show existing fixture status"
 
     def run(self, args) -> bool:
-
         existing = []
         all = self.svc_fixture.scan()
+        if len(all) != len(set(all)):
+            # @todo: use rick.util.misc.list_duplicates()
+            duplicates = []
+            seen = set()
+            for item in all:
+                if item in seen:
+                    duplicates.append(item)
+                else:
+                    seen.add(item)
+            self.tty.error(
+                "Duplicated fixture(s) found: {}".format(",".join(duplicates))
+            )
+            return False
 
         for r in self.svc_fixture.list():
             existing.append(r.name)
 
         for name in all:
             self.tty.write("Fixture {}: ".format(name), eol=False)
             if name in existing:
```

### Comparing `Pokie-0.3.5/pokie/contrib/base/cli/job.py` & `Pokie-0.4.1/pokie/contrib/base/cli/job.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/base/module.py` & `Pokie-0.4.1/pokie/contrib/base/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,17 +19,20 @@
         "db:update": "pokie.contrib.base.cli.DbUpdateCmd",
         # worker job commands
         "job:list": "pokie.contrib.base.cli.JobListCmd",
         "job:run": "pokie.contrib.base.cli.JobRunCmd",
         # code generation
         "codegen:dto": "pokie.contrib.base.cli.GenDtoCmd",
         "codegen:request": "pokie.contrib.base.cli.GenRequestRecordCmd",
+        "codegen:module": "pokie.contrib.base.cli.ModuleGenCmd",
         # fixtures
         "fixture:run": "pokie.contrib.base.cli.RunFixtureCmd",
         "fixture:check": "pokie.contrib.base.cli.CheckFixtureCmd",
+        # tests
+        "pytest": "pokie.contrib.base.cli.PyTestCmd",
     }
 
     services = {
         # db-related validators
         SVC_VALIDATOR: "pokie.contrib.base.service.ValidatorService",
         # settings service
         SVC_SETTINGS: "pokie.contrib.base.service.SettingsService",
```

### Comparing `Pokie-0.3.5/pokie/contrib/base/repository/settings.py` & `Pokie-0.4.1/pokie/contrib/base/repository/settings.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/base/repository/validator.py` & `Pokie-0.4.1/pokie/contrib/base/repository/validator.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/base/service/autorest.py` & `Pokie-0.4.1/pokie/contrib/base/service/autorest.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/base/service/fixture.py` & `Pokie-0.4.1/pokie/contrib/base/service/fixture.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/base/service/settings.py` & `Pokie-0.4.1/pokie/contrib/base/service/settings.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/base/service/validator.py` & `Pokie-0.4.1/pokie/contrib/base/service/validator.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/base/validators/pk.py` & `Pokie-0.4.1/pokie/contrib/base/validators/pk.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/mail/cli/queue.py` & `Pokie-0.4.1/pokie/contrib/mail/cli/queue.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/mail/dto/records.py` & `Pokie-0.4.1/pokie/contrib/mail/dto/records.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/mail/helpers.py` & `Pokie-0.4.1/pokie/contrib/mail/helpers.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/mail/job/queue.py` & `Pokie-0.4.1/pokie/contrib/mail/job/queue.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/mail/module.py` & `Pokie-0.4.1/pokie/contrib/mail/module.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 
     services = {
         SVC_MESSAGE_TEMPLATE: "pokie.contrib.mail.service.MessageTemplateService",
         SVC_MESSAGE_QUEUE: "pokie.contrib.mail.service.MessageQueueService",
     }
 
     cmd = {
-        'mail:purge': 'pokie.contrib.mail.cli.PurgeQueueCmd',
-        'mail:run': 'pokie.contrib.mail.cli.RunQueueCmd',
+        "mail:purge": "pokie.contrib.mail.cli.PurgeQueueCmd",
+        "mail:run": "pokie.contrib.mail.cli.RunQueueCmd",
     }
 
     jobs = [
         "pokie.contrib.mail.job.MailQueueJob",
     ]
```

### Comparing `Pokie-0.3.5/pokie/contrib/mail/repository/repositories.py` & `Pokie-0.4.1/pokie/contrib/mail/repository/repositories.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         if record is not None:
             record.status = status
             if status == "S":
                 record.sent = iso8601_now()
             self.update(record)
 
     def find_first_and_lock(
-            self, channel: int, status: str = "Q"
+        self, channel: int, status: str = "Q"
     ) -> Optional[MessageQueueRecord]:
         """
         Locks a queued message and returns the record
         :param status: previous status of record to be locked
         :return:
         """
 
@@ -58,25 +58,27 @@
         with self._db.cursor() as c:
             result = c.fetchall(sql, values, self._record)
             if len(result) > 0:
                 return result[0]
             return None
 
     def truncate(self):
-        sql = "TRUNCATE TABLE {}".format(self.dialect().table(self._tablename, schema=self._schema))
+        sql = "TRUNCATE TABLE {}".format(
+            self.dialect().table(self._tablename, schema=self._schema)
+        )
         with self._db.cursor() as c:
             c.exec(sql)
 
 
 class MessageTemplateRepository(Repository):
     def __init__(self, db):
         super().__init__(db, MessageTemplateRecord)
 
     def find_template(
-            self, template: str, language: str, channel: int
+        self, template: str, language: str, channel: int
     ) -> Optional[MessageTemplateRecord]:
         sql, values = (
             self.select()
             .where(MessageTemplateRecord.template, "=", template)
             .where(MessageTemplateRecord.language, "=", language)
             .where(MessageTemplateRecord.channel, "=", channel)
             .limit(1)
```

### Comparing `Pokie-0.3.5/pokie/contrib/mail/service/queue.py` & `Pokie-0.4.1/pokie/contrib/mail/service/queue.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,7 @@
         :return:
         """
         return self.repo_queue.truncate()
 
     @property
     def repo_queue(self) -> MessageQueueRepository:
         return MessageQueueRepository(self.get_di().get(DI_DB))
-
```

### Comparing `Pokie-0.3.5/pokie/contrib/mail/service/template.py` & `Pokie-0.4.1/pokie/contrib/mail/service/template.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/contrib/mail/sql/001-mail.sql` & `Pokie-0.4.1/pokie/contrib/mail/sql/001-mail.sql`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/core/application.py` & `Pokie-0.4.1/pokie/core/application.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 from .module import BaseModule
 from .command import CliCommand
 from pokie.util.cli_args import ArgParser
 from .signal import SignalManager
 
 
 class FlaskApplication:
+    CLI_CMD_SUCCESS = 0
+    CLI_CMD_FAILED = 1
+    CLI_CMD_NOT_FOUND = 2
+
     module_file_name = "module"  # module class file name
     module_class_name = "Module"  # default module class name
 
     system_modules = [
         "pokie.contrib.base",
     ]  # system modules to always be included
 
@@ -132,40 +136,27 @@
             module.build(self)
 
         return self.app
 
     def http(self, **kwargs):
         self.app.run(**kwargs)
 
-    def cli(self, **kwargs):
-        """
-        Execute CLI commands
-        :param kwargs: optional parameters for ArgumentParse
-        :return:
-        """
+    def cli_runner(self, command: str, args: list = None, **kwargs) -> int:
+        # either console or inline commands
+        if args is None:
+            args = []
+
+        # parameter parser
+        parser = ArgParser(**kwargs)
+
         if "writer" in kwargs.keys():
             tty = kwargs["writer"]
         else:
             tty = ConsoleWriter()
 
-        # default command when no args detected
-        command = "list"
-        # extract command if specified
-        if len(sys.argv) > 1:
-            command = str(sys.argv[1])
-
-        if "add_help" not in kwargs.keys():
-            kwargs["add_help"] = False
-        if "usage" not in kwargs.keys():
-            kwargs["usage"] = "{} {} [OPTIONS...]".format(
-                os.path.basename(sys.argv[0]), command
-            )
-
-        parser = ArgParser(**kwargs)
-
         # lookup handler
         for _, module in self.modules.items():
             if command in module.cmd.keys():
                 handler = load_class(module.cmd[command])
                 if not handler:
                     raise RuntimeError(
                         "cli(): handler class '{}' not found".format(
@@ -173,22 +164,49 @@
                         )
                     )
                 if not issubclass(handler, CliCommand):
                     raise RuntimeError(
                         "cli(): command handler does not extend CliCommand"
                     )
                 handler = handler(self.di, writer=tty)  # type: CliCommand
-                handler.arguments(parser)
-                args = parser.parse_args(sys.argv[2:])
-                if parser.failed:
-                    # invalid/insufficient args
-                    tty.error(parser.error_message)
-                    parser.print_help(tty.stderr)
-                    exit(1)
-
-                if not handler.run(args):
-                    exit(1)
-                exit(0)
+                if not handler.skipargs:  # skipargs controls usage of argparser
+                    handler.arguments(parser)
+                    args = parser.parse_args(args)
+                    if parser.failed:
+                        # invalid/insufficient args
+                        tty.error(parser.error_message)
+                        parser.print_help(tty.stderr)
+                        return self.CLI_CMD_FAILED
+                else:
+                    # skipargs is true, all argparsing is ignored
+                    # this allow for custom cli arg handling
+                    args = None
+
+                if handler.run(args):
+                    return self.CLI_CMD_SUCCESS
+                return self.CLI_CMD_FAILED
 
         # command not found
         tty.error("error executing '{}': command not found".format(command))
-        exit(2)
+        return self.CLI_CMD_NOT_FOUND
+
+    def cli(self, **kwargs):
+        """
+        Execute CLI commands
+        :param kwargs: optional parameters for ArgumentParse
+        :return:
+        """
+        # default command when no args detected
+        command = "list"
+        # extract command if specified
+        if len(sys.argv) > 1:
+            command = str(sys.argv[1])
+
+        if "add_help" not in kwargs.keys():
+            kwargs["add_help"] = False
+        if "usage" not in kwargs.keys():
+            kwargs["usage"] = "{} {} [OPTIONS...]".format(
+                os.path.basename(sys.argv[0]), command
+            )
+
+        # exit code directly maps return codes
+        exit(self.cli_runner(command, sys.argv[2:], **kwargs))
```

### Comparing `Pokie-0.3.5/pokie/core/command.py` & `Pokie-0.4.1/pokie/core/command.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from rick.mixin import Injectable
 
 from pokie.constants import DI_TTY
 
 
 class CliCommand(ABC, Injectable):
     description = "command description"
+    skipargs = False
 
     def __init__(self, di: Di, writer=None):
         self.set_di(di)
         if not writer:
             if di.has(DI_TTY):
                 writer = di.get(DI_TTY)
             else:
```

### Comparing `Pokie-0.3.5/pokie/core/factories/login.py` & `Pokie-0.4.1/pokie/core/factories/login.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/core/factories/pgsql.py` & `Pokie-0.4.1/pokie/core/factories/pgsql.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/core/factories/redis.py` & `Pokie-0.4.1/pokie/core/factories/redis.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/core/signal.py` & `Pokie-0.4.1/pokie/core/signal.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/http/helpers.py` & `Pokie-0.4.1/pokie/http/helpers.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/http/rest.py` & `Pokie-0.4.1/pokie/http/rest.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/http/routes.py` & `Pokie-0.4.1/pokie/http/routes.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/http/view.py` & `Pokie-0.4.1/pokie/http/view.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/plugins/auth.py` & `Pokie-0.4.1/pokie/plugins/auth.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/rest/mixin.py` & `Pokie-0.4.1/pokie/rest/mixin.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/pokie/rest/service.py` & `Pokie-0.4.1/pokie/rest/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,32 +35,32 @@
     def update(self, id_record, record):
         return self.repository.update(record, id_record)
 
     def exists(self, id_record):
         return self.repository.valid_pk(id_record)
 
     def list(
-            self,
-            search_fields: list,
-            search_text: str = None,
-            match_fields: dict = None,
-            limit: int = None,
-            offset: int = None,
-            sort_fields: dict = None,
-            search_filter: list = None
+        self,
+        search_fields: list,
+        search_text: str = None,
+        match_fields: dict = None,
+        limit: int = None,
+        offset: int = None,
+        sort_fields: dict = None,
+        search_filter: list = None,
     ):
         grid = DbGrid(self.repository, search_fields, DbGrid.SEARCH_ANY)
         return grid.run(
             None,
             search_text=search_text,
             match_fields=match_fields,
             limit=limit,
             offset=offset,
             sort_fields=sort_fields,
-            search_fields=search_filter
+            search_fields=search_filter,
         )
 
     @property
     def repository(self) -> Repository:
         if self._record_cls is None:
             raise RuntimeError("Missing record class for repository")
         if self._repository_cls is None:
```

### Comparing `Pokie-0.3.5/pokie/util/cli_args.py` & `Pokie-0.4.1/pokie/util/cli_args.py`

 * *Files identical despite different names*

### Comparing `Pokie-0.3.5/setup.cfg` & `Pokie-0.4.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [metadata]
 name = Pokie
 version = attr: pokie.__version__
-url = https://github.com/oddbit-project/pokie
+url = https://git.oddbit.org/OddBit/pokie
 author = João Pinheiro
 description = A high-level Python REST web framework based on Flask, Rick and RickDb.
 long_description = file: README.md
+long_description_content_type = text/markdown
 license = BSD-3-Clause
 classifiers = 
 	Environment :: Web Environment
 	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
@@ -19,38 +20,41 @@
 	Programming Language :: Python :: 3.11
 	Topic :: Internet :: WWW/HTTP
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 	Topic :: Internet :: WWW/HTTP :: WSGI
 	Topic :: Software Development :: Libraries :: Application Frameworks
 	Topic :: Software Development :: Libraries :: Python Modules
 project_urls = 
-	Documentation = https://oddbit-project.github.io/pokie/
-	Source = https://github.com/oddbit-project/pokie
+	Documentation = https://docs.oddbit.org/pokie/
+	Source = https://git.oddbit.org/OddBit/pokie
 
 [options]
 python_requires = >=3.8
 packages = find:
 include_package_data = true
 zip_safe = false
 install_requires = 
-	rick-db~=1.0.6
-	rick~=0.4.6
-	rick-mailer~=1.0.0
-	Flask~=2.2.2
-	Flask-Login==0.6.2
-	iso8601~=0.1.16
+	rick-db>=1.1.2
+	rick>=0.6.0
+	rick-mailer>=1.0.1
+	Flask>=2.2.2
+	Flask-Login>=0.6.2
+	iso8601>=0.1.16
 	setuptools>=60.0.0
-	tabulate==0.9.0
+	tabulate>=0.9.0
 
 [options.extras_require]
 redis = redis
 jwt = pyjwt
 
 [bdist_rpm]
-doc_files = docs README.md
+doc_files = 
+	docs
+	README.md
+	pokie/contrib/base/template
 
 [flake8]
 exclude = dist,build,.git,.tox,./tests/
 extend-ignore = E501, W504 ,F401
 max-line-length = 120
 
 [egg_info]
```

